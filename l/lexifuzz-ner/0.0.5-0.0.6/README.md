# Comparing `tmp/lexifuzz_ner-0.0.5.tar.gz` & `tmp/lexifuzz_ner-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexifuzz_ner-0.0.5.tar", max compression
+gzip compressed data, was "lexifuzz_ner-0.0.6.tar", max compression
```

## Comparing `lexifuzz_ner-0.0.5.tar` & `lexifuzz_ner-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1097 2023-09-12 04:08:59.142483 lexifuzz_ner-0.0.5/LICENSE
--rwxr-xr-x   0        0        0     2993 2024-04-17 10:22:18.366558 lexifuzz_ner-0.0.5/README.md
--rwxr-xr-x   0        0        0      640 2024-04-17 10:29:27.097513 lexifuzz_ner-0.0.5/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-09-12 04:29:12.919915 lexifuzz_ner-0.0.5/src/lexifuzz_ner/__init__.py
--rwxr-xr-x   0        0        0     6700 2024-04-17 10:22:18.375566 lexifuzz_ner-0.0.5/src/lexifuzz_ner/ner.py
--rw-r--r--   0        0        0     3718 1970-01-01 00:00:00.000000 lexifuzz_ner-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1097 2023-09-12 04:08:59.142483 lexifuzz_ner-0.0.6/LICENSE
+-rwxr-xr-x   0        0        0     2993 2024-04-17 10:22:18.366558 lexifuzz_ner-0.0.6/README.md
+-rwxr-xr-x   0        0        0      640 2024-04-17 10:41:56.371613 lexifuzz_ner-0.0.6/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-09-12 04:29:12.919915 lexifuzz_ner-0.0.6/src/lexifuzz_ner/__init__.py
+-rwxr-xr-x   0        0        0     6745 2024-04-17 10:41:45.449387 lexifuzz_ner-0.0.6/src/lexifuzz_ner/ner.py
+-rw-r--r--   0        0        0     3718 1970-01-01 00:00:00.000000 lexifuzz_ner-0.0.6/PKG-INFO
```

### Comparing `lexifuzz_ner-0.0.5/LICENSE` & `lexifuzz_ner-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lexifuzz_ner-0.0.5/README.md` & `lexifuzz_ner-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lexifuzz_ner-0.0.5/pyproject.toml` & `lexifuzz_ner-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "lexifuzz-ner"
-version = "0.0.5"
+version = "0.0.6"
 authors = ["Hanif Yuli Abdillah P <hanifabd23@gmail.com>"]
 description = "Python package for detecting entities in text based on a dictionary and fuzzy similarity"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `lexifuzz_ner-0.0.5/src/lexifuzz_ner/ner.py` & `lexifuzz_ner-0.0.6/src/lexifuzz_ner/ner.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
       # Check if the entity's indices overlap with previously covered indices
       if all(start > end_covered or end < start_covered for start_covered, end_covered in indices_covered):
           new_entities.append(entity)
           # Update the covered indices
           indices_covered.add((start, end))
 
   # Update the entities in the data dictionary
-  data['entities'] = new_entities
+  data['entities'] = sorted(new_entities, key=lambda x: (x['index']['start']))
   return data
 
 def annotate_text(entities = None):
   """
     This function is used to annotate specific substrings within a text by adding custom tags around them, making it useful for highlighting or marking specific entities or elements within the text.
   """
```

### Comparing `lexifuzz_ner-0.0.5/PKG-INFO` & `lexifuzz_ner-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexifuzz-ner
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package for detecting entities in text based on a dictionary and fuzzy similarity
 Author: Hanif Yuli Abdillah P
 Author-email: hanifabd23@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

