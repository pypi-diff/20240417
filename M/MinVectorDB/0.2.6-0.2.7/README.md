# Comparing `tmp/minvectordb-0.2.6.tar.gz` & `tmp/minvectordb-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minvectordb-0.2.6.tar", last modified: Tue Apr 16 06:40:02 2024, max compression
+gzip compressed data, was "minvectordb-0.2.7.tar", last modified: Wed Apr 17 08:50:41 2024, max compression
```

## Comparing `minvectordb-0.2.6.tar` & `minvectordb-0.2.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.631423 minvectordb-0.2.6/
--rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 minvectordb-0.2.6/LICENSE
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.630909 minvectordb-0.2.6/MinVectorDB.egg-info/
--rw-r--r--   0 guobingming   (501) staff       (20)    17718 2024-04-16 06:40:02.000000 minvectordb-0.2.6/MinVectorDB.egg-info/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)     1102 2024-04-16 06:40:02.000000 minvectordb-0.2.6/MinVectorDB.egg-info/SOURCES.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-04-16 06:40:02.000000 minvectordb-0.2.6/MinVectorDB.egg-info/dependency_links.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 minvectordb-0.2.6/MinVectorDB.egg-info/not-zip-safe
--rw-r--r--   0 guobingming   (501) staff       (20)      173 2024-04-16 06:40:02.000000 minvectordb-0.2.6/MinVectorDB.egg-info/requires.txt
--rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-04-16 06:40:02.000000 minvectordb-0.2.6/MinVectorDB.egg-info/top_level.txt
--rw-r--r--   0 guobingming   (501) staff       (20)    17718 2024-04-16 06:40:02.631180 minvectordb-0.2.6/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)    16402 2024-04-15 04:50:27.000000 minvectordb-0.2.6/README.md
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.627604 minvectordb-0.2.6/min_vec/
--rw-r--r--   0 guobingming   (501) staff       (20)      115 2024-04-15 13:22:42.000000 minvectordb-0.2.6/min_vec/__init__.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.627849 minvectordb-0.2.6/min_vec/api/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:42.000000 minvectordb-0.2.6/min_vec/api/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    11906 2024-04-16 06:35:02.000000 minvectordb-0.2.6/min_vec/api/api.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.628091 minvectordb-0.2.6/min_vec/computational_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 minvectordb-0.2.6/min_vec/computational_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)      931 2024-04-13 16:15:59.000000 minvectordb-0.2.6/min_vec/computational_layer/engines.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.628450 minvectordb-0.2.6/min_vec/configs/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 minvectordb-0.2.6/min_vec/configs/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2896 2024-04-12 07:35:09.000000 minvectordb-0.2.6/min_vec/configs/config.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3405 2024-04-15 03:56:30.000000 minvectordb-0.2.6/min_vec/configs/parameters_validator.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.629234 minvectordb-0.2.6/min_vec/data_structures/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 minvectordb-0.2.6/min_vec/data_structures/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2316 2024-04-03 03:58:31.000000 minvectordb-0.2.6/min_vec/data_structures/fields_mapper.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1036 2024-03-06 14:55:44.000000 minvectordb-0.2.6/min_vec/data_structures/filter.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1545 2024-04-12 07:35:09.000000 minvectordb-0.2.6/min_vec/data_structures/kmeans.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1282 2024-04-13 15:42:07.000000 minvectordb-0.2.6/min_vec/data_structures/limited_dict.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2587 2024-04-12 07:35:09.000000 minvectordb-0.2.6/min_vec/data_structures/limited_sort.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3811 2024-04-12 09:25:04.000000 minvectordb-0.2.6/min_vec/data_structures/scaler.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.629879 minvectordb-0.2.6/min_vec/execution_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 minvectordb-0.2.6/min_vec/execution_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2541 2024-04-13 15:41:43.000000 minvectordb-0.2.6/min_vec/execution_layer/cluster_worker.py
--rw-r--r--   0 guobingming   (501) staff       (20)    20159 2024-04-16 06:35:02.000000 minvectordb-0.2.6/min_vec/execution_layer/matrix_serializer.py
--rw-r--r--   0 guobingming   (501) staff       (20)     9989 2024-04-13 15:53:22.000000 minvectordb-0.2.6/min_vec/execution_layer/query.py
--rw-r--r--   0 guobingming   (501) staff       (20)      362 2024-02-26 09:43:31.000000 minvectordb-0.2.6/min_vec/execution_layer/session.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.630090 minvectordb-0.2.6/min_vec/storage_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 minvectordb-0.2.6/min_vec/storage_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    17239 2024-04-16 06:35:02.000000 minvectordb-0.2.6/min_vec/storage_layer/storage.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.630340 minvectordb-0.2.6/min_vec/utils/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 minvectordb-0.2.6/min_vec/utils/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3389 2024-04-15 04:05:21.000000 minvectordb-0.2.6/min_vec/utils/utils.py
--rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-04-16 06:40:02.631464 minvectordb-0.2.6/setup.cfg
--rw-r--r--   0 guobingming   (501) staff       (20)     1471 2024-04-15 13:22:42.000000 minvectordb-0.2.6/setup.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.630688 minvectordb-0.2.6/test/
--rw-r--r--   0 guobingming   (501) staff       (20)       31 2024-01-31 10:38:44.000000 minvectordb-0.2.6/test/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1834 2024-04-15 04:04:57.000000 minvectordb-0.2.6/test/test_initial.py
--rw-r--r--   0 guobingming   (501) staff       (20)    11844 2024-04-12 07:35:09.000000 minvectordb-0.2.6/test/test_save_and_query.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.823442 minvectordb-0.2.7/
+-rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 minvectordb-0.2.7/LICENSE
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.822956 minvectordb-0.2.7/MinVectorDB.egg-info/
+-rw-r--r--   0 guobingming   (501) staff       (20)    17247 2024-04-17 08:50:41.000000 minvectordb-0.2.7/MinVectorDB.egg-info/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)     1102 2024-04-17 08:50:41.000000 minvectordb-0.2.7/MinVectorDB.egg-info/SOURCES.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-04-17 08:50:41.000000 minvectordb-0.2.7/MinVectorDB.egg-info/dependency_links.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 minvectordb-0.2.7/MinVectorDB.egg-info/not-zip-safe
+-rw-r--r--   0 guobingming   (501) staff       (20)      173 2024-04-17 08:50:41.000000 minvectordb-0.2.7/MinVectorDB.egg-info/requires.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-04-17 08:50:41.000000 minvectordb-0.2.7/MinVectorDB.egg-info/top_level.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)    17247 2024-04-17 08:50:41.823199 minvectordb-0.2.7/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)    15931 2024-04-17 05:54:49.000000 minvectordb-0.2.7/README.md
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.818629 minvectordb-0.2.7/min_vec/
+-rw-r--r--   0 guobingming   (501) staff       (20)      115 2024-04-16 07:36:11.000000 minvectordb-0.2.7/min_vec/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.818872 minvectordb-0.2.7/min_vec/api/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:42.000000 minvectordb-0.2.7/min_vec/api/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    13736 2024-04-17 08:23:55.000000 minvectordb-0.2.7/min_vec/api/api.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.819102 minvectordb-0.2.7/min_vec/computational_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 minvectordb-0.2.7/min_vec/computational_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      890 2024-04-17 08:04:09.000000 minvectordb-0.2.7/min_vec/computational_layer/engines.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.819443 minvectordb-0.2.7/min_vec/configs/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 minvectordb-0.2.7/min_vec/configs/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2553 2024-04-17 05:52:07.000000 minvectordb-0.2.7/min_vec/configs/config.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3611 2024-04-17 06:40:43.000000 minvectordb-0.2.7/min_vec/configs/parameters_validator.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.820762 minvectordb-0.2.7/min_vec/data_structures/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 minvectordb-0.2.7/min_vec/data_structures/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2316 2024-04-03 03:58:31.000000 minvectordb-0.2.7/min_vec/data_structures/fields_mapper.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1036 2024-03-06 14:55:44.000000 minvectordb-0.2.7/min_vec/data_structures/filter.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1545 2024-04-12 07:35:09.000000 minvectordb-0.2.7/min_vec/data_structures/kmeans.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1282 2024-04-13 15:42:07.000000 minvectordb-0.2.7/min_vec/data_structures/limited_dict.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2977 2024-04-17 08:45:02.000000 minvectordb-0.2.7/min_vec/data_structures/limited_sort.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3811 2024-04-12 09:25:04.000000 minvectordb-0.2.7/min_vec/data_structures/scaler.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.821481 minvectordb-0.2.7/min_vec/execution_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 minvectordb-0.2.7/min_vec/execution_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2316 2024-04-16 09:40:39.000000 minvectordb-0.2.7/min_vec/execution_layer/cluster_worker.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    19379 2024-04-16 10:23:42.000000 minvectordb-0.2.7/min_vec/execution_layer/matrix_serializer.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     7818 2024-04-17 08:40:57.000000 minvectordb-0.2.7/min_vec/execution_layer/query.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      362 2024-02-26 09:43:31.000000 minvectordb-0.2.7/min_vec/execution_layer/session.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.821821 minvectordb-0.2.7/min_vec/storage_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 minvectordb-0.2.7/min_vec/storage_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    16764 2024-04-16 10:15:07.000000 minvectordb-0.2.7/min_vec/storage_layer/storage.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.822055 minvectordb-0.2.7/min_vec/utils/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 minvectordb-0.2.7/min_vec/utils/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3389 2024-04-15 04:05:21.000000 minvectordb-0.2.7/min_vec/utils/utils.py
+-rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-04-17 08:50:41.823498 minvectordb-0.2.7/setup.cfg
+-rw-r--r--   0 guobingming   (501) staff       (20)     1471 2024-04-16 07:36:11.000000 minvectordb-0.2.7/setup.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.822661 minvectordb-0.2.7/test/
+-rw-r--r--   0 guobingming   (501) staff       (20)       31 2024-01-31 10:38:44.000000 minvectordb-0.2.7/test/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1834 2024-04-15 04:04:57.000000 minvectordb-0.2.7/test/test_initial.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    11844 2024-04-12 07:35:09.000000 minvectordb-0.2.7/test/test_save_and_query.py
```

### Comparing `minvectordb-0.2.6/LICENSE` & `minvectordb-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.6/MinVectorDB.egg-info/PKG-INFO` & `minvectordb-0.2.7/MinVectorDB.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MinVectorDB
-Version: 0.2.6
+Version: 0.2.7
 Summary: MinVectorDB is a pure Python-implemented, lightweight, serverless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
 Home-page: https://github.com/BirchKwok/MinVectorDB
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: vector database
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -34,17 +34,14 @@
 <div align="center">
   <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
   <h3>A pure Python-implemented, lightweight, serverless, locally deployed vector database.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
-    <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/dm/MinVectorDB" alt="PyPI - Downloads"></a>
-    <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/implementation/MinVectorDB" alt="PyPI - Implementation"></a>
-    <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/wheel/MinVectorDB" alt="PyPI - Wheel"></a>
     <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
   </p>
 </div>
 
 ⚡ **Serverless, simple parameters, simple API.**
 
 ⚡ **Fast, memory-efficient, easily scales to millions of vectors.**
@@ -100,37 +97,33 @@
 # clustering settings
 # kmeans epochs
 os.environ['MVDB_KMEANS_EPOCHS'] = '500'  # default: 100
 
 # query cache size
 os.environ['MVDB_QUERY_CACHE_SIZE'] = '10000'  # default: 10000
 
-# cosine similarity threshold for cache result matching 
-os.environ['MVDB_COSINE_SIMILARITY_THRESHOLD'] = '0.9'  # 'None' for disable this feature, default to 0.85
-
 # specify the number of chunks in the memory cache
 os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20'  # default to '20', must be integer-like string
 ```
 
 
 ```python
 import min_vec
 print("MinVectorDB version is: ", min_vec.__version__)
 print("MinVectorDB all configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in min_vec.get_all_configs().items()]))
 ```
 
-    MinVectorDB version is:  0.2.5
+    MinVectorDB version is:  0.2.7
     MinVectorDB all configs:  
      - MVDB_LOG_LEVEL: INFO
      - MVDB_LOG_PATH: ./min_vec_db.log
      - MVDB_TRUNCATE_LOG: True
      - MVDB_LOG_WITH_TIME: False
      - MVDB_KMEANS_EPOCHS: 500
      - MVDB_QUERY_CACHE_SIZE: 10000
-     - MVDB_COSINE_SIMILARITY_THRESHOLD: 0.9
      - MVDB_DATALOADER_BUFFER_SIZE: 20
 
 
 ### Sequentially add vectors.
 
 
 ```python
@@ -145,15 +138,15 @@
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
 # distance can be 'L2' or 'cosine'
 # index_mode can be 'FLAT' or 'IVF-FLAT', default is 'IVF-FLAT'
 db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', index_mode='FLAT',
-                 chunk_size=100000, use_cache=False, scaler_bits=8, n_threads=10, distance='cosine')
+                 chunk_size=100000, use_cache=False, scaler_bits=8, n_threads=10)
 
 # ========== Use automatic commit statements. Recommended. =============
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():
     # Define the initial ID.
     id = 0
     for t in tqdm(get_test_vectors((1000000, 1024)), total=1000000, unit="vector"):
@@ -162,48 +155,50 @@
             query_id = 0
             query_field = None
         # Vectors will be normalized after writing to the database.
         db.add_item(t, index=id)
 
         id += 1
 
-res = db.query(query, k=10, return_similarity=True)
+res = db.query(query, k=10, return_similarity=True, distance='cosine')
 
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
+
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
     //    n_clusters=16, chunk_size=100000,
     //    distance='cosine', index_mode='FLAT', 
-    //    dtypes='float32', use_cache=True, 
+    //    dtypes='float32', use_cache=False, 
     //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
-    100%|██████████| 1000000/1000000 [00:12<00:00, 81258.92vector/s]
+    100%|██████████| 1000000/1000000 [00:14<00:00, 69817.44vector/s]
 
 
       - Query sample id:  0
       - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (1000000, 1024)
-    | - Query time: 0.52161 s
+    | - Database Shape: (1000000, 1024)
+    | - Query Time: 0.30313 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [     0 126163 934623 376250 136782 927723  67927 454821 909201 226748]
-    | - Top 10 results similarity: [0.996918 0.783403 0.779208 0.778662 0.778039 0.777809 0.777673 0.777481
+    | - Top 10 Results Index: [     0 126163 934623 376250 136782 927723  67927 454821 909201 226748]
+    | - Top 10 Results Similarity: [0.996918 0.783403 0.779208 0.778662 0.778039 0.777809 0.777673 0.777481
      0.777456 0.777079]
     * - END OF REPORT -
     
 
 
 ### Bulk add vectors
 
@@ -260,19 +255,20 @@
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
       - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.10599 s
+    | - Database Shape: (100000, 1024)
+    | - Query Time: 0.03939 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [    0 67927 53447 47665 13859  5788 41949 64134 38082 18507]
-    | - Top 10 results similarity: [0.997411 0.778021 0.774815 0.774266 0.77306  0.77304  0.772899 0.772897
+    | - Top 10 Results Index: [    0 67927 53447 47665 13859  5788 41949 64134 38082 18507]
+    | - Top 10 Results Similarity: [0.997411 0.778021 0.774815 0.774266 0.77306  0.77304  0.772899 0.772897
      0.772079 0.771447]
     * - END OF REPORT -
     
 
 
 ### Use field to improve Searching Recall
 
@@ -331,19 +327,20 @@
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.08010 s
+    | - Database Shape: (100000, 1024)
+    | - Query Time: 0.00303 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [ 0 60 76 63 52 14 27 61 83 79]
-    | - Top 10 results similarity: [0.997411 0.75152  0.748989 0.748342 0.746665 0.745256 0.743775 0.739018
+    | - Top 10 Results Index: [ 0 60 76 63 52 14 27 61 83 79]
+    | - Top 10 Results Similarity: [0.997411 0.75152  0.748989 0.748342 0.746665 0.745256 0.743775 0.739018
      0.730766 0.728236]
     * - END OF REPORT -
     
 
 
 ### Use subset_indices to narrow down the search range
 
@@ -401,19 +398,20 @@
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.05818 s
+    | - Database Shape: (100000, 1024)
+    | - Query Time: 0.00596 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [ 0  9 14  7  3  1 19 18  8 17]
-    | - Top 10 results similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
+    | - Top 10 Results Index: [ 0  9 14  7  3  1 19 18  8 17]
+    | - Top 10 Results Similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
      0.737088   0.734952   0.733552   0.730605  ]
     * - END OF REPORT -
     
 
 
 ### Conduct searches by specifying both subset_indices and fields simultaneously.
 
@@ -473,16 +471,17 @@
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.00418 s
+    | - Database Shape: (100000, 1024)
+    | - Query Time: 0.00638 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [ 0  9 14  7  3  1 19 18  8 17]
-    | - Top 10 results similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
+    | - Top 10 Results Index: [ 0  9 14  7  3  1 19 18  8 17]
+    | - Top 10 Results Similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
      0.737088   0.734952   0.733552   0.730605  ]
     * - END OF REPORT -
```

### Comparing `minvectordb-0.2.6/MinVectorDB.egg-info/SOURCES.txt` & `minvectordb-0.2.7/MinVectorDB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.6/PKG-INFO` & `minvectordb-0.2.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MinVectorDB
-Version: 0.2.6
+Version: 0.2.7
 Summary: MinVectorDB is a pure Python-implemented, lightweight, serverless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
 Home-page: https://github.com/BirchKwok/MinVectorDB
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: vector database
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -34,17 +34,14 @@
 <div align="center">
   <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
   <h3>A pure Python-implemented, lightweight, serverless, locally deployed vector database.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
-    <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/dm/MinVectorDB" alt="PyPI - Downloads"></a>
-    <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/implementation/MinVectorDB" alt="PyPI - Implementation"></a>
-    <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/wheel/MinVectorDB" alt="PyPI - Wheel"></a>
     <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
   </p>
 </div>
 
 ⚡ **Serverless, simple parameters, simple API.**
 
 ⚡ **Fast, memory-efficient, easily scales to millions of vectors.**
@@ -100,37 +97,33 @@
 # clustering settings
 # kmeans epochs
 os.environ['MVDB_KMEANS_EPOCHS'] = '500'  # default: 100
 
 # query cache size
 os.environ['MVDB_QUERY_CACHE_SIZE'] = '10000'  # default: 10000
 
-# cosine similarity threshold for cache result matching 
-os.environ['MVDB_COSINE_SIMILARITY_THRESHOLD'] = '0.9'  # 'None' for disable this feature, default to 0.85
-
 # specify the number of chunks in the memory cache
 os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20'  # default to '20', must be integer-like string
 ```
 
 
 ```python
 import min_vec
 print("MinVectorDB version is: ", min_vec.__version__)
 print("MinVectorDB all configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in min_vec.get_all_configs().items()]))
 ```
 
-    MinVectorDB version is:  0.2.5
+    MinVectorDB version is:  0.2.7
     MinVectorDB all configs:  
      - MVDB_LOG_LEVEL: INFO
      - MVDB_LOG_PATH: ./min_vec_db.log
      - MVDB_TRUNCATE_LOG: True
      - MVDB_LOG_WITH_TIME: False
      - MVDB_KMEANS_EPOCHS: 500
      - MVDB_QUERY_CACHE_SIZE: 10000
-     - MVDB_COSINE_SIMILARITY_THRESHOLD: 0.9
      - MVDB_DATALOADER_BUFFER_SIZE: 20
 
 
 ### Sequentially add vectors.
 
 
 ```python
@@ -145,15 +138,15 @@
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
 # distance can be 'L2' or 'cosine'
 # index_mode can be 'FLAT' or 'IVF-FLAT', default is 'IVF-FLAT'
 db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', index_mode='FLAT',
-                 chunk_size=100000, use_cache=False, scaler_bits=8, n_threads=10, distance='cosine')
+                 chunk_size=100000, use_cache=False, scaler_bits=8, n_threads=10)
 
 # ========== Use automatic commit statements. Recommended. =============
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():
     # Define the initial ID.
     id = 0
     for t in tqdm(get_test_vectors((1000000, 1024)), total=1000000, unit="vector"):
@@ -162,48 +155,50 @@
             query_id = 0
             query_field = None
         # Vectors will be normalized after writing to the database.
         db.add_item(t, index=id)
 
         id += 1
 
-res = db.query(query, k=10, return_similarity=True)
+res = db.query(query, k=10, return_similarity=True, distance='cosine')
 
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
+
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
     //    n_clusters=16, chunk_size=100000,
     //    distance='cosine', index_mode='FLAT', 
-    //    dtypes='float32', use_cache=True, 
+    //    dtypes='float32', use_cache=False, 
     //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
-    100%|██████████| 1000000/1000000 [00:12<00:00, 81258.92vector/s]
+    100%|██████████| 1000000/1000000 [00:14<00:00, 69817.44vector/s]
 
 
       - Query sample id:  0
       - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (1000000, 1024)
-    | - Query time: 0.52161 s
+    | - Database Shape: (1000000, 1024)
+    | - Query Time: 0.30313 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [     0 126163 934623 376250 136782 927723  67927 454821 909201 226748]
-    | - Top 10 results similarity: [0.996918 0.783403 0.779208 0.778662 0.778039 0.777809 0.777673 0.777481
+    | - Top 10 Results Index: [     0 126163 934623 376250 136782 927723  67927 454821 909201 226748]
+    | - Top 10 Results Similarity: [0.996918 0.783403 0.779208 0.778662 0.778039 0.777809 0.777673 0.777481
      0.777456 0.777079]
     * - END OF REPORT -
     
 
 
 ### Bulk add vectors
 
@@ -260,19 +255,20 @@
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
       - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.10599 s
+    | - Database Shape: (100000, 1024)
+    | - Query Time: 0.03939 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [    0 67927 53447 47665 13859  5788 41949 64134 38082 18507]
-    | - Top 10 results similarity: [0.997411 0.778021 0.774815 0.774266 0.77306  0.77304  0.772899 0.772897
+    | - Top 10 Results Index: [    0 67927 53447 47665 13859  5788 41949 64134 38082 18507]
+    | - Top 10 Results Similarity: [0.997411 0.778021 0.774815 0.774266 0.77306  0.77304  0.772899 0.772897
      0.772079 0.771447]
     * - END OF REPORT -
     
 
 
 ### Use field to improve Searching Recall
 
@@ -331,19 +327,20 @@
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.08010 s
+    | - Database Shape: (100000, 1024)
+    | - Query Time: 0.00303 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [ 0 60 76 63 52 14 27 61 83 79]
-    | - Top 10 results similarity: [0.997411 0.75152  0.748989 0.748342 0.746665 0.745256 0.743775 0.739018
+    | - Top 10 Results Index: [ 0 60 76 63 52 14 27 61 83 79]
+    | - Top 10 Results Similarity: [0.997411 0.75152  0.748989 0.748342 0.746665 0.745256 0.743775 0.739018
      0.730766 0.728236]
     * - END OF REPORT -
     
 
 
 ### Use subset_indices to narrow down the search range
 
@@ -401,19 +398,20 @@
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.05818 s
+    | - Database Shape: (100000, 1024)
+    | - Query Time: 0.00596 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [ 0  9 14  7  3  1 19 18  8 17]
-    | - Top 10 results similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
+    | - Top 10 Results Index: [ 0  9 14  7  3  1 19 18  8 17]
+    | - Top 10 Results Similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
      0.737088   0.734952   0.733552   0.730605  ]
     * - END OF REPORT -
     
 
 
 ### Conduct searches by specifying both subset_indices and fields simultaneously.
 
@@ -473,16 +471,17 @@
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.00418 s
+    | - Database Shape: (100000, 1024)
+    | - Query Time: 0.00638 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [ 0  9 14  7  3  1 19 18  8 17]
-    | - Top 10 results similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
+    | - Top 10 Results Index: [ 0  9 14  7  3  1 19 18  8 17]
+    | - Top 10 Results Similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
      0.737088   0.734952   0.733552   0.730605  ]
     * - END OF REPORT -
```

### Comparing `minvectordb-0.2.6/README.md` & `minvectordb-0.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 <div align="center">
   <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
   <h3>A pure Python-implemented, lightweight, serverless, locally deployed vector database.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
-    <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/dm/MinVectorDB" alt="PyPI - Downloads"></a>
-    <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/implementation/MinVectorDB" alt="PyPI - Implementation"></a>
-    <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/wheel/MinVectorDB" alt="PyPI - Wheel"></a>
     <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
   </p>
 </div>
 
 ⚡ **Serverless, simple parameters, simple API.**
 
 ⚡ **Fast, memory-efficient, easily scales to millions of vectors.**
@@ -67,37 +64,33 @@
 # clustering settings
 # kmeans epochs
 os.environ['MVDB_KMEANS_EPOCHS'] = '500'  # default: 100
 
 # query cache size
 os.environ['MVDB_QUERY_CACHE_SIZE'] = '10000'  # default: 10000
 
-# cosine similarity threshold for cache result matching 
-os.environ['MVDB_COSINE_SIMILARITY_THRESHOLD'] = '0.9'  # 'None' for disable this feature, default to 0.85
-
 # specify the number of chunks in the memory cache
 os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20'  # default to '20', must be integer-like string
 ```
 
 
 ```python
 import min_vec
 print("MinVectorDB version is: ", min_vec.__version__)
 print("MinVectorDB all configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in min_vec.get_all_configs().items()]))
 ```
 
-    MinVectorDB version is:  0.2.5
+    MinVectorDB version is:  0.2.7
     MinVectorDB all configs:  
      - MVDB_LOG_LEVEL: INFO
      - MVDB_LOG_PATH: ./min_vec_db.log
      - MVDB_TRUNCATE_LOG: True
      - MVDB_LOG_WITH_TIME: False
      - MVDB_KMEANS_EPOCHS: 500
      - MVDB_QUERY_CACHE_SIZE: 10000
-     - MVDB_COSINE_SIMILARITY_THRESHOLD: 0.9
      - MVDB_DATALOADER_BUFFER_SIZE: 20
 
 
 ### Sequentially add vectors.
 
 
 ```python
@@ -112,15 +105,15 @@
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
 # distance can be 'L2' or 'cosine'
 # index_mode can be 'FLAT' or 'IVF-FLAT', default is 'IVF-FLAT'
 db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', index_mode='FLAT',
-                 chunk_size=100000, use_cache=False, scaler_bits=8, n_threads=10, distance='cosine')
+                 chunk_size=100000, use_cache=False, scaler_bits=8, n_threads=10)
 
 # ========== Use automatic commit statements. Recommended. =============
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():
     # Define the initial ID.
     id = 0
     for t in tqdm(get_test_vectors((1000000, 1024)), total=1000000, unit="vector"):
@@ -129,48 +122,50 @@
             query_id = 0
             query_field = None
         # Vectors will be normalized after writing to the database.
         db.add_item(t, index=id)
 
         id += 1
 
-res = db.query(query, k=10, return_similarity=True)
+res = db.query(query, k=10, return_similarity=True, distance='cosine')
 
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
+
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
     //    n_clusters=16, chunk_size=100000,
     //    distance='cosine', index_mode='FLAT', 
-    //    dtypes='float32', use_cache=True, 
+    //    dtypes='float32', use_cache=False, 
     //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
-    100%|██████████| 1000000/1000000 [00:12<00:00, 81258.92vector/s]
+    100%|██████████| 1000000/1000000 [00:14<00:00, 69817.44vector/s]
 
 
       - Query sample id:  0
       - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (1000000, 1024)
-    | - Query time: 0.52161 s
+    | - Database Shape: (1000000, 1024)
+    | - Query Time: 0.30313 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [     0 126163 934623 376250 136782 927723  67927 454821 909201 226748]
-    | - Top 10 results similarity: [0.996918 0.783403 0.779208 0.778662 0.778039 0.777809 0.777673 0.777481
+    | - Top 10 Results Index: [     0 126163 934623 376250 136782 927723  67927 454821 909201 226748]
+    | - Top 10 Results Similarity: [0.996918 0.783403 0.779208 0.778662 0.778039 0.777809 0.777673 0.777481
      0.777456 0.777079]
     * - END OF REPORT -
     
 
 
 ### Bulk add vectors
 
@@ -227,19 +222,20 @@
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
       - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.10599 s
+    | - Database Shape: (100000, 1024)
+    | - Query Time: 0.03939 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [    0 67927 53447 47665 13859  5788 41949 64134 38082 18507]
-    | - Top 10 results similarity: [0.997411 0.778021 0.774815 0.774266 0.77306  0.77304  0.772899 0.772897
+    | - Top 10 Results Index: [    0 67927 53447 47665 13859  5788 41949 64134 38082 18507]
+    | - Top 10 Results Similarity: [0.997411 0.778021 0.774815 0.774266 0.77306  0.77304  0.772899 0.772897
      0.772079 0.771447]
     * - END OF REPORT -
     
 
 
 ### Use field to improve Searching Recall
 
@@ -298,19 +294,20 @@
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.08010 s
+    | - Database Shape: (100000, 1024)
+    | - Query Time: 0.00303 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [ 0 60 76 63 52 14 27 61 83 79]
-    | - Top 10 results similarity: [0.997411 0.75152  0.748989 0.748342 0.746665 0.745256 0.743775 0.739018
+    | - Top 10 Results Index: [ 0 60 76 63 52 14 27 61 83 79]
+    | - Top 10 Results Similarity: [0.997411 0.75152  0.748989 0.748342 0.746665 0.745256 0.743775 0.739018
      0.730766 0.728236]
     * - END OF REPORT -
     
 
 
 ### Use subset_indices to narrow down the search range
 
@@ -368,19 +365,20 @@
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.05818 s
+    | - Database Shape: (100000, 1024)
+    | - Query Time: 0.00596 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [ 0  9 14  7  3  1 19 18  8 17]
-    | - Top 10 results similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
+    | - Top 10 Results Index: [ 0  9 14  7  3  1 19 18  8 17]
+    | - Top 10 Results Similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
      0.737088   0.734952   0.733552   0.730605  ]
     * - END OF REPORT -
     
 
 
 ### Conduct searches by specifying both subset_indices and fields simultaneously.
 
@@ -440,16 +438,17 @@
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.00418 s
+    | - Database Shape: (100000, 1024)
+    | - Query Time: 0.00638 s
+    | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 results index: [ 0  9 14  7  3  1 19 18  8 17]
-    | - Top 10 results similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
+    | - Top 10 Results Index: [ 0  9 14  7  3  1 19 18  8 17]
+    | - Top 10 Results Similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
      0.737088   0.734952   0.733552   0.730605  ]
     * - END OF REPORT -
```

### Comparing `minvectordb-0.2.6/min_vec/api/api.py` & `minvectordb-0.2.7/min_vec/api/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 
 class MinVectorDB:
     """
     A class for managing a vector database stored in .mvdb files and computing vectors similarity.
     """
 
     @ParametersValidator(
-        update_configs=['dim', 'database_path', 'n_clusters', 'chunk_size', 'index_mode', 'dtypes', 'scaler_bits',
-                        'distance'],
+        update_configs=['dim', 'n_clusters', 'chunk_size', 'index_mode', 'dtypes', 'scaler_bits'],
         logger=logger
     )
     @ParameterTypeAssert({
         'dim': int,
         'database_path': str,
         'n_clusters': int,
         'chunk_size': int,
@@ -44,15 +43,15 @@
         'scaler_bits': (None, int),
         'n_threads': (None, int),
         'warm_up': bool
     }, func_name='MinVectorDB')
     def __init__(
             self, dim: int, database_path: str, n_clusters: int = 16, chunk_size: int = 100_000,
             distance: str = 'cosine', index_mode: str = 'IVF-FLAT', dtypes: str = 'float32',
-            use_cache: bool = True, scaler_bits: int = 8, n_threads: int = None,
+            use_cache: bool = True, scaler_bits: Union[int, None] = 8, n_threads: Union[int, None] = 10,
             warm_up: bool = False
     ) -> None:
         """
         Initialize the vector database.
 
         Parameters:
             dim (int): Dimension of the vectors.
@@ -65,17 +64,17 @@
                 Options are 'FLAT' or 'IVF-FLAT'. Default is 'IVF-FLAT'.
             dtypes (str): The data type of the vectors. Default is 'float32'.
                 Options are 'float16', 'float32' or 'float64'.
             use_cache (bool): Whether to use cache for query. Default is True.
             scaler_bits (int): The number of bits for scalar quantization.
                 Options are 8, 16, or 32. The default is None, which means no scalar quantization.
                 The 8 for 8-bit, 16 for 16-bit, and 32 for 32-bit.
-            n_threads (int): The number of threads to use for parallel processing. Default is None, which means using
-                twice the number of CPU cores.
+            n_threads (int): The number of threads to use for parallel processing. Default is 10.
             warm_up (bool): Whether to warm up the database. Default is False.
+                .. versionadded:: 0.2.6
 
         Raises:
             ValueError: If `chunk_size` is less than or equal to 1.
         """
         raise_if(ValueError, not str(database_path).endswith('mvdb'), 'database_path must end with .mvdb')
         raise_if(ValueError, chunk_size <= 1, 'chunk_size must greater than 1')
         raise_if(ValueError, distance not in ('cosine', 'L2'), 'distance must be "cosine" or "L2"')
@@ -98,15 +97,14 @@
             raise ValueError('chunk_size must be greater than 1')
 
         self._matrix_serializer = MatrixSerializer(
             dim=dim,
             database_path=database_path,
             n_clusters=n_clusters,
             chunk_size=chunk_size,
-            distance=distance,
             index_mode=index_mode,
             logger=logger,
             dtypes=dtypes,
             scaler_bits=scaler_bits,
             warm_up=warm_up
         )
         self._data_loader = self._matrix_serializer.iterable_dataloader
@@ -117,15 +115,16 @@
         self._distance = distance
 
         raise_if(TypeError, n_threads is not None and not isinstance(n_threads, int), "n_threads must be an integer.")
         raise_if(ValueError, n_threads is not None and n_threads <= 0, "n_threads must be greater than 0.")
 
         self._query = Query(
             matrix_serializer=self._matrix_serializer,
-            n_threads=n_threads if n_threads else min(32, os.cpu_count() + 4)
+            n_threads=n_threads if n_threads else min(32, os.cpu_count() + 4),
+            distance=distance
         )
 
         self._query.query.clear_cache()
 
         self._most_recent_query_report = {}
 
     @unavailable_if_deleted
@@ -167,54 +166,89 @@
         """
         Save the database, ensuring that all data is written to disk.
         This method is required to be called after saving vectors to query them.
         """
         self._matrix_serializer.commit()
 
     @unavailable_if_deleted
-    def query(self, vector: np.ndarray, k: Union[int, str] = 12, *, fields: List = None, subset_indices: List = None,
+    def query(self, vector: np.ndarray, k: int = 12, *,
+              fields: Union[List, None] = None,
+              subset_indices: Union[List, None] = None,
+              distance: Union[str, None] = None,
               return_similarity: bool = True):
         """
         Query the database for the vectors most similar to the given vector in batches.
 
         Parameters:
             vector (np.ndarray): The query vector.
-            k (int or str): The number of nearest vectors to return. if be 'all', return all vectors.
+            k (int): The number of nearest vectors to return.
             fields (list, optional): The target of the vector.
             subset_indices (list, optional): The subset of indices to query.
+            distance (str): The distance metric to use for the query.
+                .. versionadded:: 0.2.7
             return_similarity (bool): Whether to return the similarity scores.Default is True.
+                .. versionadded:: 0.2.5
 
         Returns:
             Tuple: The indices and similarity scores of the top k nearest vectors.
 
         Raises:
             ValueError: If the database is empty.
         """
         import datetime
 
+        logger.debug(f'Query vector: {vector.tolist()}')
+        logger.debug(f'Query k: {k}')
+        logger.debug(f'Query fields: {fields}')
+        logger.debug(f'Query subset_indices: {subset_indices}')
+
+        raise_if(TypeError, not isinstance(k, int) and not (isinstance(k, str) and k != 'all'),
+                 'k must be int or "all".')
+        raise_if(ValueError, k <= 0, 'k must be greater than 0.')
+        raise_if(ValueError, not isinstance(fields, list) and fields is not None,
+                 'fields must be list or None.')
+        raise_if(ValueError, not isinstance(subset_indices, list) and subset_indices is not None,
+                 'subset_indices must be list or None.')
+        raise_if(ValueError, vector is None, 'vector must be not None.')
+        raise_if(ValueError, len(vector) != self._matrix_serializer.shape[1],
+                 'vector must be same dim with database.')
+        raise_if(ValueError, not isinstance(vector, np.ndarray), 'vector must be np.ndarray.')
+        raise_if(ValueError, vector.ndim != 1, 'vector must be 1d array.')
+        raise_if(ValueError, not isinstance(return_similarity, bool), 'return_similarity must be bool.')
+        raise_if(ValueError, distance is not None and distance not in ['cosine', 'L2'],
+                 'distance must be "cosine" or "L2" or None.')
+
+        if self._matrix_serializer.shape[0] == 0:
+            raise ValueError('database is empty.')
+
+        if k > self._matrix_serializer.shape[0]:
+            k = self._matrix_serializer.shape[0]
+
         self._most_recent_query_report = {}
 
         self._timer.start()
         if self._use_cache:
             res = self._query.query(vector=vector, k=k, fields=fields,
                                     subset_indices=subset_indices, index_mode=self._matrix_serializer.index_mode,
-                                    distance=self._distance, return_similarity=return_similarity)
+                                    distance=distance, return_similarity=return_similarity)
         else:
             res = self._query.query(vector=vector, k=k, fields=fields,
                                     subset_indices=subset_indices, index_mode=self._matrix_serializer.index_mode,
-                                    now_time=datetime.datetime.now().timestamp(), distance=self._distance,
+                                    now_time=datetime.datetime.now().strftime('%Y%m%d%H%M%S%f'),
+                                    distance=distance,
                                     return_similarity=return_similarity)
 
         time_cost = self._timer.last_timestamp_diff()
-        self._most_recent_query_report['Database shape'] = self.shape
-        self._most_recent_query_report['Query time'] = f"{time_cost :>.5f} s"
+        self._most_recent_query_report['Database Shape'] = self.shape
+        self._most_recent_query_report['Query Time'] = f"{time_cost :>.5f} s"
+        self._most_recent_query_report['Query Distance'] = self._distance if distance is None else distance
         self._most_recent_query_report['Query K'] = k
-        self._most_recent_query_report[f'Top {k} results index'] = res[0]
+        self._most_recent_query_report[f'Top {k} Results Index'] = res[0]
         if return_similarity:
-            self._most_recent_query_report[f'Top {k} results similarity'] = np.array([round(i, 6) for i in res[1]])
+            self._most_recent_query_report[f'Top {k} Results Similarity'] = np.array([round(i, 6) for i in res[1]])
 
         return res
 
     @property
     def shape(self):
         """
         Return the shape of the entire database.
```

### Comparing `minvectordb-0.2.6/min_vec/computational_layer/engines.py` & `minvectordb-0.2.7/min_vec/computational_layer/engines.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import numpy as np
 import jax.numpy as jnp
 
 
 def to_normalize(vec: np.ndarray):
     if vec.ndim == 1:
         return vec / np.linalg.norm(vec)
-    elif vec.ndim == 2:
-        return vec / jnp.linalg.norm(vec, axis=1)[:, np.newaxis]
     else:
-        raise ValueError("vec must be 1d or 2d array")
+        return vec / np.linalg.norm(vec, axis=1)[:, np.newaxis]
 
 
 def cosine_distance(vec1, vec2):
-    return jnp.dot(vec2, vec1)
+    return jnp.dot(vec2, vec1).block_until_ready()
 
 
 def euclidean_distance(vec1, vec2):
-    return jnp.linalg.norm(vec1 - vec2, axis=1)
+    return jnp.linalg.norm(vec1 - vec2, axis=1).block_until_ready()
 
 
 def argsort_topk(arr, k):
     """
     Argsort the array and return the top k indices.
 
     Parameters
@@ -34,10 +32,10 @@
     -------
     np.ndarray
         The top k indices.
     """
     if k >= arr.size:
         return np.argsort(arr)
 
-    indices = jnp.argpartition(arr, k)[:k]
+    indices = np.argpartition(arr, k)[:k]
     sorted_indices = indices[np.argsort(arr[indices])]
     return sorted_indices
```

### Comparing `minvectordb-0.2.6/min_vec/configs/config.py` & `minvectordb-0.2.7/min_vec/configs/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -58,29 +58,22 @@
     def MVDB_QUERY_CACHE_SIZE(self):
         return self.get_env_variable('MVDB_QUERY_CACHE_SIZE', 10000, int, [int])
 
     @property
     def MVDB_DATALOADER_BUFFER_SIZE(self):
         return self.get_env_variable('MVDB_DATALOADER_BUFFER_SIZE', 20, int, [int, None])
 
-    @property
-    def MVDB_COSINE_SIMILARITY_THRESHOLD(self):
-        value = os.environ.get('MVDB_COSINE_SIMILARITY_THRESHOLD', 0.85)
-        return None if value == 'None' else float(value)
-
     def get_all_configs(self):
         return {
             'MVDB_LOG_LEVEL': self.MVDB_LOG_LEVEL,
             'MVDB_LOG_PATH': self.MVDB_LOG_PATH,
             'MVDB_TRUNCATE_LOG': self.MVDB_TRUNCATE_LOG,
             'MVDB_LOG_WITH_TIME': self.MVDB_LOG_WITH_TIME,
             'MVDB_KMEANS_EPOCHS': self.MVDB_KMEANS_EPOCHS,
             'MVDB_QUERY_CACHE_SIZE': self.MVDB_QUERY_CACHE_SIZE,
-            'MVDB_COSINE_SIMILARITY_THRESHOLD': self.MVDB_COSINE_SIMILARITY_THRESHOLD,
-            # 'MVDB_COMPUTE_DEVICE': self.MVDB_COMPUTE_DEVICE,
             'MVDB_DATALOADER_BUFFER_SIZE': self.MVDB_DATALOADER_BUFFER_SIZE
         }
 
 
 config = Config()
 
 get_all_configs = config.get_all_configs
```

### Comparing `minvectordb-0.2.6/min_vec/configs/parameters_validator.py` & `minvectordb-0.2.7/min_vec/configs/parameters_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 from pathlib import Path
 
 from spinesUtils.asserts import raise_if, generate_function_kwargs
 from spinesUtils.logging import Logger
 
 
 class ParametersValidator:
-    """Database configuration, define once and can not be changed."""
+    """Database configuration, define once and can not be changed.
+
+        .. versionadded:: 0.2.5
+    """
     def __init__(self, update_configs: list, logger: Logger):
         raise_if(TypeError, not isinstance(update_configs, list), "update_configs must be a list.")
 
         self.update_configs_list = update_configs
         self.logger = logger
 
     def check_configs(self, configs: dict, update_configs_dict: dict):
         """Check if the configurations are set."""
         for key, value in configs.items():
             if key not in update_configs_dict:
                 continue
             else:
                 if update_configs_dict[key] != value:
-                    self.logger.warning(f"The database configuration {key} has been set to {value}, "
+                    self.logger.warning(f"The immutable parameter `{key}` of the database has been set to {value}, "
                                         f"the new value {update_configs_dict[key]} will be ignored.")
 
         for key, value in update_configs_dict.items():
             if key not in configs:
                 self.logger.warning(f"The database configuration {key} is not set, "
                                     f"and it will be set to {value}.")
                 configs[key] = value
@@ -80,10 +83,14 @@
 
             if first_create or not configs_json.exists():
                 final_configs = self.save_configs(configs_json, update_configs_dict)
             else:
                 existing_configs = self.load_configs(configs_json)
                 final_configs = self.check_configs(existing_configs, update_configs_dict)
 
+            for i in kwargs:
+                if i not in final_configs and kwargs[i] != self_instance:
+                    final_configs[i] = kwargs[i]
+
             return func(self_instance, **final_configs)
 
         return wrapper
```

### Comparing `minvectordb-0.2.6/min_vec/data_structures/fields_mapper.py` & `minvectordb-0.2.7/min_vec/data_structures/fields_mapper.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.6/min_vec/data_structures/filter.py` & `minvectordb-0.2.7/min_vec/data_structures/filter.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.6/min_vec/data_structures/kmeans.py` & `minvectordb-0.2.7/min_vec/data_structures/kmeans.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.6/min_vec/data_structures/limited_dict.py` & `minvectordb-0.2.7/min_vec/data_structures/limited_dict.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.6/min_vec/data_structures/scaler.py` & `minvectordb-0.2.7/min_vec/data_structures/scaler.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.6/min_vec/execution_layer/cluster_worker.py` & `minvectordb-0.2.7/min_vec/execution_layer/cluster_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,30 +25,24 @@
 
     def _kmeans_clustering(self, data):
         """kmeans clustering"""
         self.ann_model = self.ann_model.partial_fit(data)
 
         return self.ann_model.labels_
 
-    def build_index(self, scaler=None, distance='cosine'):
+    def build_index(self, scaler=None):
         """
         Build the IVF index more efficiently.
         """
         max_len = 0
         # 初始化每个聚类的存储列表
         temp_clusters = {i: ([], [], []) for i in range(self.n_clusters)}
 
-        if scaler is not None and distance == 'L2':
-            decoder = scaler.decode
-        else:
-            decoder = None
-
         for data, indices, fields in self.iterable_dataloader(read_chunk_only=True, mode='lazy'):
-            decode_data = data if decoder is None else decoder(data)
-            labels = self._kmeans_clustering(decode_data)
+            labels = self._kmeans_clustering(data)
 
             # 直接按标签将数据分配到相应的聚类
             for d, idx, f, label in zip(data, indices, fields, labels):
                 temp_clusters[label][0].append(d)
                 temp_clusters[label][1].append(idx)
                 temp_clusters[label][2].append(f)
                 max_len += 1
```

### Comparing `minvectordb-0.2.6/min_vec/execution_layer/matrix_serializer.py` & `minvectordb-0.2.7/min_vec/execution_layer/matrix_serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,31 +20,28 @@
     """
     The MatrixSerializer class is used to serialize and deserialize the matrix data.
     """
     def __init__(
             self,
             dim: int,
             database_path: str,
-            distance: str,
             logger: Logger,
             n_clusters: int = 16,
             chunk_size: int = 1_000_000,
             index_mode: str = 'IVF-FLAT',
             dtypes: str = 'float32',
             scaler_bits=None,
             warm_up: bool = False
     ) -> None:
         """
         Initialize the vector database.
 
         Parameters:
             dim (int): Dimension of the vectors.
             database_path (str): Path to the database file.
-            distance (str): Method for calculating vector distance.
-                Options are 'cosine' or 'L2' for Euclidean distance.
             logger (Logger): The logger object.
             n_clusters (int): The number of clusters for the IVF-FLAT index. Default is 16.
             chunk_size (int): The size of each data chunk. Default is 1_000_000.
             index_mode (str): The index mode of the database.
                 Options are 'FLAT' or 'IVF-FLAT'. Default is 'IVF-FLAT'.
             dtypes (str): The data type of the vectors. Default is 'float32'.
                 Options are 'float16', 'float32' or 'float64'.
@@ -67,16 +64,14 @@
         self.logger = logger
 
         # set parent path
         self._initialize_parent_path(database_path)
 
         self._dtypes_map = {'float16': np.float16, 'float32': np.float32, 'float64': np.float64}
 
-        # set distance
-        self.distance = distance
         # set dtypes
         self.dtypes = self._dtypes_map[dtypes]
         # set index mode
         self.index_mode = index_mode
         # set n_clusters
         self.n_clusters = n_clusters
         # set dim
@@ -118,36 +113,20 @@
             iterable_dataloader=self.iterable_dataloader,
             ann_model=self.ann_model,
             storage_worker=self.storage_worker,
             save_data=self.save_data,
             n_clusters=self.n_clusters
         )
 
-        # save initial parameters
-        self._write_params(dtypes=dtypes)
-
         if self._get_cluster_dataset_num() > 0 and self.index_mode == 'FLAT':
             # cause the index mode is FLAT, but the cluster dataset is not empty,
             # so the clustered datasets will also be traversed during querying.
             self.logger.warning('The index mode is FLAT, but the cluster dataset is not empty, '
                                 'so the clustered datasets will also be traversed during querying.')
 
-    def _write_params(self, dtypes):
-        attrs = {
-            'dim': self.dim,
-            'chunk_size': self.chunk_size,
-            'distance': self.distance,
-            'dtypes': dtypes
-        }
-
-        if self.scaler_bits is not None:
-            attrs['sq_bits'] = self.scaler_bits
-
-        self.storage_worker.write_file_attributes(attrs)
-
     def _initialize_parent_path(self, database_path):
         """make directory if not exist"""
         self.database_path_parent = Path(database_path).parent.absolute() / Path(
             '.mvdb'.join(Path(database_path).absolute().name.split('.mvdb')[:-1]))
 
         self.database_path_parent.mkdir(parents=True, exist_ok=True)
 
@@ -352,17 +331,14 @@
 
                 # save ivf index and k-means model
                 self.logger.debug('Saving ann model...')
                 self.ann_model.save(self.database_path_parent / 'ann_model.mvdb')
 
             self.reset_database()
 
-            # save params
-            self.storage_worker.write_file_attributes({'index_mode': self.index_mode})
-
             if self.scaler_bits is not None:
                 self.scaler.save(self.database_path_parent / 'sq_model.mvdb')
 
             self.COMMIT_FLAG = True
 
             self.last_commit_time = datetime.now()
 
@@ -515,13 +491,13 @@
         # clear cache
         self.storage_worker.clear_cache()
 
     def build_index(self):
         """
         Build the IVF index.
         """
-        self.cluster_worker.build_index(self.scaler, self.distance)
+        self.cluster_worker.build_index(self.scaler)
 
     @property
     def shape(self):
         self.check_commit()
         return tuple(self.storage_worker.get_shape(read_type='all'))
```

### Comparing `minvectordb-0.2.6/min_vec/execution_layer/query.py` & `minvectordb-0.2.7/min_vec/execution_layer/query.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 from min_vec.utils.utils import QueryVectorCache
 from min_vec.data_structures.limited_sort import LimitedSorted
 
 
 class Query:
     """Query the database for the vectors most similar to the given vector."""
 
-    def __init__(self, matrix_serializer: MatrixSerializer, n_threads=10) -> None:
+    def __init__(self, matrix_serializer: MatrixSerializer, n_threads=10, distance='cosine') -> None:
         """
         Query the database for the vectors most similar to the given vector.
 
         Parameters:
             matrix_serializer (MatrixSerializer): The database to be queried.
             n_threads (int): The number of threads to use for querying the database.
+            distance (str): The distance metric to use for the query.
+                .. versionadded:: 0.2.7
         """
         self.matrix_serializer = matrix_serializer
 
         self.logger = self.matrix_serializer.logger
         # attributes
         self.dtypes = self.matrix_serializer.dtypes
-        self.distance = self.matrix_serializer.distance
-        self.distance_func = cosine_distance if self.distance == 'cosine' else euclidean_distance
+        self.distance = distance
         self.is_reversed = -1 if self.distance == 'cosine' else 1
         self.chunk_size = self.matrix_serializer.chunk_size
 
         self.fields_mapper = self.matrix_serializer.fields_mapper
 
         self.n_threads = n_threads
 
@@ -56,138 +57,112 @@
         Returns:
             Tuple: The indices and similarity scores of the nearest vectors in the chunk.
         """
         field_condition = None
         si_condition = None
 
         if field is not None:
-            if isinstance(field, str):
-                field = [self.fields_mapper.fields_str_mapper.get(field, -1)]
-            else:
-                field = [self.fields_mapper.fields_str_mapper.get(f, -1) for f in field]
+            field = [self.fields_mapper.fields_str_mapper.get(f, -1) for f in field]
 
             field_condition = np.isin(vector_field, field)
 
-        if subset_indices is not None:
-            subset_indices = sorted(list(set(subset_indices)))
+        if subset_indices:
             si_condition = np.isin(index_chunk, subset_indices)
 
         if field_condition is not None and si_condition is not None:
             condition = np.logical_and(field_condition, si_condition)
-            database_chunk = database_chunk[condition]
-            index_chunk = index_chunk[condition]
         elif field_condition is not None:
             condition = field_condition
-            database_chunk = database_chunk[condition]
-            index_chunk = index_chunk[condition]
         elif si_condition is not None:
             condition = si_condition
+        else:
+            condition = False
+
+        if condition is not False:
             database_chunk = database_chunk[condition]
             index_chunk = index_chunk[condition]
 
         if len(index_chunk) == 0:
             return [], []
 
-        if self.distance != 'cosine' and self.scaler is not None:
-            database_chunk = self.scaler.decode(database_chunk)
-
         # Distance calculation core code
-        scores = self.distance_func(vector, database_chunk)
+        scores = cosine_distance(vector, database_chunk)
 
-        if scores.ndim == 0:
-            scores = np.array([scores])
-        elif scores.ndim == 2:
-            scores = scores.squeeze()
+        if scores.ndim != 1:
+            if scores.ndim == 0:
+                scores = np.array([scores])
+            elif scores.ndim == 2:
+                scores = scores.squeeze()
 
-        if limited_sorted is not None and self.distance == 'cosine':
+        if limited_sorted is not None:
             limited_sorted.add(scores, index_chunk, database_chunk)
 
         return index_chunk, scores
 
     @QueryVectorCache(config.MVDB_QUERY_CACHE_SIZE)
-    def query(self, vector, k = 12,
-              fields = None, subset_indices=None, return_similarity=False, **kwargs):
+    def query(self, vector, k=12,
+              fields=None, subset_indices=None, distance=None, return_similarity=False, **kwargs):
         """
         Query the database for the vectors most similar to the given vector in batches.
 
         Parameters:
             vector (np.ndarray): The query vector.
-            k (int or str): The number of nearest vectors to return. if be 'all', return all vectors.
+            k (int): The number of nearest vectors to return.
             fields (list, optional): The target of the vector.
             subset_indices (list, optional): The subset of indices to query.
+            distance (str): The distance metric to use for the query.
+                .. versionadded:: 0.2.7
             return_similarity (bool): Whether to return the similarity scores of the nearest vectors.
+                .. versionadded:: 0.2.5
 
         Returns:
             Tuple: The indices and similarity scores of the top k nearest vectors.
 
         Raises:
             ValueError: If the database is empty.
         """
-        self.logger.debug(f'Query vector: {vector.tolist()}')
-        self.logger.debug(f'Query k: {k}')
-        self.logger.debug(f'Query fields: {fields}')
-        self.logger.debug(f'Query subset_indices: {subset_indices}')
-
-        raise_if(TypeError, not isinstance(k, int) and not (isinstance(k, str) and k != 'all'),
-                 'k must be int or "all".')
-        raise_if(ValueError, k <= 0, 'k must be greater than 0.')
-        raise_if(ValueError, not isinstance(fields, list) and fields is not None,
-                 'fields must be list or None.')
-        raise_if(ValueError, not isinstance(subset_indices, list) and subset_indices is not None,
-                 'subset_indices must be list or None.')
-        raise_if(ValueError, vector is None, 'vector must be not None.')
-        raise_if(ValueError, len(vector) != self.matrix_serializer.shape[1],
-                 'vector must be same dim with database.')
-        raise_if(ValueError, not isinstance(vector, np.ndarray), 'vector must be np.ndarray.')
-        raise_if(ValueError, vector.ndim != 1, 'vector must be 1d array.')
-
-        if self.matrix_serializer.shape[0] == 0:
-            raise ValueError('database is empty.')
-
-        if k > self.matrix_serializer.shape[0]:
-            k = self.matrix_serializer.shape[0]
+        if distance is not None:
+            is_reversed = -1 if distance == 'cosine' else 1
+        else:
+            is_reversed = self.is_reversed
+            distance = self.distance
 
         vector = vector.astype(self.dtypes) if vector.dtype != self.dtypes else vector
 
         vector = to_normalize(vector)
 
-        if self.scaler is not None and return_similarity and self.distance == 'cosine':
-            limited_sorted = LimitedSorted(vector, k, self.scaler)
+        if return_similarity:
+            limited_sorted = LimitedSorted(vector, k, self.scaler, distance=distance, chunk_size=self.chunk_size)
         else:
             limited_sorted = None
 
         all_scores = []
         all_index = []
 
         def sort_results(all_s, all_i):
-            all_scores_i = np.array(all_s)
-            all_index_i = np.array(all_i)
-
-            top_k_indices = argsort_topk(self.is_reversed * all_scores_i, k)
-
-            return all_index_i[top_k_indices], all_scores_i[top_k_indices]
+            return np.array(all_i)[argsort_topk(is_reversed * np.array(all_s), k)], None
 
         def batch_query(vector, fields=None, subset_indices=None, is_ivf=True, cluster_id=None, sort=True):
             nonlocal all_scores, all_index, limited_sorted
 
             dataloader = self.matrix_serializer.cluster_dataloader(cluster_id, mode='lazy') \
                 if is_ivf and self.matrix_serializer.ann_model \
                 else self.matrix_serializer.iterable_dataloader(mode='lazy')
 
             futures = [i for i in self.executors.map(
                 lambda x: self._query_chunk(x[0], x[1], x[2], vector, fields,
                                             subset_indices, limited_sorted), dataloader)
                        if len(i[0]) != 0]
 
-            if not futures:
-                return [], []
-
-            if return_similarity and self.scaler is not None and sort and self.distance == 'cosine':
+            if return_similarity and sort:
                 return limited_sorted.get_top_n()
 
+            if not futures:
+                return None, None
+
             index, scores = zip(*futures)
 
             # if index[0] is iterable, then index is a tuple of numpy ndarray, so we need to flatten it
             if len(index[0].shape) > 0:
                 index = np.concatenate(index).ravel()
                 scores = np.concatenate(scores).ravel()
 
@@ -197,31 +172,25 @@
             return sort_results(all_scores, all_index) if sort else None
 
         # if the index mode is FLAT, use FLAT
         if not (self.matrix_serializer.ann_model is not None and self.matrix_serializer.ann_model.fitted):
             return batch_query(vector, fields, subset_indices, False)
 
         # otherwise, use IVF-FLAT
-        if self.distance != 'cosine' and self.scaler is not None:
-            cluster_distances = self.distance_func(vector,
-                                                   self.scaler.decode(
-                                                       self.matrix_serializer.ann_model.cluster_centers_)).squeeze()
-        else:
-            cluster_distances = self.distance_func(vector, self.matrix_serializer.ann_model.cluster_centers_).squeeze()
-
-        cluster_id_sorted = np.argsort(cluster_distances)[::-1] if self.distance == 'cosine' else np.argsort(
-            cluster_distances)
+        cluster_id_sorted = np.argsort(
+            -cosine_distance(vector, self.matrix_serializer.ann_model.cluster_centers_)
+        )
 
         for cluster_id in cluster_id_sorted:
-            batch_query(vector, fields, subset_indices, cluster_id=str(cluster_id), sort=False)
+            batch_query(vector, fields, subset_indices, cluster_id=cluster_id, sort=False)
 
             if len(all_index) >= k:
                 break
 
-        if return_similarity and self.scaler is not None and self.distance == 'cosine':
+        if return_similarity:
             return limited_sorted.get_top_n()
 
         return sort_results(all_scores, all_index)
 
     def __del__(self):
         self.executors.shutdown(wait=True)
         self.logger.debug('DatabaseQuery executor shutdown.')
```

### Comparing `minvectordb-0.2.6/min_vec/storage_layer/storage.py` & `minvectordb-0.2.7/min_vec/storage_layer/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,26 +316,14 @@
                 shape[0] += len(data)
             return shape
 
         elif read_type == 'all':
             with open(self.database_path / 'info.json', 'r') as f:
                 return json.load(f)['total_shape']
 
-    def write_file_attributes(self, attributes):
-        """Write the attributes to the file."""
-        # use json to save the attributes
-        with open(self.database_path / 'attributes.json', 'w') as f:
-            json.dump(attributes, f)
-
-    def read_file_attributes(self):
-        """Read the attributes from the file."""
-        # use json to read the attributes
-        with open(self.database_path / 'attributes.json', 'r') as f:
-            return json.load(f)
-
     def delete_chunk(self):
         """Delete the chunk files."""
         for file in self.database_chunk_path.glob('*'):
             file.unlink()
         for file in self.database_chunk_indices_path.glob('*'):
             file.unlink()
         for file in self.database_chunk_fields_path.glob('*'):
```

### Comparing `minvectordb-0.2.6/min_vec/utils/utils.py` & `minvectordb-0.2.7/min_vec/utils/utils.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.6/setup.py` & `minvectordb-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='MinVectorDB',
-    version="0.2.6",
+    version="0.2.7",
     description='MinVectorDB is a pure Python-implemented, lightweight, serverless vector, locally deployed database' \
                 'that offers clear and concise Python APIs, aimed at lowering the barrier to ' \
                 'the use of vector databases.',
     keywords='vector database',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `minvectordb-0.2.6/test/test_initial.py` & `minvectordb-0.2.7/test/test_initial.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.6/test/test_save_and_query.py` & `minvectordb-0.2.7/test/test_save_and_query.py`

 * *Files identical despite different names*

