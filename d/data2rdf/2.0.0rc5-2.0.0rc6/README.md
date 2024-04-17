# Comparing `tmp/data2rdf-2.0.0rc5.tar.gz` & `tmp/data2rdf-2.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2rdf-2.0.0rc5.tar", last modified: Tue Apr 16 22:03:09 2024, max compression
+gzip compressed data, was "data2rdf-2.0.0rc6.tar", last modified: Tue Apr 16 23:40:23 2024, max compression
```

## Comparing `data2rdf-2.0.0rc5.tar` & `data2rdf-2.0.0rc6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.855882 data2rdf-2.0.0rc5/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 22:03:09.855882 data2rdf-2.0.0rc5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.847882 data2rdf-2.0.0rc5/data2rdf/
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2115 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.847882 data2rdf-2.0.0rc5/data2rdf/models/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/models/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/data2rdf/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/parsers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/parsers/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/parsers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/data2rdf/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/pipelines/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/pipelines/abox_scaffolding_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5656 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/pipelines/annotation_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/data2rdf/qudt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/qudt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/qudt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/data2rdf/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/data2rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 22:03:09.000000 data2rdf-2.0.0rc5/data2rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 22:03:09.000000 data2rdf-2.0.0rc5/data2rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:03:09.000000 data2rdf-2.0.0rc5/data2rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 22:03:09.000000 data2rdf-2.0.0rc5/data2rdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 22:03:09.000000 data2rdf-2.0.0rc5/data2rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 22:03:09.000000 data2rdf-2.0.0rc5/data2rdf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-16 22:03:09.855882 data2rdf-2.0.0rc5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/tests/csv_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/csv_pipeline_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/tests/csv_pipeline_test/input/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/csv_pipeline_test/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/csv_pipeline_test/test_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5333 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/csv_pipeline_test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:09.851882 data2rdf-2.0.0rc5/tests/xls_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/xls_pipeline_test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6450 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/xls_pipeline_test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-16 22:03:06.000000 data2rdf-2.0.0rc5/tests/xls_pipeline_test/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.172926 data2rdf-2.0.0rc6/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 23:40:23.172926 data2rdf-2.0.0rc6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.164926 data2rdf-2.0.0rc6/data2rdf/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2115 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.164926 data2rdf-2.0.0rc6/data2rdf/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/models/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/data2rdf/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/parsers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/parsers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/data2rdf/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/pipelines/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/pipelines/abox_scaffolding_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5656 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/pipelines/annotation_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/data2rdf/qudt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/qudt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/qudt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/data2rdf/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/data2rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 23:40:23.000000 data2rdf-2.0.0rc6/data2rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 23:40:23.000000 data2rdf-2.0.0rc6/data2rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 23:40:23.000000 data2rdf-2.0.0rc6/data2rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 23:40:23.000000 data2rdf-2.0.0rc6/data2rdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 23:40:23.000000 data2rdf-2.0.0rc6/data2rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 23:40:23.000000 data2rdf-2.0.0rc6/data2rdf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-16 23:40:23.172926 data2rdf-2.0.0rc6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/tests/csv_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/csv_pipeline_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/tests/csv_pipeline_test/input/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/csv_pipeline_test/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/csv_pipeline_test/test_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5333 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/csv_pipeline_test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:23.168926 data2rdf-2.0.0rc6/tests/xls_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/xls_pipeline_test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6450 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/xls_pipeline_test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-16 23:40:19.000000 data2rdf-2.0.0rc6/tests/xls_pipeline_test/test_pipeline.py
```

### Comparing `data2rdf-2.0.0rc5/LICENSE` & `data2rdf-2.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/PKG-INFO` & `data2rdf-2.0.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc5
+Version: 2.0.0rc6
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-2.0.0rc5/README.md` & `data2rdf-2.0.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/data2rdf/config.py` & `data2rdf-2.0.0rc6/data2rdf/config.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/data2rdf/models/mapping.py` & `data2rdf-2.0.0rc6/data2rdf/models/mapping.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/data2rdf/parsers/base.py` & `data2rdf-2.0.0rc6/data2rdf/parsers/base.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/data2rdf/parsers/csv.py` & `data2rdf-2.0.0rc6/data2rdf/parsers/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,15 @@
                 # instanciate model
                 model_data = {
                     "key": key,
                     "value": metadatum.get("value"),
                     "unit": unit,
                     "iri": mapping_match.iri,
                     "annotation": mapping_match.annotation or None,
+                    "config": self.config,
                 }
                 if model_data.get("unit"):
                     model = QuantityMapping(**model_data)
                 else:
                     model = PropertyMapping(**model_data)
                 self._general_metadata.append(model)
             else:
@@ -213,14 +214,15 @@
 
                 # assign model
                 model = QuantityMapping(
                     key=key,
                     unit=unit,
                     iri=mapping_match.iri,
                     annotation=mapping_match.annotation or None,
+                    config=self.config,
                 )
 
                 # append model
                 self.time_series_metadata.append(model)
 
                 # assign time series data
                 self._time_series[model.suffix] = time_series[key][
```

### Comparing `data2rdf-2.0.0rc5/data2rdf/parsers/excel.py` & `data2rdf-2.0.0rc6/data2rdf/parsers/excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,14 +217,15 @@
 
             # make model
             model_data = {
                 "key": datum.key,
                 "unit": unit,
                 "iri": datum.iri,
                 "annotation": datum.annotation,
+                "config": self.config,
             }
 
             if datum.value_location and not datum.time_series_start:
                 value = worksheet[datum.value_location].value
                 if model_data.get("unit") and value:
                     model_data["value"] = value
                 elif not model_data.get("unit") and value:
```

### Comparing `data2rdf-2.0.0rc5/data2rdf/parsers/utils.py` & `data2rdf-2.0.0rc6/data2rdf/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/data2rdf/pipelines/abox_scaffolding_pipeline.py` & `data2rdf-2.0.0rc6/data2rdf/pipelines/abox_scaffolding_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/data2rdf/pipelines/annotation_pipeline.py` & `data2rdf-2.0.0rc6/data2rdf/pipelines/annotation_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/data2rdf/qudt/utils.py` & `data2rdf-2.0.0rc6/data2rdf/qudt/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/data2rdf/utils.py` & `data2rdf-2.0.0rc6/data2rdf/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/data2rdf.egg-info/PKG-INFO` & `data2rdf-2.0.0rc6/data2rdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc5
+Version: 2.0.0rc6
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-2.0.0rc5/data2rdf.egg-info/SOURCES.txt` & `data2rdf-2.0.0rc6/data2rdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/data2rdf.egg-info/requires.txt` & `data2rdf-2.0.0rc6/data2rdf.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/setup.cfg` & `data2rdf-2.0.0rc6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data2rdf
-version = v2.0.0rc5
+version = v2.0.0rc6
 description = A generic pipeline that can be used to map raw data to RDF.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/data2rdf
 author = Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 license = BSD-3-Clause
```

### Comparing `data2rdf-2.0.0rc5/tests/csv_pipeline_test/test_parser.py` & `data2rdf-2.0.0rc6/tests/csv_pipeline_test/test_parser.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/tests/csv_pipeline_test/test_pipeline.py` & `data2rdf-2.0.0rc6/tests/csv_pipeline_test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/tests/test_models.py` & `data2rdf-2.0.0rc6/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/tests/test_utils.py` & `data2rdf-2.0.0rc6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/tests/xls_pipeline_test/test_parser.py` & `data2rdf-2.0.0rc6/tests/xls_pipeline_test/test_parser.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc5/tests/xls_pipeline_test/test_pipeline.py` & `data2rdf-2.0.0rc6/tests/xls_pipeline_test/test_pipeline.py`

 * *Files identical despite different names*

