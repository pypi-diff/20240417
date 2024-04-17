# Comparing `tmp/research_roc_utils-0.0.6.tar.gz` & `tmp/research_roc_utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "research_roc_utils-0.0.6.tar", last modified: Tue Apr 16 10:14:53 2024, max compression
+gzip compressed data, was "research_roc_utils-0.0.7.tar", last modified: Tue Apr 16 10:23:58 2024, max compression
```

## Comparing `research_roc_utils-0.0.6.tar` & `research_roc_utils-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 10:14:53.961041 research_roc_utils-0.0.6/
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1080 2024-04-12 08:42:51.000000 research_roc_utils-0.0.6/LICENSE
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 10:14:53.960811 research_roc_utils-0.0.6/PKG-INFO
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-10 14:34:49.000000 research_roc_utils-0.0.6/README.md
-drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 10:14:53.959365 research_roc_utils-0.0.6/research_roc_utils/
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 07:47:53.000000 research_roc_utils-0.0.6/research_roc_utils/__init__.py
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)    19157 2024-04-16 10:10:04.000000 research_roc_utils-0.0.6/research_roc_utils/research_roc_utils.py
-drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 10:14:53.960559 research_roc_utils-0.0.6/research_roc_utils.egg-info/
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 10:14:53.000000 research_roc_utils-0.0.6/research_roc_utils.egg-info/PKG-INFO
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      307 2024-04-16 10:14:53.000000 research_roc_utils-0.0.6/research_roc_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-16 10:14:53.000000 research_roc_utils-0.0.6/research_roc_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      125 2024-04-16 10:14:53.000000 research_roc_utils-0.0.6/research_roc_utils.egg-info/requires.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       19 2024-04-16 10:14:53.000000 research_roc_utils-0.0.6/research_roc_utils.egg-info/top_level.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       38 2024-04-16 10:14:53.961085 research_roc_utils-0.0.6/setup.cfg
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1176 2024-04-16 10:14:41.000000 research_roc_utils-0.0.6/setup.py
+drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 10:23:58.434210 research_roc_utils-0.0.7/
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1080 2024-04-12 08:42:51.000000 research_roc_utils-0.0.7/LICENSE
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 10:23:58.433911 research_roc_utils-0.0.7/PKG-INFO
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-10 14:34:49.000000 research_roc_utils-0.0.7/README.md
+drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 10:23:58.428121 research_roc_utils-0.0.7/research_roc_utils/
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 07:47:53.000000 research_roc_utils-0.0.7/research_roc_utils/__init__.py
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)    19157 2024-04-16 10:10:04.000000 research_roc_utils-0.0.7/research_roc_utils/roc_utils.py
+drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 10:23:58.433493 research_roc_utils-0.0.7/research_roc_utils.egg-info/
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 10:23:58.000000 research_roc_utils-0.0.7/research_roc_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      298 2024-04-16 10:23:58.000000 research_roc_utils-0.0.7/research_roc_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-16 10:23:58.000000 research_roc_utils-0.0.7/research_roc_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      125 2024-04-16 10:23:58.000000 research_roc_utils-0.0.7/research_roc_utils.egg-info/requires.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       19 2024-04-16 10:23:58.000000 research_roc_utils-0.0.7/research_roc_utils.egg-info/top_level.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       38 2024-04-16 10:23:58.434461 research_roc_utils-0.0.7/setup.cfg
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1177 2024-04-16 10:23:37.000000 research_roc_utils-0.0.7/setup.py
```

### Comparing `research_roc_utils-0.0.6/LICENSE` & `research_roc_utils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `research_roc_utils-0.0.6/PKG-INFO` & `research_roc_utils-0.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research_roc_utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utility functions to assist in the computation of ROC curve comparisons based on academic research.
 Home-page: https://github.com/jpbruehw/research-roc-utils
 Author: JP Bruehwiler
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.2
```

### Comparing `research_roc_utils-0.0.6/research_roc_utils/research_roc_utils.py` & `research_roc_utils-0.0.7/research_roc_utils/roc_utils.py`

 * *Files identical despite different names*

### Comparing `research_roc_utils-0.0.6/research_roc_utils.egg-info/PKG-INFO` & `research_roc_utils-0.0.7/research_roc_utils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research-roc-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utility functions to assist in the computation of ROC curve comparisons based on academic research.
 Home-page: https://github.com/jpbruehw/research-roc-utils
 Author: JP Bruehwiler
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.2
```

### Comparing `research_roc_utils-0.0.6/setup.py` & `research_roc_utils-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Python setup.py for project_name package"""
 import io
 import os
 from setuptools import find_packages, setup
 
 def read(*paths, **kwargs):
     """Read the contents of a text file safely.
-    >>> read("research_roc_utils", "0.0.6")
-    '0.0.6
+    >>> read("research_roc_utils", "0.0.7")
+    '0.0.7'
     >>> read("README.md")
     ...
     """
 
     content = ""
     with io.open(
         os.path.join(os.path.dirname(__file__), *paths),
@@ -22,15 +22,15 @@
 def read_requirements(path):
     return [
         line.strip()
         for line in read(path).split("\n")
         if not line.startswith(('"', "#", "-", "git+"))
     ]
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 
 setup(
     name="research_roc_utils",
     version=VERSION,
     description="Utility functions to assist in the computation of ROC curve comparisons based on academic research.",
     url="https://github.com/jpbruehw/research-roc-utils",
     long_description=read("README.md"),
```

