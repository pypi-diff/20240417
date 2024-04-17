# Comparing `tmp/kimchima-0.4.5.tar.gz` & `tmp/kimchima-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimchima-0.4.5.tar", max compression
+gzip compressed data, was "kimchima-0.4.7.tar", max compression
```

## Comparing `kimchima-0.4.5.tar` & `kimchima-0.4.7.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0    11343 2024-04-15 10:18:14.173492 kimchima-0.4.5/LICENSE
--rw-r--r--   0        0        0      908 2024-04-15 10:18:14.173492 kimchima-0.4.5/README.md
--rw-r--r--   0        0        0     2595 2024-04-15 10:18:14.177492 kimchima-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1160 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/__init__.py
--rw-r--r--   0        0        0      684 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/chat_template/__init__.py
--rw-r--r--   0        0        0     1844 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/chat_template/chat_template_factory.py
--rw-r--r--   0        0        0        0 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/cmds/__init__.py
--rw-r--r--   0        0        0     1566 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/cmds/auto_cli.py
--rw-r--r--   0        0        0     1344 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/cmds/kimchima_cli.py
--rw-r--r--   0        0        0        0 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/models/__init__.py
--rw-r--r--   0        0        0      674 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pipelines/__init__.py
--rw-r--r--   0        0        0     2347 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pipelines/pipelines_factory.py
--rw-r--r--   0        0        0     1015 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/__init__.py
--rw-r--r--   0        0        0     1598 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/devices.py
--rw-r--r--   0        0        0     3222 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/embedding_factory.py
--rw-r--r--   0        0        0     5564 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/logging.py
--rw-r--r--   0        0        0     4727 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/model_factory.py
--rw-r--r--   0        0        0     1838 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/quantization_factory.py
--rw-r--r--   0        0        0     2735 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/streamer_factory.py
--rw-r--r--   0        0        0     3558 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/tokenizer_factory.py
--rw-r--r--   0        0        0        0 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/__init__.py
--rw-r--r--   0        0        0     1966 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/test_chat.py
--rw-r--r--   0        0        0     2290 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/test_chat_template_factory.py
--rw-r--r--   0        0        0     1818 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/test_devices.py
--rw-r--r--   0        0        0     2032 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/test_embedding_factory.py
--rw-r--r--   0        0        0     2509 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/test_pipelines_factory.py
--rw-r--r--   0        0        0     1084 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/test_quantization_factory.py
--rw-r--r--   0        0        0      702 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/utils/__init__.py
--rw-r--r--   0        0        0     1817 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/utils/chat.py
--rw-r--r--   0        0        0     1384 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/utils/downloader.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 kimchima-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-17 14:44:32.421839 kimchima-0.4.7/LICENSE
+-rw-r--r--   0        0        0      908 2024-04-17 14:44:32.421839 kimchima-0.4.7/README.md
+-rw-r--r--   0        0        0     2595 2024-04-17 14:44:32.421839 kimchima-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     1160 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/__init__.py
+-rw-r--r--   0        0        0      684 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/chat_template/__init__.py
+-rw-r--r--   0        0        0     1844 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/chat_template/chat_template_factory.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/cmds/__init__.py
+-rw-r--r--   0        0        0     1566 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/cmds/auto_cli.py
+-rw-r--r--   0        0        0     1344 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/cmds/kimchima_cli.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/models/__init__.py
+-rw-r--r--   0        0        0      674 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/pipelines/__init__.py
+-rw-r--r--   0        0        0     2347 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/pipelines/pipelines_factory.py
+-rw-r--r--   0        0        0     1015 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/pkg/__init__.py
+-rw-r--r--   0        0        0     1598 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/pkg/devices.py
+-rw-r--r--   0        0        0     3222 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/pkg/embedding_factory.py
+-rw-r--r--   0        0        0     5564 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/pkg/logging.py
+-rw-r--r--   0        0        0     4712 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/pkg/model_factory.py
+-rw-r--r--   0        0        0     1838 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/pkg/quantization_factory.py
+-rw-r--r--   0        0        0     2735 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/pkg/streamer_factory.py
+-rw-r--r--   0        0        0     3558 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/pkg/tokenizer_factory.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/__init__.py
+-rw-r--r--   0        0        0     1966 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_chat.py
+-rw-r--r--   0        0        0     2290 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_chat_template_factory.py
+-rw-r--r--   0        0        0     1818 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_devices.py
+-rw-r--r--   0        0        0     3587 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_downloadr.py
+-rw-r--r--   0        0        0     2032 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_embedding_factory.py
+-rw-r--r--   0        0        0     2509 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_pipelines_factory.py
+-rw-r--r--   0        0        0     1084 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_quantization_factory.py
+-rw-r--r--   0        0        0      702 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/utils/__init__.py
+-rw-r--r--   0        0        0     1817 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/utils/chat.py
+-rw-r--r--   0        0        0     4024 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/utils/downloader.py
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 kimchima-0.4.7/PKG-INFO
```

### Comparing `kimchima-0.4.5/LICENSE` & `kimchima-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/README.md` & `kimchima-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/pyproject.toml` & `kimchima-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kimchima"
-version = "0.4.5"
+version = "0.4.7"
 description = "The collections of tools for ML model development."
 authors = ["Aisuko <urakiny@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Aisuko/kimchi"
 repository = "https://github.com/Aisuko/kimchi"
 keywords = ["transformers", "pytorch"]
```

### Comparing `kimchima-0.4.5/src/kimchima/__init__.py` & `kimchima-0.4.7/src/kimchima/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/chat_template/__init__.py` & `kimchima-0.4.7/src/kimchima/chat_template/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/chat_template/chat_template_factory.py` & `kimchima-0.4.7/src/kimchima/chat_template/chat_template_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/cmds/auto_cli.py` & `kimchima-0.4.7/src/kimchima/cmds/auto_cli.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/cmds/kimchima_cli.py` & `kimchima-0.4.7/src/kimchima/cmds/kimchima_cli.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/pipelines/__init__.py` & `kimchima-0.4.7/src/kimchima/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/pipelines/pipelines_factory.py` & `kimchima-0.4.7/src/kimchima/pipelines/pipelines_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/pkg/__init__.py` & `kimchima-0.4.7/src/kimchima/pkg/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/pkg/devices.py` & `kimchima-0.4.7/src/kimchima/pkg/devices.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/pkg/embedding_factory.py` & `kimchima-0.4.7/src/kimchima/pkg/embedding_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/pkg/logging.py` & `kimchima-0.4.7/src/kimchima/pkg/logging.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/pkg/quantization_factory.py` & `kimchima-0.4.7/src/kimchima/pkg/quantization_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/pkg/streamer_factory.py` & `kimchima-0.4.7/src/kimchima/pkg/streamer_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/pkg/tokenizer_factory.py` & `kimchima-0.4.7/src/kimchima/pkg/tokenizer_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/tests/test_chat.py` & `kimchima-0.4.7/src/kimchima/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/tests/test_chat_template_factory.py` & `kimchima-0.4.7/src/kimchima/tests/test_chat_template_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/tests/test_devices.py` & `kimchima-0.4.7/src/kimchima/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/tests/test_embedding_factory.py` & `kimchima-0.4.7/src/kimchima/tests/test_embedding_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/tests/test_pipelines_factory.py` & `kimchima-0.4.7/src/kimchima/tests/test_pipelines_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/tests/test_quantization_factory.py` & `kimchima-0.4.7/src/kimchima/tests/test_quantization_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/utils/__init__.py` & `kimchima-0.4.7/src/kimchima/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/src/kimchima/utils/chat.py` & `kimchima-0.4.7/src/kimchima/utils/chat.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.5/PKG-INFO` & `kimchima-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimchima
-Version: 0.4.5
+Version: 0.4.7
 Summary: The collections of tools for ML model development.
 Home-page: https://github.com/Aisuko/kimchi
 License: Apache-2.0
 Keywords: transformers,pytorch
 Author: Aisuko
 Author-email: urakiny@gmail.com
 Requires-Python: >=3.11,<4.0
```

