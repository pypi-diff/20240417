# Comparing `tmp/pyam_iamc-2.2.0.tar.gz` & `tmp/pyam_iamc-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyam_iamc-2.2.0.tar", max compression
+gzip compressed data, was "pyam_iamc-2.2.1.tar", max compression
```

## Comparing `pyam_iamc-2.2.0.tar` & `pyam_iamc-2.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1591 2024-03-21 12:28:09.585996 pyam_iamc-2.2.0/AUTHORS.rst
--rw-r--r--   0        0        0    10141 2024-03-21 12:28:09.589996 pyam_iamc-2.2.0/LICENSE
--rw-r--r--   0        0        0      605 2024-03-21 12:28:09.589996 pyam_iamc-2.2.0/NOTICE.md
--rw-r--r--   0        0        0     7626 2024-03-21 12:28:09.589996 pyam_iamc-2.2.0/README.md
--rw-r--r--   0        0        0      892 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/__init__.py
--rw-r--r--   0        0        0      622 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/_compare.py
--rw-r--r--   0        0        0      423 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/_debiasing.py
--rw-r--r--   0        0        0     6959 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/_ops.py
--rw-r--r--   0        0        0     3630 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/_style.py
--rw-r--r--   0        0        0     9863 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/aggregation.py
--rw-r--r--   0        0        0     9929 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/compute.py
--rwxr-xr-x   0        0        0   108859 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/core.py
--rwxr-xr-x   0        0        0     2572 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/figures.py
--rw-r--r--   0        0        0     3922 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/filter.py
--rw-r--r--   0        0        0    26714 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/iiasa.py
--rw-r--r--   0        0        0     4070 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/index.py
--rw-r--r--   0        0        0     4206 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/ixmp4.py
--rw-r--r--   0        0        0      466 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/logging.conf
--rw-r--r--   0        0        0     1391 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/logging.py
--rw-r--r--   0        0        0    40912 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/plotting.py
--rw-r--r--   0        0        0     4022 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/run_control.py
--rw-r--r--   0        0        0     2557 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/slice.py
--rw-r--r--   0        0        0    12102 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/statistics.py
--rw-r--r--   0        0        0     4448 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/str.py
--rw-r--r--   0        0        0     1050 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/testing.py
--rw-r--r--   0        0        0     2820 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/time.py
--rw-r--r--   0        0        0     5643 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/timeseries.py
--rw-r--r--   0        0        0     5261 2024-03-21 12:28:09.609995 pyam_iamc-2.2.0/pyam/unfccc.py
--rw-r--r--   0        0        0     4711 2024-03-21 12:28:09.613995 pyam_iamc-2.2.0/pyam/units.py
--rw-r--r--   0        0        0    21225 2024-03-21 12:28:09.613995 pyam_iamc-2.2.0/pyam/utils.py
--rw-r--r--   0        0        0     4592 2024-03-21 12:28:09.613995 pyam_iamc-2.2.0/pyam/validation.py
--rw-r--r--   0        0        0     2322 2024-03-21 12:28:09.613995 pyam_iamc-2.2.0/pyam/worldbank.py
--rw-r--r--   0        0        0     4405 2024-03-21 12:28:27.385841 pyam_iamc-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     8995 1970-01-01 00:00:00.000000 pyam_iamc-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1591 2024-04-17 10:12:28.770833 pyam_iamc-2.2.1/AUTHORS.rst
+-rw-r--r--   0        0        0    10141 2024-04-17 10:12:28.770833 pyam_iamc-2.2.1/LICENSE
+-rw-r--r--   0        0        0      605 2024-04-17 10:12:28.770833 pyam_iamc-2.2.1/NOTICE.md
+-rw-r--r--   0        0        0     7626 2024-04-17 10:12:28.770833 pyam_iamc-2.2.1/README.md
+-rw-r--r--   0        0        0      892 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/__init__.py
+-rw-r--r--   0        0        0      622 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/_compare.py
+-rw-r--r--   0        0        0      423 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/_debiasing.py
+-rw-r--r--   0        0        0     6959 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/_ops.py
+-rw-r--r--   0        0        0     3630 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/_style.py
+-rw-r--r--   0        0        0     9863 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/aggregation.py
+-rw-r--r--   0        0        0     9929 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/compute.py
+-rwxr-xr-x   0        0        0   108859 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/core.py
+-rwxr-xr-x   0        0        0     2572 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/figures.py
+-rw-r--r--   0        0        0     3922 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/filter.py
+-rw-r--r--   0        0        0    26714 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/iiasa.py
+-rw-r--r--   0        0        0     4070 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/index.py
+-rw-r--r--   0        0        0     4206 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/ixmp4.py
+-rw-r--r--   0        0        0      466 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/logging.conf
+-rw-r--r--   0        0        0     1391 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/logging.py
+-rw-r--r--   0        0        0    40912 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/plotting.py
+-rw-r--r--   0        0        0     4022 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/run_control.py
+-rw-r--r--   0        0        0     2557 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/slice.py
+-rw-r--r--   0        0        0    12102 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/statistics.py
+-rw-r--r--   0        0        0     4448 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/str.py
+-rw-r--r--   0        0        0     1050 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/testing.py
+-rw-r--r--   0        0        0     2820 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/time.py
+-rw-r--r--   0        0        0     5643 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/timeseries.py
+-rw-r--r--   0        0        0     5261 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/unfccc.py
+-rw-r--r--   0        0        0     4711 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/units.py
+-rw-r--r--   0        0        0    21224 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/utils.py
+-rw-r--r--   0        0        0     4592 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/validation.py
+-rw-r--r--   0        0        0     2322 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/worldbank.py
+-rw-r--r--   0        0        0     4426 2024-04-17 10:12:49.390940 pyam_iamc-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9029 1970-01-01 00:00:00.000000 pyam_iamc-2.2.1/PKG-INFO
```

### Comparing `pyam_iamc-2.2.0/AUTHORS.rst` & `pyam_iamc-2.2.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/LICENSE` & `pyam_iamc-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/NOTICE.md` & `pyam_iamc-2.2.1/NOTICE.md`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/README.md` & `pyam_iamc-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/__init__.py` & `pyam_iamc-2.2.1/pyam/__init__.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/_compare.py` & `pyam_iamc-2.2.1/pyam/_compare.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/_ops.py` & `pyam_iamc-2.2.1/pyam/_ops.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/_style.py` & `pyam_iamc-2.2.1/pyam/_style.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/aggregation.py` & `pyam_iamc-2.2.1/pyam/aggregation.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/compute.py` & `pyam_iamc-2.2.1/pyam/compute.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/core.py` & `pyam_iamc-2.2.1/pyam/core.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/figures.py` & `pyam_iamc-2.2.1/pyam/figures.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/filter.py` & `pyam_iamc-2.2.1/pyam/filter.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/iiasa.py` & `pyam_iamc-2.2.1/pyam/iiasa.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/index.py` & `pyam_iamc-2.2.1/pyam/index.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/ixmp4.py` & `pyam_iamc-2.2.1/pyam/ixmp4.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/logging.py` & `pyam_iamc-2.2.1/pyam/logging.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/plotting.py` & `pyam_iamc-2.2.1/pyam/plotting.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/run_control.py` & `pyam_iamc-2.2.1/pyam/run_control.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/slice.py` & `pyam_iamc-2.2.1/pyam/slice.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/statistics.py` & `pyam_iamc-2.2.1/pyam/statistics.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/str.py` & `pyam_iamc-2.2.1/pyam/str.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/testing.py` & `pyam_iamc-2.2.1/pyam/testing.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/time.py` & `pyam_iamc-2.2.1/pyam/time.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/timeseries.py` & `pyam_iamc-2.2.1/pyam/timeseries.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/unfccc.py` & `pyam_iamc-2.2.1/pyam/unfccc.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/units.py` & `pyam_iamc-2.2.1/pyam/units.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/utils.py` & `pyam_iamc-2.2.1/pyam/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     df.to_excel(writer, name, index=False)
     for i, col in enumerate(df.columns):
         if df.dtypes[col].name.startswith(("float", "int")):
             width = len(str(col)) + 2
         else:
             width = min(
                 max([df[col].map(lambda x: len(str(x or "None"))).max(), len(col)]) + 2,
-                100,  # make sure that column width is not too large
+                80,  # make sure that column width is not too large
             )
         writer.sheets[name].set_column(i, i, width)  # assumes xlsxwriter as engine
 
 
 def read_pandas(path, sheet_name=["data*", "Data*"], *args, **kwargs):
     """Read a file and return a pandas.DataFrame"""
```

### Comparing `pyam_iamc-2.2.0/pyam/validation.py` & `pyam_iamc-2.2.1/pyam/validation.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyam/worldbank.py` & `pyam_iamc-2.2.1/pyam/worldbank.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.0/pyproject.toml` & `pyam_iamc-2.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyam-iamc"
-version = "2.2.0"
+version = "2.2.1"
 description = "Analysis & visualization of integrated-assessment scenarios"
 authors = [
     "Matthew Gidden <gidden@iiasa.ac.at>",
     "Daniel Huppmann <huppmann@iiasa.ac.at>",
     "Zebedee Nicholls <znicholls@unknown.com>",
     "Nikolay Kushin <zikolach@unknown.com>",
     "Robin Lamboll <Rlamboll@unknown.com>",
@@ -50,16 +50,17 @@
 openpyxl = ">=3.1.2"
 pandas = ">=2.1.2"
 Pint = ">=0.13"
 PyYAML = ">=6.0.1"
 scipy = ">=1.10.0"
 seaborn = ">=0.11"
 six = ">=1.16.0"
+requests = ">2.27.1"
 wquantiles = ">=0.6"
-XlsxWriter = ">=3.2.0"
+XlsxWriter = ">=3.0.3"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ruff = ">=0.2.1"
 coverage = ">=6.5.0"
```

### Comparing `pyam_iamc-2.2.0/PKG-INFO` & `pyam_iamc-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyam-iamc
-Version: 2.2.0
+Version: 2.2.1
 Summary: Analysis & visualization of integrated-assessment scenarios
 Home-page: https://github.com/IAMconsortium/pyam
 License: Apache-2.0
 Author: Matthew Gidden
 Author-email: gidden@iiasa.ac.at
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,21 +15,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: Pint (>=0.13)
 Requires-Dist: PyYAML (>=6.0.1)
-Requires-Dist: XlsxWriter (>=3.2.0)
+Requires-Dist: XlsxWriter (>=3.0.3)
 Requires-Dist: iam-units (>=2020.4.21)
 Requires-Dist: ixmp4 (>=0.8.0)
 Requires-Dist: matplotlib (>=3.6.0)
 Requires-Dist: numpy (>=1.26.0)
 Requires-Dist: openpyxl (>=3.1.2)
 Requires-Dist: pandas (>=2.1.2)
+Requires-Dist: requests (>2.27.1)
 Requires-Dist: scipy (>=1.10.0)
 Requires-Dist: seaborn (>=0.11)
 Requires-Dist: six (>=1.16.0)
 Requires-Dist: wquantiles (>=0.6)
 Project-URL: Documentation, https://pyam-iamc.readthedocs.io
 Project-URL: Repository, https://github.com/IAMconsortium/pyam
 Description-Content-Type: text/markdown
```

