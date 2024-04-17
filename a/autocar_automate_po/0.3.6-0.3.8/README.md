# Comparing `tmp/autocar_automate_po-0.3.6.tar.gz` & `tmp/autocar_automate_po-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocar_automate_po-0.3.6.tar", last modified: Mon Dec 12 02:01:47 2022, max compression
+gzip compressed data, was "autocar_automate_po-0.3.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `autocar_automate_po-0.3.6.tar` & `autocar_automate_po-0.3.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1920 2022-12-12 01:10:12.059029 autocar_automate_po-0.3.6/.gitignore
--rw-r--r--   0        0        0     1068 2022-12-12 01:10:12.059029 autocar_automate_po-0.3.6/LICENSE
--rw-r--r--   0        0        0       21 2022-12-12 01:10:12.059029 autocar_automate_po-0.3.6/README.md
--rw-r--r--   0        0        0       51 2022-12-12 02:00:29.509761 autocar_automate_po-0.3.6/autocar_automate_po/__init__.py
--rw-r--r--   0        0        0    27883 2022-12-12 01:10:12.059029 autocar_automate_po-0.3.6/autocar_automate_po/automate_po_process.py
--rw-r--r--   0        0        0     2256 2022-12-12 01:59:49.142196 autocar_automate_po-0.3.6/autocar_automate_po/print_po.py
--rw-r--r--   0        0        0      436 2022-12-12 01:10:12.059029 autocar_automate_po-0.3.6/pyproject.toml
--rw-r--r--   0        0        0       78 2022-12-12 01:10:12.059029 autocar_automate_po-0.3.6/requirements.txt
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 autocar_automate_po-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1920 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/.gitignore
+-rw-r--r--   0        0        0     1068 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/LICENSE
+-rw-r--r--   0        0        0       21 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/README.md
+-rw-r--r--   0        0        0       51 2024-04-17 16:34:25.891431 autocar_automate_po-0.3.8/autocar_automate_po/__init__.py
+-rw-r--r--   0        0        0    27865 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/autocar_automate_po/automate_po_process.py
+-rw-r--r--   0        0        0     2262 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/autocar_automate_po/print_po.py
+-rw-r--r--   0        0        0      436 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/requirements.txt
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 autocar_automate_po-0.3.8/PKG-INFO
```

### Comparing `autocar_automate_po-0.3.6/.gitignore` & `autocar_automate_po-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `autocar_automate_po-0.3.6/LICENSE` & `autocar_automate_po-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autocar_automate_po-0.3.6/autocar_automate_po/automate_po_process.py` & `autocar_automate_po-0.3.8/autocar_automate_po/automate_po_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,17 +101,15 @@
         excel_2003_files.append(path.stem)
     # Loop po files
     counter = 1
     for path in Path('Files_To_Process').glob('*.xlsx'):
         print_progress_bar(counter, files_to_process)
         try:
             _ = pyxl.load_workbook(filename=path)
-            df = df.append(
-                load_file_data(path=path, po_identifier=time_identifier + '-' + str(i_identifier), file_name=path.stem)
-            )
+            df = pd.concat([df, load_file_data(path=path, po_identifier=time_identifier + '-' + str(i_identifier), file_name=path.stem)])
         except PermissionError:
             files_not_opened.append(path.stem)
         counter += 1
         i_identifier += 1
     # Check if df is empty
     if df.empty:
         print('Error: No files loaded')
@@ -565,15 +563,15 @@
             'Cost_Center': '',
             'Line_Comments': line_comments,
             'Ship_To': ship_to_nr,
             'Header_Comments': 'Please reference this Purchase Order on the Invoice. Email the Invoice to ap@autocartruck.com',
             'Supplier_Number': supplier_nr,
             'Supplier_Name': supplier_name
         }
-        df = df.append(data_to_df, ignore_index=True)
+        df = pd.concat([df, data_to_df], ignore_index=True)
     return df
 
 
 def populate_export(check_filename, time_identifier):
     def df_check_read_excel():
         df_check = pd.read_excel(check_filename, converters={
             'Supplier_Number': str,
```

### Comparing `autocar_automate_po-0.3.6/autocar_automate_po/print_po.py` & `autocar_automate_po-0.3.8/autocar_automate_po/print_po.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from datetime import datetime
 import os
 from time import sleep
-from shutil import move
+from shutil import copy, move
 
 try:
     import openpyxl as pyxl
     from openpyxl.styles import Alignment
 except ImportError:
     print('Please install the following dependencies:')
     print('openpyxl')
@@ -41,15 +41,15 @@
             i_identifier += 1
         except Exception:
             files_not_opened.append(path.stem)
 
     print('Moving files to P drive...')
     for path in files_to_move:
         try:
-            move(Path('export') / path, Path(NETWORK_SAVE) / path)
+            copy(Path('export') / path, Path(NETWORK_SAVE) / path)
         except Exception:
             files_not_moved.append(path)
 
     for path in Path('Files_To_Process').glob('*.xlsx'):
         try:
             move(path, Path('complete') / path.name)
         except Exception:
```

