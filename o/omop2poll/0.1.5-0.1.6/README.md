# Comparing `tmp/omop2poll-0.1.5.tar.gz` & `tmp/omop2poll-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omop2poll-0.1.5.tar", max compression
+gzip compressed data, was "omop2poll-0.1.6.tar", max compression
```

## Comparing `omop2poll-0.1.5.tar` & `omop2poll-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4515 2024-03-30 02:01:42.491653 omop2poll-0.1.5/README.md
--rw-r--r--   0        0        0      289 2024-04-17 01:38:52.402143 omop2poll-0.1.5/omop2poll/__init__.py
--rw-r--r--   0        0        0     3452 2024-04-17 01:38:52.393408 omop2poll-0.1.5/omop2poll/codebook.py
--rw-r--r--   0        0        0     1473 2024-04-17 01:38:52.395700 omop2poll-0.1.5/omop2poll/map_responses.py
--rw-r--r--   0        0        0     1190 2024-04-17 01:38:52.399108 omop2poll-0.1.5/omop2poll/pivot_data.py
--rw-r--r--   0        0        0      795 2024-04-17 01:38:52.397487 omop2poll-0.1.5/omop2poll/recode_missing.py
--rw-r--r--   0        0        0    42126 2024-04-16 23:50:27.759328 omop2poll-0.1.5/omop2poll/survey_healthcare.csv
--rw-r--r--   0        0        0      754 2024-04-17 01:44:21.811180 omop2poll-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5341 1970-01-01 00:00:00.000000 omop2poll-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4515 2024-03-30 02:01:42.491653 omop2poll-0.1.6/README.md
+-rw-r--r--   0        0        0      288 2024-04-17 02:09:19.565951 omop2poll-0.1.6/omop2poll/__init__.py
+-rw-r--r--   0        0        0     3452 2024-04-16 23:47:54.624690 omop2poll-0.1.6/omop2poll/codebook.py
+-rw-r--r--   0        0        0     1473 2024-04-16 23:52:37.337631 omop2poll-0.1.6/omop2poll/map_responses.py
+-rw-r--r--   0        0        0     1190 2024-04-16 23:47:54.633321 omop2poll-0.1.6/omop2poll/pivot_data.py
+-rw-r--r--   0        0        0      795 2024-04-16 23:39:52.869164 omop2poll-0.1.6/omop2poll/recode_missing.py
+-rw-r--r--   0        0        0    42126 2024-04-16 23:50:27.759328 omop2poll-0.1.6/omop2poll/survey_healthcare.csv
+-rw-r--r--   0        0        0      716 2024-04-17 02:15:26.029930 omop2poll-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 omop2poll-0.1.6/PKG-INFO
```

### Comparing `omop2poll-0.1.5/README.md` & `omop2poll-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `omop2poll-0.1.5/omop2poll/codebook.py` & `omop2poll-0.1.6/omop2poll/codebook.py`

 * *Files identical despite different names*

### Comparing `omop2poll-0.1.5/omop2poll/map_responses.py` & `omop2poll-0.1.6/omop2poll/map_responses.py`

 * *Files identical despite different names*

### Comparing `omop2poll-0.1.5/omop2poll/pivot_data.py` & `omop2poll-0.1.6/omop2poll/pivot_data.py`

 * *Files identical despite different names*

### Comparing `omop2poll-0.1.5/omop2poll/recode_missing.py` & `omop2poll-0.1.6/omop2poll/recode_missing.py`

 * *Files identical despite different names*

### Comparing `omop2poll-0.1.5/omop2poll/survey_healthcare.csv` & `omop2poll-0.1.6/omop2poll/survey_healthcare.csv`

 * *Files identical despite different names*

### Comparing `omop2poll-0.1.5/pyproject.toml` & `omop2poll-0.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "omop2poll"
-version = "0.1.5"
+version = "0.1.6"
 description = "The 'omop2poll' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis."
 authors = ["Elif Dede Yildirim <elifdy@auburn.edu>"]
 repository = "https://github.com/elifdy/omop2poll.git"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.8"
 pandas = "^2.2.2"
-
-[tool.poetry.group.dev.dependencies]
-tabulate = "^0.9.0"
 openpyxl = "^3.1.2"
+tabulate = "^0.9.0"
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `omop2poll-0.1.5/PKG-INFO` & `omop2poll-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: omop2poll
-Version: 0.1.5
+Version: 0.1.6
 Summary: The 'omop2poll' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis.
 Home-page: https://github.com/elifdy/omop2poll.git
 License: MIT
 Author: Elif Dede Yildirim
 Author-email: elifdy@auburn.edu
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/elifdy/omop2poll.git
 Description-Content-Type: text/markdown
 
 The **'omop2poll'** Python package offers a comprehensive solution for transforming standardized response codes from the Observational Medical Outcomes Partnership (OMOP) Common Data Model (CDM) survey variables into numeric values, streamlining the data preparation process. By automating the mapping and conversion of response codes, as well as the handling of missing data, it makes data analysis more accessible and reliable. The package provides a range of functions designed to help researchers and data analysts efficiently work through OMOP CDM survey data, ensuring accurate mappings of responses and effective management of data discrepancies. This package is a helpful tool for those working with OMOP CDM survey data, offering a path to more profound and accurate analyses by dramatically lowering the burden of data preprocessing.
 
 ## load_data.py
 >
```

