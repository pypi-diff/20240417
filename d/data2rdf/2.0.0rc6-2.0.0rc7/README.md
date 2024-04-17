# Comparing `tmp/data2rdf-2.0.0rc6.tar.gz` & `tmp/data2rdf-2.0.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2rdf-2.0.0rc6.tar", last modified: Tue Apr 16 23:40:23 2024, max compression
+gzip compressed data, was "data2rdf-2.0.0rc7.tar", last modified: Wed Apr 17 12:33:36 2024, max compression
```

## Comparing `data2rdf-2.0.0rc6.tar` & `data2rdf-2.0.0rc7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.172926 data2rdf-2.0.0rc6/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 23:40:23.172926 data2rdf-2.0.0rc6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.164926 data2rdf-2.0.0rc6/data2rdf/
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2115 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.164926 data2rdf-2.0.0rc6/data2rdf/models/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/models/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/data2rdf/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/parsers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/parsers/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/parsers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/data2rdf/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/pipelines/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/pipelines/abox_scaffolding_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5656 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/pipelines/annotation_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/data2rdf/qudt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/qudt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/qudt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/data2rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 23:40:23.000000 data2rdf-2.0.0rc6/data2rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 23:40:23.000000 data2rdf-2.0.0rc6/data2rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 23:40:23.000000 data2rdf-2.0.0rc6/data2rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 23:40:23.000000 data2rdf-2.0.0rc6/data2rdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 23:40:23.000000 data2rdf-2.0.0rc6/data2rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 23:40:23.000000 data2rdf-2.0.0rc6/data2rdf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-16 23:40:23.172926 data2rdf-2.0.0rc6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/tests/csv_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/csv_pipeline_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/tests/csv_pipeline_test/input/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/csv_pipeline_test/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/csv_pipeline_test/test_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5333 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/csv_pipeline_test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/tests/xls_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/xls_pipeline_test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6450 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/xls_pipeline_test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/xls_pipeline_test/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.150654 data2rdf-2.0.0rc7/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-17 12:33:36.150654 data2rdf-2.0.0rc7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.142654 data2rdf-2.0.0rc7/data2rdf/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1732 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/data2rdf/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/models/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/data2rdf/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/parsers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/parsers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/data2rdf/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/pipelines/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/pipelines/abox_scaffolding_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5656 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/pipelines/annotation_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/data2rdf/qudt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/qudt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/qudt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.150654 data2rdf-2.0.0rc7/data2rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-17 12:33:36.000000 data2rdf-2.0.0rc7/data2rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-17 12:33:36.000000 data2rdf-2.0.0rc7/data2rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:33:36.000000 data2rdf-2.0.0rc7/data2rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 12:33:36.000000 data2rdf-2.0.0rc7/data2rdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-17 12:33:36.000000 data2rdf-2.0.0rc7/data2rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 12:33:36.000000 data2rdf-2.0.0rc7/data2rdf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-17 12:33:36.150654 data2rdf-2.0.0rc7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/tests/csv_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/csv_pipeline_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/tests/csv_pipeline_test/input/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/csv_pipeline_test/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/csv_pipeline_test/test_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5333 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/csv_pipeline_test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.150654 data2rdf-2.0.0rc7/tests/xls_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/xls_pipeline_test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6450 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/xls_pipeline_test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/xls_pipeline_test/test_pipeline.py
```

### Comparing `data2rdf-2.0.0rc6/LICENSE` & `data2rdf-2.0.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/PKG-INFO` & `data2rdf-2.0.0rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc6
+Version: 2.0.0rc7
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-2.0.0rc6/README.md` & `data2rdf-2.0.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/data2rdf/config.py` & `data2rdf-2.0.0rc7/data2rdf/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,19 +45,8 @@
     )
 
     remove_from_unit: List[str] = Field(
         ["[", "]", '"', " "],
         description="Characters which should be removed from the input value for the unit",
     )
 
-    unit_macro_location: int = Field(
-        -1,
-        description="Index where the marco for the unit in an excel cell might be located.",
-    )
-
-    max_row_iteration: int = Field(
-        1e12,
-        description="""In Excel files, the parser is scanning for the end of the time series.
-        In order to prevent a frozen process, this maximum row number is set.""",
-    )
-
     model_config = ConfigDict(extra="ignore")
```

### Comparing `data2rdf-2.0.0rc6/data2rdf/models/mapping.py` & `data2rdf-2.0.0rc7/data2rdf/models/mapping.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/data2rdf/parsers/base.py` & `data2rdf-2.0.0rc7/data2rdf/parsers/base.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/data2rdf/parsers/csv.py` & `data2rdf-2.0.0rc7/data2rdf/parsers/csv.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/data2rdf/parsers/excel.py` & `data2rdf-2.0.0rc7/data2rdf/parsers/excel.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,33 @@
 
 from .base import DataParser
 from .utils import _find_end_of_series, _strip_unit, load_mapping_file
 
 
 class ExcelParser(DataParser):
     """
-    Parses a data file of type CSV
+    Parses a data file of type excel
     """
 
+    unit_from_macro: bool = Field(
+        True,
+        description="When disabled, units coming from excel macros are neglected.",
+    )
+
+    unit_macro_location: int = Field(
+        -1,
+        description="Index where the marco for the unit in an excel cell might be located.",
+    )
+
+    max_row_iteration: int = Field(
+        1e12,
+        description="""In Excel files, the parser is scanning for the end of the time series.
+        In order to prevent a frozen process, this maximum row number is set.""",
+    )
+
     # OVERRIDE
     mapping: Union[str, Dict[str, ExcelConceptMapping]] = Field(
         ...,
         description="""File path to the mapping file to be parsed or
         a dictionary with the mapping.""",
     )
 
@@ -163,15 +179,15 @@
                 )
 
             # find data for time series
             if datum.time_series_start:
                 time_series_end = _find_end_of_series(
                     worksheet,
                     datum.time_series_start,
-                    self.config.max_row_iteration,
+                    self.max_row_iteration,
                 )
 
                 column = worksheet[datum.time_series_start : time_series_end]
                 if column:
                     self.time_series[suffix] = [
                         cell[0].value for cell in column
                     ]
@@ -180,23 +196,21 @@
                                   does not have a time series from `{datum.time_series_start}`
                                   until `{time_series_end}` .
                                   Concept will be omitted in graph.
                                   """
                     warnings.warn(message, MappingMissmatchWarning)
 
             # check if there is a macro for the unit of the entity
-            if datum.value_location:
+            if self.unit_from_macro and datum.value_location:
                 macro_worksheet = macros[datum.worksheet]
                 macro_value_cell = macro_worksheet[
                     datum.value_location
                 ].number_format.split()
                 if len(macro_value_cell) != 1:
-                    macro_unit = macro_value_cell[
-                        self.config.unit_macro_location
-                    ]
+                    macro_unit = macro_value_cell[self.unit_macro_location]
                 else:
                     macro_unit = None
             else:
                 macro_unit = None
 
             # check if there is a unit somewhere in the sheet
             if datum.unit_location:
```

### Comparing `data2rdf-2.0.0rc6/data2rdf/parsers/utils.py` & `data2rdf-2.0.0rc7/data2rdf/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/data2rdf/pipelines/abox_scaffolding_pipeline.py` & `data2rdf-2.0.0rc7/data2rdf/pipelines/abox_scaffolding_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/data2rdf/pipelines/annotation_pipeline.py` & `data2rdf-2.0.0rc7/data2rdf/pipelines/annotation_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/data2rdf/qudt/utils.py` & `data2rdf-2.0.0rc7/data2rdf/qudt/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/data2rdf/utils.py` & `data2rdf-2.0.0rc7/data2rdf/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/data2rdf.egg-info/PKG-INFO` & `data2rdf-2.0.0rc7/data2rdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc6
+Version: 2.0.0rc7
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-2.0.0rc6/data2rdf.egg-info/SOURCES.txt` & `data2rdf-2.0.0rc7/data2rdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/data2rdf.egg-info/requires.txt` & `data2rdf-2.0.0rc7/data2rdf.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/setup.cfg` & `data2rdf-2.0.0rc7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data2rdf
-version = v2.0.0rc6
+version = v2.0.0rc7
 description = A generic pipeline that can be used to map raw data to RDF.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/data2rdf
 author = Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 license = BSD-3-Clause
```

### Comparing `data2rdf-2.0.0rc6/tests/csv_pipeline_test/test_parser.py` & `data2rdf-2.0.0rc7/tests/csv_pipeline_test/test_parser.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/tests/csv_pipeline_test/test_pipeline.py` & `data2rdf-2.0.0rc7/tests/csv_pipeline_test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/tests/test_models.py` & `data2rdf-2.0.0rc7/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/tests/test_utils.py` & `data2rdf-2.0.0rc7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/tests/xls_pipeline_test/test_parser.py` & `data2rdf-2.0.0rc7/tests/xls_pipeline_test/test_parser.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc6/tests/xls_pipeline_test/test_pipeline.py` & `data2rdf-2.0.0rc7/tests/xls_pipeline_test/test_pipeline.py`

 * *Files identical despite different names*

