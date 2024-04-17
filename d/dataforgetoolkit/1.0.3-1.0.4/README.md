# Comparing `tmp/dataforgetoolkit-1.0.3-py3-none-any.whl.zip` & `tmp/dataforgetoolkit-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4028 bytes, number of entries: 7
+Zip file size: 4093 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      875 b- defN 24-Apr-17 09:58 dataforgetoolkit/__init__.py
 -rw-r--r--  2.0 unx      212 b- defN 24-Apr-17 09:19 dataforgetoolkit/common_utils.py
--rw-r--r--  2.0 unx     3694 b- defN 24-Apr-17 09:21 dataforgetoolkit/datamapper.py
--rw-r--r--  2.0 unx     2003 b- defN 24-Apr-17 10:13 dataforgetoolkit-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 10:13 dataforgetoolkit-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-17 10:13 dataforgetoolkit-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      593 b- defN 24-Apr-17 10:13 dataforgetoolkit-1.0.3.dist-info/RECORD
-7 files, 7486 bytes uncompressed, 2966 bytes compressed:  60.4%
+-rw-r--r--  2.0 unx     3929 b- defN 24-Apr-17 15:00 dataforgetoolkit/datamapper.py
+-rw-r--r--  2.0 unx     2003 b- defN 24-Apr-17 15:05 dataforgetoolkit-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 15:05 dataforgetoolkit-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-17 15:05 dataforgetoolkit-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      593 b- defN 24-Apr-17 15:05 dataforgetoolkit-1.0.4.dist-info/RECORD
+7 files, 7721 bytes uncompressed, 3031 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: dataforgetoolkit/common_utils.py
 Comment: 
 
 Filename: dataforgetoolkit/datamapper.py
 Comment: 
 
-Filename: dataforgetoolkit-1.0.3.dist-info/METADATA
+Filename: dataforgetoolkit-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: dataforgetoolkit-1.0.3.dist-info/WHEEL
+Filename: dataforgetoolkit-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: dataforgetoolkit-1.0.3.dist-info/top_level.txt
+Filename: dataforgetoolkit-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: dataforgetoolkit-1.0.3.dist-info/RECORD
+Filename: dataforgetoolkit-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dataforgetoolkit/datamapper.py

```diff
@@ -10,15 +10,21 @@
     Args:
         report_file_path (str): Path to the CSV or Excel file.
         transformation_file_path (str): Path to the JSON transformation file.
 
     Returns:
         dict: Mapped data in dictionary format.
     """
-    df = df = pd.read_csv(report_file_path)
+    if report_file_path.endswith('.csv'):
+        df = pd.read_csv(report_file_path)
+    elif report_file_path.endswith('.xlsx'):
+        df = pd.read_excel(report_file_path)
+    else:
+        return {"error": "Unsupported file format. Only CSV and Excel files are supported."}
+
     df = df.fillna('')
     try:
         with open(transformation_file_path, "r") as json_file:
             transformations = json.load(json_file)['transformation_mapping']
     except json.JSONDecodeError:
         return {"error": "Invalid JSON format for transformations."}
```

## Comparing `dataforgetoolkit-1.0.3.dist-info/METADATA` & `dataforgetoolkit-1.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataforgetoolkit
-Version: 1.0.3
+Version: 1.0.4
 Summary: It is a library that facilitates converting CSV files to various formats (such as DataFrames or other CSV/Excel files) based on a JSON mapping
 Home-page: https://github.com/amitsingh7668/dataforgetoolkit
 Author: Amit Singh
 Author-email: 2singh.amit3@gmail.com
 License: Amit Singh
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `dataforgetoolkit-1.0.3.dist-info/RECORD` & `dataforgetoolkit-1.0.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 dataforgetoolkit/__init__.py,sha256=zkyUri73xFqI869Ok73yH2SidWrsS7D7a7y0foTFatE,875
 dataforgetoolkit/common_utils.py,sha256=pjPA-SU6f8V_l6ICe9YLmLUVxvlWJQeIOLyvBJXTjDs,212
-dataforgetoolkit/datamapper.py,sha256=xnjB3__KSsEiH3d-KVCf62rHh-AD2U2ZjOCcpO1t3Cg,3694
-dataforgetoolkit-1.0.3.dist-info/METADATA,sha256=5Q5lUAjVTiynf4bZ_iW5psaJk9zxwZP9xRb0Qhmk89w,2003
-dataforgetoolkit-1.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dataforgetoolkit-1.0.3.dist-info/top_level.txt,sha256=WL_asJIhhKds6gBhWlc8rIVvUF_KWPJ03uzY92r6tcg,17
-dataforgetoolkit-1.0.3.dist-info/RECORD,,
+dataforgetoolkit/datamapper.py,sha256=5hP_c91zky_wW9wNfay0y6xtjn1JHd71uE1gh_NWemY,3929
+dataforgetoolkit-1.0.4.dist-info/METADATA,sha256=7IOSs8JqJHrYUZU59xkn115kXgBX7kWK_kJ40NPcJ84,2003
+dataforgetoolkit-1.0.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dataforgetoolkit-1.0.4.dist-info/top_level.txt,sha256=WL_asJIhhKds6gBhWlc8rIVvUF_KWPJ03uzY92r6tcg,17
+dataforgetoolkit-1.0.4.dist-info/RECORD,,
```

