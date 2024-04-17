# Comparing `tmp/pfio-2.7.1.tar.gz` & `tmp/pfio-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfio-2.7.1.tar", last modified: Fri Oct  6 07:00:34 2023, max compression
+gzip compressed data, was "pfio-2.8.0.tar", last modified: Tue Apr 16 23:55:58 2024, max compression
```

## Comparing `pfio-2.7.1.tar` & `pfio-2.8.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-10-06 07:00:34.302127 pfio-2.7.1/
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1064 2022-07-29 03:35:32.000000 pfio-2.7.1/LICENSE
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     2866 2023-10-06 07:00:34.298794 pfio-2.7.1/PKG-INFO
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1340 2023-06-26 00:06:34.000000 pfio-2.7.1/README.md
-drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-10-06 07:00:34.292127 pfio-2.7.1/pfio/
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)       94 2022-07-29 03:35:32.000000 pfio-2.7.1/pfio/__init__.py
-drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-10-06 07:00:34.295461 pfio-2.7.1/pfio/cache/
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     2046 2023-09-13 07:16:14.000000 pfio-2.7.1/pfio/cache/__init__.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    12899 2023-09-13 07:16:14.000000 pfio-2.7.1/pfio/cache/file_cache.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     7908 2023-09-13 07:16:14.000000 pfio-2.7.1/pfio/cache/http_cache.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     3537 2023-09-13 07:16:14.000000 pfio-2.7.1/pfio/cache/mmap_file_cache.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    14863 2023-09-13 07:16:14.000000 pfio-2.7.1/pfio/cache/multiprocess_file_cache.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1141 2023-09-13 07:16:14.000000 pfio-2.7.1/pfio/cache/naive.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    18668 2023-09-13 07:16:14.000000 pfio-2.7.1/pfio/cache/sparse_file.py
-drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-10-06 07:00:34.298794 pfio-2.7.1/pfio/testing/
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     4164 2023-09-13 07:16:14.000000 pfio-2.7.1/pfio/testing/__init__.py
-drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-10-06 07:00:34.298794 pfio-2.7.1/pfio/v2/
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      829 2023-10-06 06:45:45.000000 pfio-2.7.1/pfio/v2/__init__.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1520 2023-09-13 07:16:14.000000 pfio-2.7.1/pfio/v2/config.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    15125 2023-10-06 06:45:45.000000 pfio-2.7.1/pfio/v2/fs.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    12844 2023-10-06 06:45:45.000000 pfio-2.7.1/pfio/v2/hdfs.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     8115 2023-10-06 06:45:45.000000 pfio-2.7.1/pfio/v2/http_cache.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     5782 2023-10-06 06:45:45.000000 pfio-2.7.1/pfio/v2/local.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     7527 2023-09-13 07:16:14.000000 pfio-2.7.1/pfio/v2/pathlib.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    19992 2023-10-06 06:45:45.000000 pfio-2.7.1/pfio/v2/s3.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    10812 2023-10-06 06:45:45.000000 pfio-2.7.1/pfio/v2/zip.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)       22 2023-10-06 06:58:28.000000 pfio-2.7.1/pfio/version.py
-drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-10-06 07:00:34.295461 pfio-2.7.1/pfio.egg-info/
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     2866 2023-10-06 07:00:34.000000 pfio-2.7.1/pfio.egg-info/PKG-INFO
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      602 2023-10-06 07:00:34.000000 pfio-2.7.1/pfio.egg-info/SOURCES.txt
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)        1 2023-10-06 07:00:34.000000 pfio-2.7.1/pfio.egg-info/dependency_links.txt
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)        1 2022-09-26 06:27:07.000000 pfio-2.7.1/pfio.egg-info/not-zip-safe
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      205 2023-10-06 07:00:34.000000 pfio-2.7.1/pfio.egg-info/requires.txt
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)        5 2023-10-06 07:00:34.000000 pfio-2.7.1/pfio.egg-info/top_level.txt
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      343 2023-10-06 07:00:34.302127 pfio-2.7.1/setup.cfg
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     2142 2023-08-01 14:49:37.000000 pfio-2.7.1/setup.py
+drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2024-04-16 23:55:58.701737 pfio-2.8.0/
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1064 2022-07-29 03:35:32.000000 pfio-2.8.0/LICENSE
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     3017 2024-04-16 23:55:58.701737 pfio-2.8.0/PKG-INFO
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1433 2024-04-16 23:12:46.000000 pfio-2.8.0/README.md
+drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2024-04-16 23:55:58.698403 pfio-2.8.0/pfio/
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)       94 2022-07-29 03:35:32.000000 pfio-2.8.0/pfio/__init__.py
+drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2024-04-16 23:55:58.701737 pfio-2.8.0/pfio/cache/
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1874 2024-04-16 23:12:46.000000 pfio-2.8.0/pfio/cache/__init__.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    12899 2023-10-27 10:04:47.000000 pfio-2.8.0/pfio/cache/file_cache.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     7908 2024-01-24 01:40:07.000000 pfio-2.8.0/pfio/cache/http_cache.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     3537 2023-09-13 07:16:14.000000 pfio-2.8.0/pfio/cache/mmap_file_cache.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    14863 2023-09-13 07:16:14.000000 pfio-2.8.0/pfio/cache/multiprocess_file_cache.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1141 2023-09-13 07:16:14.000000 pfio-2.8.0/pfio/cache/naive.py
+drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2024-04-16 23:55:58.701737 pfio-2.8.0/pfio/testing/
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     4164 2023-10-27 10:04:47.000000 pfio-2.8.0/pfio/testing/__init__.py
+drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2024-04-16 23:55:58.701737 pfio-2.8.0/pfio/v2/
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      829 2024-01-24 01:40:07.000000 pfio-2.8.0/pfio/v2/__init__.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1520 2024-01-24 01:40:07.000000 pfio-2.8.0/pfio/v2/config.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    15125 2024-01-24 01:40:07.000000 pfio-2.8.0/pfio/v2/fs.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    12844 2024-01-24 01:40:07.000000 pfio-2.8.0/pfio/v2/hdfs.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     8115 2024-01-24 01:40:07.000000 pfio-2.8.0/pfio/v2/http_cache.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     5782 2024-01-24 01:40:07.000000 pfio-2.8.0/pfio/v2/local.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    22643 2024-04-16 23:12:46.000000 pfio-2.8.0/pfio/v2/pathlib.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    19992 2024-01-24 01:40:07.000000 pfio-2.8.0/pfio/v2/s3.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     9281 2024-04-16 23:12:46.000000 pfio-2.8.0/pfio/v2/zip.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)       22 2024-04-16 23:44:52.000000 pfio-2.8.0/pfio/version.py
+drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2024-04-16 23:55:58.701737 pfio-2.8.0/pfio.egg-info/
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     3017 2024-04-16 23:55:58.000000 pfio-2.8.0/pfio.egg-info/PKG-INFO
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      576 2024-04-16 23:55:58.000000 pfio-2.8.0/pfio.egg-info/SOURCES.txt
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)        1 2024-04-16 23:55:58.000000 pfio-2.8.0/pfio.egg-info/dependency_links.txt
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)        1 2022-09-26 06:27:07.000000 pfio-2.8.0/pfio.egg-info/not-zip-safe
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      212 2024-04-16 23:55:58.000000 pfio-2.8.0/pfio.egg-info/requires.txt
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)        5 2024-04-16 23:55:58.000000 pfio-2.8.0/pfio.egg-info/top_level.txt
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      343 2024-04-16 23:55:58.701737 pfio-2.8.0/setup.cfg
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     2199 2024-04-16 23:12:46.000000 pfio-2.8.0/setup.py
```

### Comparing `pfio-2.7.1/LICENSE` & `pfio-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/PKG-INFO` & `pfio-2.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 Metadata-Version: 2.1
 Name: pfio
-Version: 2.7.1
+Version: 2.8.0
 Summary: PFN IO library
 Home-page: http://github.com/pfnet/pfio
 Author: Tianqi Xu, Kota Uenishi
 Author-email: tianqi@preferred.jp, kota@preferred.jp
 Keywords: filesystem hdfs chainer development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Filesystems
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: deprecation
 Requires-Dist: urllib3
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: autopep8; extra == "test"
 Requires-Dist: parameterized; extra == "test"
 Requires-Dist: isort; extra == "test"
-Requires-Dist: moto[server]; extra == "test"
+Requires-Dist: moto[server]>=5.0.0; extra == "test"
 Requires-Dist: numpy; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
 Provides-Extra: bench
 Requires-Dist: numpy>=1.19.5; extra == "bench"
 Requires-Dist: torch>=1.9.0; extra == "bench"
 Requires-Dist: Pillow<=8.2.0; extra == "bench"
 Provides-Extra: hdfs
 Requires-Dist: pyarrow>=6.0.0; extra == "hdfs"
 
 ## PFIO
 
+![Doc Status Badge](https://readthedocs.org/projects/pfio/badge/?version=master&style=flat)
+
 PFIO is an IO abstraction library developed by PFN, optimized for deep
 learning training with batteries included. It supports
 
 - Filesystem API abstraction with unified error semantics,
 - Explicit user-land caching system,
 - IO performance tracing and metrics stats, and
 - Fileset container utilities to save metadata.
```

### Comparing `pfio-2.7.1/README.md` & `pfio-2.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 ## PFIO
 
+![Doc Status Badge](https://readthedocs.org/projects/pfio/badge/?version=master&style=flat)
+
 PFIO is an IO abstraction library developed by PFN, optimized for deep
 learning training with batteries included. It supports
 
 - Filesystem API abstraction with unified error semantics,
 - Explicit user-land caching system,
 - IO performance tracing and metrics stats, and
 - Fileset container utilities to save metadata.
```

### Comparing `pfio-2.7.1/pfio/cache/__init__.py` & `pfio-2.8.0/pfio/cache/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -57,10 +57,7 @@
 
 
 from pfio.cache.file_cache import FileCache  # NOQA
 from pfio.cache.http_cache import HTTPCache, HTTPConnector  # NOQA
 from pfio.cache.mmap_file_cache import ReadOnlyFileCache  # NOQA
 from pfio.cache.multiprocess_file_cache import MultiprocessFileCache  # NOQA
 from pfio.cache.naive import NaiveCache  # NOQA
-from pfio.cache.sparse_file import CachedWrapper as SparseFileCache  # NOQA
-from pfio.cache.sparse_file import \
-    MPCachedWrapper as MultiprocessSparseFileCache  # NOQA
```

### Comparing `pfio-2.7.1/pfio/cache/file_cache.py` & `pfio-2.8.0/pfio/cache/file_cache.py`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/pfio/cache/http_cache.py` & `pfio-2.8.0/pfio/cache/http_cache.py`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/pfio/cache/mmap_file_cache.py` & `pfio-2.8.0/pfio/cache/mmap_file_cache.py`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/pfio/cache/multiprocess_file_cache.py` & `pfio-2.8.0/pfio/cache/multiprocess_file_cache.py`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/pfio/cache/naive.py` & `pfio-2.8.0/pfio/cache/naive.py`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/pfio/testing/__init__.py` & `pfio-2.8.0/pfio/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/pfio/v2/__init__.py` & `pfio-2.8.0/pfio/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/pfio/v2/config.py` & `pfio-2.8.0/pfio/v2/config.py`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/pfio/v2/fs.py` & `pfio-2.8.0/pfio/v2/fs.py`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/pfio/v2/hdfs.py` & `pfio-2.8.0/pfio/v2/hdfs.py`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/pfio/v2/http_cache.py` & `pfio-2.8.0/pfio/v2/http_cache.py`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/pfio/v2/local.py` & `pfio-2.8.0/pfio/v2/local.py`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/pfio/v2/s3.py` & `pfio-2.8.0/pfio/v2/s3.py`

 * *Files identical despite different names*

### Comparing `pfio-2.7.1/pfio/v2/zip.py` & `pfio-2.8.0/pfio/v2/zip.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import io
 import logging
 import os
-import warnings
 import zipfile
 from datetime import datetime
 from typing import Optional, Set
 
-from pfio.cache.sparse_file import MPCachedWrapper
-
 from .fs import FS, FileStat, format_repr
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.StreamHandler())
 
 
 class ZipFileStat(FileStat):
@@ -49,19 +46,14 @@
                   'volume', 'internal_attr', 'external_attr', 'CRC',
                   'header_offset', 'compress_size', 'compress_type'):
             setattr(self, k, getattr(zip_info, k))
 
 
 class Zip(FS):
     _readonly = True
-    '''
-            local_cache (bool): use sparse file cache for opening ZIP file
-
-            local_cachedir (dir): local path to store sparse file cache
-    '''
 
     def __init__(self, backend, file_path, mode='r', create=False,
                  local_cache=False, local_cachedir=None, **kwargs):
         super().__init__()
         self.backend = backend
         self.file_path = file_path
         self.mode = mode
@@ -72,58 +64,23 @@
 
         if 'r' in mode and 'w' in mode:
             raise io.UnsupportedOperation('Read-write mode is not supported')
 
         if 'w' in mode:
             self._readonly = False
 
-        self.local_cache = local_cache
-        self.local_cachedir = local_cachedir
-        self.local_cachefile = None
-        self.local_indexfile = None
+        if local_cache or local_cachedir:
+            raise NotImplementedError("Sparse file cache has been removed.")
 
         self._reset()
 
     def _reset(self):
-        buffering = self.kwargs.get('buffering', 16*1024*1024)
-
-        if self.local_cache:
-            # Don't use io.BufferedReader for sparse file cache
-            self.kwargs['buffering'] = 0
-
         obj = self.backend.open(self.file_path,
                                 self.mode + 'b',
                                 **self.kwargs)
-
-        if 'w' not in self.mode:
-            stat = self.backend.stat(self.file_path)
-
-        # Use sparse file cache: Optimization for a remote object
-        # store system e.g. AWS S3 or HDFS
-        if self.local_cache:
-            # Will be removed in 2.8
-            warnings.warn("Sparse file cache deprecated in 2.7",
-                          DeprecationWarning)
-
-            self.kwargs['buffering'] = buffering
-
-            obj = MPCachedWrapper(obj, stat.size, self.local_cachedir,
-                                  local_cachefile=self.local_cachefile,
-                                  local_indexfile=self.local_indexfile,
-                                  close_on_close=True,
-                                  multithread_safe=True)
-
-            # Update local cachefile in case of being forked
-            self.local_cachefile = obj.local_cachefile
-            self.local_indexfile = obj.local_indexfile
-
-            # Default 16MB buffer size
-            if buffering > 0:
-                obj = io.BufferedReader(obj, buffer_size=buffering)
-
         self.fileobj = obj
 
         assert self.fileobj is not None
         self.zipobj = zipfile.ZipFile(self.fileobj, self.mode)
         self.name_cache: Optional[Set[str]] = None
         if self._readonly:
             self.name_cache = self._names()
```

### Comparing `pfio-2.7.1/pfio.egg-info/PKG-INFO` & `pfio-2.8.0/pfio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 Metadata-Version: 2.1
 Name: pfio
-Version: 2.7.1
+Version: 2.8.0
 Summary: PFN IO library
 Home-page: http://github.com/pfnet/pfio
 Author: Tianqi Xu, Kota Uenishi
 Author-email: tianqi@preferred.jp, kota@preferred.jp
 Keywords: filesystem hdfs chainer development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Filesystems
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: deprecation
 Requires-Dist: urllib3
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: autopep8; extra == "test"
 Requires-Dist: parameterized; extra == "test"
 Requires-Dist: isort; extra == "test"
-Requires-Dist: moto[server]; extra == "test"
+Requires-Dist: moto[server]>=5.0.0; extra == "test"
 Requires-Dist: numpy; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
 Provides-Extra: bench
 Requires-Dist: numpy>=1.19.5; extra == "bench"
 Requires-Dist: torch>=1.9.0; extra == "bench"
 Requires-Dist: Pillow<=8.2.0; extra == "bench"
 Provides-Extra: hdfs
 Requires-Dist: pyarrow>=6.0.0; extra == "hdfs"
 
 ## PFIO
 
+![Doc Status Badge](https://readthedocs.org/projects/pfio/badge/?version=master&style=flat)
+
 PFIO is an IO abstraction library developed by PFN, optimized for deep
 learning training with batteries included. It supports
 
 - Filesystem API abstraction with unified error semantics,
 - Explicit user-land caching system,
 - IO performance tracing and metrics stats, and
 - Fileset container utilities to save metadata.
```

### Comparing `pfio-2.7.1/pfio.egg-info/SOURCES.txt` & `pfio-2.8.0/pfio.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 pfio.egg-info/top_level.txt
 pfio/cache/__init__.py
 pfio/cache/file_cache.py
 pfio/cache/http_cache.py
 pfio/cache/mmap_file_cache.py
 pfio/cache/multiprocess_file_cache.py
 pfio/cache/naive.py
-pfio/cache/sparse_file.py
 pfio/testing/__init__.py
 pfio/v2/__init__.py
 pfio/v2/config.py
 pfio/v2/fs.py
 pfio/v2/hdfs.py
 pfio/v2/http_cache.py
 pfio/v2/local.py
```

### Comparing `pfio-2.7.1/setup.py` & `pfio-2.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,23 +39,24 @@
         'Operating System :: POSIX',
         'Operating System :: POSIX :: Linux',
 
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
 
         'Topic :: System :: Filesystems',
     ],
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     package_data={'pfio': package_data},
     extras_require={
-        'test': ['pytest', 'flake8', 'autopep8', 'parameterized', 'isort', 'moto[server]', 'numpy', 'mypy'],
+        'test': ['pytest', 'flake8', 'autopep8', 'parameterized', 'isort', 'moto[server]>=5.0.0', 'numpy', 'mypy'],
         # When updating doc deps, docs/requirements.txt should be updated too
         'doc': ['sphinx', 'sphinx_rtd_theme'],
         'bench': ['numpy>=1.19.5', 'torch>=1.9.0', 'Pillow<=8.2.0'],
         'hdfs': ['pyarrow>=6.0.0'],
     },
     # When updating install requires, docs/requirements.txt should be updated too
     install_requires=['boto3', 'deprecation', 'urllib3'],
```

