# Comparing `tmp/hidrokit-0.5.0.tar.gz` & `tmp/hidrokit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hidrokit-0.5.0.tar", last modified: Tue Apr 16 04:31:49 2024, max compression
+gzip compressed data, was "hidrokit-0.5.1.tar", last modified: Wed Apr 17 14:54:39 2024, max compression
```

## Comparing `hidrokit-0.5.0.tar` & `hidrokit-0.5.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.520059 hidrokit-0.5.0/
--rw-rw-rw-   0        0        0     6060 2024-04-14 07:31:59.000000 hidrokit-0.5.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    15622 2024-04-11 05:03:58.000000 hidrokit-0.5.0/CHANGELOG_gen.md
--rw-rw-rw-   0        0        0     6464 2024-04-14 07:31:59.000000 hidrokit-0.5.0/CHANGELOG_old.md
--rw-rw-rw-   0        0        0     3369 2024-04-11 05:03:58.000000 hidrokit-0.5.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0      128 2024-04-11 05:03:58.000000 hidrokit-0.5.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1109 2024-04-14 07:31:59.000000 hidrokit-0.5.0/LICENSE.txt
--rw-rw-rw-   0        0        0      141 2024-04-11 05:03:58.000000 hidrokit-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5958 2024-04-16 04:31:49.518831 hidrokit-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     4628 2024-04-14 07:31:59.000000 hidrokit-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.409858 hidrokit-0.5.0/hidrokit/
--rw-rw-rw-   0        0        0      299 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-14 07:31:59.000000 hidrokit-0.5.0/hidrokit/__version__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.449004 hidrokit-0.5.0/hidrokit/analysis/
--rw-rw-rw-   0        0        0        0 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.450409 hidrokit-0.5.0/hidrokit/contrib/
--rw-rw-rw-   0        0        0       46 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.494658 hidrokit-0.5.0/hidrokit/contrib/taruma/
--rw-rw-rw-   0        0        0     2436 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/__init__.py
--rw-rw-rw-   0        0        0      549 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/anfrek.py
--rw-rw-rw-   0        0        0     9158 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/bmkg_utils.py
--rw-rw-rw-   0        0        0    11048 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/chi_square.py
--rw-rw-rw-   0        0        0     4218 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/dataframe_to_tensor.py
--rw-rw-rw-   0        0        0     4657 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/dependable_flow.py
--rw-rw-rw-   0        0        0    20229 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/evapotranspiration.py
--rw-rw-rw-   0        0        0     6927 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/fjmock_model.py
--rw-rw-rw-   0        0        0    18688 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/gumbel.py
--rw-rw-rw-   0        0        0     8396 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/hidrokit_excel_parser.py
--rw-rw-rw-   0        0        0     6021 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/hidrokit_hourly_excel_parser.py
--rw-rw-rw-   0        0        0     9264 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/kolmogorov_smirnov.py
--rw-rw-rw-   0        0        0     7290 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/lognormal.py
--rw-rw-rw-   0        0        0    24565 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/logpearson3.py
--rw-rw-rw-   0        0        0     3293 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/model_calibration.py
--rw-rw-rw-   0        0        0     8668 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/normal.py
--rw-rw-rw-   0        0        0     8127 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/nreca_model.py
--rw-rw-rw-   0        0        0     6436 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/outlier_hydrology.py
--rw-rw-rw-   0        0        0    11543 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/pamarayan_excel_data_extraction.py
--rw-rw-rw-   0        0        0     3827 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/statistic_summary.py
--rw-rw-rw-   0        0        0     4156 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/statistical_coefficients.py
--rw-rw-rw-   0        0        0     5752 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/summary_hourly.py
--rw-rw-rw-   0        0        0     2484 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/thiessen.py
--rw-rw-rw-   0        0        0      411 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/ujidist.py
--rw-rw-rw-   0        0        0     3469 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/upsampling.py
--rw-rw-rw-   0        0        0     1667 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.500779 hidrokit-0.5.0/hidrokit/prep/
--rw-rw-rw-   0        0        0       86 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/prep/__init__.py
--rw-rw-rw-   0        0        0     3931 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/prep/excel.py
--rw-rw-rw-   0        0        0     2217 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/prep/read.py
--rw-rw-rw-   0        0        0     4217 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/prep/timeseries.py
-drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.506052 hidrokit-0.5.0/hidrokit/viz/
--rw-rw-rw-   0        0        0       62 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/viz/__init__.py
--rw-rw-rw-   0        0        0     1286 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/viz/graph.py
--rw-rw-rw-   0        0        0     1253 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/viz/table.py
-drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.447448 hidrokit-0.5.0/hidrokit.egg-info/
--rw-rw-rw-   0        0        0     5958 2024-04-16 04:31:49.000000 hidrokit-0.5.0/hidrokit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1778 2024-04-16 04:31:49.000000 hidrokit-0.5.0/hidrokit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 04:31:49.000000 hidrokit-0.5.0/hidrokit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2024-04-16 04:31:49.000000 hidrokit-0.5.0/hidrokit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-16 04:31:49.000000 hidrokit-0.5.0/hidrokit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2024-04-16 04:31:49.528183 hidrokit-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     3134 2024-04-14 07:33:33.000000 hidrokit-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.514300 hidrokit-0.5.0/tests/
--rw-rw-rw-   0        0        0     1797 2024-04-11 05:03:58.000000 hidrokit-0.5.0/tests/test_prep_excel.py
--rw-rw-rw-   0        0        0      844 2024-04-11 05:03:58.000000 hidrokit-0.5.0/tests/test_prep_read.py
--rw-rw-rw-   0        0        0     5086 2024-04-11 05:03:58.000000 hidrokit-0.5.0/tests/test_prep_timeseries.py
--rw-rw-rw-   0        0        0      477 2024-04-11 05:03:58.000000 hidrokit-0.5.0/tests/test_viz_graph.py
--rw-rw-rw-   0        0        0     1632 2024-04-11 05:03:58.000000 hidrokit-0.5.0/tests/test_viz_table.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.541784 hidrokit-0.5.1/
+-rw-rw-rw-   0        0        0     6060 2024-04-14 07:31:59.000000 hidrokit-0.5.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0    15622 2024-04-11 05:03:58.000000 hidrokit-0.5.1/CHANGELOG_gen.md
+-rw-rw-rw-   0        0        0     6464 2024-04-14 07:31:59.000000 hidrokit-0.5.1/CHANGELOG_old.md
+-rw-rw-rw-   0        0        0     3369 2024-04-11 05:03:58.000000 hidrokit-0.5.1/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0      128 2024-04-11 05:03:58.000000 hidrokit-0.5.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1109 2024-04-14 07:31:59.000000 hidrokit-0.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      141 2024-04-11 05:03:58.000000 hidrokit-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5956 2024-04-17 14:54:39.541784 hidrokit-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4626 2024-04-16 06:22:26.000000 hidrokit-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.466771 hidrokit-0.5.1/hidrokit/
+-rw-rw-rw-   0        0        0      299 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-17 14:53:46.000000 hidrokit-0.5.1/hidrokit/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.480399 hidrokit-0.5.1/hidrokit/analysis/
+-rw-rw-rw-   0        0        0        0 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.481393 hidrokit-0.5.1/hidrokit/contrib/
+-rw-rw-rw-   0        0        0       46 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.520721 hidrokit-0.5.1/hidrokit/contrib/taruma/
+-rw-rw-rw-   0        0        0     2436 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/__init__.py
+-rw-rw-rw-   0        0        0      549 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/anfrek.py
+-rw-rw-rw-   0        0        0     9158 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/bmkg_utils.py
+-rw-rw-rw-   0        0        0    11049 2024-04-17 14:41:16.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/chi_square.py
+-rw-rw-rw-   0        0        0     4218 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/dataframe_to_tensor.py
+-rw-rw-rw-   0        0        0     4657 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/dependable_flow.py
+-rw-rw-rw-   0        0        0    20229 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/evapotranspiration.py
+-rw-rw-rw-   0        0        0     6927 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/fjmock_model.py
+-rw-rw-rw-   0        0        0    18688 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/gumbel.py
+-rw-rw-rw-   0        0        0     8396 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/hidrokit_excel_parser.py
+-rw-rw-rw-   0        0        0     6021 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/hidrokit_hourly_excel_parser.py
+-rw-rw-rw-   0        0        0     9264 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/kolmogorov_smirnov.py
+-rw-rw-rw-   0        0        0     7815 2024-04-17 14:41:16.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/lognormal.py
+-rw-rw-rw-   0        0        0    24565 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/logpearson3.py
+-rw-rw-rw-   0        0        0     3293 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/model_calibration.py
+-rw-rw-rw-   0        0        0     8668 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/normal.py
+-rw-rw-rw-   0        0        0     8127 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/nreca_model.py
+-rw-rw-rw-   0        0        0     6436 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/outlier_hydrology.py
+-rw-rw-rw-   0        0        0    11543 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/pamarayan_excel_data_extraction.py
+-rw-rw-rw-   0        0        0     3827 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/statistic_summary.py
+-rw-rw-rw-   0        0        0     4156 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/statistical_coefficients.py
+-rw-rw-rw-   0        0        0     5752 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/summary_hourly.py
+-rw-rw-rw-   0        0        0     2484 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/thiessen.py
+-rw-rw-rw-   0        0        0      411 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/ujidist.py
+-rw-rw-rw-   0        0        0     3469 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/upsampling.py
+-rw-rw-rw-   0        0        0     1667 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.526234 hidrokit-0.5.1/hidrokit/prep/
+-rw-rw-rw-   0        0        0       86 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/prep/__init__.py
+-rw-rw-rw-   0        0        0     3931 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/prep/excel.py
+-rw-rw-rw-   0        0        0     2217 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/prep/read.py
+-rw-rw-rw-   0        0        0     4217 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/prep/timeseries.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.531237 hidrokit-0.5.1/hidrokit/viz/
+-rw-rw-rw-   0        0        0       62 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/viz/__init__.py
+-rw-rw-rw-   0        0        0     1286 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/viz/graph.py
+-rw-rw-rw-   0        0        0     1253 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/viz/table.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.478355 hidrokit-0.5.1/hidrokit.egg-info/
+-rw-rw-rw-   0        0        0     5956 2024-04-17 14:54:39.000000 hidrokit-0.5.1/hidrokit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1778 2024-04-17 14:54:39.000000 hidrokit-0.5.1/hidrokit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 14:54:39.000000 hidrokit-0.5.1/hidrokit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-04-17 14:54:39.000000 hidrokit-0.5.1/hidrokit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-17 14:54:39.000000 hidrokit-0.5.1/hidrokit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2024-04-17 14:54:39.544407 hidrokit-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     3134 2024-04-14 07:33:33.000000 hidrokit-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.538789 hidrokit-0.5.1/tests/
+-rw-rw-rw-   0        0        0     1797 2024-04-11 05:03:58.000000 hidrokit-0.5.1/tests/test_prep_excel.py
+-rw-rw-rw-   0        0        0      844 2024-04-11 05:03:58.000000 hidrokit-0.5.1/tests/test_prep_read.py
+-rw-rw-rw-   0        0        0     5086 2024-04-11 05:03:58.000000 hidrokit-0.5.1/tests/test_prep_timeseries.py
+-rw-rw-rw-   0        0        0      477 2024-04-11 05:03:58.000000 hidrokit-0.5.1/tests/test_viz_graph.py
+-rw-rw-rw-   0        0        0     1632 2024-04-11 05:03:58.000000 hidrokit-0.5.1/tests/test_viz_table.py
```

### Comparing `hidrokit-0.5.0/CHANGELOG.md` & `hidrokit-0.5.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/CHANGELOG_gen.md` & `hidrokit-0.5.1/CHANGELOG_gen.md`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/CHANGELOG_old.md` & `hidrokit-0.5.1/CHANGELOG_old.md`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/CODE_OF_CONDUCT.md` & `hidrokit-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/LICENSE.txt` & `hidrokit-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/PKG-INFO` & `hidrokit-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidrokit
-Version: 0.5.0
+Version: 0.5.1
 Summary: analisis hidrologi dengan python
 Home-page: https://github.com/hidrokit/hidrokit
 Author: Taruma Sakti Megariansyah
 Author-email: hi@taruma.info
 License: MIT
 Project-URL: Documentation, https://hidrokit.github.io/hidrokit
 Project-URL: ReadTheDocs, https://hidrokit.readthedocs.io/en/stable/
@@ -35,15 +35,15 @@
 
 
 <div align="center">
 <a href="https://hidrokit.github.io/hidrokit"><img src="https://hidrokit.github.io/hidrokit/assets/images/presskit/hidrokit-800x200-transparent.png" alt="logo hidrokit"></a><br>
 
 ![PyPI - Status](https://img.shields.io/pypi/status/hidrokit.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hidrokit.svg)
-[![GitHub license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://github.com/hidrokit/hidrokit/blob/master/LICENSE)
+[![GitHub license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://github.com/hidrokit/hidrokit/blob/main/LICENSE)
 [![DOI](https://zenodo.org/badge/145389179.svg)](https://zenodo.org/badge/latestdoi/145389179)
 
 <a href="https://hidrokit.github.io/hidrokit"><b>Kunjungi situs resmi hidrokit.</b></a>
 </div>
 
 `hidrokit` adalah proyek _open source_ paket *python* yang dapat digunakan untuk membantu proses analisis hidrologi dimulai dari pengolahan data, analisis data, dan visualisasi data. [Baca lebih lanjut mengenai hidrokit](https://hidrokit.github.io/hidrokit/tentang-hidrokit).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hidrokit Version: 0.5.0 Summary: analisis hidrologi
+Metadata-Version: 2.1 Name: hidrokit Version: 0.5.1 Summary: analisis hidrologi
 dengan python Home-page: https://github.com/hidrokit/hidrokit Author: Taruma
 Sakti Megariansyah Author-email: hi@taruma.info License: MIT Project-URL:
 Documentation, https://hidrokit.github.io/hidrokit Project-URL: ReadTheDocs,
 https://hidrokit.readthedocs.io/en/stable/ Project-URL: Bug Reports, https://
 github.com/hidrokit/hidrokit/issues Project-URL: Source, https://github.com/
 hidrokit/hidrokit/ Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
@@ -15,15 +15,15 @@
 numpy>=1.25 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.11 Requires-
 Dist: xlrd>=2.0 Provides-Extra: excel Requires-Dist: openpyxl; extra == "excel"
 Requires-Dist: xlrd; extra == "excel" Requires-Dist: xlwt; extra == "excel"
                                 _[_l_o_g_o_ _h_i_d_r_o_k_i_t_]
   ![PyPI - Status](https://img.shields.io/pypi/status/hidrokit.svg) ![PyPI -
 Python Version](https://img.shields.io/pypi/pyversions/hidrokit.svg) [![GitHub
 license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://
- github.com/hidrokit/hidrokit/blob/master/LICENSE) [![DOI](https://zenodo.org/
+  github.com/hidrokit/hidrokit/blob/main/LICENSE) [![DOI](https://zenodo.org/
  badge/145389179.svg)](https://zenodo.org/badge/latestdoi/145389179) _KK_uu_nn_jj_uu_nn_gg_ii
                              _ss_ii_tt_uu_ss_ _rr_ee_ss_mm_ii_ _hh_ii_dd_rr_oo_kk_ii_tt_..
 `hidrokit` adalah proyek _open source_ paket *python* yang dapat digunakan
 untuk membantu proses analisis hidrologi dimulai dari pengolahan data, analisis
 data, dan visualisasi data. [Baca lebih lanjut mengenai hidrokit](https://
 hidrokit.github.io/hidrokit/tentang-hidrokit). ## Release
 RReelleeaassee  PPyyPPII             GGiitthhuubb          GGiitthhuubb ((PPrree--rreelleeaassee))
```

### Comparing `hidrokit-0.5.0/README.md` & `hidrokit-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 <div align="center">
 <a href="https://hidrokit.github.io/hidrokit"><img src="https://hidrokit.github.io/hidrokit/assets/images/presskit/hidrokit-800x200-transparent.png" alt="logo hidrokit"></a><br>
 
 ![PyPI - Status](https://img.shields.io/pypi/status/hidrokit.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hidrokit.svg)
-[![GitHub license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://github.com/hidrokit/hidrokit/blob/master/LICENSE)
+[![GitHub license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://github.com/hidrokit/hidrokit/blob/main/LICENSE)
 [![DOI](https://zenodo.org/badge/145389179.svg)](https://zenodo.org/badge/latestdoi/145389179)
 
 <a href="https://hidrokit.github.io/hidrokit"><b>Kunjungi situs resmi hidrokit.</b></a>
 </div>
 
 `hidrokit` adalah proyek _open source_ paket *python* yang dapat digunakan untuk membantu proses analisis hidrologi dimulai dari pengolahan data, analisis data, dan visualisasi data. [Baca lebih lanjut mengenai hidrokit](https://hidrokit.github.io/hidrokit/tentang-hidrokit).
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
                                 _[_l_o_g_o_ _h_i_d_r_o_k_i_t_]
   ![PyPI - Status](https://img.shields.io/pypi/status/hidrokit.svg) ![PyPI -
 Python Version](https://img.shields.io/pypi/pyversions/hidrokit.svg) [![GitHub
 license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://
- github.com/hidrokit/hidrokit/blob/master/LICENSE) [![DOI](https://zenodo.org/
+  github.com/hidrokit/hidrokit/blob/main/LICENSE) [![DOI](https://zenodo.org/
  badge/145389179.svg)](https://zenodo.org/badge/latestdoi/145389179) _KK_uu_nn_jj_uu_nn_gg_ii
                              _ss_ii_tt_uu_ss_ _rr_ee_ss_mm_ii_ _hh_ii_dd_rr_oo_kk_ii_tt_..
 `hidrokit` adalah proyek _open source_ paket *python* yang dapat digunakan
 untuk membantu proses analisis hidrologi dimulai dari pengolahan data, analisis
 data, dan visualisasi data. [Baca lebih lanjut mengenai hidrokit](https://
 hidrokit.github.io/hidrokit/tentang-hidrokit). ## Release
 RReelleeaassee  PPyyPPII             GGiitthhuubb          GGiitthhuubb ((PPrree--rreelleeaassee))
```

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/__init__.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/__init__.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/anfrek.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/anfrek.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/bmkg_utils.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/bmkg_utils.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/chi_square.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/chi_square.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
     prob_class = 1 / k
     prob_list = np.linspace(0, 1, k + 1)[::-1]
     prob_seq = prob_list[1:-1]
 
     func = frequency_analysis_methods[distribution.lower()]
 
     T = 1 / prob_seq
-    val_x = func(data.x, return_period=T, source=distribution_source)
+    val_x = func(data.x, return_periods=T, source=distribution_source)
 
     # Chi Square Table
     calc_df = pd.DataFrame()
     min_value = data.x.min()
     max_value = data.x.max()
     seq_x = np.concatenate([[min_value], val_x, [max_value]])
```

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/dataframe_to_tensor.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/dataframe_to_tensor.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/dependable_flow.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/dependable_flow.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/evapotranspiration.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/evapotranspiration.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/fjmock_model.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/fjmock_model.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/gumbel.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/gumbel.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/hidrokit_excel_parser.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/hidrokit_excel_parser.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/hidrokit_hourly_excel_parser.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/hidrokit_hourly_excel_parser.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/kolmogorov_smirnov.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/kolmogorov_smirnov.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/lognormal.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/lognormal.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,40 +84,53 @@
         return_period = np.array(return_period)
         k_values = stats.norm.ppf(1 - 1 / return_period)
     else:
         raise ValueError(f"Unknown source: {source}")
     return k_values
 
 
-def calc_x_lognormal(x, return_period=None, source="scipy", show_stat=False):
+def calc_x_lognormal(
+    input_array, return_periods=None, source="scipy", display_stat=False, **kwargs
+):
     """
     Calculate the value of x for a given return period using the lognormal distribution.
 
     Parameters:
-        x (array-like): Input data array.
-        return_period (array-like, optional):
+        input_array (array-like): Input data array.
+        return_periods (array-like, optional):
             Return period(s) for which to calculate the value of x.
             Default is [5].
         source (str, optional): Source of the K factor.
             Default is "scipy".
-        show_stat (bool, optional): Whether to display the calculated statistics.
+        display_stat (bool, optional): Whether to display the calculated statistics.
             Default is False.
+        **kwargs: Additional keyword arguments for handling deprecated parameters.
 
     Returns:
         array-like: The calculated value(s) of x for the given return period(s).
     """
-    return_period = [5] if return_period is None else return_period
-    return_period = np.array(return_period)
-    y = np.log10(x)
+    # handle deprecated params
+    input_array = handle_deprecated_params(kwargs, "x", "input_array") or input_array
+    return_periods = (
+        handle_deprecated_params(kwargs, "return_period", "return_periods")
+        or return_periods
+    )
+    display_stat = (
+        handle_deprecated_params(kwargs, "show_stat", "display_stat") or display_stat
+    )
+
+    return_periods = [5] if return_periods is None else return_periods
+    return_periods = np.array(return_periods)
+    y = np.log10(input_array)
     y_mean = np.mean(y)
     y_std = np.std(y, ddof=1)
 
-    k = find_K(return_period, source=source)
+    k = find_K(return_periods, source=source)
 
-    if show_stat:
+    if display_stat:
         print(f"y_mean = {y_mean:.5f}")
         print(f"y_std = {y_std:.5f}")
         print(f"k = {k}")
 
     val_y = y_mean + k * y_std
     val_x = np.power(10, val_y)
     return val_x
@@ -180,15 +193,15 @@
     )
 
     target_column = dataframe.columns[0] if target_column is None else target_column
 
     x = dataframe[target_column].copy()
 
     arr = calc_x_lognormal(
-        x, return_period=return_periods, show_stat=display_stat, source=source
+        x, return_periods=return_periods, display_stat=display_stat, source=source
     )
 
     result = pd.DataFrame(data=arr, index=return_periods, columns=[out_column_name])
 
     result.index.name = out_index_name
     return result
```

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/logpearson3.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/logpearson3.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/model_calibration.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/model_calibration.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/normal.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/normal.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/nreca_model.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/nreca_model.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/outlier_hydrology.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/outlier_hydrology.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/pamarayan_excel_data_extraction.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/pamarayan_excel_data_extraction.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/statistic_summary.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/statistic_summary.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/statistical_coefficients.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/statistical_coefficients.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/summary_hourly.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/summary_hourly.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/thiessen.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/thiessen.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/upsampling.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/upsampling.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/contrib/taruma/utils.py` & `hidrokit-0.5.1/hidrokit/contrib/taruma/utils.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/prep/excel.py` & `hidrokit-0.5.1/hidrokit/prep/excel.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/prep/read.py` & `hidrokit-0.5.1/hidrokit/prep/read.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/prep/timeseries.py` & `hidrokit-0.5.1/hidrokit/prep/timeseries.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/viz/graph.py` & `hidrokit-0.5.1/hidrokit/viz/graph.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit/viz/table.py` & `hidrokit-0.5.1/hidrokit/viz/table.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/hidrokit.egg-info/PKG-INFO` & `hidrokit-0.5.1/hidrokit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidrokit
-Version: 0.5.0
+Version: 0.5.1
 Summary: analisis hidrologi dengan python
 Home-page: https://github.com/hidrokit/hidrokit
 Author: Taruma Sakti Megariansyah
 Author-email: hi@taruma.info
 License: MIT
 Project-URL: Documentation, https://hidrokit.github.io/hidrokit
 Project-URL: ReadTheDocs, https://hidrokit.readthedocs.io/en/stable/
@@ -35,15 +35,15 @@
 
 
 <div align="center">
 <a href="https://hidrokit.github.io/hidrokit"><img src="https://hidrokit.github.io/hidrokit/assets/images/presskit/hidrokit-800x200-transparent.png" alt="logo hidrokit"></a><br>
 
 ![PyPI - Status](https://img.shields.io/pypi/status/hidrokit.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hidrokit.svg)
-[![GitHub license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://github.com/hidrokit/hidrokit/blob/master/LICENSE)
+[![GitHub license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://github.com/hidrokit/hidrokit/blob/main/LICENSE)
 [![DOI](https://zenodo.org/badge/145389179.svg)](https://zenodo.org/badge/latestdoi/145389179)
 
 <a href="https://hidrokit.github.io/hidrokit"><b>Kunjungi situs resmi hidrokit.</b></a>
 </div>
 
 `hidrokit` adalah proyek _open source_ paket *python* yang dapat digunakan untuk membantu proses analisis hidrologi dimulai dari pengolahan data, analisis data, dan visualisasi data. [Baca lebih lanjut mengenai hidrokit](https://hidrokit.github.io/hidrokit/tentang-hidrokit).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hidrokit Version: 0.5.0 Summary: analisis hidrologi
+Metadata-Version: 2.1 Name: hidrokit Version: 0.5.1 Summary: analisis hidrologi
 dengan python Home-page: https://github.com/hidrokit/hidrokit Author: Taruma
 Sakti Megariansyah Author-email: hi@taruma.info License: MIT Project-URL:
 Documentation, https://hidrokit.github.io/hidrokit Project-URL: ReadTheDocs,
 https://hidrokit.readthedocs.io/en/stable/ Project-URL: Bug Reports, https://
 github.com/hidrokit/hidrokit/issues Project-URL: Source, https://github.com/
 hidrokit/hidrokit/ Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
@@ -15,15 +15,15 @@
 numpy>=1.25 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.11 Requires-
 Dist: xlrd>=2.0 Provides-Extra: excel Requires-Dist: openpyxl; extra == "excel"
 Requires-Dist: xlrd; extra == "excel" Requires-Dist: xlwt; extra == "excel"
                                 _[_l_o_g_o_ _h_i_d_r_o_k_i_t_]
   ![PyPI - Status](https://img.shields.io/pypi/status/hidrokit.svg) ![PyPI -
 Python Version](https://img.shields.io/pypi/pyversions/hidrokit.svg) [![GitHub
 license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://
- github.com/hidrokit/hidrokit/blob/master/LICENSE) [![DOI](https://zenodo.org/
+  github.com/hidrokit/hidrokit/blob/main/LICENSE) [![DOI](https://zenodo.org/
  badge/145389179.svg)](https://zenodo.org/badge/latestdoi/145389179) _KK_uu_nn_jj_uu_nn_gg_ii
                              _ss_ii_tt_uu_ss_ _rr_ee_ss_mm_ii_ _hh_ii_dd_rr_oo_kk_ii_tt_..
 `hidrokit` adalah proyek _open source_ paket *python* yang dapat digunakan
 untuk membantu proses analisis hidrologi dimulai dari pengolahan data, analisis
 data, dan visualisasi data. [Baca lebih lanjut mengenai hidrokit](https://
 hidrokit.github.io/hidrokit/tentang-hidrokit). ## Release
 RReelleeaassee  PPyyPPII             GGiitthhuubb          GGiitthhuubb ((PPrree--rreelleeaassee))
```

### Comparing `hidrokit-0.5.0/hidrokit.egg-info/SOURCES.txt` & `hidrokit-0.5.1/hidrokit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/setup.py` & `hidrokit-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/tests/test_prep_excel.py` & `hidrokit-0.5.1/tests/test_prep_excel.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/tests/test_prep_read.py` & `hidrokit-0.5.1/tests/test_prep_read.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/tests/test_prep_timeseries.py` & `hidrokit-0.5.1/tests/test_prep_timeseries.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.0/tests/test_viz_table.py` & `hidrokit-0.5.1/tests/test_viz_table.py`

 * *Files identical despite different names*

