# Comparing `tmp/data2rdf-2.0.0rc4.tar.gz` & `tmp/data2rdf-2.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2rdf-2.0.0rc4.tar", last modified: Tue Apr 16 13:07:35 2024, max compression
+gzip compressed data, was "data2rdf-2.0.0rc5.tar", last modified: Tue Apr 16 22:03:09 2024, max compression
```

## Comparing `data2rdf-2.0.0rc4.tar` & `data2rdf-2.0.0rc5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.082656 data2rdf-2.0.0rc4/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 13:07:35.082656 data2rdf-2.0.0rc4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.078656 data2rdf-2.0.0rc4/data2rdf/
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2115 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.078656 data2rdf-2.0.0rc4/data2rdf/models/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/models/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.078656 data2rdf-2.0.0rc4/data2rdf/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/parsers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/parsers/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/parsers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.078656 data2rdf-2.0.0rc4/data2rdf/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/pipelines/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/pipelines/abox_scaffolding_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5656 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/pipelines/annotation_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.078656 data2rdf-2.0.0rc4/data2rdf/qudt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/qudt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/qudt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.082656 data2rdf-2.0.0rc4/data2rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 13:07:35.000000 data2rdf-2.0.0rc4/data2rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 13:07:35.000000 data2rdf-2.0.0rc4/data2rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:07:35.000000 data2rdf-2.0.0rc4/data2rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 13:07:35.000000 data2rdf-2.0.0rc4/data2rdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 13:07:35.000000 data2rdf-2.0.0rc4/data2rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 13:07:35.000000 data2rdf-2.0.0rc4/data2rdf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-16 13:07:35.086656 data2rdf-2.0.0rc4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.078656 data2rdf-2.0.0rc4/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.082656 data2rdf-2.0.0rc4/tests/csv_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/csv_pipeline_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.082656 data2rdf-2.0.0rc4/tests/csv_pipeline_test/input/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/csv_pipeline_test/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/csv_pipeline_test/test_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4980 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/csv_pipeline_test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.082656 data2rdf-2.0.0rc4/tests/xls_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/xls_pipeline_test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6059 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/xls_pipeline_test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/xls_pipeline_test/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.855882 data2rdf-2.0.0rc5/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 22:03:09.855882 data2rdf-2.0.0rc5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.847882 data2rdf-2.0.0rc5/data2rdf/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2115 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.847882 data2rdf-2.0.0rc5/data2rdf/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/models/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/data2rdf/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/parsers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/parsers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/data2rdf/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/pipelines/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/pipelines/abox_scaffolding_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5656 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/pipelines/annotation_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/data2rdf/qudt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/qudt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/qudt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/data2rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 22:03:09.000000 data2rdf-2.0.0rc5/data2rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 22:03:09.000000 data2rdf-2.0.0rc5/data2rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:03:09.000000 data2rdf-2.0.0rc5/data2rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 22:03:09.000000 data2rdf-2.0.0rc5/data2rdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 22:03:09.000000 data2rdf-2.0.0rc5/data2rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 22:03:09.000000 data2rdf-2.0.0rc5/data2rdf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-16 22:03:09.855882 data2rdf-2.0.0rc5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/tests/csv_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/csv_pipeline_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/tests/csv_pipeline_test/input/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/csv_pipeline_test/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/csv_pipeline_test/test_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5333 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/csv_pipeline_test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/tests/xls_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/xls_pipeline_test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6450 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/xls_pipeline_test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/xls_pipeline_test/test_pipeline.py
```

### Comparing `data2rdf-2.0.0rc4/LICENSE` & `data2rdf-2.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc4/PKG-INFO` & `data2rdf-2.0.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc4
+Version: 2.0.0rc5
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-2.0.0rc4/README.md` & `data2rdf-2.0.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc4/data2rdf/config.py` & `data2rdf-2.0.0rc5/data2rdf/config.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc4/data2rdf/models/mapping.py` & `data2rdf-2.0.0rc5/data2rdf/models/mapping.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc4/data2rdf/parsers/base.py` & `data2rdf-2.0.0rc5/data2rdf/parsers/base.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc4/data2rdf/parsers/csv.py` & `data2rdf-2.0.0rc5/data2rdf/parsers/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,24 +208,28 @@
             if mapping_match:
                 # get unit
                 unit = mapping_match.unit or time_series[key].iloc[0] or None
                 if unit:
                     unit = _strip_unit(unit, self.config.remove_from_unit)
 
                 # assign model
-                model_data = {
-                    "key": key,
-                    "unit": unit,
-                    "iri": mapping_match.iri,
-                    "annotation": mapping_match.annotation or None,
-                }
-                self.time_series_metadata.append(QuantityMapping(**model_data))
+                model = QuantityMapping(
+                    key=key,
+                    unit=unit,
+                    iri=mapping_match.iri,
+                    annotation=mapping_match.annotation or None,
+                )
+
+                # append model
+                self.time_series_metadata.append(model)
 
                 # assign time series data
-                self._time_series[key] = time_series[key][1:].to_list()
+                self._time_series[model.suffix] = time_series[key][
+                    1:
+                ].to_list()
 
             else:
                 warnings.warn(
                     f"No match found in mapping for key `{key}`",
                     MappingMissmatchWarning,
                 )
```

### Comparing `data2rdf-2.0.0rc4/data2rdf/parsers/excel.py` & `data2rdf-2.0.0rc5/data2rdf/parsers/excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,16 @@
 
         self._general_metadata = []
         self._time_series_metadata = []
         self._time_series = {}
         for key, datum in mapping.items():
             worksheet = datafile[datum.worksheet]
 
+            suffix = str(datum.iri).split(self.config.separator)[-1]
+
             if datum.value_location and datum.time_series_start:
                 raise RuntimeError(
                     """Both, `value_location` and `time_series_start
                        are set. Only one of them must be set."""
                 )
 
             # find data for time series
@@ -166,19 +168,21 @@
                     worksheet,
                     datum.time_series_start,
                     self.config.max_row_iteration,
                 )
 
                 column = worksheet[datum.time_series_start : time_series_end]
                 if column:
-                    self.time_series[key] = [cell[0].value for cell in column]
+                    self.time_series[suffix] = [
+                        cell[0].value for cell in column
+                    ]
                 else:
                     message = f"""Concept with key `{key}`
                                   does not have a time series from `{datum.time_series_start}`
-                                  until ``{time_series_end}` .
+                                  until `{time_series_end}` .
                                   Concept will be omitted in graph.
                                   """
                     warnings.warn(message, MappingMissmatchWarning)
 
             # check if there is a macro for the unit of the entity
             if datum.value_location:
                 macro_worksheet = macros[datum.worksheet]
@@ -228,15 +232,15 @@
                 else:
                     message = f"""Concept with key `{key}`
                                   does not have a value at location `{datum.value_location}`.
                                   Concept will be omitted in graph.
                                   """
                     warnings.warn(message, MappingMissmatchWarning)
 
-            if model_data.get("value") or key in self.time_series:
+            if model_data.get("value") or suffix in self.time_series:
                 if model_data.get("unit"):
                     model = QuantityMapping(**model_data)
                 else:
                     model = PropertyMapping(**model_data)
 
                 if model_data.get("value"):
                     self._general_metadata.append(model)
```

### Comparing `data2rdf-2.0.0rc4/data2rdf/parsers/utils.py` & `data2rdf-2.0.0rc5/data2rdf/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc4/data2rdf/pipelines/abox_scaffolding_pipeline.py` & `data2rdf-2.0.0rc5/data2rdf/pipelines/abox_scaffolding_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc4/data2rdf/pipelines/annotation_pipeline.py` & `data2rdf-2.0.0rc5/data2rdf/pipelines/annotation_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc4/data2rdf/qudt/utils.py` & `data2rdf-2.0.0rc5/data2rdf/qudt/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc4/data2rdf/utils.py` & `data2rdf-2.0.0rc5/data2rdf/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc4/data2rdf.egg-info/PKG-INFO` & `data2rdf-2.0.0rc5/data2rdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc4
+Version: 2.0.0rc5
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-2.0.0rc4/data2rdf.egg-info/SOURCES.txt` & `data2rdf-2.0.0rc5/data2rdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc4/data2rdf.egg-info/requires.txt` & `data2rdf-2.0.0rc5/data2rdf.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc4/setup.cfg` & `data2rdf-2.0.0rc5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data2rdf
-version = v2.0.0rc4
+version = v2.0.0rc5
 description = A generic pipeline that can be used to map raw data to RDF.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/data2rdf
 author = Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 license = BSD-3-Clause
```

### Comparing `data2rdf-2.0.0rc4/tests/csv_pipeline_test/test_parser.py` & `data2rdf-2.0.0rc5/tests/csv_pipeline_test/test_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,23 @@
     "SpecimenWidth": 20.04,
     "TestingRate": 0.1,
     "Preload": 2,
     "Temperature": 22,
     "Remark": "",
 }
 
+columns = [
+    "TestTime",
+    "StandardForce",
+    "Extension",
+    "Elongation",
+    "AbsoluteCrossheadTravel",
+    "WidthChange",
+]
+
 normal_config = {"graph_identifier": "https://www.example.org"}
 bad_config = {"graph_identifier": "https://www.example.org", "foorbar": 123}
 
 
 def test_csv_parser_bad_mapping() -> None:
     from rdflib import Graph
 
@@ -63,14 +72,15 @@
         )
 
     assert len(parser.time_series_metadata) == 6
     for row in parser.time_series_metadata:
         assert isinstance(row, QuantityMapping)
 
     assert len(parser.time_series) == 6
+    assert sorted(list(parser.time_series.keys())) == sorted(columns)
     for row in parser.time_series.values():
         assert len(row) == 5734
         assert isinstance(row, list)
 
     assert parser.graph.isomorphic(expected_graph)
 
 
@@ -111,14 +121,15 @@
         )
 
     assert len(parser.time_series_metadata) == 6
     for row in parser.time_series_metadata:
         assert isinstance(row, QuantityMapping)
 
     assert len(parser.time_series) == 6
+    assert sorted(list(parser.time_series.keys())) == sorted(columns)
     for row in parser.time_series.values():
         assert len(row) == 5734
         assert isinstance(row, list)
 
     assert parser.graph.isomorphic(expected_graph)
 
 
@@ -135,14 +146,15 @@
         config=config,
     )
     expected_graph = Graph()
     expected_graph.parse(expected)
 
     assert parser.graph.isomorphic(expected_graph)
     assert str(parser.graph.identifier) == config["graph_identifier"]
+    assert sorted(list(parser.time_series.keys())) == sorted(columns)
 
 
 @pytest.mark.parametrize("extension", ["xlsx", "json", dict])
 def test_parser_csv(extension) -> None:
     from rdflib import Graph
 
     from data2rdf.models import PropertyMapping, QuantityMapping
@@ -167,14 +179,15 @@
         )
 
     assert len(parser.time_series_metadata) == 6
     for row in parser.time_series_metadata:
         assert isinstance(row, QuantityMapping)
 
     assert len(parser.time_series) == 6
+    assert sorted(list(parser.time_series.keys())) == sorted(columns)
     for row in parser.time_series.values():
         assert len(row) == 5734
         assert isinstance(row, list)
 
     expected_graph = Graph()
     expected_graph.parse(expected)
```

### Comparing `data2rdf-2.0.0rc4/tests/csv_pipeline_test/test_pipeline.py` & `data2rdf-2.0.0rc5/tests/csv_pipeline_test/test_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,23 @@
     "SpecimenWidth": 20.04,
     "TestingRate": 0.1,
     "Preload": 2,
     "Temperature": 22,
     "Remark": "",
 }
 
+columns = [
+    "TestTime",
+    "StandardForce",
+    "Extension",
+    "Elongation",
+    "AbsoluteCrossheadTravel",
+    "WidthChange",
+]
+
 normal_config = {"graph_identifier": "https://www.example.org"}
 bad_config = {"graph_identifier": "https://www.example.org", "foorbar": 123}
 
 
 def test_csv_pipeline_bad_mapping() -> None:
     from rdflib import Graph
 
@@ -91,14 +100,15 @@
     ]
     assert len(missmatches) == 1
 
     expected_graph = Graph()
     expected_graph.parse(expected)
 
     assert pipeline.graph.isomorphic(expected_graph)
+    assert sorted(list(pipeline.time_series.keys())) == sorted(columns)
 
 
 @pytest.mark.parametrize("config", [normal_config, bad_config])
 def test_csv_pipeline_config(config) -> None:
     from rdflib import Graph
 
     from data2rdf import (  # isort:skip
@@ -115,14 +125,15 @@
         config=config,
     )
     expected_graph = Graph()
     expected_graph.parse(expected)
 
     assert pipeline.graph.isomorphic(expected_graph)
     assert str(pipeline.graph.identifier) == config["graph_identifier"]
+    assert sorted(list(pipeline.time_series.keys())) == sorted(columns)
 
 
 @pytest.mark.parametrize("extension", ["xlsx", "json", dict])
 def test_csv_pipeline(extension) -> None:
     from rdflib import Graph
 
     from data2rdf import (  # isort:skip
@@ -157,14 +168,15 @@
         )
 
     assert len(pipeline.time_series_metadata) == 6
     for row in pipeline.time_series_metadata:
         assert isinstance(row, QuantityMapping)
 
     assert len(pipeline.time_series) == 6
+    assert sorted(list(pipeline.time_series.keys())) == sorted(columns)
     for row in pipeline.time_series.values():
         assert len(row) == 5734
         assert isinstance(row, list)
 
     expected_graph = Graph()
     expected_graph.parse(expected)
```

### Comparing `data2rdf-2.0.0rc4/tests/test_models.py` & `data2rdf-2.0.0rc5/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 
 normal_config = {"graph_identifier": "https://www.example.org"}
 bad_config = {"graph_identifier": "https://www.example.org", "foorbar": 123}
 
 
 @pytest.mark.parametrize("config", [normal_config, bad_config])
-def test_csv_parser_config(config) -> None:
+def test_quantity_model(config) -> None:
     from rdflib import Graph
 
     from data2rdf import QuantityMapping
 
     expected = """@prefix fileid: <https://www.example.org/> .
     @prefix qudt: <http://qudt.org/schema/qudt/> .
     @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
```

### Comparing `data2rdf-2.0.0rc4/tests/test_utils.py` & `data2rdf-2.0.0rc5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc4/tests/xls_pipeline_test/test_parser.py` & `data2rdf-2.0.0rc5/tests/xls_pipeline_test/test_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,23 @@
     "OriginalGaugeLength": 15,
     "SpecimenThickness": 1.5,
     "SpecimenWidth": 9.5,
     "TestingRate": 0.02,
     "Temperature": 25,
 }
 
+columns = [
+    "TestTime",
+    "StandardForce",
+    "Extension",
+    "PercentageElongation",
+    "AbsoluteCrossheadTravel",
+    "WidthChange",
+]
+
 
 normal_config = {"graph_identifier": "https://www.example.org"}
 bad_config = {"graph_identifier": "https://www.example.org", "foorbar": 123}
 
 
 def test_xlsx_parser_no_match_in_metadata_from_mapping() -> None:
     from rdflib import Graph
@@ -66,14 +75,15 @@
         )
 
     assert len(parser.time_series_metadata) == 6
     for row in parser.time_series_metadata:
         assert isinstance(row, QuantityMapping)
 
     assert len(parser.time_series) == 6
+    assert sorted(list(parser.time_series.keys())) == sorted(columns)
     for row in parser.time_series.values():
         assert len(row) == 460
         assert isinstance(row, list)
 
 
 def test_xlsx_parser_no_match_in_timeseries_from_mapping() -> None:
     from rdflib import Graph
@@ -109,15 +119,16 @@
         )
 
     assert len(parser.time_series_metadata) == 5
     for row in parser.time_series_metadata:
         assert isinstance(row, QuantityMapping)
 
     assert len(parser.time_series) == 5
-    for row in parser.time_series.values():
+    for key, row in parser.time_series.items():
+        assert key in columns
         assert len(row) == 460
         assert isinstance(row, list)
 
     assert parser.plain_metadata == metadata
 
 
 @pytest.mark.parametrize("config", [normal_config, bad_config])
@@ -145,14 +156,15 @@
 
     expected_graph = Graph()
     expected_graph.parse(expected)
 
     assert parser.graph.isomorphic(expected_graph)
     assert str(parser.graph.identifier) == config["graph_identifier"]
     assert parser.plain_metadata == metadata
+    assert sorted(list(parser.time_series.keys())) == sorted(columns)
 
 
 @pytest.mark.parametrize("extension", ["xlsx", "json", dict])
 def test_parser_excel(extension) -> None:
     from rdflib import Graph
 
     from data2rdf.models import PropertyMapping, QuantityMapping
@@ -188,14 +200,15 @@
         )
 
     assert len(parser.time_series_metadata) == 6
     for row in parser.time_series_metadata:
         assert isinstance(row, QuantityMapping)
 
     assert len(parser.time_series) == 6
+    assert sorted(list(parser.time_series.keys())) == sorted(columns)
     for row in parser.time_series.values():
         assert len(row) == 460
         assert isinstance(row, list)
 
     expected_graph = Graph()
     expected_graph.parse(expected)
```

### Comparing `data2rdf-2.0.0rc4/tests/xls_pipeline_test/test_pipeline.py` & `data2rdf-2.0.0rc5/tests/xls_pipeline_test/test_pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,22 @@
     "OriginalGaugeLength": 15,
     "SpecimenThickness": 1.5,
     "SpecimenWidth": 9.5,
     "TestingRate": 0.02,
     "Temperature": 25,
 }
 
+columns = [
+    "TestTime",
+    "StandardForce",
+    "Extension",
+    "PercentageElongation",
+    "AbsoluteCrossheadTravel",
+    "WidthChange",
+]
 
 normal_config = {"graph_identifier": "https://www.example.org"}
 bad_config = {"graph_identifier": "https://www.example.org", "foorbar": 123}
 
 
 @pytest.mark.parametrize("config", [normal_config, bad_config])
 def test_csv_pipeline_config(config) -> None:
@@ -68,15 +76,17 @@
     assert len(missmatches) == 1
 
     expected_graph = Graph()
     expected_graph.parse(expected)
 
     assert pipeline.graph.isomorphic(expected_graph)
     assert str(pipeline.graph.identifier) == config["graph_identifier"]
+
     assert pipeline.plain_metadata == metadata
+    assert sorted(list(pipeline.time_series.keys())) == sorted(columns)
 
 
 @pytest.mark.parametrize("extension", ["xlsx", "json", dict])
 def test_excel_pipeline(extension) -> None:
     from rdflib import Graph
 
     from data2rdf.warnings import MappingMissmatchWarning
@@ -122,14 +132,15 @@
         )
 
     assert len(pipeline.time_series_metadata) == 6
     for row in pipeline.time_series_metadata:
         assert isinstance(row, QuantityMapping)
 
     assert len(pipeline.time_series) == 6
+    assert sorted(list(pipeline.time_series.keys())) == sorted(columns)
     for row in pipeline.time_series.values():
         assert len(row) == 460
         assert isinstance(row, list)
 
     expected_graph = Graph()
     expected_graph.parse(expected)
```

