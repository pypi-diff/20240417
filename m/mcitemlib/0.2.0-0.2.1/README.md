# Comparing `tmp/mcitemlib-0.2.0.tar.gz` & `tmp/mcitemlib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcitemlib-0.2.0.tar", max compression
+gzip compressed data, was "mcitemlib-0.2.1.tar", max compression
```

## Comparing `mcitemlib-0.2.0.tar` & `mcitemlib-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2024-03-20 01:07:11.643195 mcitemlib-0.2.0/LICENSE
--rw-r--r--   0        0        0      599 2024-03-22 02:04:24.820036 mcitemlib-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-20 01:07:11.643195 mcitemlib-0.2.0/mcitemlib/__init__.py
--rw-r--r--   0        0        0    17725 2024-04-16 14:00:32.162781 mcitemlib-0.2.0/mcitemlib/itemlib.py
--rw-r--r--   0        0        0     8053 2024-04-15 15:23:13.976056 mcitemlib-0.2.0/mcitemlib/style.py
--rw-r--r--   0        0        0      432 2024-04-16 14:06:02.895928 mcitemlib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 mcitemlib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-03-20 01:07:11.643195 mcitemlib-0.2.1/LICENSE
+-rw-r--r--   0        0        0      599 2024-03-22 02:04:24.820036 mcitemlib-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 01:07:11.643195 mcitemlib-0.2.1/mcitemlib/__init__.py
+-rw-r--r--   0        0        0    17709 2024-04-16 14:37:33.570484 mcitemlib-0.2.1/mcitemlib/itemlib.py
+-rw-r--r--   0        0        0     8073 2024-04-16 14:37:33.570484 mcitemlib-0.2.1/mcitemlib/style.py
+-rw-r--r--   0        0        0      432 2024-04-16 14:36:47.450324 mcitemlib-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 mcitemlib-0.2.1/PKG-INFO
```

### Comparing `mcitemlib-0.2.0/LICENSE` & `mcitemlib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mcitemlib-0.2.0/README.md` & `mcitemlib-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mcitemlib-0.2.0/mcitemlib/itemlib.py` & `mcitemlib-0.2.1/mcitemlib/itemlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import json
 import time
 import socket
 import websocket
 import nbtlib
 from typing import List, Literal
-from mcitemlib.style import StyledString, ampersand_to_section_format, snake_to_capitalized, PyNbtStyleException
+from mcitemlib.style import StyledString, ampersand_to_section_format, snake_to_capitalized, McItemlibStyleException
 
 
 BOOK_ITEMS = {
     'minecraft:writable_book',
     'minecraft:written_book'
 }
 
@@ -135,20 +135,19 @@
             'Count': count,
         })
         if item_id == 'written_book':
             self.nbt['tag']['author'] = 'pynbt'
             self.nbt['tag']['title'] = 'Written Book'
     
 
-    @staticmethod
-    def from_nbt(nbt: str):
-        i = Item('stone')
-        print(nbtlib.parse_nbt(nbt))
-        nbt = convert_nbt_tag(nbtlib.parse_nbt(nbt))
-        i.nbt = nbt
+    @classmethod
+    def from_nbt(cls, nbt: str):
+        i = cls('stone')
+        nbt_dict = convert_nbt_tag(nbtlib.parse_nbt(nbt))
+        i.nbt = nbt_dict
         return i
     
 
     def __repr__(self):
         return f'Item({self.nbt.__repr__()})'
     
 
@@ -574,10 +573,10 @@
     elif isinstance(nbt_tag, nbtlib.List):
         return [convert_nbt_tag(t) for t in nbt_tag]
     elif isinstance(nbt_tag, nbtlib.Numeric):
         return _TypedInt(nbt_tag.unpack(), nbt_tag.suffix)
     elif isinstance(nbt_tag, nbtlib.String):
         try:
             return StyledString.from_nbt(nbt_tag.unpack())
-        except PyNbtStyleException:
+        except McItemlibStyleException:
             return nbt_tag.unpack()
     return nbt_tag.unpack()
```

### Comparing `mcitemlib-0.2.0/mcitemlib/style.py` & `mcitemlib-0.2.1/mcitemlib/style.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import re
 import json
 from typing import List, Any
 
 
-class PyNbtStyleException(Exception):
+class McItemlibStyleException(Exception):
     pass
 
 STYLE_CODE_REGEX = r'(&([0-9A-Fa-fklmnorKLMNOR]|x&[0-9A-Fa-f]&[0-9A-Fa-f]&[0-9A-Fa-f]&[0-9A-Fa-f]&[0-9A-Fa-f]&[0-9A-Fa-f]))+'
 
 COLOR_CODES = {
     '0': 'black',
     '1': 'dark_blue',
@@ -149,15 +149,15 @@
                 sub.data[FORMAT_CODES[c]] = True
             elif c == 'r':
                 sub.reset()
             elif c == 'x':
                 sub.data['color'] = f'#{raw_code[i+1:i+7].upper()}'
                 i += 6
             else:
-                raise PyNbtStyleException(f'Unexpected format character "{c}" found in substring.')
+                raise McItemlibStyleException(f'Unexpected format character "{c}" found in substring.')
             i += 1
         return sub
     
 
     @staticmethod
     def from_nbt(nbt: str|dict):
         style_data = nbt
@@ -240,29 +240,29 @@
 
     @staticmethod
     def from_nbt(nbt: str):
         try:
             nbt_dict = json.loads(nbt)
             if 'text' in nbt_dict:
                 return StyledString.from_nbt_dict(nbt_dict)
-            raise PyNbtStyleException('String is not a formatted styled string.')
+            raise McItemlibStyleException('String is not a formatted styled string.')
         except json.JSONDecodeError:
-            raise PyNbtStyleException('Invalid JSON string.')
+            raise McItemlibStyleException('Invalid JSON string.')
         
 
     def to_string(self) -> str:
         """
         Returns an unformatted representation of this string.
         """
         return ''.join([sub.data['text'] for sub in self.substrings])
     
 
     def format(self):
         amount_substrings = len(self.substrings)
         if amount_substrings == 0:
-            raise PyNbtStyleException('Cannot format styled string without any substrings.')
+            raise McItemlibStyleException('Cannot format styled string without any substrings.')
         if amount_substrings == 1:
             return self.substrings[0].format()
 
         formatted_substrings = [s.format() for s in self.substrings]
         extra = ','.join(formatted_substrings)
         return f'{{"extra":[{extra}],"text":""}}'
```

### Comparing `mcitemlib-0.2.0/PKG-INFO` & `mcitemlib-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcitemlib
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library for creating and editing Minecraft items using python.
 Home-page: https://github.com/Amp63/mcitemlib
 License: MIT
 Keywords: minecraft,item,block,nbt
 Author: Amp
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

