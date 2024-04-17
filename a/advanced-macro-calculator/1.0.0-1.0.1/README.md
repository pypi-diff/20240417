# Comparing `tmp/advanced_macro_calculator-1.0.0.tar.gz` & `tmp/advanced_macro_calculator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advanced_macro_calculator-1.0.0.tar", last modified: Wed Apr 17 00:04:54 2024, max compression
+gzip compressed data, was "advanced_macro_calculator-1.0.1.tar", last modified: Wed Apr 17 01:47:35 2024, max compression
```

## Comparing `advanced_macro_calculator-1.0.0.tar` & `advanced_macro_calculator-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-17 00:04:54.857876 advanced_macro_calculator-1.0.0/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1072 2024-04-08 16:15:12.000000 advanced_macro_calculator-1.0.0/LICENSE
--rw-rw-r--   0 laptop    (1000) laptop    (1000)       34 2024-04-16 23:54:21.000000 advanced_macro_calculator-1.0.0/MANIFEST.in
--rw-r--r--   0 laptop    (1000) laptop    (1000)    19928 2024-04-17 00:04:54.857876 advanced_macro_calculator-1.0.0/PKG-INFO
--rw-rw-r--   0 laptop    (1000) laptop    (1000)    19438 2024-04-15 00:52:04.000000 advanced_macro_calculator-1.0.0/README.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-17 00:04:54.857876 advanced_macro_calculator-1.0.0/advanced_macro_calculator/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)        0 2024-04-16 23:30:02.000000 advanced_macro_calculator-1.0.0/advanced_macro_calculator/__init__.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      453 2024-04-16 23:32:44.000000 advanced_macro_calculator-1.0.0/advanced_macro_calculator/__main__.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)    11231 2024-04-16 23:28:34.000000 advanced_macro_calculator-1.0.0/advanced_macro_calculator/calculations.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     7623 2024-04-16 23:20:58.000000 advanced_macro_calculator-1.0.0/advanced_macro_calculator/input_handlers.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     3241 2024-04-16 23:35:22.000000 advanced_macro_calculator-1.0.0/advanced_macro_calculator/outputs.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-17 00:04:54.857876 advanced_macro_calculator-1.0.0/advanced_macro_calculator.egg-info/
--rw-r--r--   0 laptop    (1000) laptop    (1000)    19928 2024-04-17 00:04:54.000000 advanced_macro_calculator-1.0.0/advanced_macro_calculator.egg-info/PKG-INFO
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      495 2024-04-17 00:04:54.000000 advanced_macro_calculator-1.0.0/advanced_macro_calculator.egg-info/SOURCES.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)        1 2024-04-17 00:04:54.000000 advanced_macro_calculator-1.0.0/advanced_macro_calculator.egg-info/dependency_links.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)       86 2024-04-17 00:04:54.000000 advanced_macro_calculator-1.0.0/advanced_macro_calculator.egg-info/entry_points.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)       26 2024-04-17 00:04:54.000000 advanced_macro_calculator-1.0.0/advanced_macro_calculator.egg-info/top_level.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      688 2024-04-17 00:04:54.858877 advanced_macro_calculator-1.0.0/setup.cfg
--rw-rw-r--   0 laptop    (1000) laptop    (1000)       37 2024-04-16 23:53:09.000000 advanced_macro_calculator-1.0.0/setup.py
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-17 01:47:35.670212 advanced_macro_calculator-1.0.1/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     1072 2024-04-08 16:15:12.000000 advanced_macro_calculator-1.0.1/LICENSE
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)       34 2024-04-16 23:54:21.000000 advanced_macro_calculator-1.0.1/MANIFEST.in
+-rw-r--r--   0 laptop    (1000) laptop    (1000)    20395 2024-04-17 01:47:35.670212 advanced_macro_calculator-1.0.1/PKG-INFO
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)    19675 2024-04-17 01:40:56.000000 advanced_macro_calculator-1.0.1/README.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-17 01:47:35.669211 advanced_macro_calculator-1.0.1/advanced_macro_calculator/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)        0 2024-04-16 23:30:02.000000 advanced_macro_calculator-1.0.1/advanced_macro_calculator/__init__.py
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      453 2024-04-16 23:32:44.000000 advanced_macro_calculator-1.0.1/advanced_macro_calculator/__main__.py
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)    11231 2024-04-16 23:28:34.000000 advanced_macro_calculator-1.0.1/advanced_macro_calculator/calculations.py
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     7623 2024-04-16 23:20:58.000000 advanced_macro_calculator-1.0.1/advanced_macro_calculator/input_handlers.py
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     3241 2024-04-16 23:35:22.000000 advanced_macro_calculator-1.0.1/advanced_macro_calculator/outputs.py
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-17 01:47:35.670212 advanced_macro_calculator-1.0.1/advanced_macro_calculator.egg-info/
+-rw-r--r--   0 laptop    (1000) laptop    (1000)    20395 2024-04-17 01:47:35.000000 advanced_macro_calculator-1.0.1/advanced_macro_calculator.egg-info/PKG-INFO
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      495 2024-04-17 01:47:35.000000 advanced_macro_calculator-1.0.1/advanced_macro_calculator.egg-info/SOURCES.txt
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)        1 2024-04-17 01:47:35.000000 advanced_macro_calculator-1.0.1/advanced_macro_calculator.egg-info/dependency_links.txt
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)       86 2024-04-17 01:47:35.000000 advanced_macro_calculator-1.0.1/advanced_macro_calculator.egg-info/entry_points.txt
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)       26 2024-04-17 01:47:35.000000 advanced_macro_calculator-1.0.1/advanced_macro_calculator.egg-info/top_level.txt
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      901 2024-04-17 01:47:35.671212 advanced_macro_calculator-1.0.1/setup.cfg
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)       37 2024-04-16 23:53:09.000000 advanced_macro_calculator-1.0.1/setup.py
```

### Comparing `advanced_macro_calculator-1.0.0/LICENSE` & `advanced_macro_calculator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `advanced_macro_calculator-1.0.0/PKG-INFO` & `advanced_macro_calculator-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: advanced_macro_calculator
-Version: 1.0.0
+Version: 1.0.1
 Summary: An advanced macronutrient and calorie calculator to help achieve desired body composition.
 Author: Michael Trovato
 Author-email: mtrovato@advancedmacrocalculator.com
 License: MIT
+Project-URL: Website, https://advancedmacrocalculator.com
+Project-URL: Source, https://github.com/michael-trovato/advanced-macro-calculator
+Project-URL: Tracker, https://github.com/michael-trovato/advanced-macro-calculator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/advanced-macro-calculator.svg)](https://pypi.org/project/advanced-macro-calculator/)
+ [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
 # Advanced Macro Calculator
 This calculator helps
 you optimize your nutritional intake and body composition by recommending targeted macros and calories tailored to you.
 
 With the tool being diet agnostic, it fits into any individual's diet preference.
 
 It is built on reliable scientific evidence and provides you with personalized advice based on your specific input.
```

### Comparing `advanced_macro_calculator-1.0.0/README.md` & `advanced_macro_calculator-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[![PyPI version](https://badge.fury.io/py/advanced-macro-calculator.svg)](https://pypi.org/project/advanced-macro-calculator/)
+ [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
 # Advanced Macro Calculator
 This calculator helps
 you optimize your nutritional intake and body composition by recommending targeted macros and calories tailored to you.
 
 With the tool being diet agnostic, it fits into any individual's diet preference.
 
 It is built on reliable scientific evidence and provides you with personalized advice based on your specific input.
```

### Comparing `advanced_macro_calculator-1.0.0/advanced_macro_calculator/calculations.py` & `advanced_macro_calculator-1.0.1/advanced_macro_calculator/calculations.py`

 * *Files identical despite different names*

### Comparing `advanced_macro_calculator-1.0.0/advanced_macro_calculator/input_handlers.py` & `advanced_macro_calculator-1.0.1/advanced_macro_calculator/input_handlers.py`

 * *Files identical despite different names*

### Comparing `advanced_macro_calculator-1.0.0/advanced_macro_calculator/outputs.py` & `advanced_macro_calculator-1.0.1/advanced_macro_calculator/outputs.py`

 * *Files identical despite different names*

### Comparing `advanced_macro_calculator-1.0.0/advanced_macro_calculator.egg-info/PKG-INFO` & `advanced_macro_calculator-1.0.1/advanced_macro_calculator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: advanced_macro_calculator
-Version: 1.0.0
+Version: 1.0.1
 Summary: An advanced macronutrient and calorie calculator to help achieve desired body composition.
 Author: Michael Trovato
 Author-email: mtrovato@advancedmacrocalculator.com
 License: MIT
+Project-URL: Website, https://advancedmacrocalculator.com
+Project-URL: Source, https://github.com/michael-trovato/advanced-macro-calculator
+Project-URL: Tracker, https://github.com/michael-trovato/advanced-macro-calculator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/advanced-macro-calculator.svg)](https://pypi.org/project/advanced-macro-calculator/)
+ [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
 # Advanced Macro Calculator
 This calculator helps
 you optimize your nutritional intake and body composition by recommending targeted macros and calories tailored to you.
 
 With the tool being diet agnostic, it fits into any individual's diet preference.
 
 It is built on reliable scientific evidence and provides you with personalized advice based on your specific input.
```

