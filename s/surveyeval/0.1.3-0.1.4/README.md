# Comparing `tmp/surveyeval-0.1.3.tar.gz` & `tmp/surveyeval-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surveyeval-0.1.3.tar", last modified: Tue Apr 16 20:56:30 2024, max compression
+gzip compressed data, was "surveyeval-0.1.4.tar", last modified: Tue Apr 16 21:15:06 2024, max compression
```

## Comparing `surveyeval-0.1.3.tar` & `surveyeval-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:56:30.363758 surveyeval-0.1.3/
--rw-r--r--   0 crobert    (501) staff       (20)    11357 2023-11-29 20:42:10.000000 surveyeval-0.1.3/LICENSE
--rw-r--r--   0 crobert    (501) staff       (20)    11786 2024-04-16 20:56:30.363467 surveyeval-0.1.3/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)    10430 2024-04-14 15:10:57.000000 surveyeval-0.1.3/README.rst
--rw-r--r--   0 crobert    (501) staff       (20)       38 2024-04-16 20:56:30.363808 surveyeval-0.1.3/setup.cfg
--rw-r--r--   0 crobert    (501) staff       (20)     2043 2024-04-16 20:56:22.000000 surveyeval-0.1.3/setup.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:56:30.357399 surveyeval-0.1.3/src/
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:56:30.361071 surveyeval-0.1.3/src/surveyeval/
--rw-r--r--   0 crobert    (501) staff       (20)     1058 2024-04-14 15:10:57.000000 surveyeval-0.1.3/src/surveyeval/__init__.py
--rw-r--r--   0 crobert    (501) staff       (20)    49441 2024-04-14 15:33:38.000000 surveyeval-0.1.3/src/surveyeval/core_evaluation_lenses.py
--rw-r--r--   0 crobert    (501) staff       (20)    33231 2024-04-14 16:03:22.000000 surveyeval-0.1.3/src/surveyeval/evaluation_engine.py
--rw-r--r--   0 crobert    (501) staff       (20)    56480 2024-04-14 15:27:21.000000 surveyeval-0.1.3/src/surveyeval/survey_parser.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:56:30.363043 surveyeval-0.1.3/src/surveyeval.egg-info/
--rw-r--r--   0 crobert    (501) staff       (20)    11786 2024-04-16 20:56:30.000000 surveyeval-0.1.3/src/surveyeval.egg-info/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)      352 2024-04-16 20:56:30.000000 surveyeval-0.1.3/src/surveyeval.egg-info/SOURCES.txt
--rw-r--r--   0 crobert    (501) staff       (20)        1 2024-04-16 20:56:30.000000 surveyeval-0.1.3/src/surveyeval.egg-info/dependency_links.txt
--rw-r--r--   0 crobert    (501) staff       (20)      504 2024-04-16 20:56:30.000000 surveyeval-0.1.3/src/surveyeval.egg-info/requires.txt
--rw-r--r--   0 crobert    (501) staff       (20)       11 2024-04-16 20:56:30.000000 surveyeval-0.1.3/src/surveyeval.egg-info/top_level.txt
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 21:15:06.399664 surveyeval-0.1.4/
+-rw-r--r--   0 crobert    (501) staff       (20)    11357 2023-11-29 20:42:10.000000 surveyeval-0.1.4/LICENSE
+-rw-r--r--   0 crobert    (501) staff       (20)    11239 2024-04-16 21:15:06.399381 surveyeval-0.1.4/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)    10689 2024-04-16 21:14:57.000000 surveyeval-0.1.4/README.rst
+-rw-r--r--   0 crobert    (501) staff       (20)       38 2024-04-16 21:15:06.399724 surveyeval-0.1.4/setup.cfg
+-rw-r--r--   0 crobert    (501) staff       (20)     1349 2024-04-16 21:14:57.000000 surveyeval-0.1.4/setup.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 21:15:06.393694 surveyeval-0.1.4/src/
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 21:15:06.397197 surveyeval-0.1.4/src/surveyeval/
+-rw-r--r--   0 crobert    (501) staff       (20)     1058 2024-04-14 15:10:57.000000 surveyeval-0.1.4/src/surveyeval/__init__.py
+-rw-r--r--   0 crobert    (501) staff       (20)    49441 2024-04-14 15:33:38.000000 surveyeval-0.1.4/src/surveyeval/core_evaluation_lenses.py
+-rw-r--r--   0 crobert    (501) staff       (20)    33231 2024-04-14 16:03:22.000000 surveyeval-0.1.4/src/surveyeval/evaluation_engine.py
+-rw-r--r--   0 crobert    (501) staff       (20)    56480 2024-04-14 15:27:21.000000 surveyeval-0.1.4/src/surveyeval/survey_parser.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 21:15:06.398980 surveyeval-0.1.4/src/surveyeval.egg-info/
+-rw-r--r--   0 crobert    (501) staff       (20)    11239 2024-04-16 21:15:06.000000 surveyeval-0.1.4/src/surveyeval.egg-info/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)      352 2024-04-16 21:15:06.000000 surveyeval-0.1.4/src/surveyeval.egg-info/SOURCES.txt
+-rw-r--r--   0 crobert    (501) staff       (20)        1 2024-04-16 21:15:06.000000 surveyeval-0.1.4/src/surveyeval.egg-info/dependency_links.txt
+-rw-r--r--   0 crobert    (501) staff       (20)      118 2024-04-16 21:15:06.000000 surveyeval-0.1.4/src/surveyeval.egg-info/requires.txt
+-rw-r--r--   0 crobert    (501) staff       (20)       11 2024-04-16 21:15:06.000000 surveyeval-0.1.4/src/surveyeval.egg-info/top_level.txt
```

### Comparing `surveyeval-0.1.3/LICENSE` & `surveyeval-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.3/PKG-INFO` & `surveyeval-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,23 @@
 Metadata-Version: 2.1
 Name: surveyeval
-Version: 0.1.3
+Version: 0.1.4
 Summary: A toolkit for survey evaluation
 Home-page: https://github.com/higherbar-ai/survey-eval
 Author: Christopher Robert
 Author-email: crobert@higherbar.ai
 License: Apache 2.0
 Project-URL: Documentation, https://surveyeval.readthedocs.io/
 Requires-Python: >=3.10
 License-File: LICENSE
-Requires-Dist: bs4~=0.0.1
 Requires-Dist: tiktoken~=0.5.2
 Requires-Dist: openai~=1.10.0
 Requires-Dist: langchain~=0.1.15
 Requires-Dist: langchain-openai~=0.0.5
 Requires-Dist: langchain-community~=0.0.17
-Requires-Dist: unstructured[local-inference]
-Requires-Dist: tensorboard>2.12.2
-Requires-Dist: uvicorn[standard]~=0.22.0
-Requires-Dist: pydantic~=1.10.8
-Requires-Dist: markdown~=3.4.3
-Requires-Dist: pdfkit~=1.0.0
-Requires-Dist: libmagic~=1.0
-Requires-Dist: nltk~=3.8.1
-Requires-Dist: spacy~=3.6.0
-Requires-Dist: pdfminer.six
-Requires-Dist: easyocr
-Requires-Dist: pdf2image~=1.16.3
-Requires-Dist: tabula-py~=2.9.0
-Requires-Dist: pypdf~=4.0.1
-Requires-Dist: pytesseract~=0.3.10
-Requires-Dist: tokenizers
-Requires-Dist: docx
-Requires-Dist: mammoth
-Requires-Dist: markdownify
-Requires-Dist: kor~=1.0.0
-Requires-Dist: scrapy~=2.11.1
-Requires-Dist: ipywidgets
-Requires-Dist: chromadb
-Requires-Dist: pyxform
-Requires-Dist: lxml
-Requires-Dist: requests~=2.31.0
-Requires-Dist: tqdm~=4.65.0
 Requires-Dist: overrides~=7.3.1
 
 ==========
 surveyeval
 ==========
 
 This repository contains a toolkit for AI-powered survey instrument evaluation. It's still in early development, but 
@@ -55,14 +27,19 @@
 Installation
 ------------
 
 Installing the latest version with pip::
 
     pip install surveyeval
 
+Note that you might need to install additional requirements to use the ``survey_parser`` module. Only requirements for
+the core evaluation engine are automatically installed by ``pip``. To install all requirements, run::
+
+    pip install -r requirements.txt
+
 Overview
 ---------
 
 Here are the basics:
 
 #. This toolkit includes code to read, parse, and evaluate survey instruments.
 #. The ``file-evaluation-example.ipynb`` Jupyter workbook provides a working example for evaluating a single survey
```

### Comparing `surveyeval-0.1.3/README.rst` & `surveyeval-0.1.4/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 Installation
 ------------
 
 Installing the latest version with pip::
 
     pip install surveyeval
 
+Note that you might need to install additional requirements to use the ``survey_parser`` module. Only requirements for
+the core evaluation engine are automatically installed by ``pip``. To install all requirements, run::
+
+    pip install -r requirements.txt
+
 Overview
 ---------
 
 Here are the basics:
 
 #. This toolkit includes code to read, parse, and evaluate survey instruments.
 #. The ``file-evaluation-example.ipynb`` Jupyter workbook provides a working example for evaluating a single survey
```

### Comparing `surveyeval-0.1.3/setup.py` & `surveyeval-0.1.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,51 +15,23 @@
 from setuptools import setup
 
 with open('README.rst') as file:
     readme = file.read()
 
 setup(
     name='surveyeval',
-    version='0.1.3',
+    version='0.1.4',
     packages=['surveyeval'],
     python_requires='>=3.10',
     install_requires=[
-        'bs4~=0.0.1',
         'tiktoken~=0.5.2',
         'openai~=1.10.0',
         'langchain~=0.1.15',
         'langchain-openai~=0.0.5',
         'langchain-community~=0.0.17',
-        'unstructured[local-inference]',
-        'tensorboard>2.12.2',
-        'uvicorn[standard]~=0.22.0',
-        'pydantic~=1.10.8',
-        'markdown~=3.4.3',
-        'pdfkit~=1.0.0',
-        'libmagic~=1.0',
-        'nltk~=3.8.1',
-        'spacy~=3.6.0',
-        'pdfminer.six',
-        'easyocr',
-        'pdf2image~=1.16.3',
-        'tabula-py~=2.9.0',
-        'pypdf~=4.0.1',
-        'pytesseract~=0.3.10',
-        'tokenizers',
-        'docx',
-        'mammoth',
-        'markdownify',
-        'kor~=1.0.0',
-        'scrapy~=2.11.1',
-        'ipywidgets',
-        'chromadb',
-        'pyxform',
-        'lxml',
-        'requests~=2.31.0',
-        'tqdm~=4.65.0',
         'overrides~=7.3.1',
     ],
     package_dir={'': 'src'},
     url='https://github.com/higherbar-ai/survey-eval',
     project_urls={'Documentation': 'https://surveyeval.readthedocs.io/'},
     license='Apache 2.0',
     author='Christopher Robert',
```

### Comparing `surveyeval-0.1.3/src/surveyeval/__init__.py` & `surveyeval-0.1.4/src/surveyeval/__init__.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.3/src/surveyeval/core_evaluation_lenses.py` & `surveyeval-0.1.4/src/surveyeval/core_evaluation_lenses.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.3/src/surveyeval/evaluation_engine.py` & `surveyeval-0.1.4/src/surveyeval/evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.3/src/surveyeval/survey_parser.py` & `surveyeval-0.1.4/src/surveyeval/survey_parser.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.3/src/surveyeval.egg-info/PKG-INFO` & `surveyeval-0.1.4/src/surveyeval.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,23 @@
 Metadata-Version: 2.1
 Name: surveyeval
-Version: 0.1.3
+Version: 0.1.4
 Summary: A toolkit for survey evaluation
 Home-page: https://github.com/higherbar-ai/survey-eval
 Author: Christopher Robert
 Author-email: crobert@higherbar.ai
 License: Apache 2.0
 Project-URL: Documentation, https://surveyeval.readthedocs.io/
 Requires-Python: >=3.10
 License-File: LICENSE
-Requires-Dist: bs4~=0.0.1
 Requires-Dist: tiktoken~=0.5.2
 Requires-Dist: openai~=1.10.0
 Requires-Dist: langchain~=0.1.15
 Requires-Dist: langchain-openai~=0.0.5
 Requires-Dist: langchain-community~=0.0.17
-Requires-Dist: unstructured[local-inference]
-Requires-Dist: tensorboard>2.12.2
-Requires-Dist: uvicorn[standard]~=0.22.0
-Requires-Dist: pydantic~=1.10.8
-Requires-Dist: markdown~=3.4.3
-Requires-Dist: pdfkit~=1.0.0
-Requires-Dist: libmagic~=1.0
-Requires-Dist: nltk~=3.8.1
-Requires-Dist: spacy~=3.6.0
-Requires-Dist: pdfminer.six
-Requires-Dist: easyocr
-Requires-Dist: pdf2image~=1.16.3
-Requires-Dist: tabula-py~=2.9.0
-Requires-Dist: pypdf~=4.0.1
-Requires-Dist: pytesseract~=0.3.10
-Requires-Dist: tokenizers
-Requires-Dist: docx
-Requires-Dist: mammoth
-Requires-Dist: markdownify
-Requires-Dist: kor~=1.0.0
-Requires-Dist: scrapy~=2.11.1
-Requires-Dist: ipywidgets
-Requires-Dist: chromadb
-Requires-Dist: pyxform
-Requires-Dist: lxml
-Requires-Dist: requests~=2.31.0
-Requires-Dist: tqdm~=4.65.0
 Requires-Dist: overrides~=7.3.1
 
 ==========
 surveyeval
 ==========
 
 This repository contains a toolkit for AI-powered survey instrument evaluation. It's still in early development, but 
@@ -55,14 +27,19 @@
 Installation
 ------------
 
 Installing the latest version with pip::
 
     pip install surveyeval
 
+Note that you might need to install additional requirements to use the ``survey_parser`` module. Only requirements for
+the core evaluation engine are automatically installed by ``pip``. To install all requirements, run::
+
+    pip install -r requirements.txt
+
 Overview
 ---------
 
 Here are the basics:
 
 #. This toolkit includes code to read, parse, and evaluate survey instruments.
 #. The ``file-evaluation-example.ipynb`` Jupyter workbook provides a working example for evaluating a single survey
```

