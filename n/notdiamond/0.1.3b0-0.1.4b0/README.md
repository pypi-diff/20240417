# Comparing `tmp/notdiamond-0.1.3b0.tar.gz` & `tmp/notdiamond-0.1.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notdiamond-0.1.3b0.tar", max compression
+gzip compressed data, was "notdiamond-0.1.4b0.tar", max compression
```

## Comparing `notdiamond-0.1.3b0.tar` & `notdiamond-0.1.4b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4667 2024-04-09 10:12:26.438700 notdiamond-0.1.3b0/README.md
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.001993 notdiamond-0.1.3b0/notdiamond/__init__.py
--rw-r--r--   0        0        0      440 2024-04-02 07:43:11.002696 notdiamond-0.1.3b0/notdiamond/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.002740 notdiamond-0.1.3b0/notdiamond/llms/__init__.py
--rw-r--r--   0        0        0    31309 2024-04-16 07:37:25.829978 notdiamond-0.1.3b0/notdiamond/llms/llm.py
--rw-r--r--   0        0        0     4432 2024-04-13 12:29:10.520716 notdiamond-0.1.3b0/notdiamond/llms/provider.py
--rw-r--r--   0        0        0     3638 2024-04-16 07:39:04.865174 notdiamond-0.1.3b0/notdiamond/llms/providers.py
--rw-r--r--   0        0        0    11540 2024-04-13 13:31:19.751412 notdiamond-0.1.3b0/notdiamond/llms/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004168 notdiamond-0.1.3b0/notdiamond/metrics/__init__.py
--rw-r--r--   0        0        0     1155 2024-04-02 11:25:39.891484 notdiamond-0.1.3b0/notdiamond/metrics/metric.py
--rw-r--r--   0        0        0     1100 2024-04-06 09:04:10.351693 notdiamond-0.1.3b0/notdiamond/metrics/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004898 notdiamond-0.1.3b0/notdiamond/prompts/__init__.py
--rw-r--r--   0        0        0      147 2024-04-02 07:43:11.005796 notdiamond-0.1.3b0/notdiamond/prompts/hash.py
--rw-r--r--   0        0        0     7782 2024-04-06 09:04:10.351913 notdiamond-0.1.3b0/notdiamond/prompts/prompt.py
--rw-r--r--   0        0        0     1933 2024-04-16 07:39:04.865490 notdiamond-0.1.3b0/notdiamond/settings.py
--rw-r--r--   0        0        0      972 2024-04-02 07:43:11.007948 notdiamond-0.1.3b0/notdiamond/types.py
--rw-r--r--   0        0        0     1458 2024-04-16 16:10:20.724515 notdiamond-0.1.3b0/pyproject.toml
--rw-r--r--   0        0        0     5779 1970-01-01 00:00:00.000000 notdiamond-0.1.3b0/PKG-INFO
+-rw-r--r--   0        0        0     4667 2024-04-09 10:12:26.438700 notdiamond-0.1.4b0/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.001993 notdiamond-0.1.4b0/notdiamond/__init__.py
+-rw-r--r--   0        0        0      440 2024-04-02 07:43:11.002696 notdiamond-0.1.4b0/notdiamond/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.002740 notdiamond-0.1.4b0/notdiamond/llms/__init__.py
+-rw-r--r--   0        0        0    31309 2024-04-16 19:47:33.493476 notdiamond-0.1.4b0/notdiamond/llms/llm.py
+-rw-r--r--   0        0        0     4432 2024-04-13 12:29:10.520716 notdiamond-0.1.4b0/notdiamond/llms/provider.py
+-rw-r--r--   0        0        0     3638 2024-04-16 07:39:04.865174 notdiamond-0.1.4b0/notdiamond/llms/providers.py
+-rw-r--r--   0        0        0    11540 2024-04-13 13:31:19.751412 notdiamond-0.1.4b0/notdiamond/llms/request.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004168 notdiamond-0.1.4b0/notdiamond/metrics/__init__.py
+-rw-r--r--   0        0        0     1155 2024-04-02 11:25:39.891484 notdiamond-0.1.4b0/notdiamond/metrics/metric.py
+-rw-r--r--   0        0        0     1100 2024-04-06 09:04:10.351693 notdiamond-0.1.4b0/notdiamond/metrics/request.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004898 notdiamond-0.1.4b0/notdiamond/prompts/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-02 07:43:11.005796 notdiamond-0.1.4b0/notdiamond/prompts/hash.py
+-rw-r--r--   0        0        0     7782 2024-04-06 09:04:10.351913 notdiamond-0.1.4b0/notdiamond/prompts/prompt.py
+-rw-r--r--   0        0        0     1933 2024-04-16 07:39:04.865490 notdiamond-0.1.4b0/notdiamond/settings.py
+-rw-r--r--   0        0        0      972 2024-04-02 07:43:11.007948 notdiamond-0.1.4b0/notdiamond/types.py
+-rw-r--r--   0        0        0     1458 2024-04-16 19:47:37.808413 notdiamond-0.1.4b0/pyproject.toml
+-rw-r--r--   0        0        0     5779 1970-01-01 00:00:00.000000 notdiamond-0.1.4b0/PKG-INFO
```

### Comparing `notdiamond-0.1.3b0/README.md` & `notdiamond-0.1.4b0/README.md`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.3b0/notdiamond/llms/llm.py` & `notdiamond-0.1.4b0/notdiamond/llms/llm.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.3b0/notdiamond/llms/provider.py` & `notdiamond-0.1.4b0/notdiamond/llms/provider.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.3b0/notdiamond/llms/providers.py` & `notdiamond-0.1.4b0/notdiamond/llms/providers.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.3b0/notdiamond/llms/request.py` & `notdiamond-0.1.4b0/notdiamond/llms/request.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.3b0/notdiamond/metrics/metric.py` & `notdiamond-0.1.4b0/notdiamond/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.3b0/notdiamond/metrics/request.py` & `notdiamond-0.1.4b0/notdiamond/metrics/request.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.3b0/notdiamond/prompts/prompt.py` & `notdiamond-0.1.4b0/notdiamond/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.3b0/notdiamond/settings.py` & `notdiamond-0.1.4b0/notdiamond/settings.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.3b0/notdiamond/types.py` & `notdiamond-0.1.4b0/notdiamond/types.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.3b0/pyproject.toml` & `notdiamond-0.1.4b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notdiamond"
-version = "0.1.3-beta"
+version = "0.1.4-beta"
 description = "Not Diamond Python Library"
 authors = ["Not Diamond <t5@notdiamond.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 langchain = ">=0.1.10"
```

### Comparing `notdiamond-0.1.3b0/PKG-INFO` & `notdiamond-0.1.4b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notdiamond
-Version: 0.1.3b0
+Version: 0.1.4b0
 Summary: Not Diamond Python Library
 Author: Not Diamond
 Author-email: t5@notdiamond.ai
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

