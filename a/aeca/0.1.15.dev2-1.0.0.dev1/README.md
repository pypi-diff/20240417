# Comparing `tmp/aeca-0.1.15.dev2.tar.gz` & `tmp/aeca-1.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeca-0.1.15.dev2.tar", last modified: Sat Mar 16 07:53:52 2024, max compression
+gzip compressed data, was "aeca-1.0.0.dev1.tar", last modified: Wed Apr 17 07:20:28 2024, max compression
```

## Comparing `aeca-0.1.15.dev2.tar` & `aeca-1.0.0.dev1.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 cozyhous   (501) staff       (20)        0 2024-03-16 07:53:52.403853 aeca-0.1.15.dev2/
--rw-r--r--   0 cozyhous   (501) staff       (20)    11357 2024-01-18 12:05:45.000000 aeca-0.1.15.dev2/LICENSE
--rw-r--r--   0 cozyhous   (501) staff       (20)    15857 2024-03-16 07:53:52.403591 aeca-0.1.15.dev2/PKG-INFO
--rw-r--r--   0 cozyhous   (501) staff       (20)     1498 2024-03-16 07:53:24.000000 aeca-0.1.15.dev2/README.md
--rw-r--r--   0 cozyhous   (501) staff       (20)     1432 2024-03-16 07:53:45.000000 aeca-0.1.15.dev2/pyproject.toml
--rw-r--r--   0 cozyhous   (501) staff       (20)       38 2024-03-16 07:53:52.403895 aeca-0.1.15.dev2/setup.cfg
-drwxr-xr-x   0 cozyhous   (501) staff       (20)        0 2024-03-16 07:53:52.399498 aeca-0.1.15.dev2/src/
-drwxr-xr-x   0 cozyhous   (501) staff       (20)        0 2024-03-16 07:53:52.400751 aeca-0.1.15.dev2/src/aeca/
--rw-r--r--   0 cozyhous   (501) staff       (20)      725 2024-03-16 06:40:06.000000 aeca-0.1.15.dev2/src/aeca/__init__.py
--rw-r--r--   0 cozyhous   (501) staff       (20)     1902 2024-03-16 06:40:06.000000 aeca-0.1.15.dev2/src/aeca/channel.py
--rw-r--r--   0 cozyhous   (501) staff       (20)    28226 2024-03-16 06:40:06.000000 aeca-0.1.15.dev2/src/aeca/document_db.py
--rw-r--r--   0 cozyhous   (501) staff       (20)     2967 2024-03-16 06:40:06.000000 aeca-0.1.15.dev2/src/aeca/fts_analysis_pipeline.py
--rw-r--r--   0 cozyhous   (501) staff       (20)    11147 2024-03-16 06:40:06.000000 aeca-0.1.15.dev2/src/aeca/key_value_db.py
-drwxr-xr-x   0 cozyhous   (501) staff       (20)        0 2024-03-16 07:53:52.403033 aeca-0.1.15.dev2/src/aeca/protobuf/
--rw-r--r--   0 cozyhous   (501) staff       (20)       45 2024-03-16 06:40:06.000000 aeca-0.1.15.dev2/src/aeca/protobuf/__init__.py
--rw-r--r--   0 cozyhous   (501) staff       (20)    18398 2024-03-16 07:48:33.000000 aeca-0.1.15.dev2/src/aeca/protobuf/document_db_pb2.py
--rw-r--r--   0 cozyhous   (501) staff       (20)    31425 2024-03-16 07:48:26.000000 aeca-0.1.15.dev2/src/aeca/protobuf/document_db_pb2_grpc.py
--rw-r--r--   0 cozyhous   (501) staff       (20)     2513 2024-03-16 07:48:09.000000 aeca-0.1.15.dev2/src/aeca/protobuf/document_pb2.py
--rw-r--r--   0 cozyhous   (501) staff       (20)     2889 2024-03-16 07:48:09.000000 aeca-0.1.15.dev2/src/aeca/protobuf/fts_analysis_pipeline_pb2.py
--rw-r--r--   0 cozyhous   (501) staff       (20)     4505 2024-03-16 07:48:39.000000 aeca-0.1.15.dev2/src/aeca/protobuf/fts_analysis_pipeline_pb2_grpc.py
--rw-r--r--   0 cozyhous   (501) staff       (20)     8061 2024-03-16 07:48:09.000000 aeca-0.1.15.dev2/src/aeca/protobuf/key_value_db_pb2.py
--rw-r--r--   0 cozyhous   (501) staff       (20)    19307 2024-03-16 07:48:45.000000 aeca-0.1.15.dev2/src/aeca/protobuf/key_value_db_pb2_grpc.py
--rw-r--r--   0 cozyhous   (501) staff       (20)     6617 2024-03-16 07:48:09.000000 aeca-0.1.15.dev2/src/aeca/protobuf/sentence_transformer_pb2.py
--rw-r--r--   0 cozyhous   (501) staff       (20)    10068 2024-03-16 07:48:53.000000 aeca-0.1.15.dev2/src/aeca/protobuf/sentence_transformer_pb2_grpc.py
--rw-r--r--   0 cozyhous   (501) staff       (20)     9396 2024-03-16 06:40:06.000000 aeca-0.1.15.dev2/src/aeca/sentence_transformer.py
-drwxr-xr-x   0 cozyhous   (501) staff       (20)        0 2024-03-16 07:53:52.403265 aeca-0.1.15.dev2/src/aeca.egg-info/
--rw-r--r--   0 cozyhous   (501) staff       (20)    15857 2024-03-16 07:53:52.000000 aeca-0.1.15.dev2/src/aeca.egg-info/PKG-INFO
--rw-r--r--   0 cozyhous   (501) staff       (20)      768 2024-03-16 07:53:52.000000 aeca-0.1.15.dev2/src/aeca.egg-info/SOURCES.txt
--rw-r--r--   0 cozyhous   (501) staff       (20)        1 2024-03-16 07:53:52.000000 aeca-0.1.15.dev2/src/aeca.egg-info/dependency_links.txt
--rw-r--r--   0 cozyhous   (501) staff       (20)      137 2024-03-16 07:53:52.000000 aeca-0.1.15.dev2/src/aeca.egg-info/requires.txt
--rw-r--r--   0 cozyhous   (501) staff       (20)        5 2024-03-16 07:53:52.000000 aeca-0.1.15.dev2/src/aeca.egg-info/top_level.txt
+drwxr-xr-x   0 cozyhous   (501) staff       (20)        0 2024-04-17 07:20:28.783783 aeca-1.0.0.dev1/
+-rw-r--r--   0 cozyhous   (501) staff       (20)    11357 2024-01-18 12:05:45.000000 aeca-1.0.0.dev1/LICENSE
+-rw-r--r--   0 cozyhous   (501) staff       (20)    15784 2024-04-17 07:20:28.783524 aeca-1.0.0.dev1/PKG-INFO
+-rw-r--r--   0 cozyhous   (501) staff       (20)     1498 2024-03-16 07:53:24.000000 aeca-1.0.0.dev1/README.md
+-rw-r--r--   0 cozyhous   (501) staff       (20)     1399 2024-04-17 07:02:27.000000 aeca-1.0.0.dev1/pyproject.toml
+-rw-r--r--   0 cozyhous   (501) staff       (20)       38 2024-04-17 07:20:28.783832 aeca-1.0.0.dev1/setup.cfg
+drwxr-xr-x   0 cozyhous   (501) staff       (20)        0 2024-04-17 07:20:28.777076 aeca-1.0.0.dev1/src/
+drwxr-xr-x   0 cozyhous   (501) staff       (20)        0 2024-04-17 07:20:28.779178 aeca-1.0.0.dev1/src/aeca/
+-rw-r--r--   0 cozyhous   (501) staff       (20)      725 2024-03-16 06:40:06.000000 aeca-1.0.0.dev1/src/aeca/__init__.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)     1902 2024-03-16 06:40:06.000000 aeca-1.0.0.dev1/src/aeca/channel.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)    28226 2024-03-16 06:40:06.000000 aeca-1.0.0.dev1/src/aeca/document_db.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)     2967 2024-03-16 06:40:06.000000 aeca-1.0.0.dev1/src/aeca/fts_analysis_pipeline.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)    11147 2024-03-16 06:40:06.000000 aeca-1.0.0.dev1/src/aeca/key_value_db.py
+drwxr-xr-x   0 cozyhous   (501) staff       (20)        0 2024-04-17 07:20:28.782821 aeca-1.0.0.dev1/src/aeca/protobuf/
+-rw-r--r--   0 cozyhous   (501) staff       (20)       45 2024-03-16 06:40:06.000000 aeca-1.0.0.dev1/src/aeca/protobuf/__init__.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)    18139 2024-04-17 07:12:56.000000 aeca-1.0.0.dev1/src/aeca/protobuf/document_db_pb2.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)    31308 2024-04-17 07:16:23.000000 aeca-1.0.0.dev1/src/aeca/protobuf/document_db_pb2_grpc.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)     2496 2024-04-17 06:59:46.000000 aeca-1.0.0.dev1/src/aeca/protobuf/document_pb2.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)     2868 2024-04-17 06:59:47.000000 aeca-1.0.0.dev1/src/aeca/protobuf/fts_analysis_pipeline_pb2.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)     4490 2024-04-17 07:17:09.000000 aeca-1.0.0.dev1/src/aeca/protobuf/fts_analysis_pipeline_pb2_grpc.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)     7958 2024-04-17 06:59:47.000000 aeca-1.0.0.dev1/src/aeca/protobuf/key_value_db_pb2.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)    19235 2024-04-17 07:14:50.000000 aeca-1.0.0.dev1/src/aeca/protobuf/key_value_db_pb2_grpc.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)     6558 2024-04-17 06:59:47.000000 aeca-1.0.0.dev1/src/aeca/protobuf/sentence_transformer_pb2.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)    10032 2024-04-17 07:15:12.000000 aeca-1.0.0.dev1/src/aeca/protobuf/sentence_transformer_pb2_grpc.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)     3627 2024-04-17 06:59:47.000000 aeca-1.0.0.dev1/src/aeca/protobuf/workspaces_pb2.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)     5808 2024-04-17 07:15:24.000000 aeca-1.0.0.dev1/src/aeca/protobuf/workspaces_pb2_grpc.py
+-rw-r--r--   0 cozyhous   (501) staff       (20)     9396 2024-03-16 06:40:06.000000 aeca-1.0.0.dev1/src/aeca/sentence_transformer.py
+drwxr-xr-x   0 cozyhous   (501) staff       (20)        0 2024-04-17 07:20:28.783174 aeca-1.0.0.dev1/src/aeca.egg-info/
+-rw-r--r--   0 cozyhous   (501) staff       (20)    15784 2024-04-17 07:20:28.000000 aeca-1.0.0.dev1/src/aeca.egg-info/PKG-INFO
+-rw-r--r--   0 cozyhous   (501) staff       (20)      845 2024-04-17 07:20:28.000000 aeca-1.0.0.dev1/src/aeca.egg-info/SOURCES.txt
+-rw-r--r--   0 cozyhous   (501) staff       (20)        1 2024-04-17 07:20:28.000000 aeca-1.0.0.dev1/src/aeca.egg-info/dependency_links.txt
+-rw-r--r--   0 cozyhous   (501) staff       (20)      112 2024-04-17 07:20:28.000000 aeca-1.0.0.dev1/src/aeca.egg-info/requires.txt
+-rw-r--r--   0 cozyhous   (501) staff       (20)        5 2024-04-17 07:20:28.000000 aeca-1.0.0.dev1/src/aeca.egg-info/top_level.txt
```

### Comparing `aeca-0.1.15.dev2/LICENSE` & `aeca-1.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `aeca-0.1.15.dev2/PKG-INFO` & `aeca-1.0.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeca
-Version: 0.1.15.dev2
+Version: 1.0.0.dev1
 Summary: Python client for Aeca database
 Author-email: "Aeca, Inc." <jaepil@aeca.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -226,16 +226,14 @@
 Requires-Dist: polars>=0.16.18
 Requires-Dist: pyarrow>=11.0.0
 Requires-Dist: grpcio>=1.53.0
 Requires-Dist: protobuf>=4.22.1
 Requires-Dist: pillow
 Provides-Extra: protobuf
 Requires-Dist: grpcio>=1.43.0; extra == "protobuf"
-Provides-Extra: server
-Requires-Dist: cognica-server; extra == "server"
 
 # Aeca Python Client
 
 A Python client for Aeca database server.
 
 ## Installation
```

### Comparing `aeca-0.1.15.dev2/README.md` & `aeca-1.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `aeca-0.1.15.dev2/pyproject.toml` & `aeca-1.0.0.dev1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aeca"
-version = "0.1.15.dev2"
+version = "1.0.0.dev1"
 authors = [{ name = "Aeca, Inc.", email = "jaepil@aeca.ai" }]
 description = "Python client for Aeca database"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
   "pandas>=1.5.3",
@@ -48,12 +48,11 @@
   "Programming Language :: Python :: Implementation :: CPython",
 ]
 
 [project.urls]
 "Homepage" = "https://www.aeca.ai"
 
 [project.optional-dependencies]
-  protobuf = ["grpcio>=1.43.0"]
-  server = ["cognica-server"]
+protobuf = ["grpcio>=1.43.0"]
 
 [tool.black]
 line-length = 80
```

### Comparing `aeca-0.1.15.dev2/src/aeca/__init__.py` & `aeca-1.0.0.dev1/src/aeca/__init__.py`

 * *Files identical despite different names*

### Comparing `aeca-0.1.15.dev2/src/aeca/channel.py` & `aeca-1.0.0.dev1/src/aeca/channel.py`

 * *Files identical despite different names*

### Comparing `aeca-0.1.15.dev2/src/aeca/document_db.py` & `aeca-1.0.0.dev1/src/aeca/document_db.py`

 * *Files identical despite different names*

### Comparing `aeca-0.1.15.dev2/src/aeca/fts_analysis_pipeline.py` & `aeca-1.0.0.dev1/src/aeca/fts_analysis_pipeline.py`

 * *Files identical despite different names*

### Comparing `aeca-0.1.15.dev2/src/aeca/key_value_db.py` & `aeca-1.0.0.dev1/src/aeca/key_value_db.py`

 * *Files identical despite different names*

### Comparing `aeca-0.1.15.dev2/src/aeca/protobuf/document_db_pb2.py` & `aeca-1.0.0.dev1/src/aeca/protobuf/document_db_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,118 +11,118 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import aeca.protobuf.document_pb2 as document__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x64ocument_db.proto\x12\x17\x63ognica.rpc.db.document\x1a\x0e\x64ocument.proto\"\xf9\x01\n\x0fIndexDescriptor\x12\x10\n\x08index_id\x18\x01 \x01(\r\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x0e\n\x06\x66ields\x18\x03 \x03(\t\x12\x0e\n\x06unique\x18\x04 \x01(\x08\x12\x36\n\nindex_type\x18\x05 \x01(\x0e\x32\".cognica.rpc.db.document.IndexType\x12\x34\n\x06status\x18\x06 \x01(\x0e\x32$.cognica.rpc.db.document.IndexStatus\x12\x32\n\x07options\x18\x07 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\xa6\x01\n\rFTSFieldStats\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x17\n\x0ftotal_doc_count\x18\x02 \x01(\x03\x12\x16\n\x0etotal_doc_size\x18\x03 \x01(\x03\x12\x11\n\tdoc_count\x18\x04 \x01(\x03\x12\x10\n\x08\x64oc_size\x18\x05 \x01(\x03\x12\x15\n\rsum_term_freq\x18\x06 \x01(\x03\x12\x14\n\x0csum_doc_freq\x18\x07 \x01(\x03\"q\n\rFTSIndexStats\x12\x11\n\tdoc_count\x18\x01 \x01(\x03\x12\x10\n\x08\x64oc_size\x18\x02 \x01(\x03\x12;\n\x0b\x66ield_stats\x18\x03 \x03(\x0b\x32&.cognica.rpc.db.document.FTSFieldStats\"\xcf\x02\n\nIndexStats\x12\x10\n\x08index_id\x18\x01 \x01(\r\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x19\n\x11\x61pproximated_size\x18\x03 \x01(\x04\x12\x10\n\x08num_docs\x18\x04 \x01(\x04\x12\x10\n\x08\x61\x63\x63\x65ssed\x18\x05 \x01(\x04\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x06 \x01(\x04\x12\x0f\n\x07updated\x18\x07 \x01(\x04\x12\x0f\n\x07\x64\x65leted\x18\x08 \x01(\x04\x12\x0e\n\x06merged\x18\t \x01(\x04\x12\x13\n\x0b\x61\x63\x63\x65ssed_at\x18\n \x01(\x03\x12\x10\n\x08\x61\x64\x64\x65\x64_at\x18\x0b \x01(\x03\x12\x12\n\nupdated_at\x18\x0c \x01(\x03\x12\x12\n\ndeleted_at\x18\r \x01(\x03\x12\x11\n\tmerged_at\x18\x0e \x01(\x03\x12\x39\n\tfts_stats\x18\x0f \x01(\x0b\x32&.cognica.rpc.db.document.FTSIndexStats\"\xa8\x01\n\x0e\x43ollectionInfo\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x43\n\x11index_descriptors\x18\x02 \x03(\x0b\x32(.cognica.rpc.db.document.IndexDescriptor\x12\x38\n\x0bindex_stats\x18\x03 \x03(\x0b\x32#.cognica.rpc.db.document.IndexStats\"\x7f\n\x0bProfileInfo\x12\x0f\n\x07matched\x18\x01 \x01(\x04\x12\x0f\n\x07scanned\x18\x02 \x01(\x04\x12\x10\n\x08\x66iltered\x18\x03 \x01(\x04\x12\x19\n\x11query_duration_us\x18\x04 \x01(\x04\x12!\n\x19serialization_duration_us\x18\x05 \x01(\x04\"V\n\x17\x43reateCollectionRequest\x12;\n\ncollection\x18\x01 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\"r\n\x18\x43reateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"0\n\x15\x44ropCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"p\n\x16\x44ropCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"S\n\x17RenameCollectionRequest\x12\x1b\n\x13old_collection_name\x18\x01 \x01(\t\x12\x1b\n\x13new_collection_name\x18\x02 \x01(\t\"r\n\x18RenameCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"/\n\x14GetCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"\xac\x01\n\x15GetCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12;\n\ncollection\x18\x03 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"1\n\x15GetCollectionsRequest\x12\x18\n\x10\x63ollection_names\x18\x01 \x03(\t\"\xae\x01\n\x16GetCollectionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12<\n\x0b\x63ollections\x18\x03 \x03(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"k\n\x12\x43reateIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12<\n\nindex_desc\x18\x02 \x01(\x0b\x32(.cognica.rpc.db.document.IndexDescriptor\"m\n\x13\x43reateIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"?\n\x10\x44ropIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"k\n\x11\x44ropIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"]\n\x12RenameIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x16\n\x0eold_index_name\x18\x02 \x01(\t\x12\x16\n\x0enew_index_name\x18\x03 \x01(\t\"m\n\x13RenameIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\">\n\x0fGetIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"\xfb\x01\n\x10GetIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12<\n\nindex_desc\x18\x04 \x01(\x0b\x32(.cognica.rpc.db.document.IndexDescriptor\x12\x38\n\x0bindex_stats\x18\x05 \x01(\x0b\x32#.cognica.rpc.db.document.IndexStats\x12\x35\n\x07profile\x18\x06 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"R\n\x05Query\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x30\n\x05query\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\xe4\x01\n\x0b\x46indRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\x12\r\n\x05limit\x18\x02 \x01(\x05\x12\x15\n\rindex_columns\x18\x03 \x03(\t\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12@\n\x06\x64types\x18\x05 \x03(\x0b\x32\x30.cognica.rpc.db.document.FindRequest.DtypesEntry\x1a-\n\x0b\x44typesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"|\n\x0c\x46indResponse\x12\x13\n\x0bnum_columns\x18\x01 \x01(\x05\x12\x10\n\x08num_rows\x18\x02 \x01(\x05\x12\x0e\n\x06\x62uffer\x18\x03 \x01(\x0c\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"J\n\x10\x46indBatchRequest\x12\x36\n\x08requests\x18\x01 \x03(\x0b\x32$.cognica.rpc.db.document.FindRequest\"M\n\x11\x46indBatchResponse\x12\x38\n\tresponses\x18\x01 \x03(\x0b\x32%.cognica.rpc.db.document.FindResponse\"=\n\x0c\x43ountRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"v\n\rCountResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x03\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"@\n\x0f\x43ontainsRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"y\n\x10\x43ontainsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x66ound\x18\x03 \x01(\x08\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"A\n\rInsertRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"h\n\x0eInsertResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"\x8f\x01\n\rUpdateRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x31\n\x06\x66ilter\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\x12\x32\n\x07updates\x18\x03 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"h\n\x0eUpdateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"A\n\rRemoveRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"h\n\x0eRemoveResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"A\n\x0e\x45xplainRequest\x12/\n\x07queries\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"m\n\tQueryPlan\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nindex_name\x18\x04 \x01(\t\x12\x12\n\nquery_plan\x18\x05 \x01(\t\"Z\n\x0f\x45xplainResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x37\n\x0bquery_plans\x18\x02 \x03(\x0b\x32\".cognica.rpc.db.document.QueryPlan\"4\n\x19TruncateCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"t\n\x1aTruncateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"\x18\n\x16ListCollectionsRequest\"\x8b\x01\n\x17ListCollectionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x18\n\x10\x63ollection_names\x18\x03 \x03(\t\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo*e\n\tIndexType\x12\x0f\n\x0bkPrimaryKey\x10\x00\x12\x11\n\rkSecondaryKey\x10\x01\x12\x1a\n\x16kClusteredSecondaryKey\x10\x02\x12\x18\n\x14kFullTextSearchIndex\x10\x03*\x8d\x01\n\x0bIndexStatus\x12\x0c\n\x08kEnabled\x10\x00\x12\r\n\tkDisabled\x10\x01\x12\x0f\n\x0bkReadyToUse\x10\x02\x12\x14\n\x10kBuildInProgress\x10\x03\x12\x12\n\x0ekBuildFinished\x10\x04\x12\x13\n\x0fkDropInProgress\x10\x05\x12\x11\n\rkDropFinished\x10\x06\x32\xfd\x0f\n\x11\x44ocumentDBService\x12U\n\x04\x66ind\x12$.cognica.rpc.db.document.FindRequest\x1a%.cognica.rpc.db.document.FindResponse\"\x00\x12\x65\n\nfind_batch\x12).cognica.rpc.db.document.FindBatchRequest\x1a*.cognica.rpc.db.document.FindBatchResponse\"\x00\x12X\n\x05\x63ount\x12%.cognica.rpc.db.document.CountRequest\x1a&.cognica.rpc.db.document.CountResponse\"\x00\x12\x61\n\x08\x63ontains\x12(.cognica.rpc.db.document.ContainsRequest\x1a).cognica.rpc.db.document.ContainsResponse\"\x00\x12[\n\x06insert\x12&.cognica.rpc.db.document.InsertRequest\x1a\'.cognica.rpc.db.document.InsertResponse\"\x00\x12[\n\x06update\x12&.cognica.rpc.db.document.UpdateRequest\x1a\'.cognica.rpc.db.document.UpdateResponse\"\x00\x12[\n\x06remove\x12&.cognica.rpc.db.document.RemoveRequest\x1a\'.cognica.rpc.db.document.RemoveResponse\"\x00\x12^\n\x07\x65xplain\x12\'.cognica.rpc.db.document.ExplainRequest\x1a(.cognica.rpc.db.document.ExplainResponse\"\x00\x12z\n\x11\x63reate_collection\x12\x30.cognica.rpc.db.document.CreateCollectionRequest\x1a\x31.cognica.rpc.db.document.CreateCollectionResponse\"\x00\x12t\n\x0f\x64rop_collection\x12..cognica.rpc.db.document.DropCollectionRequest\x1a/.cognica.rpc.db.document.DropCollectionResponse\"\x00\x12z\n\x11rename_collection\x12\x30.cognica.rpc.db.document.RenameCollectionRequest\x1a\x31.cognica.rpc.db.document.RenameCollectionResponse\"\x00\x12q\n\x0eget_collection\x12-.cognica.rpc.db.document.GetCollectionRequest\x1a..cognica.rpc.db.document.GetCollectionResponse\"\x00\x12t\n\x0fget_collections\x12..cognica.rpc.db.document.GetCollectionsRequest\x1a/.cognica.rpc.db.document.GetCollectionsResponse\"\x00\x12w\n\x10list_collections\x12/.cognica.rpc.db.document.ListCollectionsRequest\x1a\x30.cognica.rpc.db.document.ListCollectionsResponse\"\x00\x12\x80\x01\n\x13truncate_collection\x12\x32.cognica.rpc.db.document.TruncateCollectionRequest\x1a\x33.cognica.rpc.db.document.TruncateCollectionResponse\"\x00\x12k\n\x0c\x63reate_index\x12+.cognica.rpc.db.document.CreateIndexRequest\x1a,.cognica.rpc.db.document.CreateIndexResponse\"\x00\x12\x65\n\ndrop_index\x12).cognica.rpc.db.document.DropIndexRequest\x1a*.cognica.rpc.db.document.DropIndexResponse\"\x00\x12k\n\x0crename_index\x12+.cognica.rpc.db.document.RenameIndexRequest\x1a,.cognica.rpc.db.document.RenameIndexResponse\"\x00\x12\x62\n\tget_index\x12(.cognica.rpc.db.document.GetIndexRequest\x1a).cognica.rpc.db.document.GetIndexResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x64ocument_db.proto\x12\x14\x61\x65\x63\x61.rpc.db.document\x1a\x0e\x64ocument.proto\"\xf0\x01\n\x0fIndexDescriptor\x12\x10\n\x08index_id\x18\x01 \x01(\r\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x0e\n\x06\x66ields\x18\x03 \x03(\t\x12\x0e\n\x06unique\x18\x04 \x01(\x08\x12\x33\n\nindex_type\x18\x05 \x01(\x0e\x32\x1f.aeca.rpc.db.document.IndexType\x12\x31\n\x06status\x18\x06 \x01(\x0e\x32!.aeca.rpc.db.document.IndexStatus\x12/\n\x07options\x18\x07 \x01(\x0b\x32\x1e.aeca.rpc.db.document.Document\"\xa6\x01\n\rFTSFieldStats\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x17\n\x0ftotal_doc_count\x18\x02 \x01(\x03\x12\x16\n\x0etotal_doc_size\x18\x03 \x01(\x03\x12\x11\n\tdoc_count\x18\x04 \x01(\x03\x12\x10\n\x08\x64oc_size\x18\x05 \x01(\x03\x12\x15\n\rsum_term_freq\x18\x06 \x01(\x03\x12\x14\n\x0csum_doc_freq\x18\x07 \x01(\x03\"n\n\rFTSIndexStats\x12\x11\n\tdoc_count\x18\x01 \x01(\x03\x12\x10\n\x08\x64oc_size\x18\x02 \x01(\x03\x12\x38\n\x0b\x66ield_stats\x18\x03 \x03(\x0b\x32#.aeca.rpc.db.document.FTSFieldStats\"\xcc\x02\n\nIndexStats\x12\x10\n\x08index_id\x18\x01 \x01(\r\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x19\n\x11\x61pproximated_size\x18\x03 \x01(\x04\x12\x10\n\x08num_docs\x18\x04 \x01(\x04\x12\x10\n\x08\x61\x63\x63\x65ssed\x18\x05 \x01(\x04\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x06 \x01(\x04\x12\x0f\n\x07updated\x18\x07 \x01(\x04\x12\x0f\n\x07\x64\x65leted\x18\x08 \x01(\x04\x12\x0e\n\x06merged\x18\t \x01(\x04\x12\x13\n\x0b\x61\x63\x63\x65ssed_at\x18\n \x01(\x03\x12\x10\n\x08\x61\x64\x64\x65\x64_at\x18\x0b \x01(\x03\x12\x12\n\nupdated_at\x18\x0c \x01(\x03\x12\x12\n\ndeleted_at\x18\r \x01(\x03\x12\x11\n\tmerged_at\x18\x0e \x01(\x03\x12\x36\n\tfts_stats\x18\x0f \x01(\x0b\x32#.aeca.rpc.db.document.FTSIndexStats\"\xa2\x01\n\x0e\x43ollectionInfo\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12@\n\x11index_descriptors\x18\x02 \x03(\x0b\x32%.aeca.rpc.db.document.IndexDescriptor\x12\x35\n\x0bindex_stats\x18\x03 \x03(\x0b\x32 .aeca.rpc.db.document.IndexStats\"\x7f\n\x0bProfileInfo\x12\x0f\n\x07matched\x18\x01 \x01(\x04\x12\x0f\n\x07scanned\x18\x02 \x01(\x04\x12\x10\n\x08\x66iltered\x18\x03 \x01(\x04\x12\x19\n\x11query_duration_us\x18\x04 \x01(\x04\x12!\n\x19serialization_duration_us\x18\x05 \x01(\x04\"S\n\x17\x43reateCollectionRequest\x12\x38\n\ncollection\x18\x01 \x01(\x0b\x32$.aeca.rpc.db.document.CollectionInfo\"o\n\x18\x43reateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x32\n\x07profile\x18\x03 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\"0\n\x15\x44ropCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"m\n\x16\x44ropCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x32\n\x07profile\x18\x03 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\"S\n\x17RenameCollectionRequest\x12\x1b\n\x13old_collection_name\x18\x01 \x01(\t\x12\x1b\n\x13new_collection_name\x18\x02 \x01(\t\"o\n\x18RenameCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x32\n\x07profile\x18\x03 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\"/\n\x14GetCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"\xa6\x01\n\x15GetCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x38\n\ncollection\x18\x03 \x01(\x0b\x32$.aeca.rpc.db.document.CollectionInfo\x12\x32\n\x07profile\x18\x04 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\"1\n\x15GetCollectionsRequest\x12\x18\n\x10\x63ollection_names\x18\x01 \x03(\t\"\xa8\x01\n\x16GetCollectionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x39\n\x0b\x63ollections\x18\x03 \x03(\x0b\x32$.aeca.rpc.db.document.CollectionInfo\x12\x32\n\x07profile\x18\x04 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\"h\n\x12\x43reateIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x39\n\nindex_desc\x18\x02 \x01(\x0b\x32%.aeca.rpc.db.document.IndexDescriptor\"j\n\x13\x43reateIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x32\n\x07profile\x18\x03 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\"?\n\x10\x44ropIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"h\n\x11\x44ropIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x32\n\x07profile\x18\x03 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\"]\n\x12RenameIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x16\n\x0eold_index_name\x18\x02 \x01(\t\x12\x16\n\x0enew_index_name\x18\x03 \x01(\t\"j\n\x13RenameIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x32\n\x07profile\x18\x03 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\">\n\x0fGetIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"\xf2\x01\n\x10GetIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x39\n\nindex_desc\x18\x04 \x01(\x0b\x32%.aeca.rpc.db.document.IndexDescriptor\x12\x35\n\x0bindex_stats\x18\x05 \x01(\x0b\x32 .aeca.rpc.db.document.IndexStats\x12\x32\n\x07profile\x18\x06 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\"O\n\x05Query\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12-\n\x05query\x18\x02 \x01(\x0b\x32\x1e.aeca.rpc.db.document.Document\"\xde\x01\n\x0b\x46indRequest\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.aeca.rpc.db.document.Query\x12\r\n\x05limit\x18\x02 \x01(\x05\x12\x15\n\rindex_columns\x18\x03 \x03(\t\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12=\n\x06\x64types\x18\x05 \x03(\x0b\x32-.aeca.rpc.db.document.FindRequest.DtypesEntry\x1a-\n\x0b\x44typesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"y\n\x0c\x46indResponse\x12\x13\n\x0bnum_columns\x18\x01 \x01(\x05\x12\x10\n\x08num_rows\x18\x02 \x01(\x05\x12\x0e\n\x06\x62uffer\x18\x03 \x01(\x0c\x12\x32\n\x07profile\x18\x04 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\"G\n\x10\x46indBatchRequest\x12\x33\n\x08requests\x18\x01 \x03(\x0b\x32!.aeca.rpc.db.document.FindRequest\"J\n\x11\x46indBatchResponse\x12\x35\n\tresponses\x18\x01 \x03(\x0b\x32\".aeca.rpc.db.document.FindResponse\":\n\x0c\x43ountRequest\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.aeca.rpc.db.document.Query\"s\n\rCountResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x03\x12\x32\n\x07profile\x18\x04 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\"=\n\x0f\x43ontainsRequest\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.aeca.rpc.db.document.Query\"v\n\x10\x43ontainsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x66ound\x18\x03 \x01(\x08\x12\x32\n\x07profile\x18\x04 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\">\n\rInsertRequest\x12-\n\x08requests\x18\x01 \x03(\x0b\x32\x1b.aeca.rpc.db.document.Query\"e\n\x0eInsertResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x32\n\x07profile\x18\x03 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\"\x89\x01\n\rUpdateRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12.\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x1e.aeca.rpc.db.document.Document\x12/\n\x07updates\x18\x03 \x01(\x0b\x32\x1e.aeca.rpc.db.document.Document\"e\n\x0eUpdateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x32\n\x07profile\x18\x03 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\">\n\rRemoveRequest\x12-\n\x08requests\x18\x01 \x03(\x0b\x32\x1b.aeca.rpc.db.document.Query\"e\n\x0eRemoveResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x32\n\x07profile\x18\x03 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\">\n\x0e\x45xplainRequest\x12,\n\x07queries\x18\x01 \x03(\x0b\x32\x1b.aeca.rpc.db.document.Query\"m\n\tQueryPlan\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nindex_name\x18\x04 \x01(\t\x12\x12\n\nquery_plan\x18\x05 \x01(\t\"W\n\x0f\x45xplainResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x34\n\x0bquery_plans\x18\x02 \x03(\x0b\x32\x1f.aeca.rpc.db.document.QueryPlan\"4\n\x19TruncateCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"q\n\x1aTruncateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x32\n\x07profile\x18\x03 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo\"\x18\n\x16ListCollectionsRequest\"\x88\x01\n\x17ListCollectionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x18\n\x10\x63ollection_names\x18\x03 \x03(\t\x12\x32\n\x07profile\x18\x04 \x01(\x0b\x32!.aeca.rpc.db.document.ProfileInfo*e\n\tIndexType\x12\x0f\n\x0bkPrimaryKey\x10\x00\x12\x11\n\rkSecondaryKey\x10\x01\x12\x1a\n\x16kClusteredSecondaryKey\x10\x02\x12\x18\n\x14kFullTextSearchIndex\x10\x03*\x8d\x01\n\x0bIndexStatus\x12\x0c\n\x08kEnabled\x10\x00\x12\r\n\tkDisabled\x10\x01\x12\x0f\n\x0bkReadyToUse\x10\x02\x12\x14\n\x10kBuildInProgress\x10\x03\x12\x12\n\x0ekBuildFinished\x10\x04\x12\x13\n\x0fkDropInProgress\x10\x05\x12\x11\n\rkDropFinished\x10\x06\x32\x8a\x0f\n\x11\x44ocumentDBService\x12O\n\x04\x66ind\x12!.aeca.rpc.db.document.FindRequest\x1a\".aeca.rpc.db.document.FindResponse\"\x00\x12_\n\nfind_batch\x12&.aeca.rpc.db.document.FindBatchRequest\x1a\'.aeca.rpc.db.document.FindBatchResponse\"\x00\x12R\n\x05\x63ount\x12\".aeca.rpc.db.document.CountRequest\x1a#.aeca.rpc.db.document.CountResponse\"\x00\x12[\n\x08\x63ontains\x12%.aeca.rpc.db.document.ContainsRequest\x1a&.aeca.rpc.db.document.ContainsResponse\"\x00\x12U\n\x06insert\x12#.aeca.rpc.db.document.InsertRequest\x1a$.aeca.rpc.db.document.InsertResponse\"\x00\x12U\n\x06update\x12#.aeca.rpc.db.document.UpdateRequest\x1a$.aeca.rpc.db.document.UpdateResponse\"\x00\x12U\n\x06remove\x12#.aeca.rpc.db.document.RemoveRequest\x1a$.aeca.rpc.db.document.RemoveResponse\"\x00\x12X\n\x07\x65xplain\x12$.aeca.rpc.db.document.ExplainRequest\x1a%.aeca.rpc.db.document.ExplainResponse\"\x00\x12t\n\x11\x63reate_collection\x12-.aeca.rpc.db.document.CreateCollectionRequest\x1a..aeca.rpc.db.document.CreateCollectionResponse\"\x00\x12n\n\x0f\x64rop_collection\x12+.aeca.rpc.db.document.DropCollectionRequest\x1a,.aeca.rpc.db.document.DropCollectionResponse\"\x00\x12t\n\x11rename_collection\x12-.aeca.rpc.db.document.RenameCollectionRequest\x1a..aeca.rpc.db.document.RenameCollectionResponse\"\x00\x12k\n\x0eget_collection\x12*.aeca.rpc.db.document.GetCollectionRequest\x1a+.aeca.rpc.db.document.GetCollectionResponse\"\x00\x12n\n\x0fget_collections\x12+.aeca.rpc.db.document.GetCollectionsRequest\x1a,.aeca.rpc.db.document.GetCollectionsResponse\"\x00\x12q\n\x10list_collections\x12,.aeca.rpc.db.document.ListCollectionsRequest\x1a-.aeca.rpc.db.document.ListCollectionsResponse\"\x00\x12z\n\x13truncate_collection\x12/.aeca.rpc.db.document.TruncateCollectionRequest\x1a\x30.aeca.rpc.db.document.TruncateCollectionResponse\"\x00\x12\x65\n\x0c\x63reate_index\x12(.aeca.rpc.db.document.CreateIndexRequest\x1a).aeca.rpc.db.document.CreateIndexResponse\"\x00\x12_\n\ndrop_index\x12&.aeca.rpc.db.document.DropIndexRequest\x1a\'.aeca.rpc.db.document.DropIndexResponse\"\x00\x12\x65\n\x0crename_index\x12(.aeca.rpc.db.document.RenameIndexRequest\x1a).aeca.rpc.db.document.RenameIndexResponse\"\x00\x12\\\n\tget_index\x12%.aeca.rpc.db.document.GetIndexRequest\x1a&.aeca.rpc.db.document.GetIndexResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'document_db_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\370\001\001'
   _globals['_FINDREQUEST_DTYPESENTRY']._options = None
   _globals['_FINDREQUEST_DTYPESENTRY']._serialized_options = b'8\001'
-  _globals['_INDEXTYPE']._serialized_start=5351
-  _globals['_INDEXTYPE']._serialized_end=5452
-  _globals['_INDEXSTATUS']._serialized_start=5455
-  _globals['_INDEXSTATUS']._serialized_end=5596
-  _globals['_INDEXDESCRIPTOR']._serialized_start=63
-  _globals['_INDEXDESCRIPTOR']._serialized_end=312
-  _globals['_FTSFIELDSTATS']._serialized_start=315
-  _globals['_FTSFIELDSTATS']._serialized_end=481
-  _globals['_FTSINDEXSTATS']._serialized_start=483
-  _globals['_FTSINDEXSTATS']._serialized_end=596
-  _globals['_INDEXSTATS']._serialized_start=599
-  _globals['_INDEXSTATS']._serialized_end=934
-  _globals['_COLLECTIONINFO']._serialized_start=937
-  _globals['_COLLECTIONINFO']._serialized_end=1105
-  _globals['_PROFILEINFO']._serialized_start=1107
-  _globals['_PROFILEINFO']._serialized_end=1234
-  _globals['_CREATECOLLECTIONREQUEST']._serialized_start=1236
-  _globals['_CREATECOLLECTIONREQUEST']._serialized_end=1322
-  _globals['_CREATECOLLECTIONRESPONSE']._serialized_start=1324
-  _globals['_CREATECOLLECTIONRESPONSE']._serialized_end=1438
-  _globals['_DROPCOLLECTIONREQUEST']._serialized_start=1440
-  _globals['_DROPCOLLECTIONREQUEST']._serialized_end=1488
-  _globals['_DROPCOLLECTIONRESPONSE']._serialized_start=1490
-  _globals['_DROPCOLLECTIONRESPONSE']._serialized_end=1602
-  _globals['_RENAMECOLLECTIONREQUEST']._serialized_start=1604
-  _globals['_RENAMECOLLECTIONREQUEST']._serialized_end=1687
-  _globals['_RENAMECOLLECTIONRESPONSE']._serialized_start=1689
-  _globals['_RENAMECOLLECTIONRESPONSE']._serialized_end=1803
-  _globals['_GETCOLLECTIONREQUEST']._serialized_start=1805
-  _globals['_GETCOLLECTIONREQUEST']._serialized_end=1852
-  _globals['_GETCOLLECTIONRESPONSE']._serialized_start=1855
-  _globals['_GETCOLLECTIONRESPONSE']._serialized_end=2027
-  _globals['_GETCOLLECTIONSREQUEST']._serialized_start=2029
-  _globals['_GETCOLLECTIONSREQUEST']._serialized_end=2078
-  _globals['_GETCOLLECTIONSRESPONSE']._serialized_start=2081
-  _globals['_GETCOLLECTIONSRESPONSE']._serialized_end=2255
-  _globals['_CREATEINDEXREQUEST']._serialized_start=2257
-  _globals['_CREATEINDEXREQUEST']._serialized_end=2364
-  _globals['_CREATEINDEXRESPONSE']._serialized_start=2366
-  _globals['_CREATEINDEXRESPONSE']._serialized_end=2475
-  _globals['_DROPINDEXREQUEST']._serialized_start=2477
-  _globals['_DROPINDEXREQUEST']._serialized_end=2540
-  _globals['_DROPINDEXRESPONSE']._serialized_start=2542
-  _globals['_DROPINDEXRESPONSE']._serialized_end=2649
-  _globals['_RENAMEINDEXREQUEST']._serialized_start=2651
-  _globals['_RENAMEINDEXREQUEST']._serialized_end=2744
-  _globals['_RENAMEINDEXRESPONSE']._serialized_start=2746
-  _globals['_RENAMEINDEXRESPONSE']._serialized_end=2855
-  _globals['_GETINDEXREQUEST']._serialized_start=2857
-  _globals['_GETINDEXREQUEST']._serialized_end=2919
-  _globals['_GETINDEXRESPONSE']._serialized_start=2922
-  _globals['_GETINDEXRESPONSE']._serialized_end=3173
-  _globals['_QUERY']._serialized_start=3175
-  _globals['_QUERY']._serialized_end=3257
-  _globals['_FINDREQUEST']._serialized_start=3260
-  _globals['_FINDREQUEST']._serialized_end=3488
-  _globals['_FINDREQUEST_DTYPESENTRY']._serialized_start=3443
-  _globals['_FINDREQUEST_DTYPESENTRY']._serialized_end=3488
-  _globals['_FINDRESPONSE']._serialized_start=3490
-  _globals['_FINDRESPONSE']._serialized_end=3614
-  _globals['_FINDBATCHREQUEST']._serialized_start=3616
-  _globals['_FINDBATCHREQUEST']._serialized_end=3690
-  _globals['_FINDBATCHRESPONSE']._serialized_start=3692
-  _globals['_FINDBATCHRESPONSE']._serialized_end=3769
-  _globals['_COUNTREQUEST']._serialized_start=3771
-  _globals['_COUNTREQUEST']._serialized_end=3832
-  _globals['_COUNTRESPONSE']._serialized_start=3834
-  _globals['_COUNTRESPONSE']._serialized_end=3952
-  _globals['_CONTAINSREQUEST']._serialized_start=3954
-  _globals['_CONTAINSREQUEST']._serialized_end=4018
-  _globals['_CONTAINSRESPONSE']._serialized_start=4020
-  _globals['_CONTAINSRESPONSE']._serialized_end=4141
-  _globals['_INSERTREQUEST']._serialized_start=4143
-  _globals['_INSERTREQUEST']._serialized_end=4208
-  _globals['_INSERTRESPONSE']._serialized_start=4210
-  _globals['_INSERTRESPONSE']._serialized_end=4314
-  _globals['_UPDATEREQUEST']._serialized_start=4317
-  _globals['_UPDATEREQUEST']._serialized_end=4460
-  _globals['_UPDATERESPONSE']._serialized_start=4462
-  _globals['_UPDATERESPONSE']._serialized_end=4566
-  _globals['_REMOVEREQUEST']._serialized_start=4568
-  _globals['_REMOVEREQUEST']._serialized_end=4633
-  _globals['_REMOVERESPONSE']._serialized_start=4635
-  _globals['_REMOVERESPONSE']._serialized_end=4739
-  _globals['_EXPLAINREQUEST']._serialized_start=4741
-  _globals['_EXPLAINREQUEST']._serialized_end=4806
-  _globals['_QUERYPLAN']._serialized_start=4808
-  _globals['_QUERYPLAN']._serialized_end=4917
-  _globals['_EXPLAINRESPONSE']._serialized_start=4919
-  _globals['_EXPLAINRESPONSE']._serialized_end=5009
-  _globals['_TRUNCATECOLLECTIONREQUEST']._serialized_start=5011
-  _globals['_TRUNCATECOLLECTIONREQUEST']._serialized_end=5063
-  _globals['_TRUNCATECOLLECTIONRESPONSE']._serialized_start=5065
-  _globals['_TRUNCATECOLLECTIONRESPONSE']._serialized_end=5181
-  _globals['_LISTCOLLECTIONSREQUEST']._serialized_start=5183
-  _globals['_LISTCOLLECTIONSREQUEST']._serialized_end=5207
-  _globals['_LISTCOLLECTIONSRESPONSE']._serialized_start=5210
-  _globals['_LISTCOLLECTIONSRESPONSE']._serialized_end=5349
-  _globals['_DOCUMENTDBSERVICE']._serialized_start=5599
-  _globals['_DOCUMENTDBSERVICE']._serialized_end=7644
+  _globals['_INDEXTYPE']._serialized_start=5219
+  _globals['_INDEXTYPE']._serialized_end=5320
+  _globals['_INDEXSTATUS']._serialized_start=5323
+  _globals['_INDEXSTATUS']._serialized_end=5464
+  _globals['_INDEXDESCRIPTOR']._serialized_start=60
+  _globals['_INDEXDESCRIPTOR']._serialized_end=300
+  _globals['_FTSFIELDSTATS']._serialized_start=303
+  _globals['_FTSFIELDSTATS']._serialized_end=469
+  _globals['_FTSINDEXSTATS']._serialized_start=471
+  _globals['_FTSINDEXSTATS']._serialized_end=581
+  _globals['_INDEXSTATS']._serialized_start=584
+  _globals['_INDEXSTATS']._serialized_end=916
+  _globals['_COLLECTIONINFO']._serialized_start=919
+  _globals['_COLLECTIONINFO']._serialized_end=1081
+  _globals['_PROFILEINFO']._serialized_start=1083
+  _globals['_PROFILEINFO']._serialized_end=1210
+  _globals['_CREATECOLLECTIONREQUEST']._serialized_start=1212
+  _globals['_CREATECOLLECTIONREQUEST']._serialized_end=1295
+  _globals['_CREATECOLLECTIONRESPONSE']._serialized_start=1297
+  _globals['_CREATECOLLECTIONRESPONSE']._serialized_end=1408
+  _globals['_DROPCOLLECTIONREQUEST']._serialized_start=1410
+  _globals['_DROPCOLLECTIONREQUEST']._serialized_end=1458
+  _globals['_DROPCOLLECTIONRESPONSE']._serialized_start=1460
+  _globals['_DROPCOLLECTIONRESPONSE']._serialized_end=1569
+  _globals['_RENAMECOLLECTIONREQUEST']._serialized_start=1571
+  _globals['_RENAMECOLLECTIONREQUEST']._serialized_end=1654
+  _globals['_RENAMECOLLECTIONRESPONSE']._serialized_start=1656
+  _globals['_RENAMECOLLECTIONRESPONSE']._serialized_end=1767
+  _globals['_GETCOLLECTIONREQUEST']._serialized_start=1769
+  _globals['_GETCOLLECTIONREQUEST']._serialized_end=1816
+  _globals['_GETCOLLECTIONRESPONSE']._serialized_start=1819
+  _globals['_GETCOLLECTIONRESPONSE']._serialized_end=1985
+  _globals['_GETCOLLECTIONSREQUEST']._serialized_start=1987
+  _globals['_GETCOLLECTIONSREQUEST']._serialized_end=2036
+  _globals['_GETCOLLECTIONSRESPONSE']._serialized_start=2039
+  _globals['_GETCOLLECTIONSRESPONSE']._serialized_end=2207
+  _globals['_CREATEINDEXREQUEST']._serialized_start=2209
+  _globals['_CREATEINDEXREQUEST']._serialized_end=2313
+  _globals['_CREATEINDEXRESPONSE']._serialized_start=2315
+  _globals['_CREATEINDEXRESPONSE']._serialized_end=2421
+  _globals['_DROPINDEXREQUEST']._serialized_start=2423
+  _globals['_DROPINDEXREQUEST']._serialized_end=2486
+  _globals['_DROPINDEXRESPONSE']._serialized_start=2488
+  _globals['_DROPINDEXRESPONSE']._serialized_end=2592
+  _globals['_RENAMEINDEXREQUEST']._serialized_start=2594
+  _globals['_RENAMEINDEXREQUEST']._serialized_end=2687
+  _globals['_RENAMEINDEXRESPONSE']._serialized_start=2689
+  _globals['_RENAMEINDEXRESPONSE']._serialized_end=2795
+  _globals['_GETINDEXREQUEST']._serialized_start=2797
+  _globals['_GETINDEXREQUEST']._serialized_end=2859
+  _globals['_GETINDEXRESPONSE']._serialized_start=2862
+  _globals['_GETINDEXRESPONSE']._serialized_end=3104
+  _globals['_QUERY']._serialized_start=3106
+  _globals['_QUERY']._serialized_end=3185
+  _globals['_FINDREQUEST']._serialized_start=3188
+  _globals['_FINDREQUEST']._serialized_end=3410
+  _globals['_FINDREQUEST_DTYPESENTRY']._serialized_start=3365
+  _globals['_FINDREQUEST_DTYPESENTRY']._serialized_end=3410
+  _globals['_FINDRESPONSE']._serialized_start=3412
+  _globals['_FINDRESPONSE']._serialized_end=3533
+  _globals['_FINDBATCHREQUEST']._serialized_start=3535
+  _globals['_FINDBATCHREQUEST']._serialized_end=3606
+  _globals['_FINDBATCHRESPONSE']._serialized_start=3608
+  _globals['_FINDBATCHRESPONSE']._serialized_end=3682
+  _globals['_COUNTREQUEST']._serialized_start=3684
+  _globals['_COUNTREQUEST']._serialized_end=3742
+  _globals['_COUNTRESPONSE']._serialized_start=3744
+  _globals['_COUNTRESPONSE']._serialized_end=3859
+  _globals['_CONTAINSREQUEST']._serialized_start=3861
+  _globals['_CONTAINSREQUEST']._serialized_end=3922
+  _globals['_CONTAINSRESPONSE']._serialized_start=3924
+  _globals['_CONTAINSRESPONSE']._serialized_end=4042
+  _globals['_INSERTREQUEST']._serialized_start=4044
+  _globals['_INSERTREQUEST']._serialized_end=4106
+  _globals['_INSERTRESPONSE']._serialized_start=4108
+  _globals['_INSERTRESPONSE']._serialized_end=4209
+  _globals['_UPDATEREQUEST']._serialized_start=4212
+  _globals['_UPDATEREQUEST']._serialized_end=4349
+  _globals['_UPDATERESPONSE']._serialized_start=4351
+  _globals['_UPDATERESPONSE']._serialized_end=4452
+  _globals['_REMOVEREQUEST']._serialized_start=4454
+  _globals['_REMOVEREQUEST']._serialized_end=4516
+  _globals['_REMOVERESPONSE']._serialized_start=4518
+  _globals['_REMOVERESPONSE']._serialized_end=4619
+  _globals['_EXPLAINREQUEST']._serialized_start=4621
+  _globals['_EXPLAINREQUEST']._serialized_end=4683
+  _globals['_QUERYPLAN']._serialized_start=4685
+  _globals['_QUERYPLAN']._serialized_end=4794
+  _globals['_EXPLAINRESPONSE']._serialized_start=4796
+  _globals['_EXPLAINRESPONSE']._serialized_end=4883
+  _globals['_TRUNCATECOLLECTIONREQUEST']._serialized_start=4885
+  _globals['_TRUNCATECOLLECTIONREQUEST']._serialized_end=4937
+  _globals['_TRUNCATECOLLECTIONRESPONSE']._serialized_start=4939
+  _globals['_TRUNCATECOLLECTIONRESPONSE']._serialized_end=5052
+  _globals['_LISTCOLLECTIONSREQUEST']._serialized_start=5054
+  _globals['_LISTCOLLECTIONSREQUEST']._serialized_end=5078
+  _globals['_LISTCOLLECTIONSRESPONSE']._serialized_start=5081
+  _globals['_LISTCOLLECTIONSRESPONSE']._serialized_end=5217
+  _globals['_DOCUMENTDBSERVICE']._serialized_start=5467
+  _globals['_DOCUMENTDBSERVICE']._serialized_end=7397
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aeca-0.1.15.dev2/src/aeca/protobuf/document_db_pb2_grpc.py` & `aeca-1.0.0.dev1/src/aeca/protobuf/document_db_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,105 +11,105 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.find = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/find',
+                '/aeca.rpc.db.document.DocumentDBService/find',
                 request_serializer=document__db__pb2.FindRequest.SerializeToString,
                 response_deserializer=document__db__pb2.FindResponse.FromString,
                 )
         self.find_batch = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/find_batch',
+                '/aeca.rpc.db.document.DocumentDBService/find_batch',
                 request_serializer=document__db__pb2.FindBatchRequest.SerializeToString,
                 response_deserializer=document__db__pb2.FindBatchResponse.FromString,
                 )
         self.count = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/count',
+                '/aeca.rpc.db.document.DocumentDBService/count',
                 request_serializer=document__db__pb2.CountRequest.SerializeToString,
                 response_deserializer=document__db__pb2.CountResponse.FromString,
                 )
         self.contains = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/contains',
+                '/aeca.rpc.db.document.DocumentDBService/contains',
                 request_serializer=document__db__pb2.ContainsRequest.SerializeToString,
                 response_deserializer=document__db__pb2.ContainsResponse.FromString,
                 )
         self.insert = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/insert',
+                '/aeca.rpc.db.document.DocumentDBService/insert',
                 request_serializer=document__db__pb2.InsertRequest.SerializeToString,
                 response_deserializer=document__db__pb2.InsertResponse.FromString,
                 )
         self.update = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/update',
+                '/aeca.rpc.db.document.DocumentDBService/update',
                 request_serializer=document__db__pb2.UpdateRequest.SerializeToString,
                 response_deserializer=document__db__pb2.UpdateResponse.FromString,
                 )
         self.remove = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/remove',
+                '/aeca.rpc.db.document.DocumentDBService/remove',
                 request_serializer=document__db__pb2.RemoveRequest.SerializeToString,
                 response_deserializer=document__db__pb2.RemoveResponse.FromString,
                 )
         self.explain = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/explain',
+                '/aeca.rpc.db.document.DocumentDBService/explain',
                 request_serializer=document__db__pb2.ExplainRequest.SerializeToString,
                 response_deserializer=document__db__pb2.ExplainResponse.FromString,
                 )
         self.create_collection = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/create_collection',
+                '/aeca.rpc.db.document.DocumentDBService/create_collection',
                 request_serializer=document__db__pb2.CreateCollectionRequest.SerializeToString,
                 response_deserializer=document__db__pb2.CreateCollectionResponse.FromString,
                 )
         self.drop_collection = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/drop_collection',
+                '/aeca.rpc.db.document.DocumentDBService/drop_collection',
                 request_serializer=document__db__pb2.DropCollectionRequest.SerializeToString,
                 response_deserializer=document__db__pb2.DropCollectionResponse.FromString,
                 )
         self.rename_collection = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/rename_collection',
+                '/aeca.rpc.db.document.DocumentDBService/rename_collection',
                 request_serializer=document__db__pb2.RenameCollectionRequest.SerializeToString,
                 response_deserializer=document__db__pb2.RenameCollectionResponse.FromString,
                 )
         self.get_collection = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/get_collection',
+                '/aeca.rpc.db.document.DocumentDBService/get_collection',
                 request_serializer=document__db__pb2.GetCollectionRequest.SerializeToString,
                 response_deserializer=document__db__pb2.GetCollectionResponse.FromString,
                 )
         self.get_collections = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/get_collections',
+                '/aeca.rpc.db.document.DocumentDBService/get_collections',
                 request_serializer=document__db__pb2.GetCollectionsRequest.SerializeToString,
                 response_deserializer=document__db__pb2.GetCollectionsResponse.FromString,
                 )
         self.list_collections = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/list_collections',
+                '/aeca.rpc.db.document.DocumentDBService/list_collections',
                 request_serializer=document__db__pb2.ListCollectionsRequest.SerializeToString,
                 response_deserializer=document__db__pb2.ListCollectionsResponse.FromString,
                 )
         self.truncate_collection = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/truncate_collection',
+                '/aeca.rpc.db.document.DocumentDBService/truncate_collection',
                 request_serializer=document__db__pb2.TruncateCollectionRequest.SerializeToString,
                 response_deserializer=document__db__pb2.TruncateCollectionResponse.FromString,
                 )
         self.create_index = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/create_index',
+                '/aeca.rpc.db.document.DocumentDBService/create_index',
                 request_serializer=document__db__pb2.CreateIndexRequest.SerializeToString,
                 response_deserializer=document__db__pb2.CreateIndexResponse.FromString,
                 )
         self.drop_index = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/drop_index',
+                '/aeca.rpc.db.document.DocumentDBService/drop_index',
                 request_serializer=document__db__pb2.DropIndexRequest.SerializeToString,
                 response_deserializer=document__db__pb2.DropIndexResponse.FromString,
                 )
         self.rename_index = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/rename_index',
+                '/aeca.rpc.db.document.DocumentDBService/rename_index',
                 request_serializer=document__db__pb2.RenameIndexRequest.SerializeToString,
                 response_deserializer=document__db__pb2.RenameIndexResponse.FromString,
                 )
         self.get_index = channel.unary_unary(
-                '/cognica.rpc.db.document.DocumentDBService/get_index',
+                '/aeca.rpc.db.document.DocumentDBService/get_index',
                 request_serializer=document__db__pb2.GetIndexRequest.SerializeToString,
                 response_deserializer=document__db__pb2.GetIndexResponse.FromString,
                 )
 
 
 class DocumentDBServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -324,15 +324,15 @@
             'get_index': grpc.unary_unary_rpc_method_handler(
                     servicer.get_index,
                     request_deserializer=document__db__pb2.GetIndexRequest.FromString,
                     response_serializer=document__db__pb2.GetIndexResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'cognica.rpc.db.document.DocumentDBService', rpc_method_handlers)
+            'aeca.rpc.db.document.DocumentDBService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class DocumentDBService(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -343,15 +343,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/find',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/find',
             document__db__pb2.FindRequest.SerializeToString,
             document__db__pb2.FindResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def find_batch(request,
@@ -360,15 +360,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/find_batch',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/find_batch',
             document__db__pb2.FindBatchRequest.SerializeToString,
             document__db__pb2.FindBatchResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def count(request,
@@ -377,15 +377,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/count',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/count',
             document__db__pb2.CountRequest.SerializeToString,
             document__db__pb2.CountResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def contains(request,
@@ -394,15 +394,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/contains',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/contains',
             document__db__pb2.ContainsRequest.SerializeToString,
             document__db__pb2.ContainsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def insert(request,
@@ -411,15 +411,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/insert',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/insert',
             document__db__pb2.InsertRequest.SerializeToString,
             document__db__pb2.InsertResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def update(request,
@@ -428,15 +428,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/update',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/update',
             document__db__pb2.UpdateRequest.SerializeToString,
             document__db__pb2.UpdateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def remove(request,
@@ -445,15 +445,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/remove',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/remove',
             document__db__pb2.RemoveRequest.SerializeToString,
             document__db__pb2.RemoveResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def explain(request,
@@ -462,15 +462,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/explain',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/explain',
             document__db__pb2.ExplainRequest.SerializeToString,
             document__db__pb2.ExplainResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def create_collection(request,
@@ -479,15 +479,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/create_collection',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/create_collection',
             document__db__pb2.CreateCollectionRequest.SerializeToString,
             document__db__pb2.CreateCollectionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def drop_collection(request,
@@ -496,15 +496,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/drop_collection',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/drop_collection',
             document__db__pb2.DropCollectionRequest.SerializeToString,
             document__db__pb2.DropCollectionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def rename_collection(request,
@@ -513,15 +513,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/rename_collection',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/rename_collection',
             document__db__pb2.RenameCollectionRequest.SerializeToString,
             document__db__pb2.RenameCollectionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get_collection(request,
@@ -530,15 +530,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/get_collection',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/get_collection',
             document__db__pb2.GetCollectionRequest.SerializeToString,
             document__db__pb2.GetCollectionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get_collections(request,
@@ -547,15 +547,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/get_collections',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/get_collections',
             document__db__pb2.GetCollectionsRequest.SerializeToString,
             document__db__pb2.GetCollectionsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def list_collections(request,
@@ -564,15 +564,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/list_collections',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/list_collections',
             document__db__pb2.ListCollectionsRequest.SerializeToString,
             document__db__pb2.ListCollectionsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def truncate_collection(request,
@@ -581,15 +581,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/truncate_collection',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/truncate_collection',
             document__db__pb2.TruncateCollectionRequest.SerializeToString,
             document__db__pb2.TruncateCollectionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def create_index(request,
@@ -598,15 +598,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/create_index',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/create_index',
             document__db__pb2.CreateIndexRequest.SerializeToString,
             document__db__pb2.CreateIndexResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def drop_index(request,
@@ -615,15 +615,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/drop_index',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/drop_index',
             document__db__pb2.DropIndexRequest.SerializeToString,
             document__db__pb2.DropIndexResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def rename_index(request,
@@ -632,15 +632,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/rename_index',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/rename_index',
             document__db__pb2.RenameIndexRequest.SerializeToString,
             document__db__pb2.RenameIndexResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get_index(request,
@@ -649,12 +649,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.document.DocumentDBService/get_index',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.document.DocumentDBService/get_index',
             document__db__pb2.GetIndexRequest.SerializeToString,
             document__db__pb2.GetIndexResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `aeca-0.1.15.dev2/src/aeca/protobuf/document_pb2.py` & `aeca-1.0.0.dev1/src/aeca/protobuf/document_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x64ocument.proto\x12\x17\x63ognica.rpc.db.document\"\xdb\x01\n\x05Value\x12\x0e\n\x04null\x18\x01 \x01(\x08H\x00\x12\x0e\n\x04\x62ool\x18\x02 \x01(\x08H\x00\x12\x0f\n\x05int64\x18\x03 \x01(\x03H\x00\x12\x10\n\x06uint64\x18\x04 \x01(\x04H\x00\x12\x10\n\x06\x64ouble\x18\x05 \x01(\x01H\x00\x12\x10\n\x06string\x18\x06 \x01(\tH\x00\x12/\n\x05\x61rray\x18\x07 \x01(\x0b\x32\x1e.cognica.rpc.db.document.ArrayH\x00\x12\x31\n\x06object\x18\x08 \x01(\x0b\x32\x1f.cognica.rpc.db.document.ObjectH\x00\x42\x07\n\x05value\"6\n\x05\x41rray\x12-\n\x05value\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Value\"\x91\x01\n\x06Object\x12\x39\n\x05value\x18\x01 \x03(\x0b\x32*.cognica.rpc.db.document.Object.ValueEntry\x1aL\n\nValueEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Value:\x02\x38\x01\"U\n\x08\x44ocument\x12\x31\n\x06object\x18\x01 \x01(\x0b\x32\x1f.cognica.rpc.db.document.ObjectH\x00\x12\x0e\n\x04json\x18\x02 \x01(\tH\x00\x42\x06\n\x04typeB\x03\xf8\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x64ocument.proto\x12\x14\x61\x65\x63\x61.rpc.db.document\"\xd5\x01\n\x05Value\x12\x0e\n\x04null\x18\x01 \x01(\x08H\x00\x12\x0e\n\x04\x62ool\x18\x02 \x01(\x08H\x00\x12\x0f\n\x05int64\x18\x03 \x01(\x03H\x00\x12\x10\n\x06uint64\x18\x04 \x01(\x04H\x00\x12\x10\n\x06\x64ouble\x18\x05 \x01(\x01H\x00\x12\x10\n\x06string\x18\x06 \x01(\tH\x00\x12,\n\x05\x61rray\x18\x07 \x01(\x0b\x32\x1b.aeca.rpc.db.document.ArrayH\x00\x12.\n\x06object\x18\x08 \x01(\x0b\x32\x1c.aeca.rpc.db.document.ObjectH\x00\x42\x07\n\x05value\"3\n\x05\x41rray\x12*\n\x05value\x18\x01 \x03(\x0b\x32\x1b.aeca.rpc.db.document.Value\"\x8b\x01\n\x06Object\x12\x36\n\x05value\x18\x01 \x03(\x0b\x32\'.aeca.rpc.db.document.Object.ValueEntry\x1aI\n\nValueEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x1b.aeca.rpc.db.document.Value:\x02\x38\x01\"R\n\x08\x44ocument\x12.\n\x06object\x18\x01 \x01(\x0b\x32\x1c.aeca.rpc.db.document.ObjectH\x00\x12\x0e\n\x04json\x18\x02 \x01(\tH\x00\x42\x06\n\x04typeB\x03\xf8\x01\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'document_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\370\001\001'
   _globals['_OBJECT_VALUEENTRY']._options = None
   _globals['_OBJECT_VALUEENTRY']._serialized_options = b'8\001'
-  _globals['_VALUE']._serialized_start=44
-  _globals['_VALUE']._serialized_end=263
-  _globals['_ARRAY']._serialized_start=265
-  _globals['_ARRAY']._serialized_end=319
-  _globals['_OBJECT']._serialized_start=322
-  _globals['_OBJECT']._serialized_end=467
-  _globals['_OBJECT_VALUEENTRY']._serialized_start=391
-  _globals['_OBJECT_VALUEENTRY']._serialized_end=467
-  _globals['_DOCUMENT']._serialized_start=469
-  _globals['_DOCUMENT']._serialized_end=554
+  _globals['_VALUE']._serialized_start=41
+  _globals['_VALUE']._serialized_end=254
+  _globals['_ARRAY']._serialized_start=256
+  _globals['_ARRAY']._serialized_end=307
+  _globals['_OBJECT']._serialized_start=310
+  _globals['_OBJECT']._serialized_end=449
+  _globals['_OBJECT_VALUEENTRY']._serialized_start=376
+  _globals['_OBJECT_VALUEENTRY']._serialized_end=449
+  _globals['_DOCUMENT']._serialized_start=451
+  _globals['_DOCUMENT']._serialized_end=533
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aeca-0.1.15.dev2/src/aeca/protobuf/fts_analysis_pipeline_pb2.py` & `aeca-1.0.0.dev1/src/aeca/protobuf/fts_analysis_pipeline_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66ts_analysis_pipeline.proto\x12\x12\x63ognica.rpc.db.fts\"\"\n\x0bProfileInfo\x12\x13\n\x0b\x64uration_us\x18\x01 \x01(\x04\"k\n\x18PipelineExecutionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x13\n\x0b\x66ield_names\x18\x03 \x03(\t\x12\r\n\x05query\x18\x04 \x01(\t\"m\n\x19PipelineExecutionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x01(\t\x12\x30\n\x07profile\x18\x03 \x01(\x0b\x32\x1f.cognica.rpc.db.fts.ProfileInfo\"Y\n\x1d\x41\x64hocPipelineExecutionRequest\x12\x14\n\x0cpipeline_def\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_names\x18\x02 \x03(\t\x12\r\n\x05query\x18\x03 \x01(\t\"r\n\x1e\x41\x64hocPipelineExecutionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x01(\t\x12\x30\n\x07profile\x18\x03 \x01(\x0b\x32\x1f.cognica.rpc.db.fts.ProfileInfo2\x80\x02\n\x1a\x46TSAnalysisPipelineService\x12h\n\x07\x65xecute\x12,.cognica.rpc.db.fts.PipelineExecutionRequest\x1a-.cognica.rpc.db.fts.PipelineExecutionResponse\"\x00\x12x\n\rexecute_adhoc\x12\x31.cognica.rpc.db.fts.AdhocPipelineExecutionRequest\x1a\x32.cognica.rpc.db.fts.AdhocPipelineExecutionResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66ts_analysis_pipeline.proto\x12\x0f\x61\x65\x63\x61.rpc.db.fts\"\"\n\x0bProfileInfo\x12\x13\n\x0b\x64uration_us\x18\x01 \x01(\x04\"k\n\x18PipelineExecutionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x13\n\x0b\x66ield_names\x18\x03 \x03(\t\x12\r\n\x05query\x18\x04 \x01(\t\"j\n\x19PipelineExecutionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x01(\t\x12-\n\x07profile\x18\x03 \x01(\x0b\x32\x1c.aeca.rpc.db.fts.ProfileInfo\"Y\n\x1d\x41\x64hocPipelineExecutionRequest\x12\x14\n\x0cpipeline_def\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_names\x18\x02 \x03(\t\x12\r\n\x05query\x18\x03 \x01(\t\"o\n\x1e\x41\x64hocPipelineExecutionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x01(\t\x12-\n\x07profile\x18\x03 \x01(\x0b\x32\x1c.aeca.rpc.db.fts.ProfileInfo2\xf4\x01\n\x1a\x46TSAnalysisPipelineService\x12\x62\n\x07\x65xecute\x12).aeca.rpc.db.fts.PipelineExecutionRequest\x1a*.aeca.rpc.db.fts.PipelineExecutionResponse\"\x00\x12r\n\rexecute_adhoc\x12..aeca.rpc.db.fts.AdhocPipelineExecutionRequest\x1a/.aeca.rpc.db.fts.AdhocPipelineExecutionResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fts_analysis_pipeline_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\370\001\001'
-  _globals['_PROFILEINFO']._serialized_start=51
-  _globals['_PROFILEINFO']._serialized_end=85
-  _globals['_PIPELINEEXECUTIONREQUEST']._serialized_start=87
-  _globals['_PIPELINEEXECUTIONREQUEST']._serialized_end=194
-  _globals['_PIPELINEEXECUTIONRESPONSE']._serialized_start=196
-  _globals['_PIPELINEEXECUTIONRESPONSE']._serialized_end=305
-  _globals['_ADHOCPIPELINEEXECUTIONREQUEST']._serialized_start=307
-  _globals['_ADHOCPIPELINEEXECUTIONREQUEST']._serialized_end=396
-  _globals['_ADHOCPIPELINEEXECUTIONRESPONSE']._serialized_start=398
-  _globals['_ADHOCPIPELINEEXECUTIONRESPONSE']._serialized_end=512
-  _globals['_FTSANALYSISPIPELINESERVICE']._serialized_start=515
-  _globals['_FTSANALYSISPIPELINESERVICE']._serialized_end=771
+  _globals['_PROFILEINFO']._serialized_start=48
+  _globals['_PROFILEINFO']._serialized_end=82
+  _globals['_PIPELINEEXECUTIONREQUEST']._serialized_start=84
+  _globals['_PIPELINEEXECUTIONREQUEST']._serialized_end=191
+  _globals['_PIPELINEEXECUTIONRESPONSE']._serialized_start=193
+  _globals['_PIPELINEEXECUTIONRESPONSE']._serialized_end=299
+  _globals['_ADHOCPIPELINEEXECUTIONREQUEST']._serialized_start=301
+  _globals['_ADHOCPIPELINEEXECUTIONREQUEST']._serialized_end=390
+  _globals['_ADHOCPIPELINEEXECUTIONRESPONSE']._serialized_start=392
+  _globals['_ADHOCPIPELINEEXECUTIONRESPONSE']._serialized_end=503
+  _globals['_FTSANALYSISPIPELINESERVICE']._serialized_start=506
+  _globals['_FTSANALYSISPIPELINESERVICE']._serialized_end=750
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aeca-0.1.15.dev2/src/aeca/protobuf/fts_analysis_pipeline_pb2_grpc.py` & `aeca-1.0.0.dev1/src/aeca/protobuf/fts_analysis_pipeline_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.execute = channel.unary_unary(
-                '/cognica.rpc.db.fts.FTSAnalysisPipelineService/execute',
+                '/aeca.rpc.db.fts.FTSAnalysisPipelineService/execute',
                 request_serializer=fts__analysis__pipeline__pb2.PipelineExecutionRequest.SerializeToString,
                 response_deserializer=fts__analysis__pipeline__pb2.PipelineExecutionResponse.FromString,
                 )
         self.execute_adhoc = channel.unary_unary(
-                '/cognica.rpc.db.fts.FTSAnalysisPipelineService/execute_adhoc',
+                '/aeca.rpc.db.fts.FTSAnalysisPipelineService/execute_adhoc',
                 request_serializer=fts__analysis__pipeline__pb2.AdhocPipelineExecutionRequest.SerializeToString,
                 response_deserializer=fts__analysis__pipeline__pb2.AdhocPipelineExecutionResponse.FromString,
                 )
 
 
 class FTSAnalysisPipelineServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -52,15 +52,15 @@
             'execute_adhoc': grpc.unary_unary_rpc_method_handler(
                     servicer.execute_adhoc,
                     request_deserializer=fts__analysis__pipeline__pb2.AdhocPipelineExecutionRequest.FromString,
                     response_serializer=fts__analysis__pipeline__pb2.AdhocPipelineExecutionResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'cognica.rpc.db.fts.FTSAnalysisPipelineService', rpc_method_handlers)
+            'aeca.rpc.db.fts.FTSAnalysisPipelineService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class FTSAnalysisPipelineService(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -71,15 +71,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.fts.FTSAnalysisPipelineService/execute',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.fts.FTSAnalysisPipelineService/execute',
             fts__analysis__pipeline__pb2.PipelineExecutionRequest.SerializeToString,
             fts__analysis__pipeline__pb2.PipelineExecutionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def execute_adhoc(request,
@@ -88,12 +88,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.fts.FTSAnalysisPipelineService/execute_adhoc',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.fts.FTSAnalysisPipelineService/execute_adhoc',
             fts__analysis__pipeline__pb2.AdhocPipelineExecutionRequest.SerializeToString,
             fts__analysis__pipeline__pb2.AdhocPipelineExecutionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `aeca-0.1.15.dev2/src/aeca/protobuf/key_value_db_pb2.py` & `aeca-1.0.0.dev1/src/aeca/protobuf/key_value_db_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,70 +10,70 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12key_value_db.proto\x12\x11\x63ognica.rpc.db.kv\"\"\n\x0bProfileInfo\x12\x13\n\x0b\x64uration_us\x18\x01 \x01(\x04\"{\n\x08Response\x12-\n\x06status\x18\x01 \x01(\x0e\x32\x1d.cognica.rpc.db.kv.StatusType\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x07profile\x18\x03 \x01(\x0b\x32\x1e.cognica.rpc.db.kv.ProfileInfo\"g\n\nPutRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\x12\r\n\x05value\x18\x03 \x01(\x0c\x12\x0b\n\x03ttl\x18\x04 \x01(\x03\x12\x19\n\x11\x63reate_if_missing\x18\x05 \x01(\x08\"<\n\x0bPutResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"3\n\rRemoveRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\"?\n\x0eRemoveResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"0\n\nGetRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\"K\n\x0bGetResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\x12\r\n\x05value\x18\x02 \x01(\x0c\"6\n\x0fMultiGetRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\"R\n\x10MultiGetResponse\x12.\n\tresponses\x18\x01 \x03(\x0b\x32\x1b.cognica.rpc.db.kv.Response\x12\x0e\n\x06values\x18\x02 \x03(\x0c\"q\n\x11\x42\x61tchedPutRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\x12\x0e\n\x06values\x18\x03 \x03(\x0c\x12\x0c\n\x04ttls\x18\x04 \x03(\x03\x12\x19\n\x11\x63reate_if_missing\x18\x05 \x01(\x08\"D\n\x12\x42\x61tchedPutResponse\x12.\n\tresponses\x18\x01 \x03(\x0b\x32\x1b.cognica.rpc.db.kv.Response\";\n\x14\x42\x61tchedRemoveRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\"G\n\x15\x42\x61tchedRemoveResponse\x12.\n\tresponses\x18\x01 \x03(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"8\n\x11\x42\x61tchedGetRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\"T\n\x12\x42\x61tchedGetResponse\x12.\n\tresponses\x18\x01 \x03(\x0b\x32\x1b.cognica.rpc.db.kv.Response\x12\x0e\n\x06values\x18\x02 \x03(\x0c\".\n\x15\x43reateKeyspaceRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\"G\n\x16\x43reateKeyspaceResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\",\n\x13\x44ropKeyspaceRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\"E\n\x14\x44ropKeyspaceResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"0\n\x17TruncateKeyspaceRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\"I\n\x18TruncateKeyspaceResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"\x16\n\x14ListKeyspacesRequest\"^\n\x15ListKeyspacesResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\x12\x16\n\x0ekeyspace_names\x18\x02 \x03(\t*3\n\nStatusType\x12\x07\n\x03kOK\x10\x00\x12\r\n\tkNotFound\x10\x01\x12\r\n\tkInternal\x10\n2\xe4\x04\n\x11KeyValueDBService\x12\x46\n\x03put\x12\x1d.cognica.rpc.db.kv.PutRequest\x1a\x1e.cognica.rpc.db.kv.PutResponse\"\x00\x12O\n\x06remove\x12 .cognica.rpc.db.kv.RemoveRequest\x1a!.cognica.rpc.db.kv.RemoveResponse\"\x00\x12\x46\n\x03get\x12\x1d.cognica.rpc.db.kv.GetRequest\x1a\x1e.cognica.rpc.db.kv.GetResponse\"\x00\x12Q\n\x04mget\x12\".cognica.rpc.db.kv.MultiGetRequest\x1a#.cognica.rpc.db.kv.MultiGetResponse\"\x00\x12Z\n\tput_batch\x12$.cognica.rpc.db.kv.BatchedPutRequest\x1a%.cognica.rpc.db.kv.BatchedPutResponse\"\x00\x12\x63\n\x0cremove_batch\x12\'.cognica.rpc.db.kv.BatchedRemoveRequest\x1a(.cognica.rpc.db.kv.BatchedRemoveResponse\"\x00\x12Z\n\tget_batch\x12$.cognica.rpc.db.kv.BatchedGetRequest\x1a%.cognica.rpc.db.kv.BatchedGetResponse\"\x00\x32\xbd\x03\n\x16KeyspaceManagerService\x12h\n\x0f\x63reate_keyspace\x12(.cognica.rpc.db.kv.CreateKeyspaceRequest\x1a).cognica.rpc.db.kv.CreateKeyspaceResponse\"\x00\x12\x62\n\rdrop_keyspace\x12&.cognica.rpc.db.kv.DropKeyspaceRequest\x1a\'.cognica.rpc.db.kv.DropKeyspaceResponse\"\x00\x12n\n\x11truncate_keyspace\x12*.cognica.rpc.db.kv.TruncateKeyspaceRequest\x1a+.cognica.rpc.db.kv.TruncateKeyspaceResponse\"\x00\x12\x65\n\x0elist_keyspaces\x12\'.cognica.rpc.db.kv.ListKeyspacesRequest\x1a(.cognica.rpc.db.kv.ListKeyspacesResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12key_value_db.proto\x12\x0e\x61\x65\x63\x61.rpc.db.kv\"\"\n\x0bProfileInfo\x12\x13\n\x0b\x64uration_us\x18\x01 \x01(\x04\"u\n\x08Response\x12*\n\x06status\x18\x01 \x01(\x0e\x32\x1a.aeca.rpc.db.kv.StatusType\x12\x0f\n\x07message\x18\x02 \x01(\t\x12,\n\x07profile\x18\x03 \x01(\x0b\x32\x1b.aeca.rpc.db.kv.ProfileInfo\"g\n\nPutRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\x12\r\n\x05value\x18\x03 \x01(\x0c\x12\x0b\n\x03ttl\x18\x04 \x01(\x03\x12\x19\n\x11\x63reate_if_missing\x18\x05 \x01(\x08\"9\n\x0bPutResponse\x12*\n\x08response\x18\x01 \x01(\x0b\x32\x18.aeca.rpc.db.kv.Response\"3\n\rRemoveRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\"<\n\x0eRemoveResponse\x12*\n\x08response\x18\x01 \x01(\x0b\x32\x18.aeca.rpc.db.kv.Response\"0\n\nGetRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\"H\n\x0bGetResponse\x12*\n\x08response\x18\x01 \x01(\x0b\x32\x18.aeca.rpc.db.kv.Response\x12\r\n\x05value\x18\x02 \x01(\x0c\"6\n\x0fMultiGetRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\"O\n\x10MultiGetResponse\x12+\n\tresponses\x18\x01 \x03(\x0b\x32\x18.aeca.rpc.db.kv.Response\x12\x0e\n\x06values\x18\x02 \x03(\x0c\"q\n\x11\x42\x61tchedPutRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\x12\x0e\n\x06values\x18\x03 \x03(\x0c\x12\x0c\n\x04ttls\x18\x04 \x03(\x03\x12\x19\n\x11\x63reate_if_missing\x18\x05 \x01(\x08\"A\n\x12\x42\x61tchedPutResponse\x12+\n\tresponses\x18\x01 \x03(\x0b\x32\x18.aeca.rpc.db.kv.Response\";\n\x14\x42\x61tchedRemoveRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\"D\n\x15\x42\x61tchedRemoveResponse\x12+\n\tresponses\x18\x01 \x03(\x0b\x32\x18.aeca.rpc.db.kv.Response\"8\n\x11\x42\x61tchedGetRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\"Q\n\x12\x42\x61tchedGetResponse\x12+\n\tresponses\x18\x01 \x03(\x0b\x32\x18.aeca.rpc.db.kv.Response\x12\x0e\n\x06values\x18\x02 \x03(\x0c\".\n\x15\x43reateKeyspaceRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\"D\n\x16\x43reateKeyspaceResponse\x12*\n\x08response\x18\x01 \x01(\x0b\x32\x18.aeca.rpc.db.kv.Response\",\n\x13\x44ropKeyspaceRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\"B\n\x14\x44ropKeyspaceResponse\x12*\n\x08response\x18\x01 \x01(\x0b\x32\x18.aeca.rpc.db.kv.Response\"0\n\x17TruncateKeyspaceRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\"F\n\x18TruncateKeyspaceResponse\x12*\n\x08response\x18\x01 \x01(\x0b\x32\x18.aeca.rpc.db.kv.Response\"\x16\n\x14ListKeyspacesRequest\"[\n\x15ListKeyspacesResponse\x12*\n\x08response\x18\x01 \x01(\x0b\x32\x18.aeca.rpc.db.kv.Response\x12\x16\n\x0ekeyspace_names\x18\x02 \x03(\t*3\n\nStatusType\x12\x07\n\x03kOK\x10\x00\x12\r\n\tkNotFound\x10\x01\x12\r\n\tkInternal\x10\n2\xba\x04\n\x11KeyValueDBService\x12@\n\x03put\x12\x1a.aeca.rpc.db.kv.PutRequest\x1a\x1b.aeca.rpc.db.kv.PutResponse\"\x00\x12I\n\x06remove\x12\x1d.aeca.rpc.db.kv.RemoveRequest\x1a\x1e.aeca.rpc.db.kv.RemoveResponse\"\x00\x12@\n\x03get\x12\x1a.aeca.rpc.db.kv.GetRequest\x1a\x1b.aeca.rpc.db.kv.GetResponse\"\x00\x12K\n\x04mget\x12\x1f.aeca.rpc.db.kv.MultiGetRequest\x1a .aeca.rpc.db.kv.MultiGetResponse\"\x00\x12T\n\tput_batch\x12!.aeca.rpc.db.kv.BatchedPutRequest\x1a\".aeca.rpc.db.kv.BatchedPutResponse\"\x00\x12]\n\x0cremove_batch\x12$.aeca.rpc.db.kv.BatchedRemoveRequest\x1a%.aeca.rpc.db.kv.BatchedRemoveResponse\"\x00\x12T\n\tget_batch\x12!.aeca.rpc.db.kv.BatchedGetRequest\x1a\".aeca.rpc.db.kv.BatchedGetResponse\"\x00\x32\xa5\x03\n\x16KeyspaceManagerService\x12\x62\n\x0f\x63reate_keyspace\x12%.aeca.rpc.db.kv.CreateKeyspaceRequest\x1a&.aeca.rpc.db.kv.CreateKeyspaceResponse\"\x00\x12\\\n\rdrop_keyspace\x12#.aeca.rpc.db.kv.DropKeyspaceRequest\x1a$.aeca.rpc.db.kv.DropKeyspaceResponse\"\x00\x12h\n\x11truncate_keyspace\x12\'.aeca.rpc.db.kv.TruncateKeyspaceRequest\x1a(.aeca.rpc.db.kv.TruncateKeyspaceResponse\"\x00\x12_\n\x0elist_keyspaces\x12$.aeca.rpc.db.kv.ListKeyspacesRequest\x1a%.aeca.rpc.db.kv.ListKeyspacesResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'key_value_db_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\370\001\001'
-  _globals['_STATUSTYPE']._serialized_start=1700
-  _globals['_STATUSTYPE']._serialized_end=1751
-  _globals['_PROFILEINFO']._serialized_start=41
-  _globals['_PROFILEINFO']._serialized_end=75
-  _globals['_RESPONSE']._serialized_start=77
-  _globals['_RESPONSE']._serialized_end=200
-  _globals['_PUTREQUEST']._serialized_start=202
-  _globals['_PUTREQUEST']._serialized_end=305
-  _globals['_PUTRESPONSE']._serialized_start=307
-  _globals['_PUTRESPONSE']._serialized_end=367
-  _globals['_REMOVEREQUEST']._serialized_start=369
-  _globals['_REMOVEREQUEST']._serialized_end=420
-  _globals['_REMOVERESPONSE']._serialized_start=422
-  _globals['_REMOVERESPONSE']._serialized_end=485
-  _globals['_GETREQUEST']._serialized_start=487
-  _globals['_GETREQUEST']._serialized_end=535
-  _globals['_GETRESPONSE']._serialized_start=537
-  _globals['_GETRESPONSE']._serialized_end=612
-  _globals['_MULTIGETREQUEST']._serialized_start=614
-  _globals['_MULTIGETREQUEST']._serialized_end=668
-  _globals['_MULTIGETRESPONSE']._serialized_start=670
-  _globals['_MULTIGETRESPONSE']._serialized_end=752
-  _globals['_BATCHEDPUTREQUEST']._serialized_start=754
-  _globals['_BATCHEDPUTREQUEST']._serialized_end=867
-  _globals['_BATCHEDPUTRESPONSE']._serialized_start=869
-  _globals['_BATCHEDPUTRESPONSE']._serialized_end=937
-  _globals['_BATCHEDREMOVEREQUEST']._serialized_start=939
-  _globals['_BATCHEDREMOVEREQUEST']._serialized_end=998
-  _globals['_BATCHEDREMOVERESPONSE']._serialized_start=1000
-  _globals['_BATCHEDREMOVERESPONSE']._serialized_end=1071
-  _globals['_BATCHEDGETREQUEST']._serialized_start=1073
-  _globals['_BATCHEDGETREQUEST']._serialized_end=1129
-  _globals['_BATCHEDGETRESPONSE']._serialized_start=1131
-  _globals['_BATCHEDGETRESPONSE']._serialized_end=1215
-  _globals['_CREATEKEYSPACEREQUEST']._serialized_start=1217
-  _globals['_CREATEKEYSPACEREQUEST']._serialized_end=1263
-  _globals['_CREATEKEYSPACERESPONSE']._serialized_start=1265
-  _globals['_CREATEKEYSPACERESPONSE']._serialized_end=1336
-  _globals['_DROPKEYSPACEREQUEST']._serialized_start=1338
-  _globals['_DROPKEYSPACEREQUEST']._serialized_end=1382
-  _globals['_DROPKEYSPACERESPONSE']._serialized_start=1384
-  _globals['_DROPKEYSPACERESPONSE']._serialized_end=1453
-  _globals['_TRUNCATEKEYSPACEREQUEST']._serialized_start=1455
-  _globals['_TRUNCATEKEYSPACEREQUEST']._serialized_end=1503
-  _globals['_TRUNCATEKEYSPACERESPONSE']._serialized_start=1505
-  _globals['_TRUNCATEKEYSPACERESPONSE']._serialized_end=1578
-  _globals['_LISTKEYSPACESREQUEST']._serialized_start=1580
-  _globals['_LISTKEYSPACESREQUEST']._serialized_end=1602
-  _globals['_LISTKEYSPACESRESPONSE']._serialized_start=1604
-  _globals['_LISTKEYSPACESRESPONSE']._serialized_end=1698
-  _globals['_KEYVALUEDBSERVICE']._serialized_start=1754
-  _globals['_KEYVALUEDBSERVICE']._serialized_end=2366
-  _globals['_KEYSPACEMANAGERSERVICE']._serialized_start=2369
-  _globals['_KEYSPACEMANAGERSERVICE']._serialized_end=2814
+  _globals['_STATUSTYPE']._serialized_start=1658
+  _globals['_STATUSTYPE']._serialized_end=1709
+  _globals['_PROFILEINFO']._serialized_start=38
+  _globals['_PROFILEINFO']._serialized_end=72
+  _globals['_RESPONSE']._serialized_start=74
+  _globals['_RESPONSE']._serialized_end=191
+  _globals['_PUTREQUEST']._serialized_start=193
+  _globals['_PUTREQUEST']._serialized_end=296
+  _globals['_PUTRESPONSE']._serialized_start=298
+  _globals['_PUTRESPONSE']._serialized_end=355
+  _globals['_REMOVEREQUEST']._serialized_start=357
+  _globals['_REMOVEREQUEST']._serialized_end=408
+  _globals['_REMOVERESPONSE']._serialized_start=410
+  _globals['_REMOVERESPONSE']._serialized_end=470
+  _globals['_GETREQUEST']._serialized_start=472
+  _globals['_GETREQUEST']._serialized_end=520
+  _globals['_GETRESPONSE']._serialized_start=522
+  _globals['_GETRESPONSE']._serialized_end=594
+  _globals['_MULTIGETREQUEST']._serialized_start=596
+  _globals['_MULTIGETREQUEST']._serialized_end=650
+  _globals['_MULTIGETRESPONSE']._serialized_start=652
+  _globals['_MULTIGETRESPONSE']._serialized_end=731
+  _globals['_BATCHEDPUTREQUEST']._serialized_start=733
+  _globals['_BATCHEDPUTREQUEST']._serialized_end=846
+  _globals['_BATCHEDPUTRESPONSE']._serialized_start=848
+  _globals['_BATCHEDPUTRESPONSE']._serialized_end=913
+  _globals['_BATCHEDREMOVEREQUEST']._serialized_start=915
+  _globals['_BATCHEDREMOVEREQUEST']._serialized_end=974
+  _globals['_BATCHEDREMOVERESPONSE']._serialized_start=976
+  _globals['_BATCHEDREMOVERESPONSE']._serialized_end=1044
+  _globals['_BATCHEDGETREQUEST']._serialized_start=1046
+  _globals['_BATCHEDGETREQUEST']._serialized_end=1102
+  _globals['_BATCHEDGETRESPONSE']._serialized_start=1104
+  _globals['_BATCHEDGETRESPONSE']._serialized_end=1185
+  _globals['_CREATEKEYSPACEREQUEST']._serialized_start=1187
+  _globals['_CREATEKEYSPACEREQUEST']._serialized_end=1233
+  _globals['_CREATEKEYSPACERESPONSE']._serialized_start=1235
+  _globals['_CREATEKEYSPACERESPONSE']._serialized_end=1303
+  _globals['_DROPKEYSPACEREQUEST']._serialized_start=1305
+  _globals['_DROPKEYSPACEREQUEST']._serialized_end=1349
+  _globals['_DROPKEYSPACERESPONSE']._serialized_start=1351
+  _globals['_DROPKEYSPACERESPONSE']._serialized_end=1417
+  _globals['_TRUNCATEKEYSPACEREQUEST']._serialized_start=1419
+  _globals['_TRUNCATEKEYSPACEREQUEST']._serialized_end=1467
+  _globals['_TRUNCATEKEYSPACERESPONSE']._serialized_start=1469
+  _globals['_TRUNCATEKEYSPACERESPONSE']._serialized_end=1539
+  _globals['_LISTKEYSPACESREQUEST']._serialized_start=1541
+  _globals['_LISTKEYSPACESREQUEST']._serialized_end=1563
+  _globals['_LISTKEYSPACESRESPONSE']._serialized_start=1565
+  _globals['_LISTKEYSPACESRESPONSE']._serialized_end=1656
+  _globals['_KEYVALUEDBSERVICE']._serialized_start=1712
+  _globals['_KEYVALUEDBSERVICE']._serialized_end=2282
+  _globals['_KEYSPACEMANAGERSERVICE']._serialized_start=2285
+  _globals['_KEYSPACEMANAGERSERVICE']._serialized_end=2706
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aeca-0.1.15.dev2/src/aeca/protobuf/key_value_db_pb2_grpc.py` & `aeca-1.0.0.dev1/src/aeca/protobuf/key_value_db_pb2_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,45 +11,45 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.put = channel.unary_unary(
-                '/cognica.rpc.db.kv.KeyValueDBService/put',
+                '/aeca.rpc.db.kv.KeyValueDBService/put',
                 request_serializer=key__value__db__pb2.PutRequest.SerializeToString,
                 response_deserializer=key__value__db__pb2.PutResponse.FromString,
                 )
         self.remove = channel.unary_unary(
-                '/cognica.rpc.db.kv.KeyValueDBService/remove',
+                '/aeca.rpc.db.kv.KeyValueDBService/remove',
                 request_serializer=key__value__db__pb2.RemoveRequest.SerializeToString,
                 response_deserializer=key__value__db__pb2.RemoveResponse.FromString,
                 )
         self.get = channel.unary_unary(
-                '/cognica.rpc.db.kv.KeyValueDBService/get',
+                '/aeca.rpc.db.kv.KeyValueDBService/get',
                 request_serializer=key__value__db__pb2.GetRequest.SerializeToString,
                 response_deserializer=key__value__db__pb2.GetResponse.FromString,
                 )
         self.mget = channel.unary_unary(
-                '/cognica.rpc.db.kv.KeyValueDBService/mget',
+                '/aeca.rpc.db.kv.KeyValueDBService/mget',
                 request_serializer=key__value__db__pb2.MultiGetRequest.SerializeToString,
                 response_deserializer=key__value__db__pb2.MultiGetResponse.FromString,
                 )
         self.put_batch = channel.unary_unary(
-                '/cognica.rpc.db.kv.KeyValueDBService/put_batch',
+                '/aeca.rpc.db.kv.KeyValueDBService/put_batch',
                 request_serializer=key__value__db__pb2.BatchedPutRequest.SerializeToString,
                 response_deserializer=key__value__db__pb2.BatchedPutResponse.FromString,
                 )
         self.remove_batch = channel.unary_unary(
-                '/cognica.rpc.db.kv.KeyValueDBService/remove_batch',
+                '/aeca.rpc.db.kv.KeyValueDBService/remove_batch',
                 request_serializer=key__value__db__pb2.BatchedRemoveRequest.SerializeToString,
                 response_deserializer=key__value__db__pb2.BatchedRemoveResponse.FromString,
                 )
         self.get_batch = channel.unary_unary(
-                '/cognica.rpc.db.kv.KeyValueDBService/get_batch',
+                '/aeca.rpc.db.kv.KeyValueDBService/get_batch',
                 request_serializer=key__value__db__pb2.BatchedGetRequest.SerializeToString,
                 response_deserializer=key__value__db__pb2.BatchedGetResponse.FromString,
                 )
 
 
 class KeyValueDBServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -132,15 +132,15 @@
             'get_batch': grpc.unary_unary_rpc_method_handler(
                     servicer.get_batch,
                     request_deserializer=key__value__db__pb2.BatchedGetRequest.FromString,
                     response_serializer=key__value__db__pb2.BatchedGetResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'cognica.rpc.db.kv.KeyValueDBService', rpc_method_handlers)
+            'aeca.rpc.db.kv.KeyValueDBService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class KeyValueDBService(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -151,15 +151,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.kv.KeyValueDBService/put',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.kv.KeyValueDBService/put',
             key__value__db__pb2.PutRequest.SerializeToString,
             key__value__db__pb2.PutResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def remove(request,
@@ -168,15 +168,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.kv.KeyValueDBService/remove',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.kv.KeyValueDBService/remove',
             key__value__db__pb2.RemoveRequest.SerializeToString,
             key__value__db__pb2.RemoveResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get(request,
@@ -185,15 +185,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.kv.KeyValueDBService/get',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.kv.KeyValueDBService/get',
             key__value__db__pb2.GetRequest.SerializeToString,
             key__value__db__pb2.GetResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def mget(request,
@@ -202,15 +202,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.kv.KeyValueDBService/mget',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.kv.KeyValueDBService/mget',
             key__value__db__pb2.MultiGetRequest.SerializeToString,
             key__value__db__pb2.MultiGetResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def put_batch(request,
@@ -219,15 +219,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.kv.KeyValueDBService/put_batch',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.kv.KeyValueDBService/put_batch',
             key__value__db__pb2.BatchedPutRequest.SerializeToString,
             key__value__db__pb2.BatchedPutResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def remove_batch(request,
@@ -236,15 +236,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.kv.KeyValueDBService/remove_batch',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.kv.KeyValueDBService/remove_batch',
             key__value__db__pb2.BatchedRemoveRequest.SerializeToString,
             key__value__db__pb2.BatchedRemoveResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get_batch(request,
@@ -253,15 +253,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.kv.KeyValueDBService/get_batch',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.kv.KeyValueDBService/get_batch',
             key__value__db__pb2.BatchedGetRequest.SerializeToString,
             key__value__db__pb2.BatchedGetResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
 
 class KeyspaceManagerServiceStub(object):
@@ -270,30 +270,30 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.create_keyspace = channel.unary_unary(
-                '/cognica.rpc.db.kv.KeyspaceManagerService/create_keyspace',
+                '/aeca.rpc.db.kv.KeyspaceManagerService/create_keyspace',
                 request_serializer=key__value__db__pb2.CreateKeyspaceRequest.SerializeToString,
                 response_deserializer=key__value__db__pb2.CreateKeyspaceResponse.FromString,
                 )
         self.drop_keyspace = channel.unary_unary(
-                '/cognica.rpc.db.kv.KeyspaceManagerService/drop_keyspace',
+                '/aeca.rpc.db.kv.KeyspaceManagerService/drop_keyspace',
                 request_serializer=key__value__db__pb2.DropKeyspaceRequest.SerializeToString,
                 response_deserializer=key__value__db__pb2.DropKeyspaceResponse.FromString,
                 )
         self.truncate_keyspace = channel.unary_unary(
-                '/cognica.rpc.db.kv.KeyspaceManagerService/truncate_keyspace',
+                '/aeca.rpc.db.kv.KeyspaceManagerService/truncate_keyspace',
                 request_serializer=key__value__db__pb2.TruncateKeyspaceRequest.SerializeToString,
                 response_deserializer=key__value__db__pb2.TruncateKeyspaceResponse.FromString,
                 )
         self.list_keyspaces = channel.unary_unary(
-                '/cognica.rpc.db.kv.KeyspaceManagerService/list_keyspaces',
+                '/aeca.rpc.db.kv.KeyspaceManagerService/list_keyspaces',
                 request_serializer=key__value__db__pb2.ListKeyspacesRequest.SerializeToString,
                 response_deserializer=key__value__db__pb2.ListKeyspacesResponse.FromString,
                 )
 
 
 class KeyspaceManagerServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -343,15 +343,15 @@
             'list_keyspaces': grpc.unary_unary_rpc_method_handler(
                     servicer.list_keyspaces,
                     request_deserializer=key__value__db__pb2.ListKeyspacesRequest.FromString,
                     response_serializer=key__value__db__pb2.ListKeyspacesResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'cognica.rpc.db.kv.KeyspaceManagerService', rpc_method_handlers)
+            'aeca.rpc.db.kv.KeyspaceManagerService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class KeyspaceManagerService(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -362,15 +362,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.kv.KeyspaceManagerService/create_keyspace',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.kv.KeyspaceManagerService/create_keyspace',
             key__value__db__pb2.CreateKeyspaceRequest.SerializeToString,
             key__value__db__pb2.CreateKeyspaceResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def drop_keyspace(request,
@@ -379,15 +379,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.kv.KeyspaceManagerService/drop_keyspace',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.kv.KeyspaceManagerService/drop_keyspace',
             key__value__db__pb2.DropKeyspaceRequest.SerializeToString,
             key__value__db__pb2.DropKeyspaceResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def truncate_keyspace(request,
@@ -396,15 +396,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.kv.KeyspaceManagerService/truncate_keyspace',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.kv.KeyspaceManagerService/truncate_keyspace',
             key__value__db__pb2.TruncateKeyspaceRequest.SerializeToString,
             key__value__db__pb2.TruncateKeyspaceResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def list_keyspaces(request,
@@ -413,12 +413,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.db.kv.KeyspaceManagerService/list_keyspaces',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.db.kv.KeyspaceManagerService/list_keyspaces',
             key__value__db__pb2.ListKeyspacesRequest.SerializeToString,
             key__value__db__pb2.ListKeyspacesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `aeca-0.1.15.dev2/src/aeca/protobuf/sentence_transformer_pb2.py` & `aeca-1.0.0.dev1/src/aeca/protobuf/sentence_transformer_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,54 +10,54 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1asentence_transformer.proto\x12 cognica.rpc.sentence_transformer\"$\n\x06Tensor\x12\x0c\n\x04\x64ims\x18\x01 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\x02\"\"\n\x0bProfileInfo\x12\x13\n\x0b\x64uration_us\x18\x01 \x01(\x04\"?\n\x16SentenceEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x11\n\tsentences\x18\x02 \x03(\t\"\xe7\x01\n\x17SentenceEncoderResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.cognica.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x39\n\x07tensors\x18\x03 \x03(\x0b\x32(.cognica.rpc.sentence_transformer.Tensor\x12?\n\x08profiles\x18\x04 \x03(\x0b\x32-.cognica.rpc.sentence_transformer.ProfileInfo\"4\n\x0cSentencePair\x12\x11\n\tsentence1\x18\x01 \x01(\t\x12\x11\n\tsentence2\x18\x02 \x01(\t\"l\n\x13\x43rossEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x41\n\tsentences\x18\x02 \x03(\x0b\x32..cognica.rpc.sentence_transformer.SentencePair\"\xb9\x01\n\x14\x43rossEncoderResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.cognica.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x0e\n\x06scores\x18\x03 \x03(\x02\x12?\n\x08profiles\x18\x04 \x03(\x0b\x32-.cognica.rpc.sentence_transformer.ProfileInfo\"\xb0\x01\n\x12\x43LIPEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12P\n\x06\x66ormat\x18\x02 \x01(\x0e\x32@.cognica.rpc.sentence_transformer.CLIPEncoderRequest.InputFormat\x12\x0e\n\x06inputs\x18\x03 \x03(\x0c\"$\n\x0bInputFormat\x12\t\n\x05kText\x10\x00\x12\n\n\x06kImage\x10\x01\"\xe3\x01\n\x13\x43LIPEncoderResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.cognica.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x39\n\x07tensors\x18\x03 \x03(\x0b\x32(.cognica.rpc.sentence_transformer.Tensor\x12?\n\x08profiles\x18\x04 \x03(\x0b\x32-.cognica.rpc.sentence_transformer.ProfileInfo\"Z\n\x10QAEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x11\n\tquestions\x18\x02 \x03(\t\x12\x10\n\x08\x63ontexts\x18\x03 \x03(\t\x12\r\n\x05top_k\x18\x04 \x01(\x05\"\xa6\x03\n\x11QAEncoderResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.cognica.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12R\n\x07\x61nswers\x18\x03 \x03(\x0b\x32\x41.cognica.rpc.sentence_transformer.QAEncoderResponse.CandidateList\x12?\n\x08profiles\x18\x04 \x03(\x0b\x32-.cognica.rpc.sentence_transformer.ProfileInfo\x1a\x46\n\tCandidate\x12\r\n\x05score\x18\x01 \x01(\x02\x12\r\n\x05\x62\x65gin\x18\x02 \x01(\x05\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x05\x12\x0e\n\x06\x61nswer\x18\x04 \x01(\t\x1a\x62\n\rCandidateList\x12Q\n\ncandidates\x18\x01 \x03(\x0b\x32=.cognica.rpc.sentence_transformer.QAEncoderResponse.Candidate*3\n\nStatusType\x12\x07\n\x03kOK\x10\x00\x12\r\n\tkNotFound\x10\x01\x12\r\n\tkInternal\x10\n2\x9d\x01\n\x1aSentenceTransformerService\x12\x7f\n\x06\x65ncode\x12\x38.cognica.rpc.sentence_transformer.SentenceEncoderRequest\x1a\x39.cognica.rpc.sentence_transformer.SentenceEncoderResponse\"\x00\x32\x91\x01\n\x13\x43rossEncoderService\x12z\n\x07predict\x12\x35.cognica.rpc.sentence_transformer.CrossEncoderRequest\x1a\x36.cognica.rpc.sentence_transformer.CrossEncoderResponse\"\x00\x32\x8d\x01\n\x12\x43LIPEncoderService\x12w\n\x06\x65ncode\x12\x34.cognica.rpc.sentence_transformer.CLIPEncoderRequest\x1a\x35.cognica.rpc.sentence_transformer.CLIPEncoderResponse\"\x00\x32\x88\x01\n\x10QAEncoderService\x12t\n\x07predict\x12\x32.cognica.rpc.sentence_transformer.QAEncoderRequest\x1a\x33.cognica.rpc.sentence_transformer.QAEncoderResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1asentence_transformer.proto\x12\x1d\x61\x65\x63\x61.rpc.sentence_transformer\"$\n\x06Tensor\x12\x0c\n\x04\x64ims\x18\x01 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\x02\"\"\n\x0bProfileInfo\x12\x13\n\x0b\x64uration_us\x18\x01 \x01(\x04\"?\n\x16SentenceEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x11\n\tsentences\x18\x02 \x03(\t\"\xde\x01\n\x17SentenceEncoderResponse\x12\x39\n\x06status\x18\x01 \x01(\x0e\x32).aeca.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x36\n\x07tensors\x18\x03 \x03(\x0b\x32%.aeca.rpc.sentence_transformer.Tensor\x12<\n\x08profiles\x18\x04 \x03(\x0b\x32*.aeca.rpc.sentence_transformer.ProfileInfo\"4\n\x0cSentencePair\x12\x11\n\tsentence1\x18\x01 \x01(\t\x12\x11\n\tsentence2\x18\x02 \x01(\t\"i\n\x13\x43rossEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12>\n\tsentences\x18\x02 \x03(\x0b\x32+.aeca.rpc.sentence_transformer.SentencePair\"\xb3\x01\n\x14\x43rossEncoderResponse\x12\x39\n\x06status\x18\x01 \x01(\x0e\x32).aeca.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x0e\n\x06scores\x18\x03 \x03(\x02\x12<\n\x08profiles\x18\x04 \x03(\x0b\x32*.aeca.rpc.sentence_transformer.ProfileInfo\"\xad\x01\n\x12\x43LIPEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12M\n\x06\x66ormat\x18\x02 \x01(\x0e\x32=.aeca.rpc.sentence_transformer.CLIPEncoderRequest.InputFormat\x12\x0e\n\x06inputs\x18\x03 \x03(\x0c\"$\n\x0bInputFormat\x12\t\n\x05kText\x10\x00\x12\n\n\x06kImage\x10\x01\"\xda\x01\n\x13\x43LIPEncoderResponse\x12\x39\n\x06status\x18\x01 \x01(\x0e\x32).aeca.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x36\n\x07tensors\x18\x03 \x03(\x0b\x32%.aeca.rpc.sentence_transformer.Tensor\x12<\n\x08profiles\x18\x04 \x03(\x0b\x32*.aeca.rpc.sentence_transformer.ProfileInfo\"Z\n\x10QAEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x11\n\tquestions\x18\x02 \x03(\t\x12\x10\n\x08\x63ontexts\x18\x03 \x03(\t\x12\r\n\x05top_k\x18\x04 \x01(\x05\"\x9a\x03\n\x11QAEncoderResponse\x12\x39\n\x06status\x18\x01 \x01(\x0e\x32).aeca.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12O\n\x07\x61nswers\x18\x03 \x03(\x0b\x32>.aeca.rpc.sentence_transformer.QAEncoderResponse.CandidateList\x12<\n\x08profiles\x18\x04 \x03(\x0b\x32*.aeca.rpc.sentence_transformer.ProfileInfo\x1a\x46\n\tCandidate\x12\r\n\x05score\x18\x01 \x01(\x02\x12\r\n\x05\x62\x65gin\x18\x02 \x01(\x05\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x05\x12\x0e\n\x06\x61nswer\x18\x04 \x01(\t\x1a_\n\rCandidateList\x12N\n\ncandidates\x18\x01 \x03(\x0b\x32:.aeca.rpc.sentence_transformer.QAEncoderResponse.Candidate*3\n\nStatusType\x12\x07\n\x03kOK\x10\x00\x12\r\n\tkNotFound\x10\x01\x12\r\n\tkInternal\x10\n2\x97\x01\n\x1aSentenceTransformerService\x12y\n\x06\x65ncode\x12\x35.aeca.rpc.sentence_transformer.SentenceEncoderRequest\x1a\x36.aeca.rpc.sentence_transformer.SentenceEncoderResponse\"\x00\x32\x8b\x01\n\x13\x43rossEncoderService\x12t\n\x07predict\x12\x32.aeca.rpc.sentence_transformer.CrossEncoderRequest\x1a\x33.aeca.rpc.sentence_transformer.CrossEncoderResponse\"\x00\x32\x87\x01\n\x12\x43LIPEncoderService\x12q\n\x06\x65ncode\x12\x31.aeca.rpc.sentence_transformer.CLIPEncoderRequest\x1a\x32.aeca.rpc.sentence_transformer.CLIPEncoderResponse\"\x00\x32\x82\x01\n\x10QAEncoderService\x12n\n\x07predict\x12/.aeca.rpc.sentence_transformer.QAEncoderRequest\x1a\x30.aeca.rpc.sentence_transformer.QAEncoderResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentence_transformer_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\370\001\001'
-  _globals['_STATUSTYPE']._serialized_start=1715
-  _globals['_STATUSTYPE']._serialized_end=1766
-  _globals['_TENSOR']._serialized_start=64
-  _globals['_TENSOR']._serialized_end=100
-  _globals['_PROFILEINFO']._serialized_start=102
-  _globals['_PROFILEINFO']._serialized_end=136
-  _globals['_SENTENCEENCODERREQUEST']._serialized_start=138
-  _globals['_SENTENCEENCODERREQUEST']._serialized_end=201
-  _globals['_SENTENCEENCODERRESPONSE']._serialized_start=204
-  _globals['_SENTENCEENCODERRESPONSE']._serialized_end=435
-  _globals['_SENTENCEPAIR']._serialized_start=437
-  _globals['_SENTENCEPAIR']._serialized_end=489
-  _globals['_CROSSENCODERREQUEST']._serialized_start=491
-  _globals['_CROSSENCODERREQUEST']._serialized_end=599
-  _globals['_CROSSENCODERRESPONSE']._serialized_start=602
-  _globals['_CROSSENCODERRESPONSE']._serialized_end=787
-  _globals['_CLIPENCODERREQUEST']._serialized_start=790
-  _globals['_CLIPENCODERREQUEST']._serialized_end=966
-  _globals['_CLIPENCODERREQUEST_INPUTFORMAT']._serialized_start=930
-  _globals['_CLIPENCODERREQUEST_INPUTFORMAT']._serialized_end=966
-  _globals['_CLIPENCODERRESPONSE']._serialized_start=969
-  _globals['_CLIPENCODERRESPONSE']._serialized_end=1196
-  _globals['_QAENCODERREQUEST']._serialized_start=1198
-  _globals['_QAENCODERREQUEST']._serialized_end=1288
-  _globals['_QAENCODERRESPONSE']._serialized_start=1291
-  _globals['_QAENCODERRESPONSE']._serialized_end=1713
-  _globals['_QAENCODERRESPONSE_CANDIDATE']._serialized_start=1543
-  _globals['_QAENCODERRESPONSE_CANDIDATE']._serialized_end=1613
-  _globals['_QAENCODERRESPONSE_CANDIDATELIST']._serialized_start=1615
-  _globals['_QAENCODERRESPONSE_CANDIDATELIST']._serialized_end=1713
-  _globals['_SENTENCETRANSFORMERSERVICE']._serialized_start=1769
-  _globals['_SENTENCETRANSFORMERSERVICE']._serialized_end=1926
-  _globals['_CROSSENCODERSERVICE']._serialized_start=1929
-  _globals['_CROSSENCODERSERVICE']._serialized_end=2074
-  _globals['_CLIPENCODERSERVICE']._serialized_start=2077
-  _globals['_CLIPENCODERSERVICE']._serialized_end=2218
-  _globals['_QAENCODERSERVICE']._serialized_start=2221
-  _globals['_QAENCODERSERVICE']._serialized_end=2357
+  _globals['_STATUSTYPE']._serialized_start=1670
+  _globals['_STATUSTYPE']._serialized_end=1721
+  _globals['_TENSOR']._serialized_start=61
+  _globals['_TENSOR']._serialized_end=97
+  _globals['_PROFILEINFO']._serialized_start=99
+  _globals['_PROFILEINFO']._serialized_end=133
+  _globals['_SENTENCEENCODERREQUEST']._serialized_start=135
+  _globals['_SENTENCEENCODERREQUEST']._serialized_end=198
+  _globals['_SENTENCEENCODERRESPONSE']._serialized_start=201
+  _globals['_SENTENCEENCODERRESPONSE']._serialized_end=423
+  _globals['_SENTENCEPAIR']._serialized_start=425
+  _globals['_SENTENCEPAIR']._serialized_end=477
+  _globals['_CROSSENCODERREQUEST']._serialized_start=479
+  _globals['_CROSSENCODERREQUEST']._serialized_end=584
+  _globals['_CROSSENCODERRESPONSE']._serialized_start=587
+  _globals['_CROSSENCODERRESPONSE']._serialized_end=766
+  _globals['_CLIPENCODERREQUEST']._serialized_start=769
+  _globals['_CLIPENCODERREQUEST']._serialized_end=942
+  _globals['_CLIPENCODERREQUEST_INPUTFORMAT']._serialized_start=906
+  _globals['_CLIPENCODERREQUEST_INPUTFORMAT']._serialized_end=942
+  _globals['_CLIPENCODERRESPONSE']._serialized_start=945
+  _globals['_CLIPENCODERRESPONSE']._serialized_end=1163
+  _globals['_QAENCODERREQUEST']._serialized_start=1165
+  _globals['_QAENCODERREQUEST']._serialized_end=1255
+  _globals['_QAENCODERRESPONSE']._serialized_start=1258
+  _globals['_QAENCODERRESPONSE']._serialized_end=1668
+  _globals['_QAENCODERRESPONSE_CANDIDATE']._serialized_start=1501
+  _globals['_QAENCODERRESPONSE_CANDIDATE']._serialized_end=1571
+  _globals['_QAENCODERRESPONSE_CANDIDATELIST']._serialized_start=1573
+  _globals['_QAENCODERRESPONSE_CANDIDATELIST']._serialized_end=1668
+  _globals['_SENTENCETRANSFORMERSERVICE']._serialized_start=1724
+  _globals['_SENTENCETRANSFORMERSERVICE']._serialized_end=1875
+  _globals['_CROSSENCODERSERVICE']._serialized_start=1878
+  _globals['_CROSSENCODERSERVICE']._serialized_end=2017
+  _globals['_CLIPENCODERSERVICE']._serialized_start=2020
+  _globals['_CLIPENCODERSERVICE']._serialized_end=2155
+  _globals['_QAENCODERSERVICE']._serialized_start=2158
+  _globals['_QAENCODERSERVICE']._serialized_end=2288
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aeca-0.1.15.dev2/src/aeca/protobuf/sentence_transformer_pb2_grpc.py` & `aeca-1.0.0.dev1/src/aeca/protobuf/sentence_transformer_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.encode = channel.unary_unary(
-                '/cognica.rpc.sentence_transformer.SentenceTransformerService/encode',
+                '/aeca.rpc.sentence_transformer.SentenceTransformerService/encode',
                 request_serializer=sentence__transformer__pb2.SentenceEncoderRequest.SerializeToString,
                 response_deserializer=sentence__transformer__pb2.SentenceEncoderResponse.FromString,
                 )
 
 
 class SentenceTransformerServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -36,15 +36,15 @@
             'encode': grpc.unary_unary_rpc_method_handler(
                     servicer.encode,
                     request_deserializer=sentence__transformer__pb2.SentenceEncoderRequest.FromString,
                     response_serializer=sentence__transformer__pb2.SentenceEncoderResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'cognica.rpc.sentence_transformer.SentenceTransformerService', rpc_method_handlers)
+            'aeca.rpc.sentence_transformer.SentenceTransformerService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class SentenceTransformerService(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -55,15 +55,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.sentence_transformer.SentenceTransformerService/encode',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.sentence_transformer.SentenceTransformerService/encode',
             sentence__transformer__pb2.SentenceEncoderRequest.SerializeToString,
             sentence__transformer__pb2.SentenceEncoderResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
 
 class CrossEncoderServiceStub(object):
@@ -72,15 +72,15 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.predict = channel.unary_unary(
-                '/cognica.rpc.sentence_transformer.CrossEncoderService/predict',
+                '/aeca.rpc.sentence_transformer.CrossEncoderService/predict',
                 request_serializer=sentence__transformer__pb2.CrossEncoderRequest.SerializeToString,
                 response_deserializer=sentence__transformer__pb2.CrossEncoderResponse.FromString,
                 )
 
 
 class CrossEncoderServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -97,15 +97,15 @@
             'predict': grpc.unary_unary_rpc_method_handler(
                     servicer.predict,
                     request_deserializer=sentence__transformer__pb2.CrossEncoderRequest.FromString,
                     response_serializer=sentence__transformer__pb2.CrossEncoderResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'cognica.rpc.sentence_transformer.CrossEncoderService', rpc_method_handlers)
+            'aeca.rpc.sentence_transformer.CrossEncoderService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class CrossEncoderService(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -116,15 +116,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.sentence_transformer.CrossEncoderService/predict',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.sentence_transformer.CrossEncoderService/predict',
             sentence__transformer__pb2.CrossEncoderRequest.SerializeToString,
             sentence__transformer__pb2.CrossEncoderResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
 
 class CLIPEncoderServiceStub(object):
@@ -133,15 +133,15 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.encode = channel.unary_unary(
-                '/cognica.rpc.sentence_transformer.CLIPEncoderService/encode',
+                '/aeca.rpc.sentence_transformer.CLIPEncoderService/encode',
                 request_serializer=sentence__transformer__pb2.CLIPEncoderRequest.SerializeToString,
                 response_deserializer=sentence__transformer__pb2.CLIPEncoderResponse.FromString,
                 )
 
 
 class CLIPEncoderServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -158,15 +158,15 @@
             'encode': grpc.unary_unary_rpc_method_handler(
                     servicer.encode,
                     request_deserializer=sentence__transformer__pb2.CLIPEncoderRequest.FromString,
                     response_serializer=sentence__transformer__pb2.CLIPEncoderResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'cognica.rpc.sentence_transformer.CLIPEncoderService', rpc_method_handlers)
+            'aeca.rpc.sentence_transformer.CLIPEncoderService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class CLIPEncoderService(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -177,15 +177,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.sentence_transformer.CLIPEncoderService/encode',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.sentence_transformer.CLIPEncoderService/encode',
             sentence__transformer__pb2.CLIPEncoderRequest.SerializeToString,
             sentence__transformer__pb2.CLIPEncoderResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
 
 class QAEncoderServiceStub(object):
@@ -194,15 +194,15 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.predict = channel.unary_unary(
-                '/cognica.rpc.sentence_transformer.QAEncoderService/predict',
+                '/aeca.rpc.sentence_transformer.QAEncoderService/predict',
                 request_serializer=sentence__transformer__pb2.QAEncoderRequest.SerializeToString,
                 response_deserializer=sentence__transformer__pb2.QAEncoderResponse.FromString,
                 )
 
 
 class QAEncoderServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -219,15 +219,15 @@
             'predict': grpc.unary_unary_rpc_method_handler(
                     servicer.predict,
                     request_deserializer=sentence__transformer__pb2.QAEncoderRequest.FromString,
                     response_serializer=sentence__transformer__pb2.QAEncoderResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'cognica.rpc.sentence_transformer.QAEncoderService', rpc_method_handlers)
+            'aeca.rpc.sentence_transformer.QAEncoderService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class QAEncoderService(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -238,12 +238,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/cognica.rpc.sentence_transformer.QAEncoderService/predict',
+        return grpc.experimental.unary_unary(request, target, '/aeca.rpc.sentence_transformer.QAEncoderService/predict',
             sentence__transformer__pb2.QAEncoderRequest.SerializeToString,
             sentence__transformer__pb2.QAEncoderResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `aeca-0.1.15.dev2/src/aeca/sentence_transformer.py` & `aeca-1.0.0.dev1/src/aeca/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `aeca-0.1.15.dev2/src/aeca.egg-info/PKG-INFO` & `aeca-1.0.0.dev1/src/aeca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeca
-Version: 0.1.15.dev2
+Version: 1.0.0.dev1
 Summary: Python client for Aeca database
 Author-email: "Aeca, Inc." <jaepil@aeca.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -226,16 +226,14 @@
 Requires-Dist: polars>=0.16.18
 Requires-Dist: pyarrow>=11.0.0
 Requires-Dist: grpcio>=1.53.0
 Requires-Dist: protobuf>=4.22.1
 Requires-Dist: pillow
 Provides-Extra: protobuf
 Requires-Dist: grpcio>=1.43.0; extra == "protobuf"
-Provides-Extra: server
-Requires-Dist: cognica-server; extra == "server"
 
 # Aeca Python Client
 
 A Python client for Aeca database server.
 
 ## Installation
```

### Comparing `aeca-0.1.15.dev2/src/aeca.egg-info/SOURCES.txt` & `aeca-1.0.0.dev1/src/aeca.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 src/aeca/protobuf/document_db_pb2_grpc.py
 src/aeca/protobuf/document_pb2.py
 src/aeca/protobuf/fts_analysis_pipeline_pb2.py
 src/aeca/protobuf/fts_analysis_pipeline_pb2_grpc.py
 src/aeca/protobuf/key_value_db_pb2.py
 src/aeca/protobuf/key_value_db_pb2_grpc.py
 src/aeca/protobuf/sentence_transformer_pb2.py
-src/aeca/protobuf/sentence_transformer_pb2_grpc.py
+src/aeca/protobuf/sentence_transformer_pb2_grpc.py
+src/aeca/protobuf/workspaces_pb2.py
+src/aeca/protobuf/workspaces_pb2_grpc.py
```

