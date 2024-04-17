# Comparing `tmp/dataforgetoolkit-1.0.1-py3-none-any.whl.zip` & `tmp/dataforgetoolkit-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2632 bytes, number of entries: 7
+Zip file size: 3155 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 07:17 dataforgetoolkit/__init__.py
--rw-r--r--  2.0 unx       42 b- defN 24-Apr-17 07:17 dataforgetoolkit/common_utils.py
--rw-r--r--  2.0 unx     2064 b- defN 24-Apr-17 07:58 dataforgetoolkit/datamapper.py
--rw-r--r--  2.0 unx      865 b- defN 24-Apr-17 08:00 dataforgetoolkit-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 08:00 dataforgetoolkit-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-17 08:00 dataforgetoolkit-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      589 b- defN 24-Apr-17 08:00 dataforgetoolkit-1.0.1.dist-info/RECORD
-7 files, 3669 bytes uncompressed, 1570 bytes compressed:  57.2%
+-rw-r--r--  2.0 unx      212 b- defN 24-Apr-17 09:19 dataforgetoolkit/common_utils.py
+-rw-r--r--  2.0 unx     3694 b- defN 24-Apr-17 09:21 dataforgetoolkit/datamapper.py
+-rw-r--r--  2.0 unx      865 b- defN 24-Apr-17 09:22 dataforgetoolkit-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 09:22 dataforgetoolkit-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-17 09:22 dataforgetoolkit-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      590 b- defN 24-Apr-17 09:22 dataforgetoolkit-1.0.2.dist-info/RECORD
+7 files, 5470 bytes uncompressed, 2093 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: dataforgetoolkit/common_utils.py
 Comment: 
 
 Filename: dataforgetoolkit/datamapper.py
 Comment: 
 
-Filename: dataforgetoolkit-1.0.1.dist-info/METADATA
+Filename: dataforgetoolkit-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: dataforgetoolkit-1.0.1.dist-info/WHEEL
+Filename: dataforgetoolkit-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: dataforgetoolkit-1.0.1.dist-info/top_level.txt
+Filename: dataforgetoolkit-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dataforgetoolkit-1.0.1.dist-info/RECORD
+Filename: dataforgetoolkit-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dataforgetoolkit/common_utils.py

```diff
@@ -1,2 +1,7 @@
-DAFULT_VALUE = "*"
-FILTER_VALUE = "FILTER"
+DEFAULT_VALUE = "*"
+FILTER_VALUE = "FILTER"
+REPLACE_VALUE = "REPLACE_"
+CONCAT_VALUE = "CONCAT"
+UPPERCASE_VALUE = "UPPERCASE"
+LOWERCASE_VALUE = "LOWERCASE"
+# Path: dataforgetoolkit/dataforgetoolkit/common_utils.py
```

## dataforgetoolkit/datamapper.py

```diff
@@ -1,15 +1,23 @@
 import pandas as pd
 import json
 from dataforgetoolkit.common_utils import *
-import logging
 
-logging.basicConfig(level=logging.INFO)
 
 def map(report_file_path, transformation_file_path):
+    """
+    Map a CSV or Excel file based on a JSON transformation mapping.
+
+    Args:
+        report_file_path (str): Path to the CSV or Excel file.
+        transformation_file_path (str): Path to the JSON transformation file.
+
+    Returns:
+        dict: Mapped data in dictionary format.
+    """
     df = df = pd.read_csv(report_file_path)
     df = df.fillna('')
     try:
         with open(transformation_file_path, "r") as json_file:
             transformations = json.load(json_file)['transformation_mapping']
     except json.JSONDecodeError:
         return {"error": "Invalid JSON format for transformations."}
@@ -19,14 +27,24 @@
 
     # Update column names and values
     df = transform_model(df, transformations)
     return df.to_dict(orient='records')
 
 
 def transform_model(df, transformation):
+    """
+    Transform the DataFrame based on the provided transformation mapping.
+
+    Args:
+        df (DataFrame): Input DataFrame.
+        transformation (dict): Transformation mapping.
+
+    Returns:
+        DataFrame: Transformed DataFrame.
+    """
     # List of column names to keep
     column_names = [transformation["column"]
                     for transformation in transformation]
 
     # Drop columns not in the column_names list
     columns_to_drop = [col for col in df.columns if col not in column_names]
     df.drop(columns=columns_to_drop, inplace=True)
@@ -34,26 +52,54 @@
     # Update column names and values as per the transformation
     for transformation in transformation:
         old_name = transformation["column"]
         new_name = transformation["new_name"]
         value_mappings = transformation["value_mappings"]
 
         if old_name in df.columns:
-            logging.info(f"Updating column '{old_name}' to '{new_name}'")
+            print(f"Updating column '{old_name}' to '{new_name}'")
             df.rename(columns={old_name: new_name}, inplace=True)
 
-            logging.info(f"Updating values in column '{new_name}'")
+            print(f"Updating values in column '{new_name}'")
             for value_mapping in value_mappings:
                 for old_value, new_value in value_mapping.items():
-                    df = mapping_criteria(df, new_name, old_value, new_value)
+                    df = apply_mapping_criteria(
+                        df, new_name, old_value, new_value)
                     df[new_name] = df[new_name].replace(old_value, new_value)
 
     return df
 
 
-def mapping_criteria(df, new_name, old_value, new_value):
-    if old_value == DAFULT_VALUE:
-        df[new_name] = new_value
-        pass
-    if old_value == FILTER_VALUE:
-        df = df[df[new_name] != new_value]
-    return df
+def apply_mapping_criteria(df, column_name, old_value, new_value):
+    """
+    Apply mapping criteria to the DataFrame.
+
+    Args:
+        df (DataFrame): Input DataFrame.
+        column_name (str): Column name to apply mapping criteria.
+        old_value (str): Old value to be replaced.
+        new_value (str): New value.
+
+    Returns:
+        DataFrame: Transformed DataFrame.
+    """
+    if old_value == DEFAULT_VALUE:
+        df[column_name] = new_value
+    elif old_value == FILTER_VALUE:
+        df = df[df[column_name] != new_value]
+    elif old_value.startswith(REPLACE_VALUE):
+        # Replace substrings in column values
+        substring = old_value.split("_", 1)[1]
+        df[column_name] = df[column_name].str.replace(substring, new_value)
+    elif old_value == CONCAT_VALUE:
+        # Concatenate column values with a delimiter
+        delimiter = new_value
+        df[column_name] = df[column_name].apply(
+            lambda x: delimiter.join(x) if isinstance(x, list) else x)
+    elif old_value == UPPERCASE_VALUE:
+        # Convert column values to uppercase
+        df[column_name] = df[column_name].str.upper()
+    elif old_value == LOWERCASE_VALUE:
+        # Convert column values to lowercase
+        df[column_name] = df[column_name].str.lower()
+    # Add more conditions for other aggregations if needed
+    return df
```

## Comparing `dataforgetoolkit-1.0.1.dist-info/METADATA` & `dataforgetoolkit-1.0.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataforgetoolkit
-Version: 1.0.1
+Version: 1.0.2
 Summary: It is a library that facilitates converting CSV files to various formats (such as DataFrames or other CSV/Excel files) based on a JSON mapping
 Home-page: https://github.com/amitsingh7668/dataforgetoolkit
 Author: Amit Singh
 Author-email: 2singh.amit3@gmail.com
 License: Amit Singh
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

