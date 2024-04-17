# Comparing `tmp/fairness_datasets-0.1.0.tar.gz` & `tmp/fairness_datasets-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairness_datasets-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fairness_datasets-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fairness_datasets-0.1.0.tar` & `fairness_datasets-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3105 2023-08-16 10:00:21.878984 fairness_datasets-0.1.0/.gitignore
--rw-r--r--   0        0        0     1070 2023-08-16 09:03:18.201486 fairness_datasets-0.1.0/LICENSE
--rw-r--r--   0        0        0     2312 2024-04-12 20:01:51.471967 fairness_datasets-0.1.0/README.md
--rw-r--r--   0        0        0      269 2024-04-12 19:37:39.963121 fairness_datasets-0.1.0/fairnessdatasets/__init__.py
--rw-r--r--   0        0        0     8846 2024-04-12 19:25:16.709746 fairness_datasets-0.1.0/fairnessdatasets/adult.py
--rw-r--r--   0        0        0    15339 2024-04-12 20:02:47.287823 fairness_datasets-0.1.0/fairnessdatasets/base.py
--rw-r--r--   0        0        0     5397 2024-04-12 15:59:57.756084 fairness_datasets-0.1.0/fairnessdatasets/default.py
--rw-r--r--   0        0        0     4125 2024-04-12 19:29:43.876781 fairness_datasets-0.1.0/fairnessdatasets/law_school.py
--rw-r--r--   0        0        0     7062 2024-04-12 16:06:33.386637 fairness_datasets-0.1.0/fairnessdatasets/south_german.py
--rw-r--r--   0        0        0      783 2024-02-01 14:45:15.232276 fairness_datasets-0.1.0/noxfile.py
--rw-r--r--   0        0        0     1148 2024-04-12 15:36:24.293920 fairness_datasets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1463 2024-04-12 19:37:07.507233 fairness_datasets-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     3980 2024-04-12 19:50:13.029406 fairness_datasets-0.1.0/tests/test_column_indices.py
--rw-r--r--   0        0        0     1723 2024-04-12 19:37:07.515233 fairness_datasets-0.1.0/tests/test_download.py
--rw-r--r--   0        0        0      587 2024-04-12 12:55:35.731613 fairness_datasets-0.1.0/tests/test_output.py
--rw-r--r--   0        0        0     1658 2024-04-12 19:50:13.045406 fairness_datasets-0.1.0/tests/test_shapes.py
--rw-r--r--   0        0        0     1318 2024-04-12 15:51:37.738349 fairness_datasets-0.1.0/tests/test_use.py
--rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 fairness_datasets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3105 2023-08-16 10:00:21.878984 fairness_datasets-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1070 2023-08-16 09:03:18.201486 fairness_datasets-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2427 2024-04-17 12:43:04.913550 fairness_datasets-0.2.0/README.md
+-rw-r--r--   0        0        0      269 2024-04-17 12:42:07.101711 fairness_datasets-0.2.0/fairnessdatasets/__init__.py
+-rw-r--r--   0        0        0     8846 2024-04-12 19:25:16.709746 fairness_datasets-0.2.0/fairnessdatasets/adult.py
+-rw-r--r--   0        0        0    15339 2024-04-12 20:02:47.287823 fairness_datasets-0.2.0/fairnessdatasets/base.py
+-rw-r--r--   0        0        0     5397 2024-04-12 15:59:57.756084 fairness_datasets-0.2.0/fairnessdatasets/default.py
+-rw-r--r--   0        0        0     6471 2024-04-17 12:50:52.132263 fairness_datasets-0.2.0/fairnessdatasets/law_school.py
+-rw-r--r--   0        0        0     7062 2024-04-12 16:06:33.386637 fairness_datasets-0.2.0/fairnessdatasets/south_german.py
+-rw-r--r--   0        0        0      783 2024-02-01 14:45:15.232276 fairness_datasets-0.2.0/noxfile.py
+-rw-r--r--   0        0        0     1148 2024-04-12 15:36:24.293920 fairness_datasets-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1463 2024-04-12 19:37:07.507233 fairness_datasets-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     3980 2024-04-12 19:50:13.029406 fairness_datasets-0.2.0/tests/test_column_indices.py
+-rw-r--r--   0        0        0     1837 2024-04-17 12:40:40.261954 fairness_datasets-0.2.0/tests/test_download.py
+-rw-r--r--   0        0        0      587 2024-04-12 12:55:35.731613 fairness_datasets-0.2.0/tests/test_output.py
+-rw-r--r--   0        0        0     1658 2024-04-12 19:50:13.045406 fairness_datasets-0.2.0/tests/test_shapes.py
+-rw-r--r--   0        0        0     1318 2024-04-12 15:51:37.738349 fairness_datasets-0.2.0/tests/test_use.py
+-rw-r--r--   0        0        0     3513 1970-01-01 00:00:00.000000 fairness_datasets-0.2.0/PKG-INFO
```

### Comparing `fairness_datasets-0.1.0/.gitignore` & `fairness_datasets-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.1.0/LICENSE` & `fairness_datasets-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.1.0/README.md` & `fairness_datasets-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # fairness-datasets
+[![PyPI version](https://badge.fury.io/py/fairness-datasets.svg)](https://badge.fury.io/py/fairness-datasets)
+
 PyTorch dataset wrappers for the several popular datasets from 
 fair machine learning research.
 
 The following datasets are wrapped:
  - [Adult (Census Income)](https://archive.ics.uci.edu/dataset/2/adult).
  - [Default](https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients)
  - [Law School](https://eric.ed.gov/?id=ED469370) (data from [here](https://www.tensorflow.org/responsible_ai/fairness_indicators/tutorials/Fairness_Indicators_Pandas_Case_Study))
  - [SouthGerman](https://archive.ics.uci.edu/dataset/573/south+german+credit+update)
 
 ## Installation
 ```shell
-pip install adult-dataset
+pip install fairness-datasets
 ```
 
 ## Basic Usage
 ```python
 from fairnessdatasets import Adult
 
 # load (if necessary, download) the Adult training dataset
```

### Comparing `fairness_datasets-0.1.0/fairnessdatasets/adult.py` & `fairness_datasets-0.2.0/fairnessdatasets/adult.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.1.0/fairnessdatasets/base.py` & `fairness_datasets-0.2.0/fairnessdatasets/base.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.1.0/fairnessdatasets/default.py` & `fairness_datasets-0.2.0/fairnessdatasets/default.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.1.0/fairnessdatasets/south_german.py` & `fairness_datasets-0.2.0/fairnessdatasets/south_german.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.1.0/noxfile.py` & `fairness_datasets-0.2.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.1.0/pyproject.toml` & `fairness_datasets-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.1.0/tests/conftest.py` & `fairness_datasets-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.1.0/tests/test_column_indices.py` & `fairness_datasets-0.2.0/tests/test_column_indices.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.1.0/tests/test_download.py` & `fairness_datasets-0.2.0/tests/test_download.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,38 +12,40 @@
         (Adult, {"train": False}),
         (Adult, {"raw": True}),
         (Adult, {"train": False, "raw": True}),
         (Default, {}),
         (Default, {"raw": True}),
         (LawSchool, {}),
         (LawSchool, {"raw": True}),
+        (LawSchool, {"features": ("gender", "race1", "lsat")}),
         (SouthGerman, {"raw": False}),
         (SouthGerman, {"raw": True}),
     ],
     ids=[
         "Adult-train",
         "Adult-test",
         "Adult-raw-train",
         "Adult-raw-test",
         "Default",
         "Default-raw",
         "LawSchool",
         "LawSchool-raw",
+        "LawSchool-gender-race1-lsat",
         "SouthGerman",
         "SouthGerman-raw",
     ],
 )
 def test_download(dataset_class, init_kwargs, tmp_path):
     dataset = dataset_class(root=tmp_path, download=True, **init_kwargs)
     assert len(dataset[0]) == 2
 
 
 @pytest.mark.parametrize(
     "dataset_class",
-    [Adult, SouthGerman, Default],
+    [Adult, SouthGerman, Default, LawSchool],
 )
 def test_download_alongside_raw(dataset_class, tmp_path):
     raw = dataset_class(root=tmp_path, raw=True, download=True)
     assert len(raw[0]) == 2
     standard = dataset_class(root=tmp_path, raw=False, download=True)
     assert len(standard[0]) == 2
```

### Comparing `fairness_datasets-0.1.0/tests/test_output.py` & `fairness_datasets-0.2.0/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.1.0/tests/test_shapes.py` & `fairness_datasets-0.2.0/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.1.0/tests/test_use.py` & `fairness_datasets-0.2.0/tests/test_use.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.1.0/PKG-INFO` & `fairness_datasets-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairness-datasets
-Version: 0.1.0
+Version: 0.2.0
 Summary: PyTorch dataset wrapper for the
 Keywords: PyTorch,Dataset,Fairness,Adult,Census Income,Law School
 Author-email: David Boetius <david.boetius@uni-konstanz.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,26 +21,28 @@
 Project-URL: Bug Tracker, https://github.com/cherrywoods/fairness-datasets/issues
 Project-URL: Homepage, https://github.com/cherrywoods/fairness-datasets
 Project-URL: Repository, https://github.com/cherrywoods/fairness-datasets.git
 Provides-Extra: develop
 Provides-Extra: test
 
 # fairness-datasets
+[![PyPI version](https://badge.fury.io/py/fairness-datasets.svg)](https://badge.fury.io/py/fairness-datasets)
+
 PyTorch dataset wrappers for the several popular datasets from 
 fair machine learning research.
 
 The following datasets are wrapped:
  - [Adult (Census Income)](https://archive.ics.uci.edu/dataset/2/adult).
  - [Default](https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients)
  - [Law School](https://eric.ed.gov/?id=ED469370) (data from [here](https://www.tensorflow.org/responsible_ai/fairness_indicators/tutorials/Fairness_Indicators_Pandas_Case_Study))
  - [SouthGerman](https://archive.ics.uci.edu/dataset/573/south+german+credit+update)
 
 ## Installation
 ```shell
-pip install adult-dataset
+pip install fairness-datasets
 ```
 
 ## Basic Usage
 ```python
 from fairnessdatasets import Adult
 
 # load (if necessary, download) the Adult training dataset
```

