# Comparing `tmp/storey-1.7.7.tar.gz` & `tmp/storey-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storey-1.7.7.tar", last modified: Mon Apr  8 05:36:30 2024, max compression
+gzip compressed data, was "storey-1.7.8.tar", last modified: Wed Apr 17 05:51:24 2024, max compression
```

## Comparing `storey-1.7.7.tar` & `storey-1.7.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.523840 storey-1.7.7/
--rw-r--r--   0 root         (0) root         (0)        5 2024-01-04 06:46:34.000000 storey-1.7.7/.dockerignore
--rw-r--r--   0 root         (0) root         (0)    11357 2024-01-04 06:46:34.000000 storey-1.7.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      132 2024-01-04 06:46:34.000000 storey-1.7.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5951 2024-04-08 05:36:30.523840 storey-1.7.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4522 2024-01-04 14:25:54.000000 storey-1.7.7/README.md
--rw-r--r--   0 root         (0) root         (0)      292 2024-01-08 07:57:42.000000 storey-1.7.7/dev-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.514840 storey-1.7.7/integration/
--rw-r--r--   0 root         (0) root         (0)      571 2024-01-04 06:46:34.000000 storey-1.7.7/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5863 2024-01-04 06:46:34.000000 storey-1.7.7/integration/conftest.py
--rw-r--r--   0 root         (0) root         (0)     9748 2024-01-04 06:46:34.000000 storey-1.7.7/integration/integration_test_utils.py
--rw-r--r--   0 root         (0) root         (0)   170276 2024-01-04 06:46:34.000000 storey-1.7.7/integration/test_aggregation_integration.py
--rw-r--r--   0 root         (0) root         (0)    10034 2024-01-08 07:57:42.000000 storey-1.7.7/integration/test_azure_filesystem_integration.py
--rw-r--r--   0 root         (0) root         (0)    21267 2024-01-04 06:46:34.000000 storey-1.7.7/integration/test_filesystems_integration.py
--rw-r--r--   0 root         (0) root         (0)    45491 2024-01-28 10:46:13.000000 storey-1.7.7/integration/test_flow_integration.py
--rw-r--r--   0 root         (0) root         (0)     4316 2024-04-07 10:20:23.000000 storey-1.7.7/integration/test_kafka_integration.py
--rw-r--r--   0 root         (0) root         (0)     3179 2024-01-04 06:46:34.000000 storey-1.7.7/integration/test_redis_specific.py
--rw-r--r--   0 root         (0) root         (0)    10355 2024-01-08 07:57:42.000000 storey-1.7.7/integration/test_s3_filesystem_integration.py
--rw-r--r--   0 root         (0) root         (0)      482 2024-03-31 13:05:33.000000 storey-1.7.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       93 2024-04-08 05:36:30.524839 storey-1.7.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2524 2024-01-07 21:41:54.000000 storey-1.7.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.517840 storey-1.7.7/storey/
--rw-r--r--   0 root         (0) root         (0)     3118 2024-04-08 05:36:22.000000 storey-1.7.7/storey/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3709 2024-01-04 06:46:34.000000 storey-1.7.7/storey/aggregation_utils.py
--rw-r--r--   0 root         (0) root         (0)    17706 2024-01-04 06:46:34.000000 storey-1.7.7/storey/aggregations.py
--rw-r--r--   0 root         (0) root         (0)     4692 2024-01-04 06:46:34.000000 storey-1.7.7/storey/dataframe.py
--rw-r--r--   0 root         (0) root         (0)    28285 2024-01-28 10:46:13.000000 storey-1.7.7/storey/drivers.py
--rw-r--r--   0 root         (0) root         (0)    15755 2024-01-04 06:46:34.000000 storey-1.7.7/storey/dtypes.py
--rw-r--r--   0 root         (0) root         (0)    51707 2024-04-07 10:20:23.000000 storey-1.7.7/storey/flow.py
--rw-r--r--   0 root         (0) root         (0)     3204 2024-04-07 10:20:23.000000 storey-1.7.7/storey/queue.py
--rw-r--r--   0 root         (0) root         (0)    27946 2024-01-04 06:46:34.000000 storey-1.7.7/storey/redis_driver.py
--rw-r--r--   0 root         (0) root         (0)    46536 2024-04-07 10:20:23.000000 storey-1.7.7/storey/sources.py
--rw-r--r--   0 root         (0) root         (0)     4928 2024-01-04 06:46:34.000000 storey-1.7.7/storey/sql_driver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.519840 storey-1.7.7/storey/steps/
--rw-r--r--   0 root         (0) root         (0)      807 2024-01-04 06:46:34.000000 storey-1.7.7/storey/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5418 2024-01-04 06:46:34.000000 storey-1.7.7/storey/steps/assertion.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-01-04 06:46:34.000000 storey-1.7.7/storey/steps/flatten.py
--rw-r--r--   0 root         (0) root         (0)      903 2024-01-04 06:46:34.000000 storey-1.7.7/storey/steps/foreach.py
--rw-r--r--   0 root         (0) root         (0)     1763 2024-01-04 06:46:34.000000 storey-1.7.7/storey/steps/partition.py
--rw-r--r--   0 root         (0) root         (0)     4620 2024-01-04 06:46:34.000000 storey-1.7.7/storey/steps/sample.py
--rw-r--r--   0 root         (0) root         (0)    81368 2024-01-04 06:46:34.000000 storey-1.7.7/storey/table.py
--rw-r--r--   0 root         (0) root         (0)    52569 2024-04-07 10:20:23.000000 storey-1.7.7/storey/targets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.520840 storey-1.7.7/storey/transformations/
--rw-r--r--   0 root         (0) root         (0)     1564 2024-01-04 06:46:34.000000 storey-1.7.7/storey/transformations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11281 2024-01-07 21:41:54.000000 storey-1.7.7/storey/utils.py
--rw-r--r--   0 root         (0) root         (0)     8226 2024-01-04 06:46:34.000000 storey-1.7.7/storey/windowed_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.522840 storey-1.7.7/storey.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5951 2024-04-08 05:36:30.000000 storey-1.7.7/storey.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1330 2024-04-08 05:36:30.000000 storey-1.7.7/storey.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 05:36:30.000000 storey-1.7.7/storey.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2024-04-08 05:36:30.000000 storey-1.7.7/storey.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-08 05:36:30.000000 storey-1.7.7/storey.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.522840 storey-1.7.7/tests/
--rw-r--r--   0 root         (0) root         (0)      571 2024-01-04 06:46:34.000000 storey-1.7.7/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)   144410 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_aggregate_by_key.py
--rw-r--r--   0 root         (0) root         (0)     4853 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_aggregate_store.py
--rw-r--r--   0 root         (0) root         (0)   135406 2024-04-07 10:20:23.000000 storey-1.7.7/tests/test_flow.py
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-07 10:20:23.000000 storey-1.7.7/tests/test_queue.py
--rw-r--r--   0 root         (0) root         (0)    11002 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_steps.py
--rw-r--r--   0 root         (0) root         (0)     2506 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_types.py
--rw-r--r--   0 root         (0) root         (0)     1547 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     1459 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_v3io.py
--rw-r--r--   0 root         (0) root         (0)     2622 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_windowed_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.720724 storey-1.7.8/
+-rw-r--r--   0 root         (0) root         (0)        5 2024-01-08 04:33:02.000000 storey-1.7.8/.dockerignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-01-08 04:33:02.000000 storey-1.7.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      132 2024-01-08 04:33:02.000000 storey-1.7.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-04-17 05:51:24.720724 storey-1.7.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-17 05:48:42.000000 storey-1.7.8/README.md
+-rw-r--r--   0 root         (0) root         (0)      292 2024-04-17 05:48:42.000000 storey-1.7.8/dev-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.710724 storey-1.7.8/integration/
+-rw-r--r--   0 root         (0) root         (0)      571 2024-01-08 04:33:02.000000 storey-1.7.8/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2024-01-08 04:33:02.000000 storey-1.7.8/integration/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     9748 2024-01-08 04:33:02.000000 storey-1.7.8/integration/integration_test_utils.py
+-rw-r--r--   0 root         (0) root         (0)   170276 2024-01-08 04:33:02.000000 storey-1.7.8/integration/test_aggregation_integration.py
+-rw-r--r--   0 root         (0) root         (0)    10034 2024-02-21 07:45:19.000000 storey-1.7.8/integration/test_azure_filesystem_integration.py
+-rw-r--r--   0 root         (0) root         (0)    21267 2024-01-08 04:33:02.000000 storey-1.7.8/integration/test_filesystems_integration.py
+-rw-r--r--   0 root         (0) root         (0)    45491 2024-02-21 07:45:19.000000 storey-1.7.8/integration/test_flow_integration.py
+-rw-r--r--   0 root         (0) root         (0)     4316 2024-04-11 08:38:21.000000 storey-1.7.8/integration/test_kafka_integration.py
+-rw-r--r--   0 root         (0) root         (0)     3179 2024-01-08 04:33:02.000000 storey-1.7.8/integration/test_redis_specific.py
+-rw-r--r--   0 root         (0) root         (0)    10355 2024-02-21 07:45:19.000000 storey-1.7.8/integration/test_s3_filesystem_integration.py
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-11 08:38:21.000000 storey-1.7.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2024-04-17 05:51:24.720724 storey-1.7.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-01-08 04:33:02.000000 storey-1.7.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.713724 storey-1.7.8/storey/
+-rw-r--r--   0 root         (0) root         (0)     3118 2024-04-17 05:51:18.000000 storey-1.7.8/storey/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2024-01-08 04:33:02.000000 storey-1.7.8/storey/aggregation_utils.py
+-rw-r--r--   0 root         (0) root         (0)    17706 2024-01-08 04:33:02.000000 storey-1.7.8/storey/aggregations.py
+-rw-r--r--   0 root         (0) root         (0)     4692 2024-01-08 04:33:02.000000 storey-1.7.8/storey/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)    28287 2024-04-17 05:48:42.000000 storey-1.7.8/storey/drivers.py
+-rw-r--r--   0 root         (0) root         (0)    15755 2024-01-08 04:33:02.000000 storey-1.7.8/storey/dtypes.py
+-rw-r--r--   0 root         (0) root         (0)    51707 2024-04-17 05:48:42.000000 storey-1.7.8/storey/flow.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2024-04-11 08:38:21.000000 storey-1.7.8/storey/queue.py
+-rw-r--r--   0 root         (0) root         (0)    27946 2024-01-08 04:33:02.000000 storey-1.7.8/storey/redis_driver.py
+-rw-r--r--   0 root         (0) root         (0)    46536 2024-04-11 08:38:21.000000 storey-1.7.8/storey/sources.py
+-rw-r--r--   0 root         (0) root         (0)     4928 2024-01-08 04:33:02.000000 storey-1.7.8/storey/sql_driver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.716724 storey-1.7.8/storey/steps/
+-rw-r--r--   0 root         (0) root         (0)      807 2024-01-08 04:33:02.000000 storey-1.7.8/storey/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5418 2024-01-08 04:33:02.000000 storey-1.7.8/storey/steps/assertion.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-01-08 04:33:02.000000 storey-1.7.8/storey/steps/flatten.py
+-rw-r--r--   0 root         (0) root         (0)      903 2024-01-08 04:33:02.000000 storey-1.7.8/storey/steps/foreach.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-01-08 04:33:02.000000 storey-1.7.8/storey/steps/partition.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2024-01-08 04:33:02.000000 storey-1.7.8/storey/steps/sample.py
+-rw-r--r--   0 root         (0) root         (0)    81360 2024-04-17 05:48:42.000000 storey-1.7.8/storey/table.py
+-rw-r--r--   0 root         (0) root         (0)    52569 2024-04-11 08:38:21.000000 storey-1.7.8/storey/targets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.716724 storey-1.7.8/storey/transformations/
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-01-08 04:33:02.000000 storey-1.7.8/storey/transformations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11281 2024-01-08 04:33:02.000000 storey-1.7.8/storey/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8226 2024-01-08 04:33:02.000000 storey-1.7.8/storey/windowed_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.719724 storey-1.7.8/storey.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-04-17 05:51:24.000000 storey-1.7.8/storey.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1330 2024-04-17 05:51:24.000000 storey-1.7.8/storey.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 05:51:24.000000 storey-1.7.8/storey.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2024-04-17 05:51:24.000000 storey-1.7.8/storey.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-17 05:51:24.000000 storey-1.7.8/storey.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.718724 storey-1.7.8/tests/
+-rw-r--r--   0 root         (0) root         (0)      571 2024-01-08 04:33:02.000000 storey-1.7.8/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   144410 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_aggregate_by_key.py
+-rw-r--r--   0 root         (0) root         (0)     4853 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_aggregate_store.py
+-rw-r--r--   0 root         (0) root         (0)   135406 2024-04-11 08:38:21.000000 storey-1.7.8/tests/test_flow.py
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-11 08:38:21.000000 storey-1.7.8/tests/test_queue.py
+-rw-r--r--   0 root         (0) root         (0)    11002 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_steps.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_types.py
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1459 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_v3io.py
+-rw-r--r--   0 root         (0) root         (0)     2622 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_windowed_store.py
```

### Comparing `storey-1.7.7/LICENSE` & `storey-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/integration/__init__.py` & `storey-1.7.8/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/integration/conftest.py` & `storey-1.7.8/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/integration/integration_test_utils.py` & `storey-1.7.8/integration/integration_test_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/integration/test_aggregation_integration.py` & `storey-1.7.8/integration/test_aggregation_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/integration/test_azure_filesystem_integration.py` & `storey-1.7.8/integration/test_azure_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/integration/test_filesystems_integration.py` & `storey-1.7.8/integration/test_filesystems_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/integration/test_flow_integration.py` & `storey-1.7.8/integration/test_flow_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/integration/test_kafka_integration.py` & `storey-1.7.8/integration/test_kafka_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/integration/test_redis_specific.py` & `storey-1.7.8/integration/test_redis_specific.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/integration/test_s3_filesystem_integration.py` & `storey-1.7.8/integration/test_s3_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/setup.py` & `storey-1.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/__init__.py` & `storey-1.7.8/storey/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.7.7"
+__version__ = "1.7.8"
 
 # Importing supported filesystems explicitly so that they will get registered as an fsspec filesystem
 import v3iofs  # noqa: F401
 
 from .aggregations import AggregateByKey, QueryByKey  # noqa: F401
 from .dataframe import ReduceToDataFrame, ToDataFrame  # noqa: F401
 from .drivers import Driver, NoopDriver, V3ioDriver  # noqa: F401
```

### Comparing `storey-1.7.7/storey/aggregation_utils.py` & `storey-1.7.8/storey/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/aggregations.py` & `storey-1.7.8/storey/aggregations.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/dataframe.py` & `storey-1.7.8/storey/dataframe.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/drivers.py` & `storey-1.7.8/storey/drivers.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,17 +504,17 @@
                             if not initialized_attributes.get(array_attribute_name, -1) == expected_time:
                                 initialized_attributes[array_attribute_name] = expected_time
                                 expressions.append(
                                     f"{array_attribute_name}=init_array({bucket.total_number_of_buckets},'double',"
                                     f"{aggregation_value.default_value})"
                                 )
                             if array_time_attribute_name not in times_update_expressions:
-                                times_update_expressions[
-                                    array_time_attribute_name
-                                ] = f"{array_time_attribute_name}={expected_time_expr}"
+                                times_update_expressions[array_time_attribute_name] = (
+                                    f"{array_time_attribute_name}={expected_time_expr}"
+                                )
                             new_cached_times[name] = (
                                 array_time_attribute_name,
                                 expected_time,
                             )
 
                         # Updating the specific cells
                         if cached_time <= expected_time:
```

### Comparing `storey-1.7.7/storey/dtypes.py` & `storey-1.7.8/storey/dtypes.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/flow.py` & `storey-1.7.8/storey/flow.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/queue.py` & `storey-1.7.8/storey/queue.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/redis_driver.py` & `storey-1.7.8/storey/redis_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/sources.py` & `storey-1.7.8/storey/sources.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/sql_driver.py` & `storey-1.7.8/storey/sql_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/steps/__init__.py` & `storey-1.7.8/storey/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/steps/assertion.py` & `storey-1.7.8/storey/steps/assertion.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/steps/flatten.py` & `storey-1.7.8/storey/steps/flatten.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/steps/foreach.py` & `storey-1.7.8/storey/steps/foreach.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/steps/partition.py` & `storey-1.7.8/storey/steps/partition.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/steps/sample.py` & `storey-1.7.8/storey/steps/sample.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/table.py` & `storey-1.7.8/storey/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1458,15 +1458,15 @@
 
         self.is_fixed_window = isinstance(self.explicit_windows, FixedWindows)
         if self.is_fixed_window:
             self._round_time_func = self.explicit_windows.round_up_time_to_window
         self.period_millis = explicit_windows.period_millis
         self._window_start_time = explicit_windows.get_window_start_time_by_time(base_time)
         if self._precalculated_aggregations:
-            for (window_millis, _) in explicit_windows.windows:
+            for window_millis, _ in explicit_windows.windows:
                 for aggr in self._all_raw_aggregates:
                     self._current_aggregate_values[(aggr, window_millis)] = AggregationValue.new_from_name(
                         aggr, max_value
                     )
 
         if initial_data:
             self.last_bucket_start_time = None
@@ -1669,15 +1669,15 @@
             or current_time_bucket_index < self.get_bucket_index_by_timestamp(self._last_data_point_timestamp)
             or not self._precalculated_aggregations
         ):
             result = self.calculate_features(timestamp)
         else:
             # In case our pre aggregates already have the answer
             for aggregation_name in self._explicit_raw_aggregations:
-                for (window_millis, window_str) in self.explicit_windows.windows:
+                for window_millis, window_str in self.explicit_windows.windows:
                     value = self._current_aggregate_values[(aggregation_name, window_millis)].value
                     count_value = self._current_aggregate_values[("count", window_millis)].value
                     if value == math.inf or value == -math.inf:
                         value = math.nan
                     if count_value == 0 and aggregation_name != "count":
                         value = math.nan
                     result[f"{self.name}_{aggregation_name}_{window_str}"] = value
@@ -1687,15 +1687,15 @@
 
     def augment_virtual_features(self, features):
         if not self._virtual_aggregations:
             return
 
         args = [None, None, None]  # Avoid in-loop allocation
         for aggregate in self._virtual_aggregations:
-            for (window_millis, window_str) in self.explicit_windows.windows:
+            for window_millis, window_str in self.explicit_windows.windows:
                 for i, aggr in enumerate(aggregate.dependant_aggregates):
                     args[i] = self._current_aggregate_values[(aggr, window_millis)].value
                 features[f"{self.name}_{aggregate.name}_{window_str}"] = aggregate.aggregation_func(args)
 
     def calculate_features(self, timestamp):
         result = {}
 
@@ -1706,15 +1706,15 @@
 
         if self.is_fixed_window:
             current_time_bucket_index = self.get_bucket_index_by_timestamp(self._round_time_func(timestamp) - 1)
 
         for aggregation_name in self._all_raw_aggregates:
             self._intermediate_aggregation_values[aggregation_name].reset()
         prev_windows_millis = 0
-        for (window_millis, window_string) in self.explicit_windows.windows:
+        for window_millis, window_string in self.explicit_windows.windows:
             # In case the current bucket is outside our time range just create a feature with the current aggregated
             # value
             if current_time_bucket_index < 0:
                 for aggregation_name in self._explicit_raw_aggregations:
                     result[f"{self.name}_{aggregation_name}_{window_string}"] = self._intermediate_aggregation_values[
                         aggregation_name
                     ].value
```

### Comparing `storey-1.7.7/storey/targets.py` & `storey-1.7.8/storey/targets.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/transformations/__init__.py` & `storey-1.7.8/storey/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/utils.py` & `storey-1.7.8/storey/utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey/windowed_store.py` & `storey-1.7.8/storey/windowed_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/storey.egg-info/SOURCES.txt` & `storey-1.7.8/storey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/tests/__init__.py` & `storey-1.7.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/tests/test_aggregate_by_key.py` & `storey-1.7.8/tests/test_aggregate_by_key.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/tests/test_aggregate_store.py` & `storey-1.7.8/tests/test_aggregate_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/tests/test_flow.py` & `storey-1.7.8/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/tests/test_queue.py` & `storey-1.7.8/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/tests/test_steps.py` & `storey-1.7.8/tests/test_steps.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/tests/test_types.py` & `storey-1.7.8/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/tests/test_utils.py` & `storey-1.7.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/tests/test_v3io.py` & `storey-1.7.8/tests/test_v3io.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.7/tests/test_windowed_store.py` & `storey-1.7.8/tests/test_windowed_store.py`

 * *Files identical despite different names*

