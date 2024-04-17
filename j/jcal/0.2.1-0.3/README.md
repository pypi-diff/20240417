# Comparing `tmp/jcal-0.2.1-py3-none-any.whl.zip` & `tmp/jcal-0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7270 bytes, number of entries: 7
+Zip file size: 7242 bytes, number of entries: 7
 -rw-r--r--  2.0 unx     4695 b- defN 80-Jan-01 00:00 jcal/__init__.py
 -rw-r--r--  2.0 unx       27 b- defN 80-Jan-01 00:00 jcal/__main__.py
--rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 jcal-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1364 b- defN 80-Jan-01 00:00 jcal-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jcal-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       34 b- defN 80-Jan-01 00:00 jcal-0.2.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      519 b- defN 16-Jan-01 00:00 jcal-0.2.1.dist-info/RECORD
-7 files, 17484 bytes uncompressed, 6358 bytes compressed:  63.6%
+-rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 jcal-0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1362 b- defN 80-Jan-01 00:00 jcal-0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jcal-0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       34 b- defN 80-Jan-01 00:00 jcal-0.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      509 b- defN 16-Jan-01 00:00 jcal-0.3.dist-info/RECORD
+7 files, 17472 bytes uncompressed, 6350 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jcal/__init__.py
 Comment: 
 
 Filename: jcal/__main__.py
 Comment: 
 
-Filename: jcal-0.2.1.dist-info/LICENSE
+Filename: jcal-0.3.dist-info/LICENSE
 Comment: 
 
-Filename: jcal-0.2.1.dist-info/METADATA
+Filename: jcal-0.3.dist-info/METADATA
 Comment: 
 
-Filename: jcal-0.2.1.dist-info/WHEEL
+Filename: jcal-0.3.dist-info/WHEEL
 Comment: 
 
-Filename: jcal-0.2.1.dist-info/entry_points.txt
+Filename: jcal-0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: jcal-0.2.1.dist-info/RECORD
+Filename: jcal-0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `jcal-0.2.1.dist-info/LICENSE` & `jcal-0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jcal-0.2.1.dist-info/METADATA` & `jcal-0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: jcal
-Version: 0.2.1
+Version: 0.3
 Summary: `jcal` is a package for Japanese holiday.
 Home-page: https://github.com/SaitoTsutomu/jcal
 License: Apache-2.0
 Author: Saito Tsutomu
 Author-email: tsutomu7@hotmail.co.jp
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 
 # jcal
 
 `jcal` is a package for Japanese holiday at 2019-2021.
```

