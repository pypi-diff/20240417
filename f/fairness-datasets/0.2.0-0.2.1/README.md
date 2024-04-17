# Comparing `tmp/fairness_datasets-0.2.0.tar.gz` & `tmp/fairness_datasets-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairness_datasets-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fairness_datasets-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fairness_datasets-0.2.0.tar` & `fairness_datasets-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3105 2023-08-16 10:00:21.878984 fairness_datasets-0.2.0/.gitignore
--rw-r--r--   0        0        0     1070 2023-08-16 09:03:18.201486 fairness_datasets-0.2.0/LICENSE
--rw-r--r--   0        0        0     2427 2024-04-17 12:43:04.913550 fairness_datasets-0.2.0/README.md
--rw-r--r--   0        0        0      269 2024-04-17 12:42:07.101711 fairness_datasets-0.2.0/fairnessdatasets/__init__.py
--rw-r--r--   0        0        0     8846 2024-04-12 19:25:16.709746 fairness_datasets-0.2.0/fairnessdatasets/adult.py
--rw-r--r--   0        0        0    15339 2024-04-12 20:02:47.287823 fairness_datasets-0.2.0/fairnessdatasets/base.py
--rw-r--r--   0        0        0     5397 2024-04-12 15:59:57.756084 fairness_datasets-0.2.0/fairnessdatasets/default.py
--rw-r--r--   0        0        0     6471 2024-04-17 12:50:52.132263 fairness_datasets-0.2.0/fairnessdatasets/law_school.py
--rw-r--r--   0        0        0     7062 2024-04-12 16:06:33.386637 fairness_datasets-0.2.0/fairnessdatasets/south_german.py
--rw-r--r--   0        0        0      783 2024-02-01 14:45:15.232276 fairness_datasets-0.2.0/noxfile.py
--rw-r--r--   0        0        0     1148 2024-04-12 15:36:24.293920 fairness_datasets-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1463 2024-04-12 19:37:07.507233 fairness_datasets-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     3980 2024-04-12 19:50:13.029406 fairness_datasets-0.2.0/tests/test_column_indices.py
--rw-r--r--   0        0        0     1837 2024-04-17 12:40:40.261954 fairness_datasets-0.2.0/tests/test_download.py
--rw-r--r--   0        0        0      587 2024-04-12 12:55:35.731613 fairness_datasets-0.2.0/tests/test_output.py
--rw-r--r--   0        0        0     1658 2024-04-12 19:50:13.045406 fairness_datasets-0.2.0/tests/test_shapes.py
--rw-r--r--   0        0        0     1318 2024-04-12 15:51:37.738349 fairness_datasets-0.2.0/tests/test_use.py
--rw-r--r--   0        0        0     3513 1970-01-01 00:00:00.000000 fairness_datasets-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3105 2023-08-16 10:00:21.878984 fairness_datasets-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1070 2023-08-16 09:03:18.201486 fairness_datasets-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2427 2024-04-17 12:43:04.913550 fairness_datasets-0.2.1/README.md
+-rw-r--r--   0        0        0      269 2024-04-17 13:07:31.753291 fairness_datasets-0.2.1/fairnessdatasets/__init__.py
+-rw-r--r--   0        0        0     8846 2024-04-12 19:25:16.709746 fairness_datasets-0.2.1/fairnessdatasets/adult.py
+-rw-r--r--   0        0        0    15339 2024-04-12 20:02:47.287823 fairness_datasets-0.2.1/fairnessdatasets/base.py
+-rw-r--r--   0        0        0     5397 2024-04-12 15:59:57.756084 fairness_datasets-0.2.1/fairnessdatasets/default.py
+-rw-r--r--   0        0        0     6476 2024-04-17 13:06:56.685391 fairness_datasets-0.2.1/fairnessdatasets/law_school.py
+-rw-r--r--   0        0        0     7062 2024-04-12 16:06:33.386637 fairness_datasets-0.2.1/fairnessdatasets/south_german.py
+-rw-r--r--   0        0        0      783 2024-02-01 14:45:15.232276 fairness_datasets-0.2.1/noxfile.py
+-rw-r--r--   0        0        0     1148 2024-04-12 15:36:24.293920 fairness_datasets-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1463 2024-04-12 19:37:07.507233 fairness_datasets-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     3980 2024-04-12 19:50:13.029406 fairness_datasets-0.2.1/tests/test_column_indices.py
+-rw-r--r--   0        0        0     1837 2024-04-17 12:40:40.261954 fairness_datasets-0.2.1/tests/test_download.py
+-rw-r--r--   0        0        0      587 2024-04-12 12:55:35.731613 fairness_datasets-0.2.1/tests/test_output.py
+-rw-r--r--   0        0        0     1658 2024-04-12 19:50:13.045406 fairness_datasets-0.2.1/tests/test_shapes.py
+-rw-r--r--   0        0        0     1318 2024-04-12 15:51:37.738349 fairness_datasets-0.2.1/tests/test_use.py
+-rw-r--r--   0        0        0     3513 1970-01-01 00:00:00.000000 fairness_datasets-0.2.1/PKG-INFO
```

### Comparing `fairness_datasets-0.2.0/.gitignore` & `fairness_datasets-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/LICENSE` & `fairness_datasets-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/README.md` & `fairness_datasets-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/fairnessdatasets/adult.py` & `fairness_datasets-0.2.1/fairnessdatasets/adult.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/fairnessdatasets/base.py` & `fairness_datasets-0.2.1/fairnessdatasets/base.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/fairnessdatasets/default.py` & `fairness_datasets-0.2.1/fairnessdatasets/default.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/fairnessdatasets/law_school.py` & `fairness_datasets-0.2.1/fairnessdatasets/law_school.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         ),
         "gpa": None,
     }
 
     def __init__(
         self,
         root: Union[str, os.PathLike],
-        features: Tuple[str] = ("lsat", "zgpa", "zfygpa", "gender", "race1"),
+        features: Tuple[str, ...] = ("lsat", "zgpa", "zfygpa", "gender", "race1"),
         target: str = "pass_bar",
         raw: bool = False,
         download: bool = False,
         output_fn: Optional[Callable[[str], None]] = print,
     ):
         """
         Loads the `Law School <https://eric.ed.gov/?id=ED469370>`_ dataset.
```

### Comparing `fairness_datasets-0.2.0/fairnessdatasets/south_german.py` & `fairness_datasets-0.2.1/fairnessdatasets/south_german.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/noxfile.py` & `fairness_datasets-0.2.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/pyproject.toml` & `fairness_datasets-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/tests/conftest.py` & `fairness_datasets-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/tests/test_column_indices.py` & `fairness_datasets-0.2.1/tests/test_column_indices.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/tests/test_download.py` & `fairness_datasets-0.2.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/tests/test_output.py` & `fairness_datasets-0.2.1/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/tests/test_shapes.py` & `fairness_datasets-0.2.1/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/tests/test_use.py` & `fairness_datasets-0.2.1/tests/test_use.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.0/PKG-INFO` & `fairness_datasets-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairness-datasets
-Version: 0.2.0
+Version: 0.2.1
 Summary: PyTorch dataset wrapper for the
 Keywords: PyTorch,Dataset,Fairness,Adult,Census Income,Law School
 Author-email: David Boetius <david.boetius@uni-konstanz.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

