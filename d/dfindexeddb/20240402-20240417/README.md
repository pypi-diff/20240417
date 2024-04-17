# Comparing `tmp/dfindexeddb-20240402.tar.gz` & `tmp/dfindexeddb-20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfindexeddb-20240402.tar", last modified: Mon Apr  1 20:21:05 2024, max compression
+gzip compressed data, was "dfindexeddb-20240417.tar", last modified: Wed Apr 17 13:09:16 2024, max compression
```

## Comparing `dfindexeddb-20240402.tar` & `dfindexeddb-20240417.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.455962 dfindexeddb-20240402/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-01 20:21:00.000000 dfindexeddb-20240402/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-01 20:21:00.000000 dfindexeddb-20240402/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18098 2024-04-01 20:21:05.455962 dfindexeddb-20240402/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-01 20:21:00.000000 dfindexeddb-20240402/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.447962 dfindexeddb-20240402/dfindexeddb/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.451962 dfindexeddb-20240402/dfindexeddb/indexeddb/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.451962 dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/blink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    44731 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    21902 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/v8.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.451962 dfindexeddb-20240402/dfindexeddb/indexeddb/firefox/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/firefox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.451962 dfindexeddb-20240402/dfindexeddb/indexeddb/safari/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/safari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.455962 dfindexeddb-20240402/dfindexeddb/leveldb/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/ldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-01 20:21:01.000000 dfindexeddb-20240402/dfindexeddb/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-01 20:21:01.000000 dfindexeddb-20240402/dfindexeddb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.455962 dfindexeddb-20240402/dfindexeddb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18098 2024-04-01 20:21:05.000000 dfindexeddb-20240402/dfindexeddb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-01 20:21:05.000000 dfindexeddb-20240402/dfindexeddb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:21:05.000000 dfindexeddb-20240402/dfindexeddb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-01 20:21:05.000000 dfindexeddb-20240402/dfindexeddb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-01 20:21:05.000000 dfindexeddb-20240402/dfindexeddb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 20:21:05.000000 dfindexeddb-20240402/dfindexeddb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-01 20:21:01.000000 dfindexeddb-20240402/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:21:05.455962 dfindexeddb-20240402/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 20:21:01.000000 dfindexeddb-20240402/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.124606 dfindexeddb-20240417/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 13:09:07.000000 dfindexeddb-20240417/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-17 13:09:07.000000 dfindexeddb-20240417/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19935 2024-04-17 13:09:16.124606 dfindexeddb-20240417/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-04-17 13:09:07.000000 dfindexeddb-20240417/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.120607 dfindexeddb-20240417/dfindexeddb/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.120607 dfindexeddb-20240417/dfindexeddb/indexeddb/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.124606 dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32122 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/blink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45079 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22102 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/v8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.124606 dfindexeddb-20240417/dfindexeddb/indexeddb/firefox/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/firefox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.124606 dfindexeddb-20240417/dfindexeddb/indexeddb/safari/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/safari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.124606 dfindexeddb-20240417/dfindexeddb/leveldb/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/ldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.124606 dfindexeddb-20240417/dfindexeddb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19935 2024-04-17 13:09:16.000000 dfindexeddb-20240417/dfindexeddb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-17 13:09:16.000000 dfindexeddb-20240417/dfindexeddb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:09:16.000000 dfindexeddb-20240417/dfindexeddb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-17 13:09:16.000000 dfindexeddb-20240417/dfindexeddb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 13:09:16.000000 dfindexeddb-20240417/dfindexeddb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 13:09:16.000000 dfindexeddb-20240417/dfindexeddb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-17 13:09:07.000000 dfindexeddb-20240417/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 13:09:16.124606 dfindexeddb-20240417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 13:09:07.000000 dfindexeddb-20240417/setup.py
```

### Comparing `dfindexeddb-20240402/LICENSE` & `dfindexeddb-20240417/LICENSE`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240402/PKG-INFO` & `dfindexeddb-20240417/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfindexeddb
-Version: 20240402
+Version: 20240417
 Summary: dfindexeddb is an experimental Python tool for performing digital forensic analysis of IndexedDB and leveldb files.
 Author-email: Syd Pleno <sydp@google.com>
 Maintainer-email: dfIndexeddb Developers <dfindexeddb-dev@googlegroups.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -279,22 +279,69 @@
 installation:
 
 
 ### IndexedDB
 
 ```
 $ dfindexeddb -h
-usage: dfindexeddb [-h] -s SOURCE [-o {json,jsonl,repr}]
+usage: dfindexeddb [-h] {db,ldb,log} ...
 
 A cli tool for parsing indexeddb files
 
+positional arguments:
+  {db,ldb,log}
+    db          Parse a directory as indexeddb.
+    ldb         Parse a ldb file as indexeddb.
+    log         Parse a log file as indexeddb.
+
+options:
+  -h, --help    show this help message and exit
+```
+
+To parse Indexeddb records from a LevelDB folder, use the following command:
+
+```
+dfindexeddb db -h
+usage: dfindexeddb db [-h] -s SOURCE [--use_manifest] [-o {json,jsonl,repr}]
+
 options:
   -h, --help            show this help message and exit
   -s SOURCE, --source SOURCE
                         The source leveldb folder
+  --use_manifest        Use manifest file to determine active/recovered records.
+  -o {json,jsonl,repr}, --output {json,jsonl,repr}
+                        Output format. Default is json
+```
+
+To parse Indexeddb records from a LevelDB ldb (.ldb) file, use the following 
+command:
+
+```
+dfindexeddb ldb -h
+usage: dfindexeddb ldb [-h] -s SOURCE [-o {json,jsonl,repr}]
+
+options:
+  -h, --help            show this help message and exit
+  -s SOURCE, --source SOURCE
+                        The source .ldb file.
+  -o {json,jsonl,repr}, --output {json,jsonl,repr}
+                        Output format. Default is json
+```
+
+To parse Indexeddb records from a LevelDB log (.log) file, use the following 
+command:
+
+```
+dfindexeddb log -h
+usage: dfindexeddb log [-h] -s SOURCE [-o {json,jsonl,repr}]
+
+options:
+  -h, --help            show this help message and exit
+  -s SOURCE, --source SOURCE
+                        The source .log file.
   -o {json,jsonl,repr}, --output {json,jsonl,repr}
                         Output format. Default is json
 ```
 
 ### LevelDB
 
 ```
@@ -310,14 +357,29 @@
     ldb                 Parse a leveldb table (.ldb) file.
     descriptor          Parse a leveldb descriptor (MANIFEST) file.
 
 options:
   -h, --help            show this help message and exit
 ```
 
+To parse records from a LevelDB folder, use the following command:
+
+```
+dfindexeddb db -h
+usage: dfindexeddb db [-h] -s SOURCE [--use_manifest] [-o {json,jsonl,repr}]
+
+options:
+  -h, --help            show this help message and exit
+  -s SOURCE, --source SOURCE
+                        The source leveldb folder
+  --use_manifest        Use manifest file to determine active/recovered records.
+  -o {json,jsonl,repr}, --output {json,jsonl,repr}
+                        Output format. Default is json
+```
+
 To parse records from a LevelDB log (.log) file, use the following command:
 
 ```
 $ dfleveldb log  -s SOURCE [-o {json,jsonl,repr}] [-t {blocks,physical_records,write_batches,parsed_internal_key}]
 
 options:
   -h, --help            show this help message and exit
```

### Comparing `dfindexeddb-20240402/README.md` & `dfindexeddb-20240417/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -57,22 +57,69 @@
 installation:
 
 
 ### IndexedDB
 
 ```
 $ dfindexeddb -h
-usage: dfindexeddb [-h] -s SOURCE [-o {json,jsonl,repr}]
+usage: dfindexeddb [-h] {db,ldb,log} ...
 
 A cli tool for parsing indexeddb files
 
+positional arguments:
+  {db,ldb,log}
+    db          Parse a directory as indexeddb.
+    ldb         Parse a ldb file as indexeddb.
+    log         Parse a log file as indexeddb.
+
+options:
+  -h, --help    show this help message and exit
+```
+
+To parse Indexeddb records from a LevelDB folder, use the following command:
+
+```
+dfindexeddb db -h
+usage: dfindexeddb db [-h] -s SOURCE [--use_manifest] [-o {json,jsonl,repr}]
+
 options:
   -h, --help            show this help message and exit
   -s SOURCE, --source SOURCE
                         The source leveldb folder
+  --use_manifest        Use manifest file to determine active/recovered records.
+  -o {json,jsonl,repr}, --output {json,jsonl,repr}
+                        Output format. Default is json
+```
+
+To parse Indexeddb records from a LevelDB ldb (.ldb) file, use the following 
+command:
+
+```
+dfindexeddb ldb -h
+usage: dfindexeddb ldb [-h] -s SOURCE [-o {json,jsonl,repr}]
+
+options:
+  -h, --help            show this help message and exit
+  -s SOURCE, --source SOURCE
+                        The source .ldb file.
+  -o {json,jsonl,repr}, --output {json,jsonl,repr}
+                        Output format. Default is json
+```
+
+To parse Indexeddb records from a LevelDB log (.log) file, use the following 
+command:
+
+```
+dfindexeddb log -h
+usage: dfindexeddb log [-h] -s SOURCE [-o {json,jsonl,repr}]
+
+options:
+  -h, --help            show this help message and exit
+  -s SOURCE, --source SOURCE
+                        The source .log file.
   -o {json,jsonl,repr}, --output {json,jsonl,repr}
                         Output format. Default is json
 ```
 
 ### LevelDB
 
 ```
@@ -88,14 +135,29 @@
     ldb                 Parse a leveldb table (.ldb) file.
     descriptor          Parse a leveldb descriptor (MANIFEST) file.
 
 options:
   -h, --help            show this help message and exit
 ```
 
+To parse records from a LevelDB folder, use the following command:
+
+```
+dfindexeddb db -h
+usage: dfindexeddb db [-h] -s SOURCE [--use_manifest] [-o {json,jsonl,repr}]
+
+options:
+  -h, --help            show this help message and exit
+  -s SOURCE, --source SOURCE
+                        The source leveldb folder
+  --use_manifest        Use manifest file to determine active/recovered records.
+  -o {json,jsonl,repr}, --output {json,jsonl,repr}
+                        Output format. Default is json
+```
+
 To parse records from a LevelDB log (.log) file, use the following command:
 
 ```
 $ dfleveldb log  -s SOURCE [-o {json,jsonl,repr}] [-t {blocks,physical_records,write_batches,parsed_internal_key}]
 
 options:
   -h, --help            show this help message and exit
```

### Comparing `dfindexeddb-20240402/dfindexeddb/__init__.py` & `dfindexeddb-20240417/dfindexeddb/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240402/dfindexeddb/errors.py` & `dfindexeddb-20240417/dfindexeddb/errors.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240402/dfindexeddb/indexeddb/__init__.py` & `dfindexeddb-20240417/dfindexeddb/indexeddb/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/__init__.py` & `dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/blink.py` & `dfindexeddb-20240417/dfindexeddb/leveldb/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,109 +8,109 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Parsers for blink javascript serialized objects."""
+"""Helper/utility classes for LevelDB."""
+from __future__ import annotations
 import io
-from typing import Any
+from typing import BinaryIO, Tuple, Type, TypeVar
 
+from dfindexeddb import errors
 from dfindexeddb import utils
-from dfindexeddb.indexeddb.chromium import definitions
-from dfindexeddb.indexeddb.chromium import v8
 
 
+class LevelDBDecoder(utils.StreamDecoder):
+  """A helper class to decode data types from LevelDB files."""
 
-class V8ScriptValueDecoder:
-  """A Blink V8 Serialized Script Value (SSV) decoder.
+  def DecodeBool(self) -> Tuple[int, bool]:
+    """Returns a Tuple of the offset of decoding and the bool value."""
+    offset, buffer = self.ReadBytes(1)
+    return offset, buffer[0] is not None
 
-  Attributes:
-    deserializer (v8.ValueDeserializer): the V8 value deserializer.
-    raw_data (bytes): the raw bytes containing the serialized javascript
-        value.
-    version (int): the blink version.
-  """
-  _MIN_VERSION_FOR_SEPARATE_ENVELOPE = 16
+  def DecodeString(self) -> Tuple[int, str]:
+    """Returns a tuple of the offset of decoding and the string value.
 
-  # As defined in trailer_reader.h
-  _MIN_WIRE_FORMAT_VERSION = 21
+    Raises:
+      errors.DecoderError: when the parsed string buffer is not even (i.e.
+          cannot be decoded as a UTF-16-BE string.
+    """
+    offset = self.stream.tell()
+    buffer = self.stream.read()
+    if len(buffer) % 2:
+      raise errors.DecoderError(
+          f'Odd number of bytes encountered at offset {offset}')
+    return offset, buffer.decode('utf-16-be')
+
+  def DecodeLengthPrefixedSlice(self) -> Tuple[int, bytes]:
+    """Returns a tuple of the offset of decoding and the byte 'slice'."""
+    offset, num_bytes = self.DecodeUint32Varint()
+    _, blob = self.ReadBytes(num_bytes)
+    return offset, blob
+
+  def DecodeBlobWithLength(self) -> Tuple[int, bytes]:
+    """Returns a tuple of a the offset of decoding and the binary blob."""
+    offset, num_bytes = self.DecodeUint64Varint()
+    _, blob = self.ReadBytes(num_bytes)
+    return offset, blob
+
+  def DecodeStringWithLength(self, encoding='utf-16-be') -> Tuple[int, str]:
+    """Returns a tuple of the offset of decoding and the string value."""
+    offset, length = self.DecodeUint64Varint()
+    _, buffer = self.ReadBytes(length*2)
+    return offset, buffer.decode(encoding=encoding)
 
-  def __init__(self, raw_data: bytes):
-    self.deserializer = None
-    self.raw_data = raw_data
-    self.version = 0
 
-  def _ReadVersionEnvelope(self) -> int:
-    """Reads the Blink version envelope.
+T = TypeVar('T')
 
-    Returns:
-      The number of bytes consumed reading the Blink version envelope or zero
-          if no blink envelope is detected.
-    """
-    if not self.raw_data:
-      return 0
 
-    decoder = utils.StreamDecoder(io.BytesIO(self.raw_data))
-    _, tag_value = decoder.DecodeUint8()
-    tag = definitions.BlinkSerializationTag(tag_value)
-    if tag != definitions.BlinkSerializationTag.VERSION:
-      return 0
-
-    _, version = decoder.DecodeUint32Varint()
-    if version < self._MIN_VERSION_FOR_SEPARATE_ENVELOPE:
-      return 0
-
-    consumed_bytes = decoder.stream.tell()
-
-    if version >= self._MIN_WIRE_FORMAT_VERSION:
-      trailer_offset_data_size = 1 + 8 + 4 # 1 + sizeof(uint64) + sizeof(uint32)
-      consumed_bytes += trailer_offset_data_size
-      if consumed_bytes >= len(self.raw_data):
-        return 0
-    return consumed_bytes
+class FromDecoderMixin:
+  """A mixin for parsing dataclass attributes using a LevelDBDecoder."""
 
-  def ReadTag(self) -> definitions.BlinkSerializationTag:
-    """Reads a blink serialization tag.
+  @classmethod
+  def FromDecoder(
+      cls: Type[T], decoder: LevelDBDecoder, base_offset: int = 0) -> T:
+    """Decodes a class type from the current position of a LevelDBDecoder.
+
+    Args:
+      decoder: the LevelDBDecoder.
+      base_offset: the base offset.
 
     Returns:
-      The blink serialization tag.
-    """
-    _, tag_value = self.deserializer.decoder.DecodeUint8()
-    return definitions.BlinkSerializationTag(tag_value)
-
-  def ReadHostObject(self) -> Any:
-    """Reads a host DOM object.
+      The class instance.
 
     Raises:
-      NotImplementedError: when called.
+      NotImplementedError if the child class does not implement this method.
     """
-    tag = self.ReadTag()
-    raise NotImplementedError(
-        f'V8ScriptValueDecoder.ReadHostObject - {tag.name}')
+    raise NotImplementedError
 
-  def Deserialize(self) -> Any:
-    """Deserializes a Blink SSV.
-
-    The serialization format has two 'envelopes'.
-    [version tag] [Blink version] [version tag] [v8 version] ...
+  @classmethod
+  def FromStream(
+      cls: Type[T], stream: BinaryIO, base_offset: int = 0) -> T:
+    """Decodes a class type from the current position of a binary stream.
+
+    Args:
+      stream: the binary stream.
+      base_offset: the base offset of the binary stream.
 
     Returns:
-      The deserialized script value.
+      The class instance.
     """
-    version_envelope_size = self._ReadVersionEnvelope()
-    self.deserializer = v8.ValueDeserializer(
-        io.BytesIO(self.raw_data[version_envelope_size:]), delegate=self)
-    v8_version = self.deserializer.ReadHeader()
-    if not self.version:
-      self.version = v8_version
-    return self.deserializer.ReadValue()
+    decoder = LevelDBDecoder(stream)
+    return cls.FromDecoder(decoder=decoder, base_offset=base_offset)
 
   @classmethod
-  def FromBytes(cls, data: bytes) -> Any:
-    """Deserializes a Blink SSV from the data array.
+  def FromBytes(
+      cls: Type[T], raw_data: bytes, base_offset: int = 0) -> T:
+    """Parses a class type from raw bytes.
+
+    Args:
+      raw_data: the raw data.
+      base_offset: the base offset of the raw data.
 
     Returns:
-      The deserialized script value.
+      The class instance.
     """
-    return cls(data).Deserialize()
+    stream = io.BytesIO(raw_data)
+    return cls.FromStream(stream=stream, base_offset=base_offset)
```

### Comparing `dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/definitions.py` & `dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/definitions.py`

 * *Files 23% similar despite different names*

```diff
@@ -137,18 +137,20 @@
   RTC_ENCODED_AUDIO_FRAME = ord('A')
   RTC_ENCODED_VIDEO_FRAME = ord('V')
   AUDIO_DATA = ord('a')
   VIDEO_FRAME = ord('v')
   ENCODED_AUDIO_CHUNK = ord('y')
   ENCODED_VIDEO_CHUNK = ord('z')
   CROP_TARGET = ord('c')
+  RESTRICTION_TARGET = ord('D')
   MEDIA_SOURCE_HANDLE = ord('S')
   DEPRECATED_DETECTED_BARCODE = ord('B')
   DEPRECATED_DETECTED_FACE = ord('F')
   DEPRECATED_DETECTED_TEXT = ord('t')
+  FENCED_FRAME_CONFIG = ord('C')
   DOM_EXCEPTION = ord('x')
   TRAILER_OFFSET = 0xFE
   VERSION = 0xFF
   TRAILER_REQUIRES_INTERFACES = 0xA0
 
 
 class CryptoKeyAlgorithm(IntEnum):
@@ -300,7 +302,71 @@
   SYNTAX_ERROR_PROTOTYPE = ord('S')
   TYPE_ERROR_PROTOTYPE = ord('T')
   URI_ERROR_PROTOTYPE = ord('U')
   MESSAGE = ord('m')
   CAUSE = ord('c')
   STACK = ord('s')
   END = ord('.')
+
+
+class ImageSerializationTag(IntEnum):
+  """Image Serialization tags."""
+  END = 0
+  PREDEFINED_COLOR_SPACE = 1
+  CANVAS_PIXEL_FORMAT = 2
+  IMAGE_DATA_STORAGE_FORMAT = 3
+  ORIGIN_CLEAN = 4
+  IS_PREMULTIPLIED = 5
+  CANVAS_OPACITY_MODE = 6
+  PARAMETRIC_COLOR_SPACE = 7
+  IMAGE_ORIENTATION = 8
+  LAST = IMAGE_ORIENTATION
+
+
+class SerializedPredefinedColorSpace(IntEnum):
+  """Serialized Predefined Color Space enumeration."""
+  LEGACY_OBSOLETE = 0
+  SRGB = 1
+  REC2020 = 2
+  P3 = 3
+  REC2100HLG = 4
+  REC2100PQ = 5
+  SRGB_LINEAR = 6
+  LAST = SRGB_LINEAR
+
+
+class SerializedPixelFormat(IntEnum):
+  """Serialized Pixel Format enumeration."""
+  NATIVE8_LEGACY_OBSOLETE = 0
+  F16 = 1
+  RGBA8 = 2
+  BGRA8 = 3
+  RGBX8 = 4
+  LAST = RGBX8
+
+
+class SerializedImageDataStorageFormat(IntEnum):
+  """The Serialized Image Data Storage Format."""
+  UINT8CLAMPED = 0
+  UINT16 = 1
+  FLOAT32 = 2
+  LAST = FLOAT32
+
+
+class SerializedOpacityMode(IntEnum):
+  """The Serialized Opacity Mode."""
+  KNONOPAQUE = 0
+  KOPAQUE = 1
+  KLAST = KOPAQUE
+
+
+class SerializedImageOrientation(IntEnum):
+  """The Serialized Image Orientation."""
+  TOP_LEFT = 0
+  TOP_RIGHT = 1
+  BOTTOM_RIGHT = 2
+  BOTTOM_LEFT = 3
+  LEFT_TOP = 4
+  RIGHT_TOP = 5
+  RIGHT_BOTTOM = 6
+  LEFT_BOTTOM = 7
+  LAST = LEFT_BOTTOM
```

### Comparing `dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/record.py` & `dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/record.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 from datetime import datetime
 import io
 from typing import Any, BinaryIO, Optional, Tuple, Type, TypeVar, Union
 
 from dfindexeddb import errors
 from dfindexeddb.indexeddb.chromium import blink
 from dfindexeddb.indexeddb.chromium import definitions
-from dfindexeddb.leveldb import ldb
-from dfindexeddb.leveldb import log
+from dfindexeddb.leveldb import record
 from dfindexeddb.leveldb import utils
 
 
 T = TypeVar('T')
 
 
 @dataclass
@@ -542,31 +541,31 @@
     offset, key_type = decoder.DecodeUint8()
     if key_type != definitions.GlobalMetadataKeyType.EARLIEST_SWEEP:
       raise errors.ParserError('Not a EarliestSweepKey')
     return cls(offset=base_offset + offset, key_prefix=key_prefix)
 
 
 @dataclass
-class EarlistCompactionTimeKey(BaseIndexedDBKey):
+class EarliestCompactionTimeKey(BaseIndexedDBKey):
   """An earliest compaction time IndexedDB key."""
 
   def DecodeValue(self, decoder: utils.LevelDBDecoder) -> int:
     """Decodes the earliest compaction time value."""
     _, data = decoder.ReadBytes()
     return int.from_bytes(data, byteorder='little', signed=False)
 
   @classmethod
   def FromDecoder(
       cls, decoder: utils.LevelDBDecoder, key_prefix: KeyPrefix,
       base_offset: int = 0
-  ) -> EarlistCompactionTimeKey:
+  ) -> EarliestCompactionTimeKey:
     """Decodes the earliest compaction time key."""
     offset, key_type = decoder.DecodeUint8()
     if key_type != definitions.GlobalMetadataKeyType.EARLIEST_COMPACTION_TIME:
-      raise errors.ParserError('Not a EarlistCompactionTimeKey')
+      raise errors.ParserError('Not a EarliestCompactionTimeKey')
     return cls(offset=base_offset + offset, key_prefix=key_prefix)
 
 
 @dataclass
 class ScopesPrefixKey(BaseIndexedDBKey):
   """A scopes prefix IndexedDB key."""
 
@@ -664,15 +663,15 @@
       definitions.GlobalMetadataKeyType
           .RECOVERY_BLOB_JOURNAL: RecoveryBlobJournalKey,
       definitions.GlobalMetadataKeyType
           .ACTIVE_BLOB_JOURNAL: ActiveBlobJournalKey,
       definitions.GlobalMetadataKeyType
           .EARLIEST_SWEEP: EarliestSweepKey,
       definitions.GlobalMetadataKeyType
-          .EARLIEST_COMPACTION_TIME: EarlistCompactionTimeKey,
+          .EARLIEST_COMPACTION_TIME: EarliestCompactionTimeKey,
       definitions.GlobalMetadataKeyType
           .SCOPES_PREFIX: ScopesPrefixKey,
       definitions.GlobalMetadataKeyType
           .DATABASE_FREE_LIST: DatabaseFreeListKey,
       definitions.GlobalMetadataKeyType
           .DATABASE_NAME: DatabaseNameKey}
 
@@ -688,15 +687,15 @@
       cls, decoder: utils.LevelDBDecoder, key_prefix: KeyPrefix,
       base_offset: int = 0
   ) -> Union[Type[ActiveBlobJournalKey],
              Type[DataVersionKey],
              Type[DatabaseFreeListKey],
              Type[DatabaseNameKey],
              Type[EarliestSweepKey],
-             Type[EarlistCompactionTimeKey],
+             Type[EarliestCompactionTimeKey],
              Type[MaxDatabaseIdKey],
              Type[RecoveryBlobJournalKey],
              Type[SchemaVersionKey],
              Type[ScopesPrefixKey]]:
     """Decodes the global metadata key.
 
     Raises:
@@ -968,15 +967,15 @@
   Attributes:
     unknown: an unknown integer (possibly a sequence number?).
     is_wrapped: True if the value was wrapped.
     blob_size: the blob size, only valid if wrapped.
     blob_offset: the blob offset, only valid if wrapped.
     value: the blink serialized value, only valid if not wrapped.
   """
-  unkown: int
+  unknown: int
   is_wrapped: bool
   blob_size: Optional[int]
   blob_offset: Optional[int]
   value: Any
 
 
 @dataclass
@@ -999,23 +998,23 @@
 
     if (wrapped_header_bytes[0] == definitions.BlinkSerializationTag.VERSION and
         wrapped_header_bytes[1] == 0x11 and
         wrapped_header_bytes[2] == 0x01):
       _, blob_size = decoder.DecodeVarint()
       _, blob_offset = decoder.DecodeVarint()
       return ObjectStoreDataValue(
-          unkown=unknown_integer,
+          unknown=unknown_integer,
           is_wrapped=True,
           blob_size=blob_size,
           blob_offset=blob_offset,
           value=None)
     _, blink_bytes = decoder.ReadBytes()
     blink_value = blink.V8ScriptValueDecoder.FromBytes(blink_bytes)
     return ObjectStoreDataValue(
-        unkown=unknown_integer,
+        unknown=unknown_integer,
         is_wrapped=False,
         blob_size=None,
         blob_offset=None,
         value=blink_value)
 
   @classmethod
   def FromDecoder(
@@ -1333,28 +1332,37 @@
 
   Attributes:
     offset: the offset of the record.
     key: the key of the record.
     value: the value of the record.
     sequence_number: if available, the sequence number of the record.
     type: the type of the record.
+    level: the leveldb level, None indicates the record came from a log file.
+    recovered: True if the record is a recovered record.
   """
+  path: str
   offset: int
   key: Any
   value: Any
-  sequence_number: int
+  sequence_number: Optional[int]
   type: int
+  level: Optional[int]
+  recovered: Optional[bool]
 
   @classmethod
   def FromLevelDBRecord(
-      cls, record: Union[ldb.KeyValueRecord, log.ParsedInternalKey]
+      cls, db_record: record.LevelDBRecord
   ) -> IndexedDBRecord:
     """Returns an IndexedDBRecord from a ParsedInternalKey."""
-    idb_key = IndexedDbKey.FromBytes(record.key, base_offset=record.offset)
-    idb_value = idb_key.ParseValue(record.value)
+    idb_key = IndexedDbKey.FromBytes(
+        db_record.record.key, base_offset=db_record.record.offset)
+    idb_value = idb_key.ParseValue(db_record.record.value)
     return cls(
-      offset=record.offset,
-      key=idb_key,
-      value=idb_value,
-      sequence_number=record.sequence_number if hasattr(
-          record, 'sequence_number') else None,
-      type=record.record_type)
+        path=db_record.path,
+        offset=db_record.record.offset,
+        key=idb_key,
+        value=idb_value,
+        sequence_number=db_record.record.sequence_number if hasattr(
+            db_record.record, 'sequence_number') else None,
+        type=db_record.record.record_type,
+        level=db_record.level,
+        recovered=db_record.recovered)
```

### Comparing `dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/v8.py` & `dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/v8.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,20 @@
     Returns:
       The serialization tag or None if there is no more bytes to read.
     """
     try:
       _, tag_value = self.decoder.PeekBytes(1)
     except errors.DecoderError:
       return None
-    return definitions.V8SerializationTag(tag_value[0])
+    try:
+      return definitions.V8SerializationTag(tag_value[0])
+    except ValueError as error:
+      raise errors.ParserError(
+          f'Invalid v8 tag value {tag_value} at offset'
+          f' {self.decoder.stream.tell()}') from error
 
   def _ReadTag(self) -> definitions.V8SerializationTag:
     """Returns the next non-padding serialization tag.
 
     Raises:
       errors.ParserError: when an invalid v8 tag is read.
     """
@@ -265,15 +270,15 @@
     elif tag == definitions.V8SerializationTag.HOST_OBJECT:
       parsed_object = self.ReadHostObject()
     elif (
         tag == definitions.V8SerializationTag.SHARED_OBJECT and
             self.version >= 15):
       parsed_object = self.ReadSharedObject()
     elif self.version < 13:
-      self.decoder.stream.seek(-1)
+      self.decoder.stream.seek(-1, os.SEEK_CUR)
       parsed_object = self.ReadHostObject()
     else:
       parsed_object = None
     return tag, parsed_object
 
   def ReadString(self) -> str:
     """Reads a string from the current position.
@@ -488,15 +493,15 @@
     else:
       raise errors.ParserError(f'Invalid tag {tag}')
 
     self.objects[next_id] = value
     return value
 
   def _ReadJSRegExp(self) -> RegExp:
-    """Reads a Javscript regular expression from the current position."""
+    """Reads a Javascript regular expression from the current position."""
     next_id = self._GetNextId()
     pattern = self.ReadString()
     _, flags = self.decoder.DecodeUint32Varint()  # TODO: verify flags
     regexp = RegExp(pattern=pattern, flags=flags)
     self.objects[next_id] = regexp
     return regexp
```

### Comparing `dfindexeddb-20240402/dfindexeddb/indexeddb/firefox/__init__.py` & `dfindexeddb-20240417/dfindexeddb/indexeddb/firefox/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240402/dfindexeddb/indexeddb/safari/__init__.py` & `dfindexeddb-20240417/dfindexeddb/indexeddb/safari/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240402/dfindexeddb/leveldb/__init__.py` & `dfindexeddb-20240417/dfindexeddb/leveldb/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240402/dfindexeddb/leveldb/cli.py` & `dfindexeddb-20240417/dfindexeddb/leveldb/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,20 @@
     print(json.dumps(structure, cls=Encoder))
   elif output == 'repr':
     print(structure)
 
 
 def DbCommand(args):
   """The CLI for processing leveldb folders."""
-  for rec in record.LevelDBRecord.FromDir(args.source):
-    _Output(rec, output=args.output)
+  if args.use_manifest:
+    for rec in record.LevelDBRecord.FromManifest(args.source):
+      _Output(rec, output=args.output)
+  else:
+    for rec in record.LevelDBRecord.FromDir(args.source):
+      _Output(rec, output=args.output)
 
 
 def LdbCommand(args):
   """The CLI for processing ldb files."""
   ldb_file = ldb.FileReader(args.source)
 
   if args.structure_type == 'blocks':
@@ -156,14 +160,18 @@
       'db', help='Parse a directory as leveldb.')
   parser_db.add_argument(
       '-s', '--source',
       required=True,
       type=pathlib.Path,
       help='The source leveldb directory')
   parser_db.add_argument(
+      '--use_manifest',
+      action='store_true',
+      help='Use manifest file to determine active/deleted records.')
+  parser_db.add_argument(
       '-o',
       '--output',
       choices=[
           'json',
           'jsonl',
           'repr'],
       default='json',
```

### Comparing `dfindexeddb-20240402/dfindexeddb/leveldb/definitions.py` & `dfindexeddb-20240417/dfindexeddb/leveldb/definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 TABLE_FOOTER_SIZE = 48
 TABLE_MAGIC = b'\x57\xfb\x80\x8b\x24\x75\x47\xdb'
 
 PACKED_SEQUENCE_AND_TYPE_LENGTH = 8
 SEQUENCE_LENGTH = 7
 TYPE_LENGTH = 1
 
+MANIFEST_FILENAME_PATTERN = r'MANIFEST-[0-9]{6}'
+
 
 class BlockCompressionType(enum.IntEnum):
   """Block compression types."""
   SNAPPY = 1
   ZSTD = 2
```

### Comparing `dfindexeddb-20240402/dfindexeddb/leveldb/descriptor.py` & `dfindexeddb-20240417/dfindexeddb/leveldb/descriptor.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240402/dfindexeddb/leveldb/ldb.py` & `dfindexeddb-20240417/dfindexeddb/leveldb/ldb.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240402/dfindexeddb/leveldb/log.py` & `dfindexeddb-20240417/dfindexeddb/leveldb/log.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240402/dfindexeddb/utils.py` & `dfindexeddb-20240417/dfindexeddb/utils.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240402/dfindexeddb/version.py` & `dfindexeddb-20240417/dfindexeddb/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Version information for dfIndexeddb."""
 
 
-__version__ = "20240402"
+__version__ = "20240417"
 
 
 def GetVersion():
   """Returns the version information."""
   return __version__
```

### Comparing `dfindexeddb-20240402/dfindexeddb.egg-info/PKG-INFO` & `dfindexeddb-20240417/dfindexeddb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfindexeddb
-Version: 20240402
+Version: 20240417
 Summary: dfindexeddb is an experimental Python tool for performing digital forensic analysis of IndexedDB and leveldb files.
 Author-email: Syd Pleno <sydp@google.com>
 Maintainer-email: dfIndexeddb Developers <dfindexeddb-dev@googlegroups.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -279,22 +279,69 @@
 installation:
 
 
 ### IndexedDB
 
 ```
 $ dfindexeddb -h
-usage: dfindexeddb [-h] -s SOURCE [-o {json,jsonl,repr}]
+usage: dfindexeddb [-h] {db,ldb,log} ...
 
 A cli tool for parsing indexeddb files
 
+positional arguments:
+  {db,ldb,log}
+    db          Parse a directory as indexeddb.
+    ldb         Parse a ldb file as indexeddb.
+    log         Parse a log file as indexeddb.
+
+options:
+  -h, --help    show this help message and exit
+```
+
+To parse Indexeddb records from a LevelDB folder, use the following command:
+
+```
+dfindexeddb db -h
+usage: dfindexeddb db [-h] -s SOURCE [--use_manifest] [-o {json,jsonl,repr}]
+
 options:
   -h, --help            show this help message and exit
   -s SOURCE, --source SOURCE
                         The source leveldb folder
+  --use_manifest        Use manifest file to determine active/recovered records.
+  -o {json,jsonl,repr}, --output {json,jsonl,repr}
+                        Output format. Default is json
+```
+
+To parse Indexeddb records from a LevelDB ldb (.ldb) file, use the following 
+command:
+
+```
+dfindexeddb ldb -h
+usage: dfindexeddb ldb [-h] -s SOURCE [-o {json,jsonl,repr}]
+
+options:
+  -h, --help            show this help message and exit
+  -s SOURCE, --source SOURCE
+                        The source .ldb file.
+  -o {json,jsonl,repr}, --output {json,jsonl,repr}
+                        Output format. Default is json
+```
+
+To parse Indexeddb records from a LevelDB log (.log) file, use the following 
+command:
+
+```
+dfindexeddb log -h
+usage: dfindexeddb log [-h] -s SOURCE [-o {json,jsonl,repr}]
+
+options:
+  -h, --help            show this help message and exit
+  -s SOURCE, --source SOURCE
+                        The source .log file.
   -o {json,jsonl,repr}, --output {json,jsonl,repr}
                         Output format. Default is json
 ```
 
 ### LevelDB
 
 ```
@@ -310,14 +357,29 @@
     ldb                 Parse a leveldb table (.ldb) file.
     descriptor          Parse a leveldb descriptor (MANIFEST) file.
 
 options:
   -h, --help            show this help message and exit
 ```
 
+To parse records from a LevelDB folder, use the following command:
+
+```
+dfindexeddb db -h
+usage: dfindexeddb db [-h] -s SOURCE [--use_manifest] [-o {json,jsonl,repr}]
+
+options:
+  -h, --help            show this help message and exit
+  -s SOURCE, --source SOURCE
+                        The source leveldb folder
+  --use_manifest        Use manifest file to determine active/recovered records.
+  -o {json,jsonl,repr}, --output {json,jsonl,repr}
+                        Output format. Default is json
+```
+
 To parse records from a LevelDB log (.log) file, use the following command:
 
 ```
 $ dfleveldb log  -s SOURCE [-o {json,jsonl,repr}] [-t {blocks,physical_records,write_batches,parsed_internal_key}]
 
 options:
   -h, --help            show this help message and exit
```

### Comparing `dfindexeddb-20240402/dfindexeddb.egg-info/SOURCES.txt` & `dfindexeddb-20240417/dfindexeddb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240402/pyproject.toml` & `dfindexeddb-20240417/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dfindexeddb"
-version = "20240402"
+version = "20240417"
 requires-python = ">=3.8"
 description = "dfindexeddb is an experimental Python tool for performing digital forensic analysis of IndexedDB and leveldb files."
 license = {file = "LICENSE"}
 authors = [{name = "Syd Pleno", email = "sydp@google.com"}]
 maintainers = [
   {name = "dfIndexeddb Developers", email = "dfindexeddb-dev@googlegroups.com"},
 ]
```

### Comparing `dfindexeddb-20240402/setup.py` & `dfindexeddb-20240417/setup.py`

 * *Files identical despite different names*

