# Comparing `tmp/otlmow_converter-0.9.tar.gz` & `tmp/otlmow_converter-1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otlmow_converter-0.9.tar", last modified: Mon Mar  6 12:34:15 2023, max compression
+gzip compressed data, was "otlmow_converter-1.0rc1.tar", last modified: Wed Apr 17 17:58:45 2024, max compression
```

## Comparing `otlmow_converter-0.9.tar` & `otlmow_converter-1.0rc1.tar`

### file list

```diff
@@ -1,43 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:15.696233 otlmow_converter-0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-03-06 12:34:06.000000 otlmow_converter-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-06 12:34:06.000000 otlmow_converter-0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    43126 2023-03-06 12:34:15.696233 otlmow_converter-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-06 12:34:06.000000 otlmow_converter-0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:15.692233 otlmow_converter-0.9/otlmow_converter/
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/AssetFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/DotnotationHelper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:15.696233 otlmow_converter-0.9/otlmow_converter/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/Exceptions/BadTypeWarning.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/Exceptions/InvalidExtensionError.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/Exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileExporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:15.696233 otlmow_converter-0.9/otlmow_converter/FileFormats/
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/CsvExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/CsvImporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/DictDecoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/ExcelExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/ExcelImporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/JsonDecoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/JsonExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/JsonImporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/JsonLdExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/OtlAssetJSONEncoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/RDFExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/TableExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/TtlExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileImporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/HelperFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/OtlmowConverter.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/SettingsManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/SubsetTool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/settings_otlmow_converter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:15.696233 otlmow_converter-0.9/otlmow_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43126 2023-03-06 12:34:15.000000 otlmow_converter-0.9/otlmow_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-06 12:34:15.000000 otlmow_converter-0.9/otlmow_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 12:34:15.000000 otlmow_converter-0.9/otlmow_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-06 12:34:15.000000 otlmow_converter-0.9/otlmow_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-06 12:34:15.000000 otlmow_converter-0.9/otlmow_converter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-06 12:34:06.000000 otlmow_converter-0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 12:34:15.696233 otlmow_converter-0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:58:45.570033 otlmow_converter-1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    44283 2024-04-17 17:58:45.570033 otlmow_converter-1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:58:45.566033 otlmow_converter-1.0rc1/otlmow_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/AbstractExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/AbstractImporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/AssetFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/DotnotationDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20013 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/DotnotationDictConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18321 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/DotnotationHelper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:58:45.566033 otlmow_converter-1.0rc1/otlmow_converter/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/Exceptions/BadTypeWarning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/Exceptions/DotnotationListOfListError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/Exceptions/ExceptionsGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/Exceptions/FailedToImportFileError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/Exceptions/InvalidColumnNamesInExcelTabError.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/Exceptions/InvalidExtensionError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/Exceptions/NoTypeUriInExcelTabError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/Exceptions/NoTypeUriInTableError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/Exceptions/TypeUriNotInFirstRowError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/Exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileExporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:58:45.570033 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/CsvExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/CsvImporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/DotnotationTableConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/ExcelExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/ExcelImporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/GeoJSONExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/GeoJSONImporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/JsonDecoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/JsonExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/JsonImporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/JsonLdContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/JsonLdDecoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/JsonLdExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/JsonLdImporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/PandasConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/RDFExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/TtlExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileFormats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/FileImporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/HelperFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19915 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/OtlmowConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/SettingsManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/otlmow_converter/settings_otlmow_converter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:58:45.570033 otlmow_converter-1.0rc1/otlmow_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44283 2024-04-17 17:58:45.000000 otlmow_converter-1.0rc1/otlmow_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-17 17:58:45.000000 otlmow_converter-1.0rc1/otlmow_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:58:45.000000 otlmow_converter-1.0rc1/otlmow_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 17:58:45.000000 otlmow_converter-1.0rc1/otlmow_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 17:58:45.000000 otlmow_converter-1.0rc1/otlmow_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-17 17:58:39.000000 otlmow_converter-1.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 17:58:45.570033 otlmow_converter-1.0rc1/setup.cfg
```

### Comparing `otlmow_converter-0.9/LICENSE` & `otlmow_converter-1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.9/PKG-INFO` & `otlmow_converter-1.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otlmow_converter
-Version: 0.9
+Version: 1.0rc1
 Author-email: David Vlaminck <david.vlaminck@mow.vlaanderen.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -680,56 +680,72 @@
 Project-URL: Bug Tracker, https://github.com/davidvlaminck/OTLMOW-Converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: openpyxl>=3.0
+Requires-Dist: otlmow-model>=2.10.4.0
+Requires-Dist: rdflib>=6.0.0
+Requires-Dist: geojson>=3.0.1
+Requires-Dist: prettytable>=3.6.0
+Requires-Dist: numpy>=1.18
+Requires-Dist: lxml>=4.9.3
+Requires-Dist: pandas>=1.3.5
 
 # OTLMOW-Converter
 [![PyPI](https://img.shields.io/pypi/v/otlmow-converter?label=latest%20release)](https://pypi.org/project/otlmow-converter/)
 [![otlmow-converter-downloads](https://img.shields.io/pypi/dm/otlmow-converter)](https://pypi.org/project/otlmow-converter/)
 [![Unittests](https://github.com/davidvlaminck/OTLMOW-ModelBuilder/actions/workflows/unittest.yml/badge.svg)](https://github.com/davidvlaminck/OTLMOW-Converter/actions/workflows/unittest.yml)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/otlmow-converter)
 [![GitHub issues](https://img.shields.io/github/issues/davidvlaminck/OTLMOW-Converter)](https://github.com/davidvlaminck/OTLMOW-Converter/issues)
+[![coverage](https://github.com/davidvlaminck/OTLMOW-Converter/blob/master/UnitTests/coverage.svg)](https://htmlpreview.github.io/?https://github.com/davidvlaminck/OTLMOW-Converter/blob/master/UnitTests/htmlcov/index.html)
+
 
 ## OTLMOW Project 
 This project aims to implement the Flemish data standard OTL (https://wegenenverkeer.data.vlaanderen.be/) in Python.
 It is split into different packages to reduce compatibility issues
-- otlmow_model
-- otlmow_modelbuilder
-- otlmow_converter (you are currently looking at this package)
-- otlmow_template
-- otlmow-postenmapping
+- [otlmow_model](https://github.com/davidvlaminck/OTLMOW-Model)
+- [otlmow_modelbuilder](https://github.com/davidvlaminck/OTLMOW-ModelBuilder)
+- [otlmow_converter](https://github.com/davidvlaminck/OTLMOW-Converter) (you are currently looking at this package)
+- [otlmow_template](https://github.com/davidvlaminck/OTLMOW-Template)
+- [otlmow_postenmapping](https://github.com/davidvlaminck/OTLMOW-PostenMapping)
+- [otlmow_davie](https://github.com/davidvlaminck/OTLMOW-DAVIE)
+- [otlmow_visuals](https://github.com/davidvlaminck/OTLMOW-Visuals)
+- [otlmow_gui](https://github.com/davidvlaminck/OTLMOW-GUI)
+
 
 ## Installation and requirements
-OTLMOW-Converter has two dependencies besides the standard Python libraries: pandas and openpyxl. It will be automatically installed when installing this library. 
-Currently, you need at least Python version 3.8 to use this library.
+OTLMOW-Converter has a couple of dependencies besides the standard Python libraries. It depends on another OTLMOW package: otlmow-model. These libraries will be automatically installed when installing this library. Currently, you need at least Python version 3.7 to use this library.
 
 To install the OTL MOW project into your Python project, use pip to install it:
 ``` 
 pip install otlmow_converter
 ```
 To upgrade an existing installation use:
 ``` 
 pip install otlmow_converter --upgrade
 ```
 
-## Usage
-The core functionality of this library is creating objects of otlmow_model by, either using helper functions or reading a DAVIE file. Then the user can manipulate the objects and finally export them to a valid DAVIE file that can be imported in the application.
+## Code examples and usage
+See the [Readme notebook](https://github.com/davidvlaminck/OTLMOW-Converter/blob/master/Readme.ipynb)
 
 <!--- 
 assetfactory
 relationcreator
-otlmowconverter
-formats:
-csv
-xlsx
-json
-jsonld
-ttl
-
 -->
+## Supported formats
+The following file formats are supported in OtlmowConverter
+| File format | Read | Write | DAVIE compliant |
+| --- | --- | --- | --- |
+| CSV | Yes | Yes | Yes |
+| Excel | Yes | Yes | Yes |
+| JSON | Yes | Yes | Yes |
+| GEOJSON| Yes | Yes | Yes |
+| JSON-LD| Yes | Yes | No |
+| TTL | No | Yes | No |
```

### Comparing `otlmow_converter-0.9/otlmow_converter/AssetFactory.py` & `otlmow_converter-1.0rc1/otlmow_converter/AssetFactory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,59 @@
-﻿from typing import Union, List
+﻿from pathlib import Path
+from typing import Union, Set
 
-from otlmow_model.Classes.ImplementatieElement.AIMObject import AIMObject
-from otlmow_model.Classes.ImplementatieElement.RelatieObject import RelatieObject
-from otlmow_model.Helpers.AssetCreator import dynamic_create_instance_from_uri
-
-from otlmow_converter.FileFormats.DictDecoder import DictDecoder
+from otlmow_model.OtlmowModel.BaseClasses.OTLObject import set_value_by_dictitem, OTLObject, \
+    dynamic_create_instance_from_uri
+from otlmow_model.OtlmowModel.Classes.ImplementatieElement.AIMObject import AIMObject
+from otlmow_model.OtlmowModel.Classes.ImplementatieElement.RelatieObject import RelatieObject
 
 
 class AssetFactory:
     @staticmethod
-    def create_aimObject_using_other_aimObject_as_template(orig_aim_object: Union[AIMObject, RelatieObject], 
-                                                           typeURI: str = '', fields_to_copy: [str] = None,
-                                                           directory: str = None) -> Union[AIMObject, RelatieObject]:
-        """Creates an AIMObject, using another AIMObject as template.
-        The parameter typeURI defines the type of the new AIMObject that is created.
+    def create_otl_object_using_other_otl_object_as_template(
+            orig_otl_object: OTLObject, typeURI: str = '', fields_to_copy: Set[str] = None,
+            model_directory: Path = None) -> OTLObject:
+        """Creates an OTLObject, using another OTLObject as template.
+        The parameter typeURI defines the type of the new OTLObject that is created.
         If omitted, it is assumed the same type as the given aimObject
         The parameter fields_to_copy dictates what fields are copied from the first object
         When the types do not match, fields_to_copy can not be empty"""
 
-        if directory is None:
-            directory = 'otlmow_model.Classes'
+        if model_directory is None:
+            import otlmow_model
+            otlmow_path = otlmow_model.__path__
+            model_directory = Path(otlmow_path._path[0])
+
         if fields_to_copy is None:
             fields_to_copy = []
 
-        if not isinstance(orig_aim_object, AIMObject):
-            raise ValueError(f'{orig_aim_object} is not an AIMObject, not supported')
+        if not isinstance(orig_otl_object, OTLObject):
+            raise ValueError(f'{orig_otl_object} is not an OTLObject, not supported')
 
         if typeURI != '':
-            if typeURI != orig_aim_object.typeURI and (fields_to_copy == [] or fields_to_copy is None):
-                raise ValueError("parameter typeURI is different from orig_aim_object. parameter fields_to_copy cannot be empty")
+            if typeURI != orig_otl_object.typeURI and (fields_to_copy == [] or fields_to_copy is None):
+                raise ValueError("parameter typeURI is different from orig_otl_object. "
+                                 "Parameter fields_to_copy cannot be empty")
 
         if typeURI == '':
-            typeURI = orig_aim_object.typeURI
-        new_asset = dynamic_create_instance_from_uri(typeURI, directory=directory)
+            typeURI = orig_otl_object.typeURI
+        new_asset = dynamic_create_instance_from_uri(typeURI, model_directory=model_directory)
 
         if len(fields_to_copy) == 0:
-            fields_to_copy = AssetFactory.get_attribute_list_from_object(orig_aim_object)
+            fields_to_copy = [orig_otl_object]
 
         if 'typeURI' in fields_to_copy:
             fields_to_copy.remove('typeURI')
         if 'assetId' in fields_to_copy:
             fields_to_copy.remove('assetId')
 
-        AssetFactory.copy_fields_from_object_to_new_object(orig_aim_object, new_asset, fields_to_copy)
+        AssetFactory.copy_fields_from_object_to_new_object(orig_otl_object, new_asset, fields_to_copy)
         return new_asset
 
     @staticmethod
-    def get_attribute_list_from_object(orig_asset: Union[AIMObject, RelatieObject]) -> List:
-        if orig_asset is None:
-            raise ValueError("input can't be None")
-
-        return list(orig_asset.create_dict_from_asset().keys())
-
-    @staticmethod
     def copy_fields_from_object_to_new_object(orig_object: Union[AIMObject, RelatieObject],
                                               new_object: Union[AIMObject, RelatieObject], field_list: [str]):
         if orig_object is None:
             raise ValueError("parameter orig_object is None")
         if new_object is None:
             raise ValueError("parameter new_object is None")
         if field_list is None or field_list == []:
@@ -72,8 +69,8 @@
         for fieldName in distinct_fieldList:
             if fieldName not in instance_dict:
                 continue
             dictitem = instance_dict[fieldName]
             new_instance_dict[fieldName] = dictitem
 
         for k, v in new_instance_dict.items():
-            DictDecoder.set_value_by_dictitem(new_object, k, v, waarde_shortcut=False)
+            set_value_by_dictitem(new_object, k, v, waarde_shortcut=False)
```

### Comparing `otlmow_converter-0.9/otlmow_converter/FileFormats/RDFExporter.py` & `otlmow_converter-1.0rc1/otlmow_converter/FileFormats/RDFExporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Dict, Iterable
 
-from otlmow_model.BaseClasses.FloatOrDecimalField import FloatOrDecimalField
-from otlmow_model.BaseClasses.KeuzelijstField import KeuzelijstField
-from otlmow_model.Classes.ImplementatieElement.RelatieObject import RelatieObject
+from otlmow_model.OtlmowModel.BaseClasses.FloatOrDecimalField import FloatOrDecimalField
+from otlmow_model.OtlmowModel.BaseClasses.KeuzelijstField import KeuzelijstField
+from otlmow_model.OtlmowModel.Classes.ImplementatieElement.RelatieObject import RelatieObject
 from rdflib import Graph, FOAF, URIRef, BNode, Literal, RDF, XSD
 
 
 class RDFExporter:
     def __init__(self, dotnotation_settings: Dict = None):
 
         if dotnotation_settings is None:
             dotnotation_settings = {}
         self.settings = dotnotation_settings
 
-        for required_attribute in ['waarde_shortcut_applicable']:
+        for required_attribute in ['waarde_shortcut']:
             if required_attribute not in self.settings:
                 raise ValueError("The settings are not loaded or don't contain the full dotnotation settings")
 
     def create_graph(self, list_of_objects: Iterable = None) -> Graph:
         g = Graph()
         for ns, namespace in {'foaf': FOAF,
                               'imel': 'https://wegenenverkeer.data.vlaanderen.be/ns/implementatieelement#',
```

### Comparing `otlmow_converter-0.9/otlmow_converter/FileFormats/TtlExporter.py` & `otlmow_converter-1.0rc1/otlmow_converter/FileFormats/TtlExporter.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.9/otlmow_converter.egg-info/PKG-INFO` & `otlmow_converter-1.0rc1/otlmow_converter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: otlmow-converter
-Version: 0.9
+Name: otlmow_converter
+Version: 1.0rc1
 Author-email: David Vlaminck <david.vlaminck@mow.vlaanderen.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -680,56 +680,72 @@
 Project-URL: Bug Tracker, https://github.com/davidvlaminck/OTLMOW-Converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: openpyxl>=3.0
+Requires-Dist: otlmow-model>=2.10.4.0
+Requires-Dist: rdflib>=6.0.0
+Requires-Dist: geojson>=3.0.1
+Requires-Dist: prettytable>=3.6.0
+Requires-Dist: numpy>=1.18
+Requires-Dist: lxml>=4.9.3
+Requires-Dist: pandas>=1.3.5
 
 # OTLMOW-Converter
 [![PyPI](https://img.shields.io/pypi/v/otlmow-converter?label=latest%20release)](https://pypi.org/project/otlmow-converter/)
 [![otlmow-converter-downloads](https://img.shields.io/pypi/dm/otlmow-converter)](https://pypi.org/project/otlmow-converter/)
 [![Unittests](https://github.com/davidvlaminck/OTLMOW-ModelBuilder/actions/workflows/unittest.yml/badge.svg)](https://github.com/davidvlaminck/OTLMOW-Converter/actions/workflows/unittest.yml)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/otlmow-converter)
 [![GitHub issues](https://img.shields.io/github/issues/davidvlaminck/OTLMOW-Converter)](https://github.com/davidvlaminck/OTLMOW-Converter/issues)
+[![coverage](https://github.com/davidvlaminck/OTLMOW-Converter/blob/master/UnitTests/coverage.svg)](https://htmlpreview.github.io/?https://github.com/davidvlaminck/OTLMOW-Converter/blob/master/UnitTests/htmlcov/index.html)
+
 
 ## OTLMOW Project 
 This project aims to implement the Flemish data standard OTL (https://wegenenverkeer.data.vlaanderen.be/) in Python.
 It is split into different packages to reduce compatibility issues
-- otlmow_model
-- otlmow_modelbuilder
-- otlmow_converter (you are currently looking at this package)
-- otlmow_template
-- otlmow-postenmapping
+- [otlmow_model](https://github.com/davidvlaminck/OTLMOW-Model)
+- [otlmow_modelbuilder](https://github.com/davidvlaminck/OTLMOW-ModelBuilder)
+- [otlmow_converter](https://github.com/davidvlaminck/OTLMOW-Converter) (you are currently looking at this package)
+- [otlmow_template](https://github.com/davidvlaminck/OTLMOW-Template)
+- [otlmow_postenmapping](https://github.com/davidvlaminck/OTLMOW-PostenMapping)
+- [otlmow_davie](https://github.com/davidvlaminck/OTLMOW-DAVIE)
+- [otlmow_visuals](https://github.com/davidvlaminck/OTLMOW-Visuals)
+- [otlmow_gui](https://github.com/davidvlaminck/OTLMOW-GUI)
+
 
 ## Installation and requirements
-OTLMOW-Converter has two dependencies besides the standard Python libraries: pandas and openpyxl. It will be automatically installed when installing this library. 
-Currently, you need at least Python version 3.8 to use this library.
+OTLMOW-Converter has a couple of dependencies besides the standard Python libraries. It depends on another OTLMOW package: otlmow-model. These libraries will be automatically installed when installing this library. Currently, you need at least Python version 3.7 to use this library.
 
 To install the OTL MOW project into your Python project, use pip to install it:
 ``` 
 pip install otlmow_converter
 ```
 To upgrade an existing installation use:
 ``` 
 pip install otlmow_converter --upgrade
 ```
 
-## Usage
-The core functionality of this library is creating objects of otlmow_model by, either using helper functions or reading a DAVIE file. Then the user can manipulate the objects and finally export them to a valid DAVIE file that can be imported in the application.
+## Code examples and usage
+See the [Readme notebook](https://github.com/davidvlaminck/OTLMOW-Converter/blob/master/Readme.ipynb)
 
 <!--- 
 assetfactory
 relationcreator
-otlmowconverter
-formats:
-csv
-xlsx
-json
-jsonld
-ttl
-
 -->
+## Supported formats
+The following file formats are supported in OtlmowConverter
+| File format | Read | Write | DAVIE compliant |
+| --- | --- | --- | --- |
+| CSV | Yes | Yes | Yes |
+| Excel | Yes | Yes | Yes |
+| JSON | Yes | Yes | Yes |
+| GEOJSON| Yes | Yes | Yes |
+| JSON-LD| Yes | Yes | No |
+| TTL | No | Yes | No |
```

### Comparing `otlmow_converter-0.9/otlmow_converter.egg-info/SOURCES.txt` & `otlmow_converter-1.0rc1/otlmow_converter.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+otlmow_converter/AbstractExporter.py
+otlmow_converter/AbstractImporter.py
 otlmow_converter/AssetFactory.py
+otlmow_converter/DotnotationDict.py
+otlmow_converter/DotnotationDictConverter.py
 otlmow_converter/DotnotationHelper.py
 otlmow_converter/FileExporter.py
 otlmow_converter/FileImporter.py
 otlmow_converter/HelperFunctions.py
 otlmow_converter/OtlmowConverter.py
 otlmow_converter/SettingsManager.py
-otlmow_converter/SubsetTool.py
 otlmow_converter/__init__.py
 otlmow_converter/settings_otlmow_converter.json
 otlmow_converter.egg-info/PKG-INFO
 otlmow_converter.egg-info/SOURCES.txt
 otlmow_converter.egg-info/dependency_links.txt
 otlmow_converter.egg-info/requires.txt
 otlmow_converter.egg-info/top_level.txt
 otlmow_converter/Exceptions/BadTypeWarning.py
+otlmow_converter/Exceptions/DotnotationListOfListError.py
+otlmow_converter/Exceptions/ExceptionsGroup.py
+otlmow_converter/Exceptions/FailedToImportFileError.py
+otlmow_converter/Exceptions/InvalidColumnNamesInExcelTabError.py
 otlmow_converter/Exceptions/InvalidExtensionError.py
+otlmow_converter/Exceptions/NoTypeUriInExcelTabError.py
+otlmow_converter/Exceptions/NoTypeUriInTableError.py
+otlmow_converter/Exceptions/TypeUriNotInFirstRowError.py
 otlmow_converter/Exceptions/__init__.py
 otlmow_converter/FileFormats/CsvExporter.py
 otlmow_converter/FileFormats/CsvImporter.py
-otlmow_converter/FileFormats/DictDecoder.py
+otlmow_converter/FileFormats/DotnotationTableConverter.py
 otlmow_converter/FileFormats/ExcelExporter.py
 otlmow_converter/FileFormats/ExcelImporter.py
+otlmow_converter/FileFormats/GeoJSONExporter.py
+otlmow_converter/FileFormats/GeoJSONImporter.py
 otlmow_converter/FileFormats/JsonDecoder.py
 otlmow_converter/FileFormats/JsonExporter.py
 otlmow_converter/FileFormats/JsonImporter.py
+otlmow_converter/FileFormats/JsonLdContext.py
+otlmow_converter/FileFormats/JsonLdDecoder.py
 otlmow_converter/FileFormats/JsonLdExporter.py
-otlmow_converter/FileFormats/OtlAssetJSONEncoder.py
+otlmow_converter/FileFormats/JsonLdImporter.py
+otlmow_converter/FileFormats/PandasConverter.py
 otlmow_converter/FileFormats/RDFExporter.py
-otlmow_converter/FileFormats/TableExporter.py
 otlmow_converter/FileFormats/TtlExporter.py
 otlmow_converter/FileFormats/__init__.py
```

### Comparing `otlmow_converter-0.9/pyproject.toml` & `otlmow_converter-1.0rc1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otlmow_converter"
-version = "0.9"
+version = "1.0rc1"
 authors = [{name = "David Vlaminck", email = "david.vlaminck@mow.vlaanderen.be"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent"
 ]
 requires-python = ">=3.7"
 dependencies = [
     'openpyxl >= 3.0',
-    'otlmow_model >= 2.6.7',
+    'otlmow-model >= 2.10.4.0',
     'rdflib >= 6.0.0',
-    'PyLD>=2.0.0',
-    'prettytable>=3.6.0'
+    'geojson>=3.0.1',
+    'prettytable>=3.6.0',
+    'numpy >= 1.18',
+    'lxml>=4.9.3',
+    'pandas>=1.3.5'
 ]
 
 [tool.setuptools.packages.find]
 include = ["otlmow_converter*"]
 
 [project.urls]
 "Homepage" = "https://github.com/davidvlaminck/OTLMOW-Converter"
```

