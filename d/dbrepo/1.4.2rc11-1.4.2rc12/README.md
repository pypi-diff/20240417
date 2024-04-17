# Comparing `tmp/dbrepo-1.4.2rc11.tar.gz` & `tmp/dbrepo-1.4.2rc12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbrepo-1.4.2rc11.tar", last modified: Wed Apr 10 10:37:46 2024, max compression
+gzip compressed data, was "dbrepo-1.4.2rc12.tar", last modified: Wed Apr 17 14:04:58 2024, max compression
```

## Comparing `dbrepo-1.4.2rc11.tar` & `dbrepo-1.4.2rc12.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc11/LICENSE
--rw-r--r--   0 mweise    (1000) mweise    (1000)    18900 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)     4814 2024-04-10 10:31:38.000000 dbrepo-1.4.2rc11/README.md
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/dbrepo/
--rw-r--r--   0 mweise    (1000) mweise    (1000)     2940 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/dbrepo/AmqpClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    75175 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/dbrepo/RestClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1609 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/dbrepo/UploadClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc11/dbrepo/__init__.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/dbrepo/api/
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc11/dbrepo/api/__init__.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    21274 2024-04-09 15:48:25.000000 dbrepo-1.4.2rc11/dbrepo/api/dto.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc11/dbrepo/api/exceptions.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/dbrepo.egg-info/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    18900 2024-04-10 10:37:46.000000 dbrepo-1.4.2rc11/dbrepo.egg-info/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)      560 2024-04-10 10:37:46.000000 dbrepo-1.4.2rc11/dbrepo.egg-info/SOURCES.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-04-10 10:37:46.000000 dbrepo-1.4.2rc11/dbrepo.egg-info/dependency_links.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)       42 2024-04-10 10:37:46.000000 dbrepo-1.4.2rc11/dbrepo.egg-info/requires.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-04-10 10:37:46.000000 dbrepo-1.4.2rc11/dbrepo.egg-info/top_level.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1103 2024-04-10 10:37:18.000000 dbrepo-1.4.2rc11/pyproject.toml
--rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/setup.cfg
--rw-r--r--   0 mweise    (1000) mweise    (1000)      411 2024-04-10 10:37:18.000000 dbrepo-1.4.2rc11/setup.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/tests/
--rw-r--r--   0 mweise    (1000) mweise    (1000)      729 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_analyse.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     5565 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_container.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    26166 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_database.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11310 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_identifier.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-09 16:08:11.000000 dbrepo-1.4.2rc11/tests/test_license.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    14639 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_query.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1308 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc11/tests/test_rest_client.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    29497 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_table.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    14697 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_user.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11997 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_view.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-17 14:04:58.919491 dbrepo-1.4.2rc12/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc12/LICENSE
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18900 2024-04-17 14:04:58.919491 dbrepo-1.4.2rc12/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     4814 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc12/README.md
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-17 14:04:58.919491 dbrepo-1.4.2rc12/dbrepo/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     2940 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc12/dbrepo/AmqpClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    75175 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc12/dbrepo/RestClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1609 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc12/dbrepo/UploadClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc12/dbrepo/__init__.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-17 14:04:58.919491 dbrepo-1.4.2rc12/dbrepo/api/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc12/dbrepo/api/__init__.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    21318 2024-04-17 14:03:28.000000 dbrepo-1.4.2rc12/dbrepo/api/dto.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      368 2024-04-16 09:59:53.000000 dbrepo-1.4.2rc12/dbrepo/api/encoder.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc12/dbrepo/api/exceptions.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-17 14:04:58.919491 dbrepo-1.4.2rc12/dbrepo.egg-info/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18900 2024-04-17 14:04:58.000000 dbrepo-1.4.2rc12/dbrepo.egg-info/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      582 2024-04-17 14:04:58.000000 dbrepo-1.4.2rc12/dbrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-04-17 14:04:58.000000 dbrepo-1.4.2rc12/dbrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       42 2024-04-17 14:04:58.000000 dbrepo-1.4.2rc12/dbrepo.egg-info/requires.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-04-17 14:04:58.000000 dbrepo-1.4.2rc12/dbrepo.egg-info/top_level.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1103 2024-04-17 14:04:56.000000 dbrepo-1.4.2rc12/pyproject.toml
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-04-17 14:04:58.919491 dbrepo-1.4.2rc12/setup.cfg
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      411 2024-04-17 14:04:56.000000 dbrepo-1.4.2rc12/setup.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-17 14:04:58.919491 dbrepo-1.4.2rc12/tests/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      729 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc12/tests/test_analyse.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     5565 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc12/tests/test_container.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    26166 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc12/tests/test_database.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11310 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc12/tests/test_identifier.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc12/tests/test_license.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14639 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc12/tests/test_query.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1308 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc12/tests/test_rest_client.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    29497 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc12/tests/test_table.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14697 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc12/tests/test_user.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11997 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc12/tests/test_view.py
```

### Comparing `dbrepo-1.4.2rc11/LICENSE` & `dbrepo-1.4.2rc12/LICENSE`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/PKG-INFO` & `dbrepo-1.4.2rc12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.2rc11
+Version: 1.4.2rc12
 Summary: DBRepo Python Library
 Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `dbrepo-1.4.2rc11/README.md` & `dbrepo-1.4.2rc12/README.md`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/dbrepo/AmqpClient.py` & `dbrepo-1.4.2rc12/dbrepo/AmqpClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/dbrepo/RestClient.py` & `dbrepo-1.4.2rc12/dbrepo/RestClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/dbrepo/UploadClient.py` & `dbrepo-1.4.2rc12/dbrepo/UploadClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/dbrepo/api/dto.py` & `dbrepo-1.4.2rc12/dbrepo/api/dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 from dataclasses import field
 from enum import Enum
 import datetime
 from typing import List, Optional, Any, Annotated
 from pydantic import BaseModel, ConfigDict, PlainSerializer
 
 Timestamp = Annotated[
-    datetime.datetime, PlainSerializer(lambda v: v.isoformat(timespec='milliseconds'), return_type=str)
+    datetime.datetime, PlainSerializer(lambda v: v.strftime('%Y-%m-%dT%H:%M:%S.%f')[:-3] + 'Z', return_type=str)
 ]
 
+
 class ImageDate(BaseModel):
     id: int
     example: str
     database_format: str
     unix_format: str
     has_time: bool
     created_at: Timestamp
@@ -71,16 +72,16 @@
     id: int
     name: str
     internal_name: str
     host: str
     port: int
     image: Image
     created: Timestamp
-    sidecar_host: str
-    sidecar_port: int
+    sidecar_host: Optional[str] = None
+    sidecar_port: Optional[int] = None
     ui_host: Optional[str] = None
     ui_port: Optional[int] = None
 
 
 class ContainerBrief(BaseModel):
     id: int
     name: str
```

### Comparing `dbrepo-1.4.2rc11/dbrepo/api/exceptions.py` & `dbrepo-1.4.2rc12/dbrepo/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/dbrepo.egg-info/PKG-INFO` & `dbrepo-1.4.2rc12/dbrepo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.2rc11
+Version: 1.4.2rc12
 Summary: DBRepo Python Library
 Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `dbrepo-1.4.2rc11/dbrepo.egg-info/SOURCES.txt` & `dbrepo-1.4.2rc12/dbrepo.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 dbrepo.egg-info/PKG-INFO
 dbrepo.egg-info/SOURCES.txt
 dbrepo.egg-info/dependency_links.txt
 dbrepo.egg-info/requires.txt
 dbrepo.egg-info/top_level.txt
 dbrepo/api/__init__.py
 dbrepo/api/dto.py
+dbrepo/api/encoder.py
 dbrepo/api/exceptions.py
 tests/test_analyse.py
 tests/test_container.py
 tests/test_database.py
 tests/test_identifier.py
 tests/test_license.py
 tests/test_query.py
```

### Comparing `dbrepo-1.4.2rc11/pyproject.toml` & `dbrepo-1.4.2rc12/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbrepo"
-version = "1.4.2rc11"
+version = "1.4.2rc12"
 description = "DBRepo Python Library"
 keywords = [
     "DBRepo",
     "Database Repository"
 ]
 authors = [
     { name = "Martin Weise, TU Wien", email = "martin.weise@tuwien.ac.at" }
```

### Comparing `dbrepo-1.4.2rc11/tests/test_analyse.py` & `dbrepo-1.4.2rc12/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/tests/test_container.py` & `dbrepo-1.4.2rc12/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/tests/test_database.py` & `dbrepo-1.4.2rc12/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/tests/test_identifier.py` & `dbrepo-1.4.2rc12/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/tests/test_license.py` & `dbrepo-1.4.2rc12/tests/test_license.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/tests/test_query.py` & `dbrepo-1.4.2rc12/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/tests/test_rest_client.py` & `dbrepo-1.4.2rc12/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/tests/test_table.py` & `dbrepo-1.4.2rc12/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/tests/test_user.py` & `dbrepo-1.4.2rc12/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc11/tests/test_view.py` & `dbrepo-1.4.2rc12/tests/test_view.py`

 * *Files identical despite different names*

