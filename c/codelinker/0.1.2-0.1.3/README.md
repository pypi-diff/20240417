# Comparing `tmp/codelinker-0.1.2.tar.gz` & `tmp/codelinker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codelinker-0.1.2.tar", max compression
+gzip compressed data, was "codelinker-0.1.3.tar", max compression
```

## Comparing `codelinker-0.1.2.tar` & `codelinker-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-04-13 16:27:28.302541 codelinker-0.1.2/LICENSE
--rw-r--r--   0        0        0     1968 2024-04-13 16:27:28.302541 codelinker-0.1.2/README.md
--rw-r--r--   0        0        0     1584 2024-04-13 16:27:28.302541 codelinker-0.1.2/codelinker/__init__.py
--rw-r--r--   0        0        0     3249 2024-04-13 16:27:28.302541 codelinker-0.1.2/codelinker/config.py
--rw-r--r--   0        0        0     8283 2024-04-13 16:27:28.302541 codelinker-0.1.2/codelinker/linker.py
--rw-r--r--   0        0        0       64 2024-04-13 16:27:28.302541 codelinker-0.1.2/codelinker/models/__init__.py
--rw-r--r--   0        0        0      273 2024-04-13 16:27:28.302541 codelinker-0.1.2/codelinker/models/labels.py
--rw-r--r--   0        0        0      308 2024-04-13 16:27:28.302541 codelinker-0.1.2/codelinker/models/structuredRet.py
--rw-r--r--   0        0        0       32 2024-04-13 16:27:28.302541 codelinker-0.1.2/codelinker/request/__init__.py
--rw-r--r--   0        0        0    11665 2024-04-13 16:27:28.302541 codelinker-0.1.2/codelinker/request/objGen.py
--rw-r--r--   0        0        0     5086 2024-04-13 16:27:28.302541 codelinker-0.1.2/codelinker/request/openai.py
--rw-r--r--   0        0        0     1510 2024-04-13 16:27:28.302541 codelinker-0.1.2/codelinker/utils.py
--rw-r--r--   0        0        0      359 2024-04-13 16:27:28.302541 codelinker-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 codelinker-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-17 07:20:29.996021 codelinker-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1968 2024-04-17 07:20:29.996021 codelinker-0.1.3/README.md
+-rw-r--r--   0        0        0     1584 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/__init__.py
+-rw-r--r--   0        0        0     3249 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/config.py
+-rw-r--r--   0        0        0     8412 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/linker.py
+-rw-r--r--   0        0        0       64 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/models/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/models/labels.py
+-rw-r--r--   0        0        0      308 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/models/structuredRet.py
+-rw-r--r--   0        0        0       32 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/request/__init__.py
+-rw-r--r--   0        0        0    11665 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/request/objGen.py
+-rw-r--r--   0        0        0     5086 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/request/openai.py
+-rw-r--r--   0        0        0     1510 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/utils.py
+-rw-r--r--   0        0        0      359 2024-04-17 07:20:29.996021 codelinker-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 codelinker-0.1.3/PKG-INFO
```

### Comparing `codelinker-0.1.2/LICENSE` & `codelinker-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.2/README.md` & `codelinker-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.2/codelinker/__init__.py` & `codelinker-0.1.3/codelinker/__init__.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.2/codelinker/config.py` & `codelinker-0.1.3/codelinker/config.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.2/codelinker/linker.py` & `codelinker-0.1.3/codelinker/linker.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,21 +99,23 @@
                 prompt=prompt,
                 completions_kwargs=completions_kwargs,
             )
             setattr(func, "__smart_function_label__", label)
 
             @wraps(func)
             async def wrapper(
+                *args,
                 images:list = [],
                 messages:list = [],
                 tools: list[StructureSchema] = [],
                 tool_choice:dict = None,
                 reply_format: StructureSchema = None,
-                *args,
                 **kwargs):
+                if len(args) > 0:
+                    raise RuntimeError("Smart functions should not have positional arguments")
                 
                 label: SmartFuncLabel = getattr(func, "__smart_function_label__")
                 self.logger.log(10, f"Executing function: {label.name}")
                 
                 if len(args) > 0:
                     raise ValueError("Smart functions should not have positional arguments")
```

### Comparing `codelinker-0.1.2/codelinker/request/objGen.py` & `codelinker-0.1.3/codelinker/request/objGen.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.2/codelinker/request/openai.py` & `codelinker-0.1.3/codelinker/request/openai.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.2/codelinker/utils.py` & `codelinker-0.1.3/codelinker/utils.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.2/PKG-INFO` & `codelinker-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codelinker
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: luyaxi
 Author-email: luyaxi@live.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

