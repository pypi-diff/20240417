# Comparing `tmp/document_ingestor-0.1.0.tar.gz` & `tmp/document_ingestor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_ingestor-0.1.0.tar", last modified: Sun Apr 14 15:51:25 2024, max compression
+gzip compressed data, was "document_ingestor-0.1.1.tar", last modified: Wed Apr 17 19:10:35 2024, max compression
```

## Comparing `document_ingestor-0.1.0.tar` & `document_ingestor-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 15:51:25.485863 document_ingestor-0.1.0/
--rw-rw-rw-   0        0        0     1091 2024-03-24 16:55:37.000000 document_ingestor-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2387 2024-04-14 15:51:25.481865 document_ingestor-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-03-24 16:55:37.000000 document_ingestor-0.1.0/README.md
--rw-rw-rw-   0        0        0      869 2024-04-14 15:50:58.000000 document_ingestor-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 15:51:25.487917 document_ingestor-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-14 15:51:25.314776 document_ingestor-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-14 15:51:25.398017 document_ingestor-0.1.0/src/document_ingestor/
--rw-rw-rw-   0        0        0        0 2024-03-24 16:55:37.000000 document_ingestor-0.1.0/src/document_ingestor/__init__.py
--rw-rw-rw-   0        0        0     5779 2024-04-09 20:53:03.000000 document_ingestor-0.1.0/src/document_ingestor/embedding_process.py
--rw-rw-rw-   0        0        0     1865 2024-04-14 15:41:27.000000 document_ingestor-0.1.0/src/document_ingestor/eu_data_parser.py
--rw-rw-rw-   0        0        0     2744 2024-04-14 15:49:18.000000 document_ingestor-0.1.0/src/document_ingestor/genericParser.py
--rw-rw-rw-   0        0        0     6095 2024-04-09 20:45:08.000000 document_ingestor-0.1.0/src/document_ingestor/pdf_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:51:25.477334 document_ingestor-0.1.0/src/document_ingestor.egg-info/
--rw-rw-rw-   0        0        0     2387 2024-04-14 15:51:25.000000 document_ingestor-0.1.0/src/document_ingestor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2024-04-14 15:51:25.000000 document_ingestor-0.1.0/src/document_ingestor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 15:51:25.000000 document_ingestor-0.1.0/src/document_ingestor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-14 15:51:25.000000 document_ingestor-0.1.0/src/document_ingestor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-14 15:51:25.000000 document_ingestor-0.1.0/src/document_ingestor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 19:10:35.592475 document_ingestor-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2024-03-24 16:55:37.000000 document_ingestor-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2387 2024-04-17 19:10:35.585219 document_ingestor-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-03-24 16:55:37.000000 document_ingestor-0.1.1/README.md
+-rw-rw-rw-   0        0        0      869 2024-04-17 19:10:26.000000 document_ingestor-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 19:10:35.593008 document_ingestor-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 19:10:35.440879 document_ingestor-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 19:10:35.485819 document_ingestor-0.1.1/src/document_ingestor/
+-rw-rw-rw-   0        0        0        0 2024-03-24 16:55:37.000000 document_ingestor-0.1.1/src/document_ingestor/__init__.py
+-rw-rw-rw-   0        0        0     5779 2024-04-09 20:53:03.000000 document_ingestor-0.1.1/src/document_ingestor/embedding_process.py
+-rw-rw-rw-   0        0        0     1865 2024-04-17 14:06:55.000000 document_ingestor-0.1.1/src/document_ingestor/eu_data_parser.py
+-rw-rw-rw-   0        0        0     2744 2024-04-14 15:49:18.000000 document_ingestor-0.1.1/src/document_ingestor/genericParser.py
+-rw-rw-rw-   0        0        0     6146 2024-04-17 18:19:34.000000 document_ingestor-0.1.1/src/document_ingestor/pdf_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-17 19:10:35.580376 document_ingestor-0.1.1/src/document_ingestor.egg-info/
+-rw-rw-rw-   0        0        0     2387 2024-04-17 19:10:35.000000 document_ingestor-0.1.1/src/document_ingestor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-04-17 19:10:35.000000 document_ingestor-0.1.1/src/document_ingestor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 19:10:35.000000 document_ingestor-0.1.1/src/document_ingestor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-17 19:10:35.000000 document_ingestor-0.1.1/src/document_ingestor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-17 19:10:35.000000 document_ingestor-0.1.1/src/document_ingestor.egg-info/top_level.txt
```

### Comparing `document_ingestor-0.1.0/LICENSE.txt` & `document_ingestor-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `document_ingestor-0.1.0/PKG-INFO` & `document_ingestor-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document_ingestor
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package consumes one or more Spanish constitution PDFs and then processes them to generate embedding vectors. The vectors are generated with OpenAI service and PineCone is used to store and retrieve embedding vectors.
 Author-email: Milan Anand Raj <manandraj20@iitk.ac.in>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `document_ingestor-0.1.0/pyproject.toml` & `document_ingestor-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "document_ingestor"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name = "Milan Anand Raj", email = "manandraj20@iitk.ac.in" },
 ]
 description = "This package consumes one or more Spanish constitution PDFs and then processes them to generate embedding vectors. The vectors are generated with OpenAI service and PineCone is used to store and retrieve embedding vectors."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `document_ingestor-0.1.0/src/document_ingestor/embedding_process.py` & `document_ingestor-0.1.1/src/document_ingestor/embedding_process.py`

 * *Files identical despite different names*

### Comparing `document_ingestor-0.1.0/src/document_ingestor/eu_data_parser.py` & `document_ingestor-0.1.1/src/document_ingestor/eu_data_parser.py`

 * *Files identical despite different names*

### Comparing `document_ingestor-0.1.0/src/document_ingestor/genericParser.py` & `document_ingestor-0.1.1/src/document_ingestor/genericParser.py`

 * *Files identical despite different names*

### Comparing `document_ingestor-0.1.0/src/document_ingestor/pdf_parser.py` & `document_ingestor-0.1.1/src/document_ingestor/pdf_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,16 @@
 
             modified_block = block.replace('\n', '')
             modified_block = modified_block.strip()
 
             # modified_block = block.strip()
             # block = block.replace('\n', '')
             block = block.strip()
-
+            if not block:
+                continue
             if modified_block.startswith(current_heading.upper()) or block.startswith(current_heading) or block.startswith(current_heading.upper()) or modified_block.startswith(current_heading) or modified_block.startswith(current_heading.translate(translation_table)) or current_heading.translate(translation_table).startswith(modified_block):
                 # print(start_text+":")
                 start_text = hyperlinks.pop()
                 # print(start_text+":"+block)
                 contents_list.append(temp_list)
 
                 # contents_list.append(temp_list)
```

### Comparing `document_ingestor-0.1.0/src/document_ingestor.egg-info/PKG-INFO` & `document_ingestor-0.1.1/src/document_ingestor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document_ingestor
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package consumes one or more Spanish constitution PDFs and then processes them to generate embedding vectors. The vectors are generated with OpenAI service and PineCone is used to store and retrieve embedding vectors.
 Author-email: Milan Anand Raj <manandraj20@iitk.ac.in>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

