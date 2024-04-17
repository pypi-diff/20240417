# Comparing `tmp/mcitemlib-0.2.2.tar.gz` & `tmp/mcitemlib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcitemlib-0.2.2.tar", max compression
+gzip compressed data, was "mcitemlib-0.2.3.tar", max compression
```

## Comparing `mcitemlib-0.2.2.tar` & `mcitemlib-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2024-03-20 01:07:11.643195 mcitemlib-0.2.2/LICENSE
--rw-r--r--   0        0        0      599 2024-03-22 02:04:24.820036 mcitemlib-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-03-20 01:07:11.643195 mcitemlib-0.2.2/mcitemlib/__init__.py
--rw-r--r--   0        0        0    17639 2024-04-17 02:17:42.400125 mcitemlib-0.2.2/mcitemlib/itemlib.py
--rw-r--r--   0        0        0     8073 2024-04-16 14:37:33.570484 mcitemlib-0.2.2/mcitemlib/style.py
--rw-r--r--   0        0        0      432 2024-04-17 02:21:34.773809 mcitemlib-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 mcitemlib-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-03-20 01:07:11.643195 mcitemlib-0.2.3/LICENSE
+-rw-r--r--   0        0        0      599 2024-03-22 02:04:24.820036 mcitemlib-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 01:07:11.643195 mcitemlib-0.2.3/mcitemlib/__init__.py
+-rw-r--r--   0        0        0    17651 2024-04-17 02:28:08.906098 mcitemlib-0.2.3/mcitemlib/itemlib.py
+-rw-r--r--   0        0        0     8073 2024-04-16 14:37:33.570484 mcitemlib-0.2.3/mcitemlib/style.py
+-rw-r--r--   0        0        0      432 2024-04-17 02:28:48.594594 mcitemlib-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 mcitemlib-0.2.3/PKG-INFO
```

### Comparing `mcitemlib-0.2.2/LICENSE` & `mcitemlib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mcitemlib-0.2.2/README.md` & `mcitemlib-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mcitemlib-0.2.2/mcitemlib/itemlib.py` & `mcitemlib-0.2.3/mcitemlib/itemlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,22 +473,22 @@
     def get_nbt(self) -> str:
         """
         Returns the raw nbt data of this item as a string.
         """
         return self._format_as_nbt(self.nbt.as_dict())
 
 
-    def send_to_minecraft(self, method: Literal['recode', 'codeclient']) -> int:
+    def send_to_minecraft(self, method: Literal['recode', 'codeclient'], source: str='mcitemlib') -> int:
         """
         Builds this template and sends it to Minecraft automatically.
         
-        :param bool includeTags: If True, include item tags in code blocks. Otherwise omit them.
+        :param str source: The source program from which the item was sent.
         """
         if method == 'recode':
-            return send_recode(self)
+            return send_recode(self, source)
         if method == 'codeclient':
             return send_codeclient(self)
         return -1
 
 
 def send_recode(item: Item, source: str='mcitemlib') -> int:
     """
```

### Comparing `mcitemlib-0.2.2/mcitemlib/style.py` & `mcitemlib-0.2.3/mcitemlib/style.py`

 * *Files identical despite different names*

### Comparing `mcitemlib-0.2.2/PKG-INFO` & `mcitemlib-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcitemlib
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library for creating and editing Minecraft items using python.
 Home-page: https://github.com/Amp63/mcitemlib
 License: MIT
 Keywords: minecraft,item,block,nbt
 Author: Amp
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

