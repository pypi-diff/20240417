# Comparing `tmp/pyield-0.7.1.tar.gz` & `tmp/pyield-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyield-0.7.1.tar", last modified: Tue Apr 16 12:02:47 2024, max compression
+gzip compressed data, was "pyield-0.7.2.tar", last modified: Wed Apr 17 08:53:02 2024, max compression
```

## Comparing `pyield-0.7.1.tar` & `pyield-0.7.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.1/LICENSE
--rw-r--r--   0        0        0     5168 2024-04-16 12:01:55.675922 pyield-0.7.1/README.md
--rw-r--r--   0        0        0       22 2024-04-16 12:01:55.675922 pyield-0.7.1/pyield/__about__.py
--rw-r--r--   0        0        0      380 2024-04-14 09:19:55.868897 pyield-0.7.1/pyield/__init__.py
--rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.1/pyield/bday.py
--rw-r--r--   0        0        0     3446 2024-04-16 12:01:55.675922 pyield-0.7.1/pyield/data_access.py
--rw-r--r--   0        0        0     1250 2024-04-13 12:39:44.026704 pyield-0.7.1/pyield/data_analysis.py
--rw-r--r--   0        0        0      223 2024-04-16 12:01:55.675922 pyield-0.7.1/pyield/futures/__init__.py
--rw-r--r--   0        0        0     5615 2024-04-16 12:01:55.676922 pyield-0.7.1/pyield/futures/common.py
--rw-r--r--   0        0        0     5816 2024-04-16 12:01:55.676922 pyield-0.7.1/pyield/futures/ddi.py
--rw-r--r--   0        0        0     5847 2024-04-16 12:01:55.676922 pyield-0.7.1/pyield/futures/di.py
--rw-r--r--   0        0        0    11530 2024-04-16 12:01:55.676922 pyield-0.7.1/pyield/futures/di_xml.py
--rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.1/pyield/holidays/__init__.py
--rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.1/pyield/holidays/br_holidays_new.txt
--rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.1/pyield/holidays/br_holidays_old.txt
--rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.1/pyield/holidays/core.py
--rw-r--r--   0        0        0     2273 2024-04-14 11:04:04.016185 pyield-0.7.1/pyield/indicators.py
--rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.1/pyield/py.typed
--rw-r--r--   0        0        0     6612 2024-04-16 12:01:55.676922 pyield-0.7.1/pyield/treasuries.py
--rw-r--r--   0        0        0     2111 2024-04-14 09:43:03.423065 pyield-0.7.1/pyield/utils.py
--rw-r--r--   0        0        0     1165 2024-04-16 12:02:47.053532 pyield-0.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.1/tests/test_bday.py
--rw-r--r--   0        0        0     2554 2024-04-16 12:01:55.677922 pyield-0.7.1/tests/test_futures.py
--rw-r--r--   0        0        0     7185 1970-01-01 00:00:00.000000 pyield-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.2/LICENSE
+-rw-r--r--   0        0        0     5168 2024-04-16 12:01:55.675922 pyield-0.7.2/README.md
+-rw-r--r--   0        0        0       22 2024-04-17 08:50:38.480980 pyield-0.7.2/pyield/__about__.py
+-rw-r--r--   0        0        0      380 2024-04-14 09:19:55.868897 pyield-0.7.2/pyield/__init__.py
+-rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.2/pyield/bday.py
+-rw-r--r--   0        0        0     3446 2024-04-16 12:01:55.675922 pyield-0.7.2/pyield/data_access.py
+-rw-r--r--   0        0        0     1276 2024-04-17 08:50:12.086620 pyield-0.7.2/pyield/data_analysis.py
+-rw-r--r--   0        0        0      223 2024-04-16 12:01:55.675922 pyield-0.7.2/pyield/futures/__init__.py
+-rw-r--r--   0        0        0     5615 2024-04-16 12:01:55.676922 pyield-0.7.2/pyield/futures/common.py
+-rw-r--r--   0        0        0     5816 2024-04-16 12:01:55.676922 pyield-0.7.2/pyield/futures/ddi.py
+-rw-r--r--   0        0        0     5847 2024-04-16 12:01:55.676922 pyield-0.7.2/pyield/futures/di.py
+-rw-r--r--   0        0        0    11530 2024-04-16 12:01:55.676922 pyield-0.7.2/pyield/futures/di_xml.py
+-rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.2/pyield/holidays/__init__.py
+-rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.2/pyield/holidays/br_holidays_new.txt
+-rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.2/pyield/holidays/br_holidays_old.txt
+-rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.2/pyield/holidays/core.py
+-rw-r--r--   0        0        0     2273 2024-04-14 11:04:04.016185 pyield-0.7.2/pyield/indicators.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.2/pyield/py.typed
+-rw-r--r--   0        0        0     6612 2024-04-16 12:01:55.676922 pyield-0.7.2/pyield/treasuries.py
+-rw-r--r--   0        0        0     2111 2024-04-14 09:43:03.423065 pyield-0.7.2/pyield/utils.py
+-rw-r--r--   0        0        0     1165 2024-04-17 08:53:02.132938 pyield-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.2/tests/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.2/tests/test_bday.py
+-rw-r--r--   0        0        0     2554 2024-04-16 12:01:55.677922 pyield-0.7.2/tests/test_futures.py
+-rw-r--r--   0        0        0     7185 1970-01-01 00:00:00.000000 pyield-0.7.2/PKG-INFO
```

### Comparing `pyield-0.7.1/LICENSE` & `pyield-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/README.md` & `pyield-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/pyield/bday.py` & `pyield-0.7.2/pyield/bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/pyield/data_access.py` & `pyield-0.7.2/pyield/data_access.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/pyield/data_analysis.py` & `pyield-0.7.2/pyield/data_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import pandas as pd
 
 from . import treasuries as tr
 from .utils import _normalize_date
 
 
-def calculate_spreads(spread_type: str, reference_date: pd.Timestamp) -> pd.DataFrame:
+def calculate_spreads(
+    spread_type: str, reference_date: str | pd.Timestamp | None = None
+) -> pd.DataFrame:
     """
     Calculates spreads between assets based on the specified spread type.
     If no reference date is provided, the function uses the previous business day.
 
     Parameters:
         spread_type (str): The type of spread to calculate. Available options are:
             - "DI_vs_PRE": the spread between DI Futures and Treasury Pre-Fixed bonds.
```

### Comparing `pyield-0.7.1/pyield/futures/common.py` & `pyield-0.7.2/pyield/futures/common.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/pyield/futures/ddi.py` & `pyield-0.7.2/pyield/futures/ddi.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/pyield/futures/di.py` & `pyield-0.7.2/pyield/futures/di.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/pyield/futures/di_xml.py` & `pyield-0.7.2/pyield/futures/di_xml.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/pyield/holidays/br_holidays_new.txt` & `pyield-0.7.2/pyield/holidays/br_holidays_new.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/pyield/holidays/br_holidays_old.txt` & `pyield-0.7.2/pyield/holidays/br_holidays_old.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/pyield/holidays/core.py` & `pyield-0.7.2/pyield/holidays/core.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/pyield/indicators.py` & `pyield-0.7.2/pyield/indicators.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/pyield/treasuries.py` & `pyield-0.7.2/pyield/treasuries.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/pyield/utils.py` & `pyield-0.7.2/pyield/utils.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/pyproject.toml` & `pyield-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "pandas>=2.0.0",
     "numpy",
     "beautifulsoup4",
     "html5lib",
     "lxml",
 ]
 dynamic = []
-version = "0.7.1"
+version = "0.7.2"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/crdcj/PYield"
```

### Comparing `pyield-0.7.1/tests/test_bday.py` & `pyield-0.7.2/tests/test_bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/tests/test_futures.py` & `pyield-0.7.2/tests/test_futures.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.1/PKG-INFO` & `pyield-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PYield
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Python library for analysis of fixed income instruments in Brazil
 Keywords: fixed-income, brazil, finance, analysis, bonds
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Carlos Carvalho
```

