# Comparing `tmp/snapshooter-1.0.6.tar.gz` & `tmp/snapshooter-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapshooter-1.0.6.tar", last modified: Mon Apr 15 23:06:26 2024, max compression
+gzip compressed data, was "snapshooter-1.0.7.tar", last modified: Wed Apr 17 09:04:27 2024, max compression
```

## Comparing `snapshooter-1.0.6.tar` & `snapshooter-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:06:26.126854 snapshooter-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 23:06:09.000000 snapshooter-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 23:06:26.126854 snapshooter-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-15 23:06:09.000000 snapshooter-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 23:06:26.126854 snapshooter-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-15 23:06:09.000000 snapshooter-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:06:26.126854 snapshooter-1.0.6/snapshooter/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 23:06:17.000000 snapshooter-1.0.6/snapshooter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-15 23:06:09.000000 snapshooter-1.0.6/snapshooter/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-15 23:06:09.000000 snapshooter-1.0.6/snapshooter/fsspec_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 23:06:09.000000 snapshooter-1.0.6/snapshooter/jsonl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 23:06:09.000000 snapshooter-1.0.6/snapshooter/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35015 2024-04-15 23:06:09.000000 snapshooter-1.0.6/snapshooter/snapshooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:06:26.126854 snapshooter-1.0.6/snapshooter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 23:06:26.000000 snapshooter-1.0.6/snapshooter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-15 23:06:26.000000 snapshooter-1.0.6/snapshooter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:06:26.000000 snapshooter-1.0.6/snapshooter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 23:06:26.000000 snapshooter-1.0.6/snapshooter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 23:06:26.000000 snapshooter-1.0.6/snapshooter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 23:06:26.000000 snapshooter-1.0.6/snapshooter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:06:26.126854 snapshooter-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 23:06:09.000000 snapshooter-1.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 23:06:09.000000 snapshooter-1.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-15 23:06:09.000000 snapshooter-1.0.6/tests/test_fsspec_snapshooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 23:06:09.000000 snapshooter-1.0.6/tests/test_fsspec_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:04:27.846211 snapshooter-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 09:04:09.000000 snapshooter-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-17 09:04:27.846211 snapshooter-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-17 09:04:09.000000 snapshooter-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:04:27.846211 snapshooter-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-17 09:04:09.000000 snapshooter-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:04:27.846211 snapshooter-1.0.7/snapshooter/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-17 09:04:18.000000 snapshooter-1.0.7/snapshooter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-17 09:04:09.000000 snapshooter-1.0.7/snapshooter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-17 09:04:09.000000 snapshooter-1.0.7/snapshooter/fsspec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-17 09:04:09.000000 snapshooter-1.0.7/snapshooter/jsonl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-17 09:04:09.000000 snapshooter-1.0.7/snapshooter/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35326 2024-04-17 09:04:09.000000 snapshooter-1.0.7/snapshooter/snapshooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:04:27.846211 snapshooter-1.0.7/snapshooter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-17 09:04:27.000000 snapshooter-1.0.7/snapshooter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 09:04:27.000000 snapshooter-1.0.7/snapshooter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:04:27.000000 snapshooter-1.0.7/snapshooter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 09:04:27.000000 snapshooter-1.0.7/snapshooter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 09:04:27.000000 snapshooter-1.0.7/snapshooter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 09:04:27.000000 snapshooter-1.0.7/snapshooter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:04:27.846211 snapshooter-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:04:09.000000 snapshooter-1.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-17 09:04:09.000000 snapshooter-1.0.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-17 09:04:09.000000 snapshooter-1.0.7/tests/test_fsspec_snapshooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-17 09:04:09.000000 snapshooter-1.0.7/tests/test_fsspec_utils.py
```

### Comparing `snapshooter-1.0.6/LICENSE` & `snapshooter-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.6/PKG-INFO` & `snapshooter-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapshooter
-Version: 1.0.6
+Version: 1.0.7
 Summary: Provides a set of utilities for comparing and backing up data on different filesystems
 Home-page: https://github.com/jeromerg/snapshooter
 Author: jeromerg
 Author-email: jeromerg@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snapshooter-1.0.6/README.md` & `snapshooter-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.6/setup.py` & `snapshooter-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.6/snapshooter/cli.py` & `snapshooter-1.0.7/snapshooter/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import json
 import logging
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
-from typing import Tuple, List, Literal
+from typing import List
 
 import fsspec
 import typer
-from fsspec import AbstractFileSystem
 from typing_extensions import Annotated
 
 from snapshooter import Heap, Snapshooter, convert_snapshot_to_df, compare_snapshots as compare_snapshots_
 
-logging.basicConfig(level=logging.INFO)
+logging.basicConfig(
+    level=logging.INFO, 
+    # format: HH:MM:SS (UTC) - level - name - message
+    format="%(asctime)s (%(levelname)s) - %(name)s - %(message)s",
+)
+                    
 log = logging.getLogger(__name__)
 
 # get root logger
 root_logger = logging.getLogger()
 # shift logging for azure.core.pipeline.policies.http_logging_policy (if root logger is set to INFO, then set this to WARNING and so one)
 logging.getLogger("azure.core.pipeline.policies.http_logging_policy").setLevel(root_logger.getEffectiveLevel() + 10)
 
@@ -41,38 +45,40 @@
     snap_root               : Annotated[str, typer.Option(envvar="SNAP_ROOT"               , help="The directory containing the snapshot files. Provided as fsspec path/uri")],
     file_storage_options    : Annotated[str, typer.Option(envvar="FILE_STORAGE_OPTIONS"    , help="Additional storage options to pass to fsspec dir file system. expected JSON string")] = None,
     heap_storage_options    : Annotated[str, typer.Option(envvar="HEAP_STORAGE_OPTIONS"    , help="Additional storage options to pass to fsspec heap_dir file system. expected JSON string")] = None,
     snap_storage_options    : Annotated[str, typer.Option(envvar="SNAP_STORAGE_OPTIONS"    , help="Additional storage options to pass to fsspec snap_dir file system. expected JSON string")] = None,
     parallel_copy_to_heap   : Annotated[int, typer.Option(envvar="PARALLEL_COPY_TO_HEAP"   , help="Number of parallel threads to use for copying files to heap")] = 20,
     parallel_copy_to_file   : Annotated[int, typer.Option(envvar="PARALLEL_COPY_TO_FILE"   , help="Number of parallel threads to use for copying files to file")] = 20,
     parallel_delete_in_file : Annotated[int, typer.Option(envvar="PARALLEL_DELETE_IN_FILE" , help="Number of parallel threads to use for deleting files in file")] = 20,
-    parallel_listing        : Annotated[int, typer.Option(envvar="PARALLEL_LISTING"        , help="Number of parallel threads to use for listing files in heap")] = 20,
+    parallel_listing        : Annotated[int, typer.Option(envvar="PARALLEL_LISTING"        , help="Number of parallel threads to use for listing files in file")] = 20,
+    parallel_heap_listing   : Annotated[int, typer.Option(envvar="PARALLEL_HEAP_LISTING"   , help="Number of parallel threads to use for listing files in heap")] = 20,
 ):
     file_storage_options_dict = json.loads(file_storage_options or "{}")
     heap_storage_options_dict = json.loads(heap_storage_options or "{}")
     snap_storage_options_dict = json.loads(snap_storage_options or "{}")
 
     file_fs, file_root = fsspec.url_to_fs(file_root, **file_storage_options_dict)
     heap_fs, heap_root = fsspec.url_to_fs(heap_root, **heap_storage_options_dict)
     snap_fs, snap_root = fsspec.url_to_fs(snap_root, **snap_storage_options_dict)
 
     heap = Heap(
         heap_fs          = heap_fs, 
         heap_root        = heap_root, 
-        parallel_listing = parallel_listing
+        parallel_listing = parallel_heap_listing
     )
     snapshooter = Snapshooter(
         file_fs                 = file_fs, 
         file_root               = file_root, 
         snap_fs                 = snap_fs, 
         snap_root               = snap_root, 
         heap                    = heap,
         parallel_copy_to_heap   = parallel_copy_to_heap,
         parallel_copy_to_file   = parallel_copy_to_file,
         parallel_delete_in_file = parallel_delete_in_file,
+        parallel_listing        = parallel_listing,
     )
 
     ctx.obj = snapshooter
     ctx.ensure_object(Snapshooter)
 
 
 @main_cli.command()
```

### Comparing `snapshooter-1.0.6/snapshooter/fsspec_utils.py` & `snapshooter-1.0.7/snapshooter/fsspec_utils.py`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.6/snapshooter/jsonl_utils.py` & `snapshooter-1.0.7/snapshooter/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.6/snapshooter/snapshooter.py` & `snapshooter-1.0.7/snapshooter/snapshooter.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         self.heap_fs   = _coerce_fs(heap_fs)
         self.heap_root = _coerce_root_dir(heap_fs, heap_root)
         # Get all heap files
         log.info(f"List out heap files in {self.heap_root}")
         lister = ParallelLister(
             fs=self.heap_fs,
             root=self.heap_root,
-            parallel_listers=parallel_listing,
+            parallel_file_listing=parallel_listing,
         )
         heap_file_paths = [fi["name"] for fi in lister.list_files()]
         # basename WITHOUT EXTENSION corresponds to the md5
         self.heap_md5s = set([os.path.basename(p).split(".")[0] for p in heap_file_paths])
         log.info(f"Heap initialized: Found {len(self.heap_md5s)} files in heap")
 
     def add_file_to_heap(self, f: BufferedReader, check_interrupted_fn: Callable) -> str:
@@ -194,17 +194,18 @@
     def __init__(
         self,
         file_fs   : AbstractFileSystem,
         file_root : str,
         snap_fs   : AbstractFileSystem,
         snap_root : str,
         heap      : Heap,
-        parallel_copy_to_heap   : int = 10,
-        parallel_copy_to_file   : int = 10,
-        parallel_delete_in_file : int = 10,
+        parallel_copy_to_heap   : int = 20,
+        parallel_copy_to_file   : int = 20,
+        parallel_delete_in_file : int = 20,
+        parallel_listing        : int = 20,
     ) -> None:
         """ Create a new Snapshooter instance.
 
         :param file_fs: The file system of the source files.
         :param file_root: The root directory of the source files.
         :param snap_fs: The file system of the snapshot files.
         :param snap_root: The root directory of the snapshot files.
@@ -214,14 +215,15 @@
         self.file_root : str                = _coerce_root_dir(file_fs, file_root)
         self.snap_fs   : AbstractFileSystem = _coerce_fs(snap_fs)
         self.snap_root : str                = _coerce_root_dir(snap_fs, snap_root)
         self.heap      : Heap               = heap
         self.parallel_copy_to_heap   : int  = parallel_copy_to_heap
         self.parallel_copy_to_file   : int  = parallel_copy_to_file
         self.parallel_delete_in_file : int  = parallel_delete_in_file
+        self.parallel_listing        : int  = parallel_listing
         
 
     def convert_snapshot_timestamp_to_path(self, timestamp: datetime.datetime) -> str:
         """ Convert the given timestamp to a snapshot file path.
 
         :param timestamp: The timestamp of the snapshot.
         :return: The path of the snapshot file.
@@ -299,16 +301,16 @@
             snapshot_path = snapshot_path_by_filename[snapshot_filenames_in_reverse_order[0]]
         
         log.info(f"Found snapshot '{snapshot_path}'")
         return snapshot_path
 
     def try_read_snapshot(
         self, 
-        snapshot_path: str | None = None,
-        latest_timestamp: datetime.datetime | None = None,
+        snapshot_path    : str | None = None,
+        latest_timestamp : datetime.datetime | None = None,
     ) -> List[Dict] | None:
         if snapshot_path is None:
             if latest_timestamp is None:
                 log.info(f"Try read latest snapshot")
             else:
                 log.info(f"Try read latest snapshot before '{latest_timestamp}'")
             snapshot_path = self.try_get_snapshot_path(latest_timestamp)
@@ -335,17 +337,17 @@
         if latest_snapshot is None:
             raise Exception(f"No snapshot found in '{self.snap_root}'")
         return latest_snapshot
 
     def _make_snapshot_without_md5(self) -> List[dict]:
         log.info(f"List out src files in '{self.file_root}' (may last long)")
         lister = ParallelLister(
-            fs=self.file_fs,
-            root=self.file_root,
-            parallel_listers=10,
+            fs                    = self.file_fs,
+            root                  = self.file_root,
+            parallel_file_listing = self.parallel_listing,
         )
         src_file_infos = lister.list_files()
         log.info(f"Found {len(src_file_infos)} src files")
 
         # convert native objects to json serializable objects
         src_file_infos = jsonify_file_info(src_file_infos)
 
@@ -357,16 +359,16 @@
         # sort by name (relative path to root)
         src_file_infos.sort(key=lambda fi: fi["name"])
         
         return src_file_infos
 
     def _try_enrich_src_file_infos_with_md5_without_downloading(
         self,
-        src_file_infos: List[dict],
-        latest_snapshot: List[dict]
+        src_file_infos  : List[dict],
+        latest_snapshot : List[dict]
     ):
         """ This function uses a previous snapshot and tries to find in it the same file name, then verifies if
         the file is the same by using file system specific way to identify same file (e.g. ETAG) and if it is the same
         it copies the md5 from the previous snapshot to the current file info."""
         # get md5 getter function depending on the file system type            
         md5_getter = get_md5_getter(self.file_fs)
 
@@ -450,18 +452,18 @@
             snap_content = dumps_jsonl(snapshot)
             g.write(snap_content.encode("utf-8"))
         log.info(f"Saved snapshot")
         return new_snapshot_path
 
     def restore_snapshot(
         self,
-        snapshot_to_restore: str | List[dict] | pd.DataFrame | None = None,
-        latest_timestamp: datetime.datetime = None,
-        save_snapshot_before: bool = True,
-        save_snapshot_after: bool = False,
+        snapshot_to_restore  : str | List[dict] | pd.DataFrame | None = None,
+        latest_timestamp     : datetime.datetime = None,
+        save_snapshot_before : bool = True,
+        save_snapshot_after  : bool = False,
     ):
         log.info("Loading snapshot to restore")
         # read snapshot depending on the type of snapshot_to_restore
         if snapshot_to_restore is None:
             snap = self.read_snapshot(latest_timestamp=latest_timestamp)
             df_snapshot_to_restore = convert_snapshot_to_df(snap)
         elif isinstance(snapshot_to_restore, str):
@@ -528,26 +530,26 @@
         )
         parallel_job.process_files()
 
 
 class ParallelLister:
     def __init__(
         self,
-        fs: AbstractFileSystem,
-        root: str,
-        parallel_listers: int,
+        fs                    : AbstractFileSystem,
+        root                  : str,
+        parallel_file_listing : int,
     ):
-        self.fs = fs
-        self.root = root
-        self.parallel_listers = parallel_listers
-        self.dir_queue = queue.Queue()
-        self.result = []
-        self.errors = []
-        self.lock = threading.Lock()
-        self._is_interrupted = False
+        self.fs               = fs
+        self.root             = root
+        self.parallel_listers = parallel_file_listing
+        self.dir_queue        = queue.Queue()
+        self.result           = []
+        self.errors           = []
+        self.lock             = threading.Lock()
+        self._is_interrupted  = False
 
     def check_interrupted(self):
         if self._is_interrupted:
             raise InterruptedError("Interrupted properly")
 
     def interrupt(self):
         old_is_interrupted = self._is_interrupted
```

### Comparing `snapshooter-1.0.6/snapshooter.egg-info/PKG-INFO` & `snapshooter-1.0.7/snapshooter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapshooter
-Version: 1.0.6
+Version: 1.0.7
 Summary: Provides a set of utilities for comparing and backing up data on different filesystems
 Home-page: https://github.com/jeromerg/snapshooter
 Author: jeromerg
 Author-email: jeromerg@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snapshooter-1.0.6/tests/test_fsspec_snapshooter.py` & `snapshooter-1.0.7/tests/test_fsspec_snapshooter.py`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.6/tests/test_fsspec_utils.py` & `snapshooter-1.0.7/tests/test_fsspec_utils.py`

 * *Files identical despite different names*

