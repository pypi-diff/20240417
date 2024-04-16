# Comparing `tmp/data2rdf-2.0.0rc3.tar.gz` & `tmp/data2rdf-2.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2rdf-2.0.0rc3.tar", last modified: Tue Apr 16 11:29:24 2024, max compression
+gzip compressed data, was "data2rdf-2.0.0rc4.tar", last modified: Tue Apr 16 13:07:35 2024, max compression
```

## Comparing `data2rdf-2.0.0rc3.tar` & `data2rdf-2.0.0rc4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.944334 data2rdf-2.0.0rc3/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 11:29:24.944334 data2rdf-2.0.0rc3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.936334 data2rdf-2.0.0rc3/data2rdf/
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1882 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/data2rdf/models/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/models/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/data2rdf/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/parsers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/parsers/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/parsers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/data2rdf/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/pipelines/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/pipelines/abox_scaffolding_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5656 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/pipelines/annotation_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/data2rdf/qudt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/qudt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/qudt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.944334 data2rdf-2.0.0rc3/data2rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 11:29:24.000000 data2rdf-2.0.0rc3/data2rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 11:29:24.000000 data2rdf-2.0.0rc3/data2rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:29:24.000000 data2rdf-2.0.0rc3/data2rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 11:29:24.000000 data2rdf-2.0.0rc3/data2rdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 11:29:24.000000 data2rdf-2.0.0rc3/data2rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 11:29:24.000000 data2rdf-2.0.0rc3/data2rdf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-16 11:29:24.944334 data2rdf-2.0.0rc3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/tests/csv_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/csv_pipeline_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/tests/csv_pipeline_test/input/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/csv_pipeline_test/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/csv_pipeline_test/test_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4972 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/csv_pipeline_test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.944334 data2rdf-2.0.0rc3/tests/xls_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/xls_pipeline_test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6059 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/xls_pipeline_test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/xls_pipeline_test/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.082656 data2rdf-2.0.0rc4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 13:07:35.082656 data2rdf-2.0.0rc4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.078656 data2rdf-2.0.0rc4/data2rdf/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2115 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.078656 data2rdf-2.0.0rc4/data2rdf/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/models/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.078656 data2rdf-2.0.0rc4/data2rdf/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/parsers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/parsers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.078656 data2rdf-2.0.0rc4/data2rdf/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/pipelines/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/pipelines/abox_scaffolding_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5656 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/pipelines/annotation_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.078656 data2rdf-2.0.0rc4/data2rdf/qudt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/qudt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/qudt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/data2rdf/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.082656 data2rdf-2.0.0rc4/data2rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 13:07:35.000000 data2rdf-2.0.0rc4/data2rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 13:07:35.000000 data2rdf-2.0.0rc4/data2rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:07:35.000000 data2rdf-2.0.0rc4/data2rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 13:07:35.000000 data2rdf-2.0.0rc4/data2rdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 13:07:35.000000 data2rdf-2.0.0rc4/data2rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 13:07:35.000000 data2rdf-2.0.0rc4/data2rdf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-16 13:07:35.086656 data2rdf-2.0.0rc4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.078656 data2rdf-2.0.0rc4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.082656 data2rdf-2.0.0rc4/tests/csv_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/csv_pipeline_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.082656 data2rdf-2.0.0rc4/tests/csv_pipeline_test/input/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/csv_pipeline_test/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/csv_pipeline_test/test_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4980 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/csv_pipeline_test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:35.082656 data2rdf-2.0.0rc4/tests/xls_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/xls_pipeline_test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6059 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/xls_pipeline_test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-16 13:07:31.000000 data2rdf-2.0.0rc4/tests/xls_pipeline_test/test_pipeline.py
```

### Comparing `data2rdf-2.0.0rc3/LICENSE` & `data2rdf-2.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/PKG-INFO` & `data2rdf-2.0.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-2.0.0rc3/README.md` & `data2rdf-2.0.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/data2rdf/config.py` & `data2rdf-2.0.0rc4/data2rdf/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,8 +50,14 @@
     )
 
     unit_macro_location: int = Field(
         -1,
         description="Index where the marco for the unit in an excel cell might be located.",
     )
 
+    max_row_iteration: int = Field(
+        1e12,
+        description="""In Excel files, the parser is scanning for the end of the time series.
+        In order to prevent a frozen process, this maximum row number is set.""",
+    )
+
     model_config = ConfigDict(extra="ignore")
```

### Comparing `data2rdf-2.0.0rc3/data2rdf/models/mapping.py` & `data2rdf-2.0.0rc4/data2rdf/models/mapping.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,18 +69,14 @@
     unit_location: Optional[str] = Field(
         None, description="Cell location for the unit of the quantity"
     )
     time_series_start: Optional[str] = Field(
         None,
         description="Cell location for the start of the time series quantity",
     )
-    time_series_end: Optional[str] = Field(
-        None,
-        description="Cell location for the end of the time series quantity",
-    )
     worksheet: Optional[str] = Field(
         None,
         description="Name of the worksheet where the entity is located in the excel file",
     )
 
 
 class MergedConceptMapping(BasicConceptMapping):
@@ -92,15 +88,14 @@
         """Return dict for json-ld of graph"""
 
     @property
     def graph(cls) -> Graph:
         """Return graph object based on json-ld"""
         graph = Graph(identifier=cls.config.graph_identifier)
         graph.parse(data=json.dumps(cls.json_ld), format="json-ld")
-        print(cls.json_ld)
         return graph
 
 
 class QuantityMapping(MergedConceptMapping):
     """Mapping for a quantity without a discrete value.
     E.g. a quantity describing a column of a time series or table."""
 
@@ -199,10 +194,30 @@
         return {
             "@context": {
                 "fileid": make_prefix(cls.config),
                 "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
                 "xsd": "http://www.w3.org/2001/XMLSchema#",
             },
             "@id": f"fileid:{cls.suffix}",
-            "@type": str(cls.iri),
             "rdfs:label": cls.value,
+            **cls.types_json,
         }
+
+    @property
+    def types_json(cls) -> "Dict[str, Any]":
+        """Dict of json-ld for class types of the individual"""
+        if cls.annotation:
+            if str(cls.annotation).endswith(cls.config.separator):
+                annotation = str(cls.annotation) + cls.value
+            else:
+                annotation = (
+                    str(cls.annotation) + cls.config.separator + cls.value
+                )
+            types = {
+                "@type": [
+                    str(cls.iri),
+                    annotation,
+                ]
+            }
+        else:
+            types = {"@type": str(cls.iri)}
+        return types
```

### Comparing `data2rdf-2.0.0rc3/data2rdf/parsers/base.py` & `data2rdf-2.0.0rc4/data2rdf/parsers/base.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/data2rdf/parsers/csv.py` & `data2rdf-2.0.0rc4/data2rdf/parsers/csv.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/data2rdf/parsers/excel.py` & `data2rdf-2.0.0rc4/data2rdf/parsers/excel.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     PropertyMapping,
     QuantityMapping,
 )
 from data2rdf.utils import make_prefix
 from data2rdf.warnings import MappingMissmatchWarning
 
 from .base import DataParser
-from .utils import _strip_unit, load_mapping_file
+from .utils import _find_end_of_series, _strip_unit, load_mapping_file
 
 
 class ExcelParser(DataParser):
     """
     Parses a data file of type CSV
     """
 
@@ -150,46 +150,35 @@
 
         self._general_metadata = []
         self._time_series_metadata = []
         self._time_series = {}
         for key, datum in mapping.items():
             worksheet = datafile[datum.worksheet]
 
-            if datum.value_location and (
-                datum.time_series_start and datum.time_series_end
-            ):
+            if datum.value_location and datum.time_series_start:
                 raise RuntimeError(
-                    """Both, `value_location` and `time_series_start + `time_series_end`
+                    """Both, `value_location` and `time_series_start
                        are set. Only one of them must be set."""
                 )
-            if (
-                not datum.value_location
-                and datum.time_series_start
-                and not datum.time_series_end
-            ):
-                raise RuntimeError("Please also set `time_series_end`.")
-
-            if (
-                not datum.value_location
-                and not datum.time_series_start
-                and datum.time_series_end
-            ):
-                raise RuntimeError("Please also set `time_series_start`.")
 
             # find data for time series
-            if datum.time_series_start and datum.time_series_end:
-                column = worksheet[
-                    datum.time_series_start : datum.time_series_end
-                ]
+            if datum.time_series_start:
+                time_series_end = _find_end_of_series(
+                    worksheet,
+                    datum.time_series_start,
+                    self.config.max_row_iteration,
+                )
+
+                column = worksheet[datum.time_series_start : time_series_end]
                 if column:
                     self.time_series[key] = [cell[0].value for cell in column]
                 else:
                     message = f"""Concept with key `{key}`
                                   does not have a time series from `{datum.time_series_start}`
-                                  until ``{datum.time_series_end}` .
+                                  until ``{time_series_end}` .
                                   Concept will be omitted in graph.
                                   """
                     warnings.warn(message, MappingMissmatchWarning)
 
             # check if there is a macro for the unit of the entity
             if datum.value_location:
                 macro_worksheet = macros[datum.worksheet]
@@ -226,17 +215,15 @@
             model_data = {
                 "key": datum.key,
                 "unit": unit,
                 "iri": datum.iri,
                 "annotation": datum.annotation,
             }
 
-            if datum.value_location and not (
-                datum.time_series_start and datum.time_series_end
-            ):
+            if datum.value_location and not datum.time_series_start:
                 value = worksheet[datum.value_location].value
                 if model_data.get("unit") and value:
                     model_data["value"] = value
                 elif not model_data.get("unit") and value:
                     model_data["value"] = str(value)
                 else:
                     message = f"""Concept with key `{key}`
```

### Comparing `data2rdf-2.0.0rc3/data2rdf/pipelines/abox_scaffolding_pipeline.py` & `data2rdf-2.0.0rc4/data2rdf/pipelines/abox_scaffolding_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/data2rdf/pipelines/annotation_pipeline.py` & `data2rdf-2.0.0rc4/data2rdf/pipelines/annotation_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/data2rdf/qudt/utils.py` & `data2rdf-2.0.0rc4/data2rdf/qudt/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/data2rdf/utils.py` & `data2rdf-2.0.0rc4/data2rdf/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/data2rdf.egg-info/PKG-INFO` & `data2rdf-2.0.0rc4/data2rdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-2.0.0rc3/data2rdf.egg-info/SOURCES.txt` & `data2rdf-2.0.0rc4/data2rdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/data2rdf.egg-info/requires.txt` & `data2rdf-2.0.0rc4/data2rdf.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/setup.cfg` & `data2rdf-2.0.0rc4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data2rdf
-version = v2.0.0rc3
+version = v2.0.0rc4
 description = A generic pipeline that can be used to map raw data to RDF.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/data2rdf
 author = Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 license = BSD-3-Clause
```

### Comparing `data2rdf-2.0.0rc3/tests/csv_pipeline_test/test_parser.py` & `data2rdf-2.0.0rc4/tests/csv_pipeline_test/test_parser.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/tests/csv_pipeline_test/test_pipeline.py` & `data2rdf-2.0.0rc4/tests/csv_pipeline_test/test_pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,35 +46,35 @@
 
 
 def test_csv_pipeline_bad_mapping() -> None:
     from rdflib import Graph
 
     from data2rdf import AnnotationPipeline, Parser
 
-    parser = AnnotationPipeline(
+    pipeline = AnnotationPipeline(
         raw_data=raw_data,
         mapping=os.path.join(mapping_folder, "bad_tensile_test_mapping.json"),
         parser=Parser.csv,
         parser_args=parser_args,
         extra_triples=template,
     )
     expected_graph = Graph()
     expected_graph.parse(expected)
 
-    assert parser.graph.isomorphic(expected_graph)
+    assert pipeline.graph.isomorphic(expected_graph)
 
 
 def test_csv_pipeline_no_match_in_mapping() -> None:
     from rdflib import Graph
 
     from data2rdf import AnnotationPipeline, Parser
     from data2rdf.warnings import MappingMissmatchWarning
 
     with pytest.warns(UserWarning, match="No match found") as warnings:
-        parser = AnnotationPipeline(
+        pipeline = AnnotationPipeline(
             raw_data=os.path.join(
                 working_folder, "data", "BAD_DX56_D_FZ2_WR00_43.TXT"
             ),
             parser=Parser.csv,
             extra_triples=template,
             mapping=os.path.join(mapping_folder, "tensile_test_mapping.json"),
             parser_args={
@@ -90,15 +90,15 @@
         if warning.category == MappingMissmatchWarning
     ]
     assert len(missmatches) == 1
 
     expected_graph = Graph()
     expected_graph.parse(expected)
 
-    assert parser.graph.isomorphic(expected_graph)
+    assert pipeline.graph.isomorphic(expected_graph)
 
 
 @pytest.mark.parametrize("config", [normal_config, bad_config])
 def test_csv_pipeline_config(config) -> None:
     from rdflib import Graph
 
     from data2rdf import (  # isort:skip
```

### Comparing `data2rdf-2.0.0rc3/tests/test_models.py` & `data2rdf-2.0.0rc4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/tests/test_utils.py` & `data2rdf-2.0.0rc4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/tests/xls_pipeline_test/test_parser.py` & `data2rdf-2.0.0rc4/tests/xls_pipeline_test/test_parser.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc3/tests/xls_pipeline_test/test_pipeline.py` & `data2rdf-2.0.0rc4/tests/xls_pipeline_test/test_pipeline.py`

 * *Files identical despite different names*

