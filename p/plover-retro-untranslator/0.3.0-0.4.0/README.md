# Comparing `tmp/plover_retro_untranslator-0.3.0.tar.gz` & `tmp/plover_retro_untranslator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plover_retro_untranslator-0.3.0.tar", last modified: Thu Dec 28 05:33:23 2023, max compression
+gzip compressed data, was "dist/plover_retro_untranslator-0.4.0.tar", last modified: Wed Apr 17 11:24:36 2024, max compression
```

## Comparing `plover_retro_untranslator-0.3.0.tar` & `plover_retro_untranslator-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 josiah    (1000) josiah    (1000)        0 2023-12-28 05:33:23.000000 plover_retro_untranslator-0.3.0/
--rw-r--r--   0 josiah    (1000) josiah    (1000)    32406 2023-02-02 10:58:53.000000 plover_retro_untranslator-0.3.0/LICENSE
--rw-r--r--   0 josiah    (1000) josiah    (1000)     3137 2023-12-28 05:33:23.000000 plover_retro_untranslator-0.3.0/PKG-INFO
--rw-r--r--   0 josiah    (1000) josiah    (1000)     2194 2023-12-21 04:50:34.000000 plover_retro_untranslator-0.3.0/README.md
-drwxr-xr-x   0 josiah    (1000) josiah    (1000)        0 2023-12-28 05:33:23.000000 plover_retro_untranslator-0.3.0/plover_retro_untranslator/
--rw-r--r--   0 josiah    (1000) josiah    (1000)     2718 2023-12-28 05:13:58.000000 plover_retro_untranslator-0.3.0/plover_retro_untranslator/__init__.py
-drwxr-xr-x   0 josiah    (1000) josiah    (1000)        0 2023-12-28 05:33:23.000000 plover_retro_untranslator-0.3.0/plover_retro_untranslator.egg-info/
--rw-r--r--   0 josiah    (1000) josiah    (1000)     3137 2023-12-28 05:33:23.000000 plover_retro_untranslator-0.3.0/plover_retro_untranslator.egg-info/PKG-INFO
--rw-r--r--   0 josiah    (1000) josiah    (1000)      414 2023-12-28 05:33:23.000000 plover_retro_untranslator-0.3.0/plover_retro_untranslator.egg-info/SOURCES.txt
--rw-r--r--   0 josiah    (1000) josiah    (1000)        1 2023-12-28 05:33:23.000000 plover_retro_untranslator-0.3.0/plover_retro_untranslator.egg-info/dependency_links.txt
--rw-r--r--   0 josiah    (1000) josiah    (1000)       81 2023-12-28 05:33:23.000000 plover_retro_untranslator-0.3.0/plover_retro_untranslator.egg-info/entry_points.txt
--rw-r--r--   0 josiah    (1000) josiah    (1000)       30 2023-12-28 05:33:23.000000 plover_retro_untranslator-0.3.0/plover_retro_untranslator.egg-info/requires.txt
--rw-r--r--   0 josiah    (1000) josiah    (1000)       26 2023-12-28 05:33:23.000000 plover_retro_untranslator-0.3.0/plover_retro_untranslator.egg-info/top_level.txt
--rw-r--r--   0 josiah    (1000) josiah    (1000)        1 2023-02-02 11:32:47.000000 plover_retro_untranslator-0.3.0/plover_retro_untranslator.egg-info/zip-safe
--rw-r--r--   0 josiah    (1000) josiah    (1000)     1150 2023-12-28 05:33:23.000000 plover_retro_untranslator-0.3.0/setup.cfg
--rw-r--r--   0 josiah    (1000) josiah    (1000)       62 2023-02-02 10:58:53.000000 plover_retro_untranslator-0.3.0/setup.py
+drwxr-xr-x   0 josiah    (1000) josiah    (1000)        0 2024-04-17 11:24:36.806272 plover_retro_untranslator-0.4.0/
+-rw-r--r--   0 josiah    (1000) josiah    (1000)    32406 2024-04-17 10:00:41.000000 plover_retro_untranslator-0.4.0/LICENSE
+-rw-r--r--   0 josiah    (1000) josiah    (1000)     3601 2024-04-17 11:24:36.806272 plover_retro_untranslator-0.4.0/PKG-INFO
+-rw-r--r--   0 josiah    (1000) josiah    (1000)     2598 2024-04-17 11:19:05.000000 plover_retro_untranslator-0.4.0/README.md
+drwxr-xr-x   0 josiah    (1000) josiah    (1000)        0 2024-04-17 11:24:36.806272 plover_retro_untranslator-0.4.0/plover_retro_untranslator/
+-rw-r--r--   0 josiah    (1000) josiah    (1000)     3071 2024-04-17 11:08:50.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator/__init__.py
+-rw-r--r--   0 josiah    (1000) josiah    (1000)     2146 2024-04-17 11:06:45.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator/spelling_converter.py
+drwxr-xr-x   0 josiah    (1000) josiah    (1000)        0 2024-04-17 11:24:36.806272 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/
+-rw-r--r--   0 josiah    (1000) josiah    (1000)     3601 2024-04-17 11:24:36.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/PKG-INFO
+-rw-r--r--   0 josiah    (1000) josiah    (1000)      462 2024-04-17 11:24:36.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/SOURCES.txt
+-rw-r--r--   0 josiah    (1000) josiah    (1000)        1 2024-04-17 11:24:36.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/dependency_links.txt
+-rw-r--r--   0 josiah    (1000) josiah    (1000)       81 2024-04-17 11:24:36.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/entry_points.txt
+-rw-r--r--   0 josiah    (1000) josiah    (1000)       30 2024-04-17 11:24:36.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/requires.txt
+-rw-r--r--   0 josiah    (1000) josiah    (1000)       26 2024-04-17 11:24:36.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/top_level.txt
+-rw-r--r--   0 josiah    (1000) josiah    (1000)        1 2024-04-17 10:02:30.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/zip-safe
+-rw-r--r--   0 josiah    (1000) josiah    (1000)     1150 2024-04-17 11:24:36.810272 plover_retro_untranslator-0.4.0/setup.cfg
+-rw-r--r--   0 josiah    (1000) josiah    (1000)       62 2024-04-17 10:00:41.000000 plover_retro_untranslator-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plover_retro_untranslator-0.3.0/LICENSE` & `plover_retro_untranslator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plover_retro_untranslator-0.3.0/PKG-INFO` & `plover_retro_untranslator-0.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover_retro_untranslator
-Version: 0.3.0
+Version: 0.4.0
 Summary: Converts the last X translations to a specified format consisting of raw steno and/or a translation
 Home-page: https://github.com/Josiah-tan/plover-retro-untranslator
 Author: Josiah-tan
 License: GNU General Public License v3 (GPLv3)
 Keywords: plover
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
@@ -15,29 +15,41 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: plover>=4.0.0.dev8
+Requires-Dist: PyQt5>=5.5
 
 # plover-retro-untranslator
 
-Converts the last X translations to a specified format consisting of raw steno and/or a translation and/or definition ([video](https://www.youtube.com/watch?v=pLYZl5_l0qg))
+- Converts the last X translations to a specified format consisting of any of the following: 
+    - raw steno 
+    - translation 
+    - definition 
+    - american translation
+    - british translation
+
+([video](https://www.youtube.com/watch?v=pLYZl5_l0qg))
 
 
 # Examples
 
 put these into your dictionary:
 
 ```json
 {
-"RA*UD": "=retro_untranslator:`%r`"
-"STRO*EBGD": "=retro_untranslator:`%r` → `%T`"
-"TKAO*EFPBD": "=retro_untranslator:`%r` → `%D`"
+"RA*UD": "=retro_untranslator:`%r`",
+"STRO*EBGD": "=retro_untranslator:`%r` → `%T`",
+"TKAO*EFPBD": "=retro_untranslator:`%r` → `%D`",
+"-P": "=retro_untranslator:%G",
+"SPH-P": "=retro_untranslator:%A",
+"PWR-P: "=retro_untranslator:%B",
 }
 ```
 
 example stroke ⇒ output:
 
 ```
 KWRURPB/RA*UD ⇒ `KWRURPB`
@@ -45,20 +57,23 @@
 KWRURPB/TKAO*EFPBD ⇒ `KWRURPB` → `yes{,}your Honor`
 ```
 
 # Configuration
 
 (literally the same thing as tapey-tape)
 
-| Code | Item          | Example           |
-|:-----|:--------------|:------------------|
-| `%r` | raw steno     | `KWRURPB`         |
-| `%D` | definition    | yes{,}your Honor  |
-| `%T` | translation   | `Yes, your Honor` |
-| `%%` | an actual `%` | `%`               |
+| Code | Item                 | Example             |
+|:-----|:---------------------|:--------------------|
+| `%r` | raw steno            | `KWRURPB`           |
+| `%D` | definition           | yes{,}your Honor    |
+| `%T` | translation          | `Yes, your Honor`   |
+| `%A` | american translation | customize           |
+| `%B` | british translation  | customise           |
+| `%G` | toggle translation   | customise/customize |
+| `%%` | an actual `%`        | `%`                 |
 
 
 
 # Prerequisites
 
 - Download plover and find the executable
 	- see this [website](https://plover.readthedocs.io/en/latest/cli_reference.html) for finding the location of plover depending on which platform you are using (Linux, Windows, etc.)
```

### Comparing `plover_retro_untranslator-0.3.0/README.md` & `plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,55 @@
+Metadata-Version: 2.1
+Name: plover_retro_untranslator
+Version: 0.4.0
+Summary: Converts the last X translations to a specified format consisting of raw steno and/or a translation
+Home-page: https://github.com/Josiah-tan/plover-retro-untranslator
+Author: Josiah-tan
+License: GNU General Public License v3 (GPLv3)
+Keywords: plover
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Plugins
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: plover>=4.0.0.dev8
+Requires-Dist: PyQt5>=5.5
+
 # plover-retro-untranslator
 
-Converts the last X translations to a specified format consisting of raw steno and/or a translation and/or definition ([video](https://www.youtube.com/watch?v=pLYZl5_l0qg))
+- Converts the last X translations to a specified format consisting of any of the following: 
+    - raw steno 
+    - translation 
+    - definition 
+    - american translation
+    - british translation
+
+([video](https://www.youtube.com/watch?v=pLYZl5_l0qg))
 
 
 # Examples
 
 put these into your dictionary:
 
 ```json
 {
-"RA*UD": "=retro_untranslator:`%r`"
-"STRO*EBGD": "=retro_untranslator:`%r` → `%T`"
-"TKAO*EFPBD": "=retro_untranslator:`%r` → `%D`"
+"RA*UD": "=retro_untranslator:`%r`",
+"STRO*EBGD": "=retro_untranslator:`%r` → `%T`",
+"TKAO*EFPBD": "=retro_untranslator:`%r` → `%D`",
+"-P": "=retro_untranslator:%G",
+"SPH-P": "=retro_untranslator:%A",
+"PWR-P: "=retro_untranslator:%B",
 }
 ```
 
 example stroke ⇒ output:
 
 ```
 KWRURPB/RA*UD ⇒ `KWRURPB`
@@ -23,20 +57,23 @@
 KWRURPB/TKAO*EFPBD ⇒ `KWRURPB` → `yes{,}your Honor`
 ```
 
 # Configuration
 
 (literally the same thing as tapey-tape)
 
-| Code | Item          | Example           |
-|:-----|:--------------|:------------------|
-| `%r` | raw steno     | `KWRURPB`         |
-| `%D` | definition    | yes{,}your Honor  |
-| `%T` | translation   | `Yes, your Honor` |
-| `%%` | an actual `%` | `%`               |
+| Code | Item                 | Example             |
+|:-----|:---------------------|:--------------------|
+| `%r` | raw steno            | `KWRURPB`           |
+| `%D` | definition           | yes{,}your Honor    |
+| `%T` | translation          | `Yes, your Honor`   |
+| `%A` | american translation | customize           |
+| `%B` | british translation  | customise           |
+| `%G` | toggle translation   | customise/customize |
+| `%%` | an actual `%`        | `%`                 |
 
 
 
 # Prerequisites
 
 - Download plover and find the executable
 	- see this [website](https://plover.readthedocs.io/en/latest/cli_reference.html) for finding the location of plover depending on which platform you are using (Linux, Windows, etc.)
```

### Comparing `plover_retro_untranslator-0.3.0/plover_retro_untranslator/__init__.py` & `plover_retro_untranslator-0.4.0/plover_retro_untranslator/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 #!/usr/bin/env python
 
 from typing import List
 import itertools
 from plover.translation import Translator, Stroke, Translation
 from plover.formatting import RetroFormatter
 import re
+from plover_retro_untranslator.spelling_converter import SpellingConverter
 
 def flatten(x: List[List]) -> List:
     return list(itertools.chain.from_iterable(x))
 
 SHOW_WHITESPACE = str.maketrans({'\n': '\\n', '\r': '\\r', '\t': '\\t'})
 
 historical_translations = []
 
+spelling_converter = SpellingConverter()
+
 def expandFormatting(format_string, items): 
     # thanks for this rabbit growth!
     def replace(matchobj):
         width, letter = matchobj.groups()
         width = 0 if not width else int(width)
-        return items.get(letter, '').ljust(width)
+        return items.get(letter, '')().ljust(width)
     return re.sub(r'%(\d*)(.)', replace, format_string)
 
 def formatDefined(raw_string):
     processed_string = re.sub("([{}])", r"\\\1", raw_string)
     return processed_string
 
 def extract_number_key(stroke):
@@ -60,15 +63,18 @@
             defined = translated = raw_steno
             print("no available translation")
     else:
         defined = ""
         translated = ""
     
     items = {
-        'r': raw_steno,
-        'T': translated,
-        'D': defined,
-        '%': '%'}
+        'r': lambda: raw_steno,
+        'T': lambda: translated,
+        'D': lambda: defined,
+        'A': lambda: spelling_converter.britishToAmerican(translated),
+        'B': lambda: spelling_converter.americanToBritish(translated),
+        'G': lambda: spelling_converter.toggle(translated),
+        '%': lambda: '%'}
     formatted_result = expandFormatting(formatting, items)
     my_trans = Translation(affected_strokes + [stroke], formatted_result)
     my_trans.replaced = affected_translations
     translator.translate_translation(my_trans)
```

### Comparing `plover_retro_untranslator-0.3.0/setup.cfg` & `plover_retro_untranslator-0.4.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plover_retro_untranslator
-version = 0.3.0
+version = 0.4.0
 keywords = plover
 description = Converts the last X translations to a specified format consisting of raw steno and/or a translation
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Josiah-tan
 license = GNU General Public License v3 (GPLv3)
 url = https://github.com/Josiah-tan/plover-retro-untranslator
```

