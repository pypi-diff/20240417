# Comparing `tmp/pydocgenerator-0.0.3.tar.gz` & `tmp/pydocgenerator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydocgenerator-0.0.3.tar", last modified: Fri Apr  5 19:30:28 2024, max compression
+gzip compressed data, was "pydocgenerator-0.0.4.tar", last modified: Sat Apr  6 18:51:06 2024, max compression
```

## Comparing `pydocgenerator-0.0.3.tar` & `pydocgenerator-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 19:30:28.472619 pydocgenerator-0.0.3/
--rw-rw-rw-   0        0        0     1088 2024-03-20 14:29:16.000000 pydocgenerator-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1615 2024-04-05 19:30:28.469614 pydocgenerator-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1031 2024-04-05 19:30:14.000000 pydocgenerator-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 19:30:28.466616 pydocgenerator-0.0.3/pydocgenerator.egg-info/
--rw-rw-rw-   0        0        0     1615 2024-04-05 19:30:28.000000 pydocgenerator-0.0.3/pydocgenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2024-04-05 19:30:28.000000 pydocgenerator-0.0.3/pydocgenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 19:30:28.000000 pydocgenerator-0.0.3/pydocgenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 19:30:28.000000 pydocgenerator-0.0.3/pydocgenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      608 2024-04-05 19:28:14.000000 pydocgenerator-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 19:30:28.472619 pydocgenerator-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      196 2024-03-31 05:39:46.000000 pydocgenerator-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:51:06.292703 pydocgenerator-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2024-03-20 14:29:16.000000 pydocgenerator-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1615 2024-04-06 18:51:06.287704 pydocgenerator-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1031 2024-04-05 19:30:14.000000 pydocgenerator-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 18:51:06.271715 pydocgenerator-0.0.4/pydocgenerator.egg-info/
+-rw-rw-rw-   0        0        0     1615 2024-04-06 18:51:05.000000 pydocgenerator-0.0.4/pydocgenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2024-04-06 18:51:06.000000 pydocgenerator-0.0.4/pydocgenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 18:51:05.000000 pydocgenerator-0.0.4/pydocgenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 18:51:06.000000 pydocgenerator-0.0.4/pydocgenerator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      608 2024-04-06 18:50:33.000000 pydocgenerator-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 18:51:06.292703 pydocgenerator-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      196 2024-03-31 05:39:46.000000 pydocgenerator-0.0.4/setup.py
```

### Comparing `pydocgenerator-0.0.3/LICENSE` & `pydocgenerator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydocgenerator-0.0.3/PKG-INFO` & `pydocgenerator-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydocgenerator
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for generating Docstring for python.
 Author-email: Rijin <rijin@gmail.com>, Amal <amal76735@gmail.com>, yadhu <yadhu2309@gmail.com>
 Project-URL: Homepage, https://github.com/RijinRaju/DocGen-AI
 Project-URL: Issues, https://github.com/RijinRaju/DocGen-AI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydocgenerator-0.0.3/README.md` & `pydocgenerator-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pydocgenerator-0.0.3/pydocgenerator.egg-info/PKG-INFO` & `pydocgenerator-0.0.4/pydocgenerator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydocgenerator
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for generating Docstring for python.
 Author-email: Rijin <rijin@gmail.com>, Amal <amal76735@gmail.com>, yadhu <yadhu2309@gmail.com>
 Project-URL: Homepage, https://github.com/RijinRaju/DocGen-AI
 Project-URL: Issues, https://github.com/RijinRaju/DocGen-AI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydocgenerator-0.0.3/pyproject.toml` & `pydocgenerator-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydocgenerator"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Rijin", email="rijin@gmail.com"},
   { name="Amal", email="amal76735@gmail.com"},
   { name="yadhu", email="yadhu2309@gmail.com"}
 ]
 description = "A package for generating Docstring for python."
 readme = "README.md"
```

