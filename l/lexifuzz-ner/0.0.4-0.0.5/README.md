# Comparing `tmp/lexifuzz_ner-0.0.4.tar.gz` & `tmp/lexifuzz_ner-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexifuzz_ner-0.0.4.tar", max compression
+gzip compressed data, was "lexifuzz_ner-0.0.5.tar", max compression
```

## Comparing `lexifuzz_ner-0.0.4.tar` & `lexifuzz_ner-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1097 2023-09-12 04:08:59.142483 lexifuzz_ner-0.0.4/LICENSE
--rwxr-xr-x   0        0        0     2993 2023-09-12 09:03:52.788781 lexifuzz_ner-0.0.4/README.md
--rwxr-xr-x   0        0        0      640 2023-09-21 06:15:02.882656 lexifuzz_ner-0.0.4/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-09-12 04:29:12.919915 lexifuzz_ner-0.0.4/src/lexifuzz_ner/__init__.py
--rwxr-xr-x   0        0        0     6700 2023-09-21 06:11:38.293699 lexifuzz_ner-0.0.4/src/lexifuzz_ner/ner.py
--rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 lexifuzz_ner-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1097 2023-09-12 04:08:59.142483 lexifuzz_ner-0.0.5/LICENSE
+-rwxr-xr-x   0        0        0     2993 2024-04-17 10:22:18.366558 lexifuzz_ner-0.0.5/README.md
+-rwxr-xr-x   0        0        0      640 2024-04-17 10:29:27.097513 lexifuzz_ner-0.0.5/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-09-12 04:29:12.919915 lexifuzz_ner-0.0.5/src/lexifuzz_ner/__init__.py
+-rwxr-xr-x   0        0        0     6700 2024-04-17 10:22:18.375566 lexifuzz_ner-0.0.5/src/lexifuzz_ner/ner.py
+-rw-r--r--   0        0        0     3718 1970-01-01 00:00:00.000000 lexifuzz_ner-0.0.5/PKG-INFO
```

### Comparing `lexifuzz_ner-0.0.4/LICENSE` & `lexifuzz_ner-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lexifuzz_ner-0.0.4/README.md` & `lexifuzz_ner-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lexifuzz_ner-0.0.4/pyproject.toml` & `lexifuzz_ner-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "lexifuzz-ner"
-version = "0.0.4"
+version = "0.0.5"
 authors = ["Hanif Yuli Abdillah P <hanifabd23@gmail.com>"]
 description = "Python package for detecting entities in text based on a dictionary and fuzzy similarity"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `lexifuzz_ner-0.0.4/src/lexifuzz_ner/ner.py` & `lexifuzz_ner-0.0.5/src/lexifuzz_ner/ner.py`

 * *Files identical despite different names*

### Comparing `lexifuzz_ner-0.0.4/PKG-INFO` & `lexifuzz_ner-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: lexifuzz-ner
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for detecting entities in text based on a dictionary and fuzzy similarity
 Author: Hanif Yuli Abdillah P
 Author-email: hanifabd23@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: nltk (==3.8.1)
 Requires-Dist: thefuzz (==0.20.0)
 Description-Content-Type: text/markdown
 
 # **LexiFuzz NER: Named Entity Recognition Based on Dictionary and Fuzzy Matching**
 
 ![Image](https://github.com/hanifabd/lexifuzz-ner/blob/master/assets/lexifuzz-mascot.png)
```

