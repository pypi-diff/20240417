# Comparing `tmp/libs_zip-0.0.1-py3-none-any.whl.zip` & `tmp/libs_zip-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,9 @@
-Zip file size: 1859 bytes, number of entries: 5
--rw-------  2.0 unx     1067 b- defN 24-Apr-16 07:03 libs_zip-0.0.1.dist-info/LICENSE
--rw-------  2.0 unx      192 b- defN 24-Apr-16 07:03 libs_zip-0.0.1.dist-info/METADATA
--rw-------  2.0 unx       92 b- defN 24-Apr-16 07:03 libs_zip-0.0.1.dist-info/WHEEL
--rw-------  2.0 unx        6 b- defN 24-Apr-16 07:03 libs_zip-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      389 b- defN 24-Apr-16 07:03 libs_zip-0.0.1.dist-info/RECORD
-5 files, 1746 bytes uncompressed, 1129 bytes compressed:  35.3%
+Zip file size: 2361 bytes, number of entries: 7
+-rw-------  2.0 unx       31 b- defN 24-Apr-16 06:04 libs/test.py
+-rw-------  2.0 unx      210 b- defN 24-Apr-16 06:43 libs/web.py
+-rw-------  2.0 unx     1067 b- defN 24-Apr-16 07:13 libs_zip-0.0.2.dist-info/LICENSE
+-rw-------  2.0 unx      192 b- defN 24-Apr-16 07:13 libs_zip-0.0.2.dist-info/METADATA
+-rw-------  2.0 unx       92 b- defN 24-Apr-16 07:13 libs_zip-0.0.2.dist-info/WHEEL
+-rw-------  2.0 unx        5 b- defN 24-Apr-16 07:13 libs_zip-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      523 b- defN 24-Apr-16 07:13 libs_zip-0.0.2.dist-info/RECORD
+7 files, 2120 bytes uncompressed, 1433 bytes compressed:  32.4%
```

## zipnote {}

```diff
@@ -1,16 +1,22 @@
-Filename: libs_zip-0.0.1.dist-info/LICENSE
+Filename: libs/test.py
 Comment: 
 
-Filename: libs_zip-0.0.1.dist-info/METADATA
+Filename: libs/web.py
 Comment: 
 
-Filename: libs_zip-0.0.1.dist-info/WHEEL
+Filename: libs_zip-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: libs_zip-0.0.1.dist-info/top_level.txt
+Filename: libs_zip-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: libs_zip-0.0.1.dist-info/RECORD
+Filename: libs_zip-0.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: libs_zip-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: libs_zip-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `libs_zip-0.0.1.dist-info/LICENSE` & `libs_zip-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

