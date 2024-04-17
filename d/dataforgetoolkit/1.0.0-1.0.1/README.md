# Comparing `tmp/dataforgetoolkit-1.0.0-py3-none-any.whl.zip` & `tmp/dataforgetoolkit-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2599 bytes, number of entries: 7
+Zip file size: 2632 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 07:17 dataforgetoolkit/__init__.py
 -rw-r--r--  2.0 unx       42 b- defN 24-Apr-17 07:17 dataforgetoolkit/common_utils.py
--rw-r--r--  2.0 unx     1994 b- defN 24-Apr-17 07:37 dataforgetoolkit/datamapper.py
--rw-r--r--  2.0 unx      865 b- defN 24-Apr-17 07:44 dataforgetoolkit-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 07:44 dataforgetoolkit-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-17 07:44 dataforgetoolkit-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      589 b- defN 24-Apr-17 07:44 dataforgetoolkit-1.0.0.dist-info/RECORD
-7 files, 3599 bytes uncompressed, 1537 bytes compressed:  57.3%
+-rw-r--r--  2.0 unx     2064 b- defN 24-Apr-17 07:58 dataforgetoolkit/datamapper.py
+-rw-r--r--  2.0 unx      865 b- defN 24-Apr-17 08:00 dataforgetoolkit-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 08:00 dataforgetoolkit-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-17 08:00 dataforgetoolkit-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      589 b- defN 24-Apr-17 08:00 dataforgetoolkit-1.0.1.dist-info/RECORD
+7 files, 3669 bytes uncompressed, 1570 bytes compressed:  57.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: dataforgetoolkit/common_utils.py
 Comment: 
 
 Filename: dataforgetoolkit/datamapper.py
 Comment: 
 
-Filename: dataforgetoolkit-1.0.0.dist-info/METADATA
+Filename: dataforgetoolkit-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: dataforgetoolkit-1.0.0.dist-info/WHEEL
+Filename: dataforgetoolkit-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: dataforgetoolkit-1.0.0.dist-info/top_level.txt
+Filename: dataforgetoolkit-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dataforgetoolkit-1.0.0.dist-info/RECORD
+Filename: dataforgetoolkit-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dataforgetoolkit/datamapper.py

```diff
@@ -1,10 +1,13 @@
 import pandas as pd
 import json
 from dataforgetoolkit.common_utils import *
+import logging
+
+logging.basicConfig(level=logging.INFO)
 
 def map(report_file_path, transformation_file_path):
     df = df = pd.read_csv(report_file_path)
     df = df.fillna('')
     try:
         with open(transformation_file_path, "r") as json_file:
             transformations = json.load(json_file)['transformation_mapping']
@@ -31,18 +34,18 @@
     # Update column names and values as per the transformation
     for transformation in transformation:
         old_name = transformation["column"]
         new_name = transformation["new_name"]
         value_mappings = transformation["value_mappings"]
 
         if old_name in df.columns:
-            print(f"Updating column '{old_name}' to '{new_name}'")
+            logging.info(f"Updating column '{old_name}' to '{new_name}'")
             df.rename(columns={old_name: new_name}, inplace=True)
 
-            print(f"Updating values in column '{new_name}'")
+            logging.info(f"Updating values in column '{new_name}'")
             for value_mapping in value_mappings:
                 for old_value, new_value in value_mapping.items():
                     df = mapping_criteria(df, new_name, old_value, new_value)
                     df[new_name] = df[new_name].replace(old_value, new_value)
 
     return df
```

## Comparing `dataforgetoolkit-1.0.0.dist-info/METADATA` & `dataforgetoolkit-1.0.1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataforgetoolkit
-Version: 1.0.0
+Version: 1.0.1
 Summary: It is a library that facilitates converting CSV files to various formats (such as DataFrames or other CSV/Excel files) based on a JSON mapping
 Home-page: https://github.com/amitsingh7668/dataforgetoolkit
 Author: Amit Singh
 Author-email: 2singh.amit3@gmail.com
 License: Amit Singh
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `dataforgetoolkit-1.0.0.dist-info/RECORD` & `dataforgetoolkit-1.0.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 dataforgetoolkit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dataforgetoolkit/common_utils.py,sha256=bj6c4StQD7z0VRe83ydhy0q2GWdRE8V3iRmfihO0TAs,42
-dataforgetoolkit/datamapper.py,sha256=R-mlBOpEcj8y-fr0FJWaOorUylGxMGpy-UymbcFuKik,1994
-dataforgetoolkit-1.0.0.dist-info/METADATA,sha256=xT3AMZtUDJgLui3MZSezhgrH9CUrvmv2qa2dgB4fSqM,865
-dataforgetoolkit-1.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dataforgetoolkit-1.0.0.dist-info/top_level.txt,sha256=WL_asJIhhKds6gBhWlc8rIVvUF_KWPJ03uzY92r6tcg,17
-dataforgetoolkit-1.0.0.dist-info/RECORD,,
+dataforgetoolkit/datamapper.py,sha256=BGkk91CfDjr79ETgv6iIGV-Gt8amlv-nzdj8vbGbJ1s,2064
+dataforgetoolkit-1.0.1.dist-info/METADATA,sha256=oqPBhQOEphMaVSru_ziRd-ewEgMycdahzSwPPg4N99U,865
+dataforgetoolkit-1.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dataforgetoolkit-1.0.1.dist-info/top_level.txt,sha256=WL_asJIhhKds6gBhWlc8rIVvUF_KWPJ03uzY92r6tcg,17
+dataforgetoolkit-1.0.1.dist-info/RECORD,,
```

