# Comparing `tmp/DBSamizdat-0.8.6.tar.gz` & `tmp/dbsamizdat-0.9.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DBSamizdat-0.8.6.tar", last modified: Thu Jun  2 19:31:35 2022, max compression
+gzip compressed data, was "dbsamizdat-0.9.0b0.tar", last modified: Wed Apr 17 19:50:50 2024, max compression
```

## Comparing `DBSamizdat-0.8.6.tar` & `dbsamizdat-0.9.0b0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2022-06-02 19:31:35.842855 DBSamizdat-0.8.6/
--rw-r-----   0 boer      (1000) boer      (1000)    32474 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/LICENSE.txt
--rw-r-----   0 boer      (1000) boer      (1000)       16 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/MANIFEST.in
--rw-r-----   0 boer      (1000) boer      (1000)    27137 2022-06-02 19:31:35.843855 DBSamizdat-0.8.6/PKG-INFO
--rw-r-----   0 boer      (1000) boer      (1000)    26214 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/README.md
--rw-r-----   0 boer      (1000) boer      (1000)        6 2022-06-02 19:31:23.000000 DBSamizdat-0.8.6/VERSION
--rw-r-----   0 boer      (1000) boer      (1000)     1374 2022-06-02 19:31:35.843855 DBSamizdat-0.8.6/setup.cfg
--rwxr-x---   0 boer      (1000) boer      (1000)       61 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/setup.py
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2022-06-02 19:31:35.838855 DBSamizdat-0.8.6/src/
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2022-06-02 19:31:35.840855 DBSamizdat-0.8.6/src/DBSamizdat.egg-info/
--rw-r-----   0 boer      (1000) boer      (1000)    27137 2022-06-02 19:31:35.000000 DBSamizdat-0.8.6/src/DBSamizdat.egg-info/PKG-INFO
--rw-r-----   0 boer      (1000) boer      (1000)      741 2022-06-02 19:31:35.000000 DBSamizdat-0.8.6/src/DBSamizdat.egg-info/SOURCES.txt
--rw-r-----   0 boer      (1000) boer      (1000)        1 2022-06-02 19:31:35.000000 DBSamizdat-0.8.6/src/DBSamizdat.egg-info/dependency_links.txt
--rw-r-----   0 boer      (1000) boer      (1000)       54 2022-06-02 19:31:35.000000 DBSamizdat-0.8.6/src/DBSamizdat.egg-info/entry_points.txt
--rw-r-----   0 boer      (1000) boer      (1000)       30 2022-06-02 19:31:35.000000 DBSamizdat-0.8.6/src/DBSamizdat.egg-info/requires.txt
--rw-r-----   0 boer      (1000) boer      (1000)       11 2022-06-02 19:31:35.000000 DBSamizdat-0.8.6/src/DBSamizdat.egg-info/top_level.txt
--rw-r-----   0 boer      (1000) boer      (1000)        1 2021-11-16 16:18:44.000000 DBSamizdat-0.8.6/src/DBSamizdat.egg-info/zip-safe
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2022-06-02 19:31:35.842855 DBSamizdat-0.8.6/src/dbsamizdat/
--rw-r-----   0 boer      (1000) boer      (1000)      197 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/src/dbsamizdat/__init__.py
--rw-r-----   0 boer      (1000) boer      (1000)     1521 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/src/dbsamizdat/api.py
--rw-r-----   0 boer      (1000) boer      (1000)     4709 2022-06-01 14:43:30.000000 DBSamizdat-0.8.6/src/dbsamizdat/apps.py
--rw-r-----   0 boer      (1000) boer      (1000)     1676 2022-06-02 19:30:29.000000 DBSamizdat-0.8.6/src/dbsamizdat/django_api.py
--rw-r-----   0 boer      (1000) boer      (1000)     2693 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/src/dbsamizdat/exceptions.py
--rw-r-----   0 boer      (1000) boer      (1000)     2272 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/src/dbsamizdat/graphvizdot.py
--rw-r-----   0 boer      (1000) boer      (1000)     4924 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/src/dbsamizdat/libdb.py
--rw-r-----   0 boer      (1000) boer      (1000)     3923 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/src/dbsamizdat/libgraph.py
--rw-r-----   0 boer      (1000) boer      (1000)     2081 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/src/dbsamizdat/loader.py
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2022-06-02 19:31:35.838855 DBSamizdat-0.8.6/src/dbsamizdat/management/
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2022-06-02 19:31:35.842855 DBSamizdat-0.8.6/src/dbsamizdat/management/commands/
--rw-r-----   0 boer      (1000) boer      (1000)      793 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/src/dbsamizdat/management/commands/dbsamizdat.py
--rw-r-----   0 boer      (1000) boer      (1000)      110 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/src/dbsamizdat/models.py
--rwxr-x---   0 boer      (1000) boer      (1000)    11724 2022-03-08 12:52:33.000000 DBSamizdat-0.8.6/src/dbsamizdat/runner.py
--rw-r-----   0 boer      (1000) boer      (1000)    12888 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/src/dbsamizdat/samizdat.py
--rw-r-----   0 boer      (1000) boer      (1000)     2881 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/src/dbsamizdat/test_samizdats.py
--rw-r-----   0 boer      (1000) boer      (1000)     1116 2021-11-20 11:47:56.000000 DBSamizdat-0.8.6/src/dbsamizdat/util.py
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-17 19:50:50.365459 dbsamizdat-0.9.0b0/
+-rw-r-----   0 boer      (1000) boer      (1000)    32474 2021-11-20 11:47:56.000000 dbsamizdat-0.9.0b0/LICENSE.txt
+-rw-r-----   0 boer      (1000) boer      (1000)       16 2021-11-20 11:47:56.000000 dbsamizdat-0.9.0b0/MANIFEST.in
+-rw-r--r--   0 boer      (1000) boer      (1000)    27386 2024-04-17 19:50:50.365459 dbsamizdat-0.9.0b0/PKG-INFO
+-rw-r-----   0 boer      (1000) boer      (1000)    26401 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/README.md
+-rw-r-----   0 boer      (1000) boer      (1000)       12 2024-04-16 16:04:47.000000 dbsamizdat-0.9.0b0/VERSION
+-rw-r-----   0 boer      (1000) boer      (1000)     1374 2024-04-17 19:50:50.366459 dbsamizdat-0.9.0b0/setup.cfg
+-rwxr-x---   0 boer      (1000) boer      (1000)       61 2021-11-20 11:47:56.000000 dbsamizdat-0.9.0b0/setup.py
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-17 19:50:50.362459 dbsamizdat-0.9.0b0/src/
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-17 19:50:50.365459 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/
+-rw-r--r--   0 boer      (1000) boer      (1000)    27386 2024-04-17 19:50:50.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/PKG-INFO
+-rw-r-----   0 boer      (1000) boer      (1000)      741 2024-04-17 19:50:50.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/SOURCES.txt
+-rw-r-----   0 boer      (1000) boer      (1000)        1 2024-04-17 19:50:50.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/dependency_links.txt
+-rw-r-----   0 boer      (1000) boer      (1000)       54 2024-04-17 19:50:50.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/entry_points.txt
+-rw-r-----   0 boer      (1000) boer      (1000)       30 2024-04-17 19:50:50.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/requires.txt
+-rw-r-----   0 boer      (1000) boer      (1000)       11 2024-04-17 19:50:50.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/top_level.txt
+-rw-r-----   0 boer      (1000) boer      (1000)        1 2021-11-16 16:18:44.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/zip-safe
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-17 19:50:50.365459 dbsamizdat-0.9.0b0/src/dbsamizdat/
+-rw-r-----   0 boer      (1000) boer      (1000)      197 2024-04-16 14:15:40.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/__init__.py
+-rw-r-----   0 boer      (1000) boer      (1000)     2018 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/api.py
+-rw-r-----   0 boer      (1000) boer      (1000)     4733 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/apps.py
+-rw-r-----   0 boer      (1000) boer      (1000)     2298 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/django_api.py
+-rw-r-----   0 boer      (1000) boer      (1000)     2997 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/exceptions.py
+-rw-r-----   0 boer      (1000) boer      (1000)     2272 2024-04-16 14:15:40.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/graphvizdot.py
+-rw-r-----   0 boer      (1000) boer      (1000)     4937 2024-04-16 14:15:40.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/libdb.py
+-rw-r-----   0 boer      (1000) boer      (1000)     4810 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/libgraph.py
+-rw-r-----   0 boer      (1000) boer      (1000)     2094 2024-04-16 14:15:40.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/loader.py
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-17 19:50:50.362459 dbsamizdat-0.9.0b0/src/dbsamizdat/management/
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-17 19:50:50.365459 dbsamizdat-0.9.0b0/src/dbsamizdat/management/commands/
+-rw-r-----   0 boer      (1000) boer      (1000)      816 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/management/commands/dbsamizdat.py
+-rw-r-----   0 boer      (1000) boer      (1000)      110 2021-11-20 11:47:56.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/models.py
+-rwxr-x---   0 boer      (1000) boer      (1000)    16497 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/runner.py
+-rw-r-----   0 boer      (1000) boer      (1000)    12888 2024-04-16 14:15:40.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/samizdat.py
+-rw-r-----   0 boer      (1000) boer      (1000)     2881 2024-04-16 14:15:40.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/test_samizdats.py
+-rw-r-----   0 boer      (1000) boer      (1000)     1633 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/util.py
```

### Comparing `DBSamizdat-0.8.6/LICENSE.txt` & `dbsamizdat-0.9.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DBSamizdat-0.8.6/PKG-INFO` & `dbsamizdat-0.9.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DBSamizdat
-Version: 0.8.6
+Version: 0.9.0b0
 Summary: dbsamizdat — the blissfully naive PostgreSQL database object manager
 Home-page: https://hub.sr.ht/~nullenenenen/DBSamizdat/
 Author: nullenenenen
 Author-email: nullenenenen@gavagai.eu
 License: GPL-3.0+
 Project-URL: Documentation, https://git.sr.ht/~nullenenenen/DBSamizdat/tree/master/item/README.md
 Project-URL: Source, https://git.sr.ht/~nullenenenen/DBSamizdat/
@@ -16,14 +16,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Database
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: psycopg2>=2.8.0
+Requires-Dist: toposort>=1.5
 
 # DBSamizdat
 
 The blissfully naive PostgreSQL database object manager.
 
 For specifics on integrating with the Django web framework, and some examples for integrating with its ORM, see the [Django integration](#django-integration) section further down.
 
@@ -197,17 +199,18 @@
   dburl                 PostgreSQL DB connection string. Trivially, this might be 'postgresql:///mydbname'.
                         See https://www.postgresql.org/docs/14/static/libpq-connect.html#id-1.7.3.8.3.6 .
   samizdatmodules       Names of modules containing Samizdat subclasses
 
 optional arguments:
   -h, --help            show this help message and exit
   --txdiscipline {checkpoint,jumbo,dryrun}, -t {checkpoint,jumbo,dryrun}
-                        Transaction discipline. The "checkpoint" level commits after every dbsamizdat-level action.
-                        The safe default of "jumbo" creates one large transaction.
+                        Transaction discipline. The default "checkpoint" level commits after every dbsamizdat-level action, and is
+                        compatible with parallelized materialized view refreshing. "jumbo" creates one large transaction.
                         "dryrun" also creates one large transaction, but rolls it back.
+  --parallel, -p        Parallelize refreshing of materialized views. Can only be used with the "checkpoint" transaction discipline.
 ```
 
 
 
 ## Class reference
 
 ### Read-only properties
```

### Comparing `DBSamizdat-0.8.6/README.md` & `dbsamizdat-0.9.0b0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -174,17 +174,18 @@
   dburl                 PostgreSQL DB connection string. Trivially, this might be 'postgresql:///mydbname'.
                         See https://www.postgresql.org/docs/14/static/libpq-connect.html#id-1.7.3.8.3.6 .
   samizdatmodules       Names of modules containing Samizdat subclasses
 
 optional arguments:
   -h, --help            show this help message and exit
   --txdiscipline {checkpoint,jumbo,dryrun}, -t {checkpoint,jumbo,dryrun}
-                        Transaction discipline. The "checkpoint" level commits after every dbsamizdat-level action.
-                        The safe default of "jumbo" creates one large transaction.
+                        Transaction discipline. The default "checkpoint" level commits after every dbsamizdat-level action, and is
+                        compatible with parallelized materialized view refreshing. "jumbo" creates one large transaction.
                         "dryrun" also creates one large transaction, but rolls it back.
+  --parallel, -p        Parallelize refreshing of materialized views. Can only be used with the "checkpoint" transaction discipline.
 ```
 
 
 
 ## Class reference
 
 ### Read-only properties
```

### Comparing `DBSamizdat-0.8.6/setup.cfg` & `dbsamizdat-0.9.0b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `DBSamizdat-0.8.6/src/DBSamizdat.egg-info/PKG-INFO` & `dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DBSamizdat
-Version: 0.8.6
+Version: 0.9.0b0
 Summary: dbsamizdat — the blissfully naive PostgreSQL database object manager
 Home-page: https://hub.sr.ht/~nullenenenen/DBSamizdat/
 Author: nullenenenen
 Author-email: nullenenenen@gavagai.eu
 License: GPL-3.0+
 Project-URL: Documentation, https://git.sr.ht/~nullenenenen/DBSamizdat/tree/master/item/README.md
 Project-URL: Source, https://git.sr.ht/~nullenenenen/DBSamizdat/
@@ -16,14 +16,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Database
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: psycopg2>=2.8.0
+Requires-Dist: toposort>=1.5
 
 # DBSamizdat
 
 The blissfully naive PostgreSQL database object manager.
 
 For specifics on integrating with the Django web framework, and some examples for integrating with its ORM, see the [Django integration](#django-integration) section further down.
 
@@ -197,17 +199,18 @@
   dburl                 PostgreSQL DB connection string. Trivially, this might be 'postgresql:///mydbname'.
                         See https://www.postgresql.org/docs/14/static/libpq-connect.html#id-1.7.3.8.3.6 .
   samizdatmodules       Names of modules containing Samizdat subclasses
 
 optional arguments:
   -h, --help            show this help message and exit
   --txdiscipline {checkpoint,jumbo,dryrun}, -t {checkpoint,jumbo,dryrun}
-                        Transaction discipline. The "checkpoint" level commits after every dbsamizdat-level action.
-                        The safe default of "jumbo" creates one large transaction.
+                        Transaction discipline. The default "checkpoint" level commits after every dbsamizdat-level action, and is
+                        compatible with parallelized materialized view refreshing. "jumbo" creates one large transaction.
                         "dryrun" also creates one large transaction, but rolls it back.
+  --parallel, -p        Parallelize refreshing of materialized views. Can only be used with the "checkpoint" transaction discipline.
 ```
 
 
 
 ## Class reference
 
 ### Read-only properties
```

### Comparing `DBSamizdat-0.8.6/src/DBSamizdat.egg-info/SOURCES.txt` & `dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DBSamizdat-0.8.6/src/dbsamizdat/api.py` & `dbsamizdat-0.9.0b0/src/dbsamizdat/django_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,82 @@
 """
-API for using dbsamizdat as a library
+API for using dbsamizdat as a library in Django
 """
 
 from argparse import Namespace as _Namespace
 from typing import Iterable, Union
 
 from .runner import cmd_refresh as _cmd_refresh, cmd_sync as _cmd_sync, cmd_nuke as _cmd_nuke, txstyle
 from .samizdat import Samizdat
+from .exceptions import WrongTransactionStyleForParallelRefresh
 
 _CMD_ARG_DEFAULTS = dict(
-    log_rather_than_print=True,
-    in_django=False,
+    in_django=True,
     verbosity=1,
+    log_rather_than_print=True,
+    parallel=False,
 )
 
 
-def refresh(dburl: str, samizdatmodules: Iterable[str], transaction_style: txstyle = txstyle.JUMBO, belownodes: Iterable[Union[str, tuple, Samizdat]] = tuple()):
-    """Refresh materialized views, in dependency order, optionally restricted to views depending directly or transitively on any of the DB objects specified in `belownodes`."""
+def refresh(
+    dbconn: str = 'default',
+    transaction_style: txstyle = txstyle.CHECKPOINT,
+    belownodes: Iterable[Union[str, tuple, Samizdat]] = tuple(),
+    samizdatmodules=tuple(),
+    parallel=False,
+):
+    """
+    Refresh materialized views, in dependency order, optionally parallelized (where the dependency tree allows), optionally restricted to views depending directly or transitively on any of the DB objects specified in `belownodes`.
+    """
+    if parallel and transaction_style != txstyle.CHECKPOINT:
+        raise WrongTransactionStyleForParallelRefresh()
     args = _Namespace(
-        **_CMD_ARG_DEFAULTS,
-        dburl=dburl,
-        samizdatmodules=samizdatmodules,
-        txdiscipline=transaction_style.value,
-        belownodes=belownodes,
+        **{
+            **_CMD_ARG_DEFAULTS,
+            'dbconn': dbconn,
+            'txdiscipline': transaction_style.value,
+            'belownodes': belownodes,
+            'samizdatmodules': samizdatmodules,
+            'parallel': parallel,
+        }
     )
     _cmd_refresh(args)
 
 
-def sync(dburl: str, samizdatmodules: Iterable[str], transaction_style: txstyle = txstyle.JUMBO):
-    """Sync dbsamizdat state to the DB."""
+def sync(
+    dbconn: str = 'default',
+    transaction_style: txstyle = txstyle.JUMBO,
+    samizdatmodules=tuple(),
+    parallel=False,
+):
+    """
+    Sync dbsamizdat state to the DB.
+    """
+    if parallel and transaction_style != txstyle.CHECKPOINT:
+        raise WrongTransactionStyleForParallelRefresh()
     args = _Namespace(
-        **_CMD_ARG_DEFAULTS,
-        dburl=dburl,
-        samizdatmodules=samizdatmodules,
-        txdiscipline=transaction_style.value,
+        **{
+            **_CMD_ARG_DEFAULTS,
+            'dbconn': dbconn,
+            'txdiscipline': transaction_style.value,
+            'samizdatmodules': samizdatmodules,
+            'parallel': parallel,
+        }
     )
     _cmd_sync(args)
 
 
-def nuke(dburl: str, transaction_style: txstyle = txstyle.JUMBO):
-    """Remove any database object tagged as samizdat."""
+def nuke(
+    dbconn: str = 'default',
+    transaction_style: txstyle = txstyle.JUMBO,
+    samizdatmodules=tuple(),
+):
+    """
+    Remove any database object tagged as samizdat.
+    """
     args = _Namespace(
         **_CMD_ARG_DEFAULTS,
-        dburl=dburl,
+        dbconn=dbconn,
         txdiscipline=transaction_style.value,
+        samizdatmodules=samizdatmodules,
     )
     _cmd_nuke(args)
```

### Comparing `DBSamizdat-0.8.6/src/dbsamizdat/apps.py` & `dbsamizdat-0.9.0b0/src/dbsamizdat/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         printprogress=True,
         verbosity=kwargs['verbosity'],
         dbconn=DBCONN,
         txdiscipline=txstyle.JUMBO.value,
         in_django=True,
         samizdatmodules=tuple(),
         log_rather_than_print=not kwargs.get('interactive'),
+        parallel=False,
     )
 
 
 def sync(**kwargs):
     cmd_sync(get_cmd_args(**kwargs))
```

### Comparing `DBSamizdat-0.8.6/src/dbsamizdat/django_api.py` & `dbsamizdat-0.9.0b0/src/dbsamizdat/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,60 @@
 """
-API for using dbsamizdat as a library in Django
+API for using dbsamizdat as a library
 """
 
 from argparse import Namespace as _Namespace
 from typing import Iterable, Union
 
 from .runner import cmd_refresh as _cmd_refresh, cmd_sync as _cmd_sync, cmd_nuke as _cmd_nuke, txstyle
 from .samizdat import Samizdat
+from .exceptions import WrongTransactionStyleForParallelRefresh
 
 _CMD_ARG_DEFAULTS = dict(
-    in_django=True,
-    verbosity=1,
     log_rather_than_print=True,
+    in_django=False,
+    verbosity=1,
+    parallel=False,
 )
 
 
-def refresh(
-    dbconn: str = 'default',
-    transaction_style: txstyle = txstyle.JUMBO,
-    belownodes: Iterable[Union[str, tuple, Samizdat]] = tuple(),
-    samizdatmodules=tuple(),
-):
-    """Refresh materialized views, in dependency order, optionally restricted to views depending directly or transitively on any of the DB objects specified in `belownodes`."""
+def refresh(dburl: str, samizdatmodules: Iterable[str], transaction_style: txstyle = txstyle.CHECKPOINT, belownodes: Iterable[Union[str, tuple, Samizdat]] = tuple(), parallel: bool = False):
+    """
+    Refresh materialized views, in dependency order, optionally parallelized (where the dependency tree allows), optionally restricted to views depending directly or transitively on any of the DB objects specified in `belownodes`.
+    """
+    if parallel and transaction_style != txstyle.CHECKPOINT:
+        raise WrongTransactionStyleForParallelRefresh()
     args = _Namespace(
         **_CMD_ARG_DEFAULTS,
-        dbconn=dbconn,
+        dburl=dburl,
+        samizdatmodules=samizdatmodules,
         txdiscipline=transaction_style.value,
         belownodes=belownodes,
-        samizdatmodules=samizdatmodules,
+        parallel=parallel,
     )
     _cmd_refresh(args)
 
 
-def sync(
-    dbconn: str = 'default',
-    transaction_style: txstyle = txstyle.JUMBO,
-    samizdatmodules=tuple(),
-):
-    """Sync dbsamizdat state to the DB."""
+def sync(dburl: str, samizdatmodules: Iterable[str], transaction_style: txstyle = txstyle.JUMBO, parallel=False):
+    """
+    Sync dbsamizdat state to the DB.
+    """
+    if parallel and transaction_style != txstyle.CHECKPOINT:
+        raise WrongTransactionStyleForParallelRefresh()
     args = _Namespace(
         **_CMD_ARG_DEFAULTS,
-        dbconn=dbconn,
-        txdiscipline=transaction_style.value,
+        dburl=dburl,
         samizdatmodules=samizdatmodules,
+        txdiscipline=transaction_style.value,
+        parallel=parallel,
     )
     _cmd_sync(args)
 
 
-def nuke(
-    dbconn: str = 'default',
-    transaction_style: txstyle = txstyle.JUMBO,
-    samizdatmodules=tuple(),
-):
+def nuke(dburl: str, transaction_style: txstyle = txstyle.JUMBO):
     """Remove any database object tagged as samizdat."""
     args = _Namespace(
         **_CMD_ARG_DEFAULTS,
-        dbconn=dbconn,
+        dburl=dburl,
         txdiscipline=transaction_style.value,
-        samizdatmodules=samizdatmodules,
     )
     _cmd_nuke(args)
```

### Comparing `DBSamizdat-0.8.6/src/dbsamizdat/exceptions.py` & `dbsamizdat-0.9.0b0/src/dbsamizdat/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,26 @@
         self.samizdat = samizdat
 
     def __str__(self):
         sd_subject = f'{repr(self.samizdat)} : ' if self.samizdat else ''
         return f'{sd_subject}{self.message}'
 
 
+class InvocationError(SamizdatException):
+    pass
+
+
+class WrongTransactionStyleForParallelRefresh(InvocationError):
+    def __init__(self, *args, **kwargs):
+        self.msg = 'Parallel refresh is only possible with the "checkpoint" transaction style.'
+
+    def __str__(self):
+        return self.msg
+
+
 class NameClashError(SamizdatException):
     pass
 
 
 class UnsuitableNameError(SamizdatException):
     pass
```

### Comparing `DBSamizdat-0.8.6/src/dbsamizdat/graphvizdot.py` & `dbsamizdat-0.9.0b0/src/dbsamizdat/graphvizdot.py`

 * *Files identical despite different names*

### Comparing `DBSamizdat-0.8.6/src/dbsamizdat/libdb.py` & `dbsamizdat-0.9.0b0/src/dbsamizdat/libdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 LEFT JOIN pg_class pc ON pt.tgrelid = pc.oid
                 LEFT JOIN pg_catalog.pg_namespace pn ON pn.oid = pc.relnamespace
             WHERE
                 pt.tgisinternal = False
             """
     }
 
-    for *stuff, jinfo in chain(*map(execfetch, map(fetches.get, entity_types))):
+    for *stuff, jinfo in chain.from_iterable(map(execfetch, map(fetches.get, entity_types))):
         objtype = DBObjectType.SAMIZDAT if (jinfo and jinfo.startswith(COMMENT_MAGIC)) else DBObjectType.FOREIGN
         if objtype & which:
             definition_hash = None
             if objtype == DBObjectType.SAMIZDAT:
                 meta = jsonloads(jinfo)['dbsamizdat']
                 hashattr = {0: 'sql_template_hash', 1: 'definition_hash'}[meta['version']]
                 definition_hash = meta[hashattr]
```

### Comparing `DBSamizdat-0.8.6/src/dbsamizdat/libgraph.py` & `dbsamizdat-0.9.0b0/src/dbsamizdat/libgraph.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,26 @@
 
 from toposort import toposort, CircularDependencyError
 
 from . import entitypes
 from .exceptions import NameClashError, DanglingReferenceError, TypeConfusionError, DependencyCycleError
 
 
+def flatten(thing):
+
+    def traverse(something):
+        if not isinstance(something, list):
+            yield something
+        else:
+            for t in something:
+                yield from traverse(t)
+
+    return list(traverse(thing))
+
+
 def gen_edges(samizdats):
     for sd in samizdats:
         for n2 in sd.fqdeps_on():
             yield (n2, sd.fq)
 
 
 def gen_autorefresh_edges(samizdats):
@@ -57,34 +69,54 @@
     """
     Samizdats directly or indirectly depending on any root in roots
     """
     sdmap = {sd.fq: sd for sd in samizdats}
     return reduce(or_, (set(filter(None, (sdmap.get(name) for name in subtree_nodes(samizdats, rootnode)))) for rootnode in roots), set())
 
 
-def depsort(samizdats):
+def deps_on_closure(samizdats):
+    sdmap = {sd.fq: sd for sd in samizdats}
+
+    def deps_on_closure_one(samizdat):
+        if fqdeps := samizdat.fqdeps_on():
+            for sd in map(sdmap.get, fqdeps):
+                yield sd
+                yield from deps_on_closure_one(sd)
+
+    return {sd: set(deps_on_closure_one(sd)) for sd in samizdats}
+
+
+def depsort(samizdats, flat=True):
     """
     Topologically sort samizdats
     """
     samizdat_map = {sd.fq: sd for sd in samizdats}
     depmap = {sd.fq: sd.fqdeps_on() for sd in samizdats}
-    return [samizdat_map[name] for name in chain(*(sorted(level) for level in toposort(depmap)))]
+    toposorted = [[samizdat_map[name] for name in sorted(level)] for level in toposort(depmap)]
+    if flat:
+        return flatten(toposorted)
+    return toposorted
 
 
-def depsort_with_sidekicks(samizdats):
+def depsort_with_sidekicks(samizdats, flat=True):
     counter = Counter()
-    return list(chain(*(sd.and_sidekicks(counter) for sd in depsort(samizdats))))
+    if flat:
+        return list(chain.from_iterable(sd.and_sidekicks(counter) for sd in depsort(samizdats)))
+    return [
+        list(chain.from_iterable((sd.and_sidekicks(counter) for sd in sdgroup)))
+        for sdgroup in depsort(samizdats, flat=False)
+    ]
 
 
 def sanity_check(samizdats):
     for sd in samizdats:
         sd.validate_name()
     sd_fqs = set(sd.fq for sd in samizdats)
-    sd_deps = set(chain(*(sd.fqdeps_on() for sd in samizdats)))
-    sd_deps_unmanaged = set(chain(*(sd.deps_on_unmanaged for sd in samizdats)))
+    sd_deps = set(chain.from_iterable(sd.fqdeps_on() for sd in samizdats))
+    sd_deps_unmanaged = set(chain.from_iterable(sd.deps_on_unmanaged for sd in samizdats))
 
     # are there any classes with ambiguous DB identity?
     if len(sd_fqs) < len(samizdats):
         cnt = Counter((sd.db_object_identity for sd in samizdats))
         nonunique = [db_id for db_id, count in cnt.items() if count > 1]
         if nonunique:
             raise NameClashError('Non-unique DB entities specified: %s' % nonunique)
```

### Comparing `DBSamizdat-0.8.6/src/dbsamizdat/loader.py` & `dbsamizdat-0.9.0b0/src/dbsamizdat/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,8 +38,8 @@
                 if not django_sdmodules:
                     logger.warn("""No settings.DBSAMIZDAT_MODULES defined, and none of your apps contain any "dbsamizdat_defs" module to autoload.""")
                 sdmodules += django_sdmodules
             except ImproperlyConfigured:
                 # assume we're not running in a fully booted Django
                 pass
 
-    return set((c for cname, c in chain(*map(lambda m: inspect.getmembers(m, issamizdat), sdmodules))))
+    return set((c for cname, c in chain.from_iterable(map(lambda m: inspect.getmembers(m, issamizdat), sdmodules))))
```

### Comparing `DBSamizdat-0.8.6/src/dbsamizdat/management/commands/dbsamizdat.py` & `dbsamizdat-0.9.0b0/src/dbsamizdat/management/commands/dbsamizdat.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,12 +13,12 @@
         return super(Command, self).create_parser(*args, **{**kwargs, **{'conflict_handler': 'resolve'}})
 
     def add_arguments(self, parser):
         augment_argument_parser(parser, in_django=True, log_rather_than_print=False)
 
     def handle(self, *args, **options):
         try:
-            options['func'](Namespace(**options))
+            options['func'](Namespace(**{'parallel': False, **options}))
         except SamizdatException as argh:
             exit(f'\n\n\nFATAL: {argh}')
         except KeyboardInterrupt:
             exit('\nInterrupted.')
```

### Comparing `DBSamizdat-0.8.6/src/dbsamizdat/samizdat.py` & `dbsamizdat-0.9.0b0/src/dbsamizdat/samizdat.py`

 * *Files identical despite different names*

### Comparing `DBSamizdat-0.8.6/src/dbsamizdat/test_samizdats.py` & `dbsamizdat-0.9.0b0/src/dbsamizdat/test_samizdats.py`

 * *Files identical despite different names*

