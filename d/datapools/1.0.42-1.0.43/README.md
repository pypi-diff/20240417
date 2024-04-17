# Comparing `tmp/datapools-1.0.42.tar.gz` & `tmp/datapools-1.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.42.tar", last modified: Mon Apr 15 13:36:18 2024, max compression
+gzip compressed data, was "datapools-1.0.43.tar", last modified: Wed Apr 17 15:03:00 2024, max compression
```

## Comparing `datapools-1.0.42.tar` & `datapools-1.0.43.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.580931 datapools-1.0.42/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 13:36:10.000000 datapools-1.0.42/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:10.000000 datapools-1.0.42/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-15 13:36:10.000000 datapools-1.0.42/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 13:36:10.000000 datapools-1.0.42/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-15 13:36:18.580931 datapools-1.0.42/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-15 13:36:10.000000 datapools-1.0.42/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.568931 datapools-1.0.42/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.568931 datapools-1.0.42/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.568931 datapools-1.0.42/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.572931 datapools-1.0.42/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.572931 datapools-1.0.42/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.572931 datapools-1.0.42/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.572931 datapools-1.0.42/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.572931 datapools-1.0.42/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.572931 datapools-1.0.42/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12113 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.572931 datapools-1.0.42/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.572931 datapools-1.0.42/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.572931 datapools-1.0.42/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.576931 datapools-1.0.42/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.576931 datapools-1.0.42/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.576931 datapools-1.0.42/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.576931 datapools-1.0.42/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.576931 datapools-1.0.42/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.576931 datapools-1.0.42/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.576931 datapools-1.0.42/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16672 2024-04-15 13:36:10.000000 datapools-1.0.42/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.576931 datapools-1.0.42/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-15 13:36:18.000000 datapools-1.0.42/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-15 13:36:18.000000 datapools-1.0.42/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:36:18.000000 datapools-1.0.42/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 13:36:18.000000 datapools-1.0.42/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-15 13:36:18.000000 datapools-1.0.42/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 13:36:18.000000 datapools-1.0.42/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:36:18.580931 datapools-1.0.42/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-15 13:36:10.000000 datapools-1.0.42/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:18.576931 datapools-1.0.42/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:36:10.000000 datapools-1.0.42/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-15 13:36:10.000000 datapools-1.0.42/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 13:36:10.000000 datapools-1.0.42/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.162591 datapools-1.0.43/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-17 15:02:48.000000 datapools-1.0.43/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:48.000000 datapools-1.0.43/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-17 15:02:48.000000 datapools-1.0.43/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 15:02:48.000000 datapools-1.0.43/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-17 15:03:00.162591 datapools-1.0.43/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-17 15:02:48.000000 datapools-1.0.43/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.154591 datapools-1.0.43/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.154591 datapools-1.0.43/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.154591 datapools-1.0.43/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.154591 datapools-1.0.43/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.154591 datapools-1.0.43/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.154591 datapools-1.0.43/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6616 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.162591 datapools-1.0.43/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.162591 datapools-1.0.43/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.162591 datapools-1.0.43/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-17 15:03:00.000000 datapools-1.0.43/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-17 15:03:00.000000 datapools-1.0.43/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:03:00.000000 datapools-1.0.43/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 15:03:00.000000 datapools-1.0.43/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-17 15:03:00.000000 datapools-1.0.43/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 15:03:00.000000 datapools-1.0.43/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:03:00.162591 datapools-1.0.43/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-17 15:02:48.000000 datapools-1.0.43/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.162591 datapools-1.0.43/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:48.000000 datapools-1.0.43/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-17 15:02:48.000000 datapools-1.0.43/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-17 15:02:48.000000 datapools-1.0.43/tests/test_base.py
```

### Comparing `datapools-1.0.42/LICENSE` & `datapools-1.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/PKG-INFO` & `datapools-1.0.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.42
+Version: 1.0.43
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.42/README.md` & `datapools-1.0.43/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/api.py` & `datapools-1.0.43/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/cli.py` & `datapools-1.0.43/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/common/backend_api.py` & `datapools-1.0.43/datapools/common/backend_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     #     return await self.get_uri( 'add-crawler-contents', { 'contents': contents } )
 
     # async def get_crawled_contents(self, limit):
     #     return await self.get_uri( 'get-crawled-contents', { 'limit': limit } )
 
     async def add_crawled_content(self, data):
         return await self.get_uri("add-crawled-content", data)
+    
+    async def add_demo_user(self, data):
+        return await self.get_uri('add-demo-user', data)
 
     # async def get_tag_datapools(self, tag_id) -> List[TagDatapool]:
     #     res = await self.get_uri(
     #         "get-tag-datapools", {"filter": {"tag_id": tag_id}}
     #     )
     #     # logger.info( f"get_tag_datapools {res=}")
     #     for i in range(len(res)):
```

### Comparing `datapools-1.0.42/datapools/common/queues/__init__.py` & `datapools-1.0.43/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/common/queues/rabbitmq.py` & `datapools-1.0.43/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/common/queues/types.py` & `datapools-1.0.43/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/common/session_manager.py` & `datapools-1.0.43/datapools/common/session_manager.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/common/stoppable.py` & `datapools-1.0.43/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/common/storage/base_storage.py` & `datapools-1.0.43/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/common/storage/file_storage.py` & `datapools-1.0.43/datapools/common/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.43/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.43/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/common/types.py` & `datapools-1.0.43/datapools/common/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 
     # None: access is configured on AWS, bucket is NOT PUBLIC
     # "": bucket is PUBLIC
     # S3_IMAGESHACK_ACCESS_KEY: Optional[str] = None
     # S3_IMAGESHACK_ACCESS_SECRET: Optional[str] = None
 
     # GOOGLE_DRIVE_API_KEY: str = ""
+    BACKEND_API_URL: str = DEFAULT_BACKEND_API_URL
 
     CLI_MODE: bool = False
 
     USE_ONLY_PLUGINS: Optional[List[str]] = None
     ADDITIONAL_PLUGINS: Optional[List[str]] = None
 
     plugins_config: dict = {}
@@ -238,15 +239,17 @@
             return 4
         raise Exception(
             f"Not supported DatapoolContentType __hash__ {self.value}"
         )
 
 
 class BaseCrawlerResult(BaseModel):
-    pass
+    def to_dict(self):
+        res = self.__dict__
+        return res
 
 
 class CrawlerContent(BaseCrawlerResult):
     tag_id: Optional[str] = None
     copyright_tag_id: Optional[str] = None
     platform_tag_id: Optional[str] = None
     type: DatapoolContentType
@@ -258,17 +261,19 @@
         res["type"] = res["type"].value
         return res
 
 
 class CrawlerBackTask(BaseCrawlerResult):
     url: str
 
-    def to_dict(self):
-        res = self.__dict__
-        return res
+    
+class CrawlerDemoUser(BaseCrawlerResult):
+    user_name: str
+    short_tag_id: str
+    platform: str
 
 
 class CrawlerNop(BaseCrawlerResult):
     pass
 
 PriorityTimestamp : TypeAlias = int
 class Evaluation(BaseModel):
```

### Comparing `datapools-1.0.42/datapools/producer/base_producer.py` & `datapools-1.0.43/datapools/producer/base_producer.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/scheduler/scheduler.py` & `datapools-1.0.43/datapools/scheduler/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
         session = self.session_manager.get(session_id)
         if session.is_stopped():
             logger.info( f'Session is stopped {session_id=}')
             return False
 
         if 'url' in task:
-            logger.info( f'{task["url"]=}')
+            #logger.info( f'{task["url"]=}')
             if not session.has_url(task['url']):
                 session.add_url(task['url'])
 
                 await self.todo_queue.push(
                     QueueMessage(session_id, QueueMessageType.Task, data=task)
                 )
             else:
```

### Comparing `datapools-1.0.42/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.43/datapools/worker/plugins/base_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 import json
 import base64
+from hashlib import md5
 from abc import abstractmethod, ABCMeta
 from typing import AsyncGenerator, Union
 from urllib.parse import urlparse, urljoin
 import dns.resolver
 from time import time
 from PIL import Image
 from PIL.ExifTags import Base as ExifTagsList
@@ -358,23 +359,27 @@
             if href is not None:
                 #logger.info( f'parse_link {href=} {type(href)=} {page.url} {type(page.url)=}')
 
                 full_local_url = BasePlugin.get_local_url(href, page.url)
                 if full_local_url:
                     # strict constraint on urls, else may get endless recursions etc
                     full_local_url = canonicalize_url(full_local_url)
-                    logger.info(full_local_url)
+                    #logger.info(full_local_url)
 
                     # logger.info( f'---------yielding {video_url=}')
                     yield CrawlerBackTask(url=full_local_url)
                     # logger.info( f'---------yielded {video_url=}')
                 else:
-                    logger.info(f"non local: {href=} {page.url=}")
+                    #logger.info(f"non local: {href=} {page.url=}")
+                    pass
 
     @staticmethod
     def make_text_storage_value(body, header=None, excerpt=None):
         data = ( (header + '\n' if header else '' ) +
                 ( excerpt + '\n' if excerpt else '' ) +
                 body
         )
         return data
-        
+        
+    @staticmethod
+    def gen_demo_tag(user_name):
+        return 'demo_' + md5(user_name.encode()).hexdigest()[-6:]
```

### Comparing `datapools-1.0.42/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.43/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/worker/plugins/default/default.py` & `datapools-1.0.43/datapools/worker/plugins/default/default.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.43/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.43/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.43/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import asyncio
 import json
 import traceback
 from typing import Union, Dict
-from hashlib import md5
 
 from playwright.async_api import TimeoutError as PlaywriteTimeoutError
 from playwright.async_api import async_playwright
 
 # import httpx
 from bs4 import BeautifulSoup
 
 from ....common.logger import logger
 from ....common.storage import BaseStorage
 from ....common.types import (
     CrawlerBackTask,
     CrawlerContent,
+    CrawlerDemoUser,
     DatapoolContentType,
 )
 from ..base_plugin import BasePlugin, BaseTag, WorkerTask
 from ....worker.utils import canonicalize_url
 
 # from typing import List
 
 DOMAIN = "imageshack.com"
 
 
 class ImageshackPlugin(BasePlugin):
-    demo_users: Dict[str, str] = {}
-
     def __init__(self, ctx, demo_tag=None):
         super().__init__(ctx)
         self.demo_tag = BaseTag( demo_tag )
 
     @staticmethod
     def is_supported(url):
         u = BasePlugin.parse_url(url)
@@ -150,17 +148,17 @@
                                 yield CrawlerBackTask(url=full_profile_url)
                                 
                                 if not self.demo_tag.is_valid():
                                     copyright_owner_tag = await self.parse_user_profile(href)
                                 else:
                                     # demo functionality for royalties spreadout demo
                                     user_name = href.split('/')[-1]
-                                    short_tag_id = md5(user_name.encode()).hexdigest()[-6:]
+                                    short_tag_id = BasePlugin.gen_demo_tag(user_name)
                                     copyright_owner_tag = BaseTag(short_tag_id)
-                                    ImageshackPlugin.demo_users[user_name] = short_tag_id
+                                    yield CrawlerDemoUser( user_name=user_name, short_tag_id=short_tag_id, platform='imageshack.com' )
 
                         if copyright_owner_tag is not None:
                             logger.info(f'found {copyright_owner_tag=}')
                             if copyright_owner_tag.is_crawling_allowed() is False:
                                 logger.info('User disabled crawling')
                                 continue
 
@@ -191,18 +189,14 @@
                                     tag_id=str(image_tag) if image_tag is not None else None,
                                     copyright_tag_id=str(copyright_owner_tag) if copyright_owner_tag is not None else None,
                                     platform_tag_id=str(platform_tag) if platform_tag is not None else None,
                                     type=DatapoolContentType.Image,
                                     storage_id=storage_id,
                                     url=full_local_url,
                                 )
-                                if self.demo_tag.is_valid():
-                                    logger.info(
-                                        '=========================================================')
-                                    logger.info(json.dumps(ImageshackPlugin.demo_users))
                                 
                             except Exception as e:
                                 logger.error(f"failed put to storage {e}")
                                 logger.error(traceback.format_exc())
                         else:
                             logger.error("failed download image")
```

### Comparing `datapools-1.0.42/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.43/datapools/worker/plugins/s3/s3.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.43/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.43/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 import json
 import requests
 from bs4 import BeautifulSoup, Comment
 from html2text import HTML2Text
 from urllib.parse import urljoin, urlparse, urlunparse
 
 from ....worker.utils import canonicalize_url
-from ..base_plugin import BasePlugin, BaseTag, WorkerTask
+from ..base_plugin import BasePlugin, BaseTag, WorkerTask, CachedPairs
 from ....common.logger import logger
 from ....common.storage import BaseStorage
 from ....common.types import (
+    CrawlerDemoUser,
     CrawlerBackTask,
     CrawlerContent,
     CrawlerNop,
     DatapoolContentType,
 )
 
 DOMAIN = "www.washingtonpost.com"
 
 
 class WashingtonPostPlugin(BasePlugin):
 
     base_url = f"https://{DOMAIN}/"
+    authors = CachedPairs()
 
     def __init__(self, ctx, demo_tag=None):
         super().__init__(ctx)
         self.demo_tag = BaseTag( demo_tag )
         
     @staticmethod
     def is_supported( url):
@@ -119,23 +121,55 @@
             if full_local_url:
                 full_local_url = canonicalize_url(full_local_url)
                 #logger.info(full_local_url)
                 yield CrawlerBackTask(url=full_local_url)
             
 
         if self.is_article(url):
+            (author_tag, user_name) = self._get_author_tag(soup, url)
+            if author_tag and not author_tag.is_crawling_allowed():
+                logger.info('crawling disabled by author tag')
+                return
+            
+            if self.demo_tag and user_name:
+                yield CrawlerDemoUser(user_name=user_name, short_tag_id=author_tag._tag, platform='washingtonpost.com')
+            
             content = self.extract(soup)
             if content:
                 storage_id = BaseStorage.gen_id(url)
                 logger.info(f"putting article into {storage_id=}")
 
                 await self.ctx.storage.put(
                     storage_id,
                     BasePlugin.make_text_storage_value(content),
                 )            
                 yield CrawlerContent(
-                    tag_id=str(platform_tag) if platform_tag is not None else None,
+                    platform_tag_id=str(platform_tag) if platform_tag is not None else None,
+                    tag_id=str(author_tag) if author_tag is not None else None,
                     type=DatapoolContentType.Text,
                     storage_id=storage_id,
                     url=url,
                 )
 
+    def _get_author_tag(self, soup, url):
+        author_link = soup.find_all('a', attrs={"data-qa":"author-name"}, href=True)
+        if len(author_link) > 0:
+            logger.info(f'Author link {author_link} {author_link[0].text}')
+            user_name = author_link[0].text
+            logger.info( f'Author name {user_name}')
+            if not self.authors.contains(user_name, 3600):
+                full_author_url = BasePlugin.get_local_url(author_link[0]['href'], url)
+                logger.info( f'{full_author_url=}')
+                response = requests.get(full_author_url)
+
+                soup2 = BeautifulSoup(response.content, 'html.parser')
+            
+                if self.demo_tag:
+                    short_tag_id = BasePlugin.gen_demo_tag(user_name)
+                    tag = BaseTag(short_tag_id)
+                else:
+                    tag = BasePlugin.parse_tag_in(soup)
+                self.authors.set( user_name, tag )
+            else:
+                tag = self.authors.get( user_name )
+            return (tag, user_name)
+        return (None, None)
```

### Comparing `datapools-1.0.42/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.43/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import asyncio
 import json
 import re
-from typing import Dict, Optional, List, Set, Union
+from typing import Dict, Optional, List, Set, Union, Tuple
 
 # from bs4 import BeautifulSoup
 # from playwright.async_api import Locator, Page
 from playwright.async_api import TimeoutError as PlaywriteTimeoutError
 from playwright.async_api import async_playwright, expect
 
 from ....common.logger import logger
 from ....common.storage import BaseStorage
 from ....common.types import (
+    CrawlerDemoUser,
     CrawlerBackTask,
     CrawlerContent,
     CrawlerNop,
     DatapoolContentType,
 )
-from ..base_plugin import BasePlugin, WorkerTask, BaseTag
+from ..base_plugin import BasePlugin, WorkerTask, BaseTag, CachedPairs
 
 # import traceback
 
 
 class WikipediaPlugin(BasePlugin):
-    users: Dict[str, Optional[str]] = {}
+    users = CachedPairs()
 
     def __init__(self, ctx, demo_tag=False):
         super().__init__(ctx)
         self.demo_tag = BaseTag(demo_tag)
 
     @staticmethod
     def is_supported(url):
         u = BasePlugin.parse_url(url)
-        # logger.info( f'dataphoenix.info {u=}')
         return BasePlugin.is_same_or_subdomain(u.netloc, "wikipedia.org")
 
     async def process(self, task: WorkerTask):
         logger.info(f"wikipedia::process({task.url})")
 
         async with async_playwright() as playwright:
             self.webkit = playwright.chromium
@@ -80,24 +80,27 @@
                 #         storage_id,
                 #         json.dumps(
                 #             {"body": body_text, "users": users}
                 #         ),  # TODO: structure
                 #     )
 
                 # TODO: until shared ownership is not supported, we use creator of the article as the copyright owner
-                creator_tag = await self._get_article_creator(history_url)
+                ( creator_tag, user_name ) = await self._get_article_creator(history_url)
                 if creator_tag and not creator_tag.is_crawling_allowed():
                     return
                 if creator_tag or platform_tag:
                     storage_id = BaseStorage.gen_id(task.url)
                     logger.info(f"putting article into {storage_id=}")
 
                     await self.ctx.storage.put(
                         storage_id, BasePlugin.make_text_storage_value(body_text)
                     )
+                    
+                    if self.demo_tag and user_name:
+                        yield CrawlerDemoUser(user_name=user_name, short_tag_id=creator_tag._tag, platform='wikipedia.org')
 
                     yield CrawlerContent(
                         platform_tag_id=(
                             str(platform_tag) if platform_tag is not None else None
                         ),
                         tag_id=str(creator_tag) if creator_tag is not None else None,
                         type=DatapoolContentType.Text,
@@ -105,34 +108,42 @@
                         url=task.url,
                     )
 
             # parsing links as back tasks
             async for yielded in self.parse_links(self.page):
                 yield yielded
 
-    async def _get_article_creator(self, history_url) -> Optional[BaseTag]:
+    async def _get_article_creator(self, history_url) -> Tuple[Optional[BaseTag], Optional[str]]:
         """
         get the earliest user from the history list.
         """
         history_url += "&dir=prev"
 
         logger.info(f"loading url {history_url}")
         await self.history_page.goto(history_url)
 
         author_link = self.history_page.locator(".mw-userlink").last
         if await author_link.count() > 0:
             logger.info( f'got creator link {author_link=}')
             title = await author_link.get_attribute("title")
-            username = title[5:]  # title structure is "User:$username"
-            logger.info( f'got {username=}')
-            if not username in self.users:
-                href = await author_link.get_attribute("href")
-                user_url = BasePlugin.get_local_url(href, history_url)
-                self.users[username] = await self._parse_user_page(user_url)
-            return self.users[username]
+            if title and title[0:5] == 'User:':
+                username = title[5:]  # title structure is "User:$username"
+                logger.info( f'got {username=}')
+
+                if not self.users.contains(username, 36000):
+                    href = await author_link.get_attribute("href")
+                    if not self.demo_tag:
+                        user_url = BasePlugin.get_local_url(href, history_url)
+                        tag = await self._parse_user_page(user_url)
+                    else:
+                        short_tag_id = BasePlugin.gen_demo_tag(username)
+                        tag = BaseTag(short_tag_id)
+                    self.users.set(username, tag)
+                return (self.users.get(username), username)
+        return (None, None)
 
     # TODO: will be needed when shared ownership is implemented
     # async def _collect_users(self, history_url):
     #     """Collects users from article history page.
     #     Behavior depends on is_demo_mode flag.
     #     In demo mode all users are returned, in non demo mode only users with tag are returned
     #     TODO: not tested
```

### Comparing `datapools-1.0.42/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.43/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/datapools/worker/worker.py` & `datapools-1.0.43/datapools/worker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 from ..common.queues import (
     GenericQueue,
     QueueMessage,
     QueueMessageType,
     QueueRole,
     QueueTopicMessage,
 )
+from ..common.backend_api import BackendAPI
 from ..common.stoppable import Stoppable
 from ..common.storage import FileStorage
 from ..common.types import (
+    CrawlerDemoUser,
     CrawlerBackTask,
     CrawlerContent,
     CrawlerHintURLStatus,
     CrawlerNop,
     DatapoolContentType,
     WorkerSettings,
     InvalidUsageException,
@@ -39,14 +41,17 @@
 
 class CrawlerWorker(Stoppable):
     def __init__(self, cfg: Optional[WorkerSettings] = None):
         super().__init__()
         self.cfg = cfg if cfg is not None else WorkerSettings()
         self.id = uuid.uuid4().hex
         logger.info(f"worker id={self.id}")
+        
+        self.demo_users = {}
+        self.api = BackendAPI(url=self.cfg.BACKEND_API_URL)
 
         self.session_manager = SessionManager(
             self.cfg.REDIS_HOST, self.cfg.REDIS_PORT)
         self.storage = FileStorage(self.cfg.STORAGE_PATH)
 
         self.todo_tasks: Set[asyncio.Task] = set()
 
@@ -247,15 +252,15 @@
             for attempt in range(0, self.cfg.ATTEMPTS_PER_URL):
                 if attempt > 0:
                     logger.info(f"{attempt=}")
 
                 try:
                     session = self.session_manager.get(qm.session_id)
                     def deleted_or_stopped(session_id):
-                        nonlocal is_stopped
+                        nonlocal is_stopped, session
                         if self.session_manager.has(session_id):
                             if session.is_stopped():
                                 is_stopped = True
                                 logger.info(f'Session is stopped, breaking. {session_id=}')
                                 return True
                         else:
                             is_stopped = True
@@ -294,14 +299,22 @@
                                         "worker_id": self.id,
                                     },
                                 )
                             )
 
                         elif t is CrawlerBackTask:
                             await self._add_back_task(qm.session_id, content_or_task)
+                        elif t is CrawlerDemoUser:
+                            ct = content_or_task
+                            if ct.platform not in self.demo_users:
+                                self.demo_users[ct.platform] = {}
+                            if ct.user_name not in self.demo_users[ct.platform]:
+                                self.demo_users[ct.platform][ct.user_name] = ct.short_tag_id
+                                logger.info(f'============= {dict(ct)} ===========')
+                                await self.api.add_demo_user(dict(ct))
                         elif t is CrawlerNop:
                             pass
                         else:
                             raise Exception(f"unknown {content_or_task=}")
 
                         is_stopped = await self.is_stopped()
                         if is_stopped:
```

### Comparing `datapools-1.0.42/datapools.egg-info/PKG-INFO` & `datapools-1.0.43/datapools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.42
+Version: 1.0.43
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.42/datapools.egg-info/SOURCES.txt` & `datapools-1.0.43/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.42/setup.py` & `datapools-1.0.43/setup.py`

 * *Files identical despite different names*

