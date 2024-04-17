# Comparing `tmp/libretto_openai-1.0.2.tar.gz` & `tmp/libretto_openai-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretto_openai-1.0.2.tar", max compression
+gzip compressed data, was "libretto_openai-1.0.3.tar", max compression
```

## Comparing `libretto_openai-1.0.2.tar` & `libretto_openai-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1069 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/LICENSE
--rw-r--r--   0        0        0     9580 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/README.md
--rw-r--r--   0        0        0      400 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/__init__.py
--rw-r--r--   0        0        0     3497 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/background.py
--rw-r--r--   0        0        0     1660 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/client.py
--rw-r--r--   0        0        0    58115 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/completions.py
--rw-r--r--   0        0        0     9866 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/completions_impl.py
--rw-r--r--   0        0        0      208 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/pii/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/pii/data/__init__.py
--rw-r--r--   0        0        0   167435 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/pii/data/names.json
--rw-r--r--   0        0        0     1117 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/pii/data/names.json.LICENSE
--rw-r--r--   0        0        0     4296 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/pii/name_recognizer.py
--rw-r--r--   0        0        0      949 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/pii/nlp.py
--rw-r--r--   0        0        0     1298 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/pii/redactor.py
--rw-r--r--   0        0        0     2722 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/pii/street_address_recognizer.py
--rw-r--r--   0        0        0        0 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/py.typed
--rw-r--r--   0        0        0     8088 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/session.py
--rw-r--r--   0        0        0     1345 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/template.py
--rw-r--r--   0        0        0     1733 2024-01-11 21:22:13.544185 libretto_openai-1.0.2/libretto_openai/types.py
--rw-r--r--   0        0        0      813 2024-01-11 21:22:13.548185 libretto_openai-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    10270 1970-01-01 00:00:00.000000 libretto_openai-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      150 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/AUTHORS.rst
+-rw-r--r--   0        0        0     1069 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/LICENSE
+-rw-r--r--   0        0        0     9580 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/README.md
+-rw-r--r--   0        0        0      400 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/__init__.py
+-rw-r--r--   0        0        0     3497 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/background.py
+-rw-r--r--   0        0        0     1660 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/client.py
+-rw-r--r--   0        0        0    58115 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/completions.py
+-rw-r--r--   0        0        0     9866 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/completions_impl.py
+-rw-r--r--   0        0        0      208 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/pii/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/pii/data/__init__.py
+-rw-r--r--   0        0        0   167435 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/pii/data/names.json
+-rw-r--r--   0        0        0     1117 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/pii/data/names.json.LICENSE
+-rw-r--r--   0        0        0     4296 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/pii/name_recognizer.py
+-rw-r--r--   0        0        0      949 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/pii/nlp.py
+-rw-r--r--   0        0        0     1298 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/pii/redactor.py
+-rw-r--r--   0        0        0     2722 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/pii/street_address_recognizer.py
+-rw-r--r--   0        0        0        0 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/py.typed
+-rw-r--r--   0        0        0     8088 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/session.py
+-rw-r--r--   0        0        0     3182 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/template.py
+-rw-r--r--   0        0        0     1733 2024-04-17 19:11:27.776159 libretto_openai-1.0.3/libretto_openai/types.py
+-rw-r--r--   0        0        0      813 2024-04-17 19:11:27.780159 libretto_openai-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10270 1970-01-01 00:00:00.000000 libretto_openai-1.0.3/PKG-INFO
```

### Comparing `libretto_openai-1.0.2/LICENSE` & `libretto_openai-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/README.md` & `libretto_openai-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/libretto_openai/background.py` & `libretto_openai-1.0.3/libretto_openai/background.py`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/libretto_openai/client.py` & `libretto_openai-1.0.3/libretto_openai/client.py`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/libretto_openai/completions.py` & `libretto_openai-1.0.3/libretto_openai/completions.py`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/libretto_openai/completions_impl.py` & `libretto_openai-1.0.3/libretto_openai/completions_impl.py`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/libretto_openai/pii/data/names.json` & `libretto_openai-1.0.3/libretto_openai/pii/data/names.json`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/libretto_openai/pii/data/names.json.LICENSE` & `libretto_openai-1.0.3/libretto_openai/pii/data/names.json.LICENSE`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/libretto_openai/pii/name_recognizer.py` & `libretto_openai-1.0.3/libretto_openai/pii/name_recognizer.py`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/libretto_openai/pii/nlp.py` & `libretto_openai-1.0.3/libretto_openai/pii/nlp.py`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/libretto_openai/pii/redactor.py` & `libretto_openai-1.0.3/libretto_openai/pii/redactor.py`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/libretto_openai/pii/street_address_recognizer.py` & `libretto_openai-1.0.3/libretto_openai/pii/street_address_recognizer.py`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/libretto_openai/session.py` & `libretto_openai-1.0.3/libretto_openai/session.py`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/libretto_openai/types.py` & `libretto_openai-1.0.3/libretto_openai/types.py`

 * *Files identical despite different names*

### Comparing `libretto_openai-1.0.2/pyproject.toml` & `libretto_openai-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 line-length = 100
 target_version = ['py311']
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "libretto-openai"
-version = "1.0.2"
+version = "1.0.3"
 description = "Wrapper library for openai to send events to Libretto"
 authors = ["Alec Flett <alecf@thegp.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `libretto_openai-1.0.2/PKG-INFO` & `libretto_openai-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretto-openai
-Version: 1.0.2
+Version: 1.0.3
 Summary: Wrapper library for openai to send events to Libretto
 License: MIT
 Author: Alec Flett
 Author-email: alecf@thegp.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

