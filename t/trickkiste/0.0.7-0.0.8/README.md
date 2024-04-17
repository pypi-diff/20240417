# Comparing `tmp/trickkiste-0.0.7.tar.gz` & `tmp/trickkiste-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trickkiste-0.0.7.tar", max compression
+gzip compressed data, was "trickkiste-0.0.8.tar", max compression
```

## Comparing `trickkiste-0.0.7.tar` & `trickkiste-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      676 2023-12-10 05:33:15.492574 trickkiste-0.0.7/Readme.md
--rw-r--r--   0        0        0     1563 2024-02-08 08:54:21.463200 trickkiste-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-11 10:54:02.708905 trickkiste-0.0.7/trickkiste/__init__.py
--rw-r--r--   0        0        0       42 2024-01-11 10:54:02.712905 trickkiste-0.0.7/trickkiste/base_tui_app.css
--rw-r--r--   0        0        0     2982 2024-01-11 10:54:02.712905 trickkiste-0.0.7/trickkiste/base_tui_app.py
--rwxr-xr-x   0        0        0      978 2024-02-08 08:51:43.258359 trickkiste-0.0.7/trickkiste/examples/fancylogging.py
--rwxr-xr-x   0        0        0     1785 2024-01-11 10:54:02.716905 trickkiste-0.0.7/trickkiste/examples/fancytui.py
--rw-r--r--   0        0        0     3588 2024-02-08 08:49:35.260768 trickkiste-0.0.7/trickkiste/logging_helper.py
--rw-r--r--   0        0        0     3923 2024-02-08 08:30:20.042578 trickkiste-0.0.7/trickkiste/misc.py
--rw-r--r--   0        0        0        0 2024-01-11 10:54:02.716905 trickkiste-0.0.7/trickkiste/py.typed
--rwxr-xr-x   0        0        0     2293 2024-01-11 10:54:02.716905 trickkiste-0.0.7/trickkiste/std_suppress.py
--rw-r--r--   0        0        0     1188 1970-01-01 00:00:00.000000 trickkiste-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      676 2023-12-10 05:33:15.492574 trickkiste-0.0.8/Readme.md
+-rw-r--r--   0        0        0     1563 2024-03-20 15:20:10.709973 trickkiste-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-11 10:54:02.708905 trickkiste-0.0.8/trickkiste/__init__.py
+-rw-r--r--   0        0        0       42 2024-01-11 10:54:02.712905 trickkiste-0.0.8/trickkiste/base_tui_app.css
+-rw-r--r--   0        0        0     2982 2024-01-11 10:54:02.712905 trickkiste-0.0.8/trickkiste/base_tui_app.py
+-rwxr-xr-x   0        0        0      978 2024-02-08 08:51:43.258359 trickkiste-0.0.8/trickkiste/examples/fancylogging.py
+-rwxr-xr-x   0        0        0     1785 2024-01-11 10:54:02.716905 trickkiste-0.0.8/trickkiste/examples/fancytui.py
+-rw-r--r--   0        0        0     3588 2024-02-08 08:49:35.260768 trickkiste-0.0.8/trickkiste/logging_helper.py
+-rw-r--r--   0        0        0     5678 2024-03-20 15:13:42.588026 trickkiste-0.0.8/trickkiste/misc.py
+-rw-r--r--   0        0        0        0 2024-01-11 10:54:02.716905 trickkiste-0.0.8/trickkiste/py.typed
+-rwxr-xr-x   0        0        0     2293 2024-01-11 10:54:02.716905 trickkiste-0.0.8/trickkiste/std_suppress.py
+-rw-r--r--   0        0        0     1188 1970-01-01 00:00:00.000000 trickkiste-0.0.8/PKG-INFO
```

### Comparing `trickkiste-0.0.7/Readme.md` & `trickkiste-0.0.8/Readme.md`

 * *Files identical despite different names*

### Comparing `trickkiste-0.0.7/pyproject.toml` & `trickkiste-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trickkiste"
-version = "0.0.7"
+version = "0.0.8"
 description = "Random useful stuff"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/trickkiste.git"
 readme = "Readme.md"
 packages = [
   {include = "trickkiste"},
   # {include = "trickkiste/py.typed"},
```

### Comparing `trickkiste-0.0.7/trickkiste/base_tui_app.py` & `trickkiste-0.0.8/trickkiste/base_tui_app.py`

 * *Files identical despite different names*

### Comparing `trickkiste-0.0.7/trickkiste/examples/fancylogging.py` & `trickkiste-0.0.8/trickkiste/examples/fancylogging.py`

 * *Files identical despite different names*

### Comparing `trickkiste-0.0.7/trickkiste/examples/fancytui.py` & `trickkiste-0.0.8/trickkiste/examples/fancytui.py`

 * *Files identical despite different names*

### Comparing `trickkiste-0.0.7/trickkiste/logging_helper.py` & `trickkiste-0.0.8/trickkiste/logging_helper.py`

 * *Files identical despite different names*

### Comparing `trickkiste-0.0.7/trickkiste/std_suppress.py` & `trickkiste-0.0.8/trickkiste/std_suppress.py`

 * *Files identical despite different names*

### Comparing `trickkiste-0.0.7/PKG-INFO` & `trickkiste-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trickkiste
-Version: 0.0.7
+Version: 0.0.8
 Summary: Random useful stuff
 Home-page: https://projects.om-office.de/frans/trickkiste.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.10.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

