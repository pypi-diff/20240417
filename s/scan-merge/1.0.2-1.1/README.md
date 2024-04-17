# Comparing `tmp/scan_merge-1.0.2.tar.gz` & `tmp/scan_merge-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scan_merge-1.0.2.tar", last modified: Sat Jul 30 12:05:25 2022, max compression
+gzip compressed data, was "scan_merge-1.1.tar", last modified: Wed Apr 17 21:00:26 2024, max compression
```

## Comparing `scan_merge-1.0.2.tar` & `scan_merge-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 arvid     (1000) arvid     (1000)        0 2022-07-30 12:05:25.948491 scan_merge-1.0.2/
--rw-r--r--   0 arvid     (1000) arvid     (1000)       54 2022-07-30 11:43:38.000000 scan_merge-1.0.2/.gitignore
--rw-r--r--   0 arvid     (1000) arvid     (1000)    34916 2022-07-30 11:43:38.000000 scan_merge-1.0.2/COPYING.md
--rw-r--r--   0 arvid     (1000) arvid     (1000)     1169 2022-07-30 12:05:25.948491 scan_merge-1.0.2/PKG-INFO
--rw-r--r--   0 arvid     (1000) arvid     (1000)      475 2022-07-30 11:43:38.000000 scan_merge-1.0.2/README.md
--rw-r--r--   0 arvid     (1000) arvid     (1000)      954 2022-07-30 12:00:15.000000 scan_merge-1.0.2/pyproject.toml
--rw-r--r--   0 arvid     (1000) arvid     (1000)       38 2022-07-30 12:05:25.948491 scan_merge-1.0.2/setup.cfg
--rw-r--r--   0 arvid     (1000) arvid     (1000)       94 2022-07-30 11:55:09.000000 scan_merge-1.0.2/setup.py
-drwxr-xr-x   0 arvid     (1000) arvid     (1000)        0 2022-07-30 12:05:25.948491 scan_merge-1.0.2/src/
-drwxr-xr-x   0 arvid     (1000) arvid     (1000)        0 2022-07-30 12:05:25.948491 scan_merge-1.0.2/src/scan_merge.egg-info/
--rw-r--r--   0 arvid     (1000) arvid     (1000)     1169 2022-07-30 12:05:25.000000 scan_merge-1.0.2/src/scan_merge.egg-info/PKG-INFO
--rw-r--r--   0 arvid     (1000) arvid     (1000)      303 2022-07-30 12:05:25.000000 scan_merge-1.0.2/src/scan_merge.egg-info/SOURCES.txt
--rw-r--r--   0 arvid     (1000) arvid     (1000)        1 2022-07-30 12:05:25.000000 scan_merge-1.0.2/src/scan_merge.egg-info/dependency_links.txt
--rw-r--r--   0 arvid     (1000) arvid     (1000)       47 2022-07-30 12:05:25.000000 scan_merge-1.0.2/src/scan_merge.egg-info/entry_points.txt
--rw-r--r--   0 arvid     (1000) arvid     (1000)       25 2022-07-30 12:05:25.000000 scan_merge-1.0.2/src/scan_merge.egg-info/requires.txt
--rw-r--r--   0 arvid     (1000) arvid     (1000)       11 2022-07-30 12:05:25.000000 scan_merge-1.0.2/src/scan_merge.egg-info/top_level.txt
--rw-r--r--   0 arvid     (1000) arvid     (1000)     1937 2022-07-30 12:04:09.000000 scan_merge-1.0.2/src/scan_merge.py
+drwxr-xr-x   0 arvid     (1000) arvid     (1000)        0 2024-04-17 21:00:26.389460 scan_merge-1.1/
+-rw-r--r--   0 arvid     (1000) arvid     (1000)       71 2022-07-30 14:36:25.000000 scan_merge-1.1/.gitignore
+-rw-r--r--   0 arvid     (1000) arvid     (1000)    34916 2022-07-30 11:43:38.000000 scan_merge-1.1/COPYING.md
+-rw-r--r--   0 arvid     (1000) arvid     (1000)     1267 2024-04-17 21:00:26.388460 scan_merge-1.1/PKG-INFO
+-rw-r--r--   0 arvid     (1000) arvid     (1000)      475 2022-07-30 11:43:38.000000 scan_merge-1.1/README.md
+-rw-r--r--   0 arvid     (1000) arvid     (1000)      961 2024-04-17 20:57:26.000000 scan_merge-1.1/pyproject.toml
+-rw-r--r--   0 arvid     (1000) arvid     (1000)       38 2024-04-17 21:00:26.389460 scan_merge-1.1/setup.cfg
+-rw-r--r--   0 arvid     (1000) arvid     (1000)       94 2022-07-30 11:55:09.000000 scan_merge-1.1/setup.py
+drwxr-xr-x   0 arvid     (1000) arvid     (1000)        0 2024-04-17 21:00:26.386460 scan_merge-1.1/src/
+drwxr-xr-x   0 arvid     (1000) arvid     (1000)        0 2024-04-17 21:00:26.388460 scan_merge-1.1/src/scan_merge.egg-info/
+-rw-r--r--   0 arvid     (1000) arvid     (1000)     1267 2024-04-17 21:00:26.000000 scan_merge-1.1/src/scan_merge.egg-info/PKG-INFO
+-rw-r--r--   0 arvid     (1000) arvid     (1000)      303 2024-04-17 21:00:26.000000 scan_merge-1.1/src/scan_merge.egg-info/SOURCES.txt
+-rw-r--r--   0 arvid     (1000) arvid     (1000)        1 2024-04-17 21:00:26.000000 scan_merge-1.1/src/scan_merge.egg-info/dependency_links.txt
+-rw-r--r--   0 arvid     (1000) arvid     (1000)       47 2024-04-17 21:00:26.000000 scan_merge-1.1/src/scan_merge.egg-info/entry_points.txt
+-rw-r--r--   0 arvid     (1000) arvid     (1000)       30 2024-04-17 21:00:26.000000 scan_merge-1.1/src/scan_merge.egg-info/requires.txt
+-rw-r--r--   0 arvid     (1000) arvid     (1000)       11 2024-04-17 21:00:26.000000 scan_merge-1.1/src/scan_merge.egg-info/top_level.txt
+-rw-r--r--   0 arvid     (1000) arvid     (1000)     1918 2024-04-17 20:56:18.000000 scan_merge-1.1/src/scan_merge.py
```

### Comparing `scan_merge-1.0.2/COPYING.md` & `scan_merge-1.1/COPYING.md`

 * *Files identical despite different names*

### Comparing `scan_merge-1.0.2/PKG-INFO` & `scan_merge-1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: scan_merge
-Version: 1.0.2
+Version: 1.1
 Summary: Tool to merge scanned PDFs from single sided document feeders
 Author-email: Arvid Norlander <VorpalBlade@users.noreply.github.com>
 License: GPL-3.0
 Project-URL: Source, https://github.com/VorpalBlade/scan_merge
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Scanners
 Description-Content-Type: text/markdown
+License-File: COPYING.md
+Requires-Dist: argcomplete
+Requires-Dist: funcy
+Requires-Dist: pypdf2>=3.0
 
 # scan_merge
 
 This is a simple tool to merge scanned PDFs if you have scanner with a document
 feeder but that doesn't support double sided pages.
 
 The idea is to scan the document stack into two PDFs, a forward one of the front
```

### Comparing `scan_merge-1.0.2/pyproject.toml` & `scan_merge-1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Topic :: Multimedia :: Graphics :: Capture :: Scanners",
 ]
 dependencies = [
     "argcomplete",
     "funcy",
-    "pypdf2"
+    "pypdf2 >= 3.0"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Source = "https://github.com/VorpalBlade/scan_merge"
 
 [project.scripts]
```

### Comparing `scan_merge-1.0.2/src/scan_merge.egg-info/PKG-INFO` & `scan_merge-1.1/src/scan_merge.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
-Name: scan-merge
-Version: 1.0.2
+Name: scan_merge
+Version: 1.1
 Summary: Tool to merge scanned PDFs from single sided document feeders
 Author-email: Arvid Norlander <VorpalBlade@users.noreply.github.com>
 License: GPL-3.0
 Project-URL: Source, https://github.com/VorpalBlade/scan_merge
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Scanners
 Description-Content-Type: text/markdown
+License-File: COPYING.md
+Requires-Dist: argcomplete
+Requires-Dist: funcy
+Requires-Dist: pypdf2>=3.0
 
 # scan_merge
 
 This is a simple tool to merge scanned PDFs if you have scanner with a document
 feeder but that doesn't support double sided pages.
 
 The idea is to scan the document stack into two PDFs, a forward one of the front
```

### Comparing `scan_merge-1.0.2/src/scan_merge.py` & `scan_merge-1.1/src/scan_merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import argparse
 from itertools import zip_longest
 from pathlib import Path
 
 import argcomplete
-from PyPDF2 import PdfFileWriter, PdfFileReader
+from PyPDF2 import PdfWriter, PdfReader
 from funcy import cat
 
 
 def interleave_longest(*sequences):
     """Interleave sequences, substituting with None if a sequence ends early"""
     return cat(zip_longest(*sequences))
 
@@ -34,26 +34,26 @@
     ).completer = pdf_completer
     parser.add_argument(
         "output_file", type=Path, help="Path of combined output file"
     ).completer = pdf_completer
     argcomplete.autocomplete(parser)
     args = parser.parse_args()
 
-    output = PdfFileWriter()
+    output = PdfWriter()
     # Load the PDFs
     with args.front_file.open(mode="rb") as front_file, args.back_file.open(
         mode="rb"
     ) as back_file:
-        input_front = PdfFileReader(front_file)
-        input_back = PdfFileReader(back_file)
+        input_front = PdfReader(front_file)
+        input_back = PdfReader(back_file)
         # Generate combined sequence of pages from both PDFs
         combined = filter(
             bool, interleave_longest(input_front.pages, reversed(input_back.pages))
         )
         for page in combined:
-            output.addPage(page)
+            output.add_page(page)
         with args.output_file.open(mode="wb") as output_file:
             output.write(output_file)
 
 
 if __name__ == "__main__":
     main()
```

