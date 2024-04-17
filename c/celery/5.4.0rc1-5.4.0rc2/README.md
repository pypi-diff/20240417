# Comparing `tmp/celery-5.4.0rc1.tar.gz` & `tmp/celery-5.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery-5.4.0rc1.tar", last modified: Wed Jan 17 17:52:21 2024, max compression
+gzip compressed data, was "celery-5.4.0rc2.tar", last modified: Wed Mar 27 15:13:31 2024, max compression
```

## Comparing `celery-5.4.0rc1.tar` & `celery-5.4.0rc2.tar`

### file list

```diff
@@ -1,798 +1,814 @@
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.218665 celery-5.4.0rc1/
--rw-r--r--   0 nusnus     (501) staff       (20)     8291 2024-01-14 21:12:59.000000 celery-5.4.0rc1/CONTRIBUTORS.txt
--rw-r--r--   0 nusnus     (501) staff       (20)    35666 2024-01-17 17:41:20.000000 celery-5.4.0rc1/Changelog.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     2717 2023-09-21 12:52:33.000000 celery-5.4.0rc1/LICENSE
--rw-r--r--   0 nusnus     (501) staff       (20)      709 2022-08-03 16:05:58.000000 celery-5.4.0rc1/MANIFEST.in
--rw-r--r--   0 nusnus     (501) staff       (20)    21172 2024-01-17 17:52:21.218493 celery-5.4.0rc1/PKG-INFO
--rw-r--r--   0 nusnus     (501) staff       (20)    16107 2024-01-17 17:47:15.000000 celery-5.4.0rc1/README.rst
--rw-r--r--   0 nusnus     (501) staff       (20)       84 2022-08-03 16:05:58.000000 celery-5.4.0rc1/TODO
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.122610 celery-5.4.0rc1/celery/
--rw-r--r--   0 nusnus     (501) staff       (20)     5950 2024-01-17 17:47:15.000000 celery-5.4.0rc1/celery/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      409 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/__main__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5029 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/_state.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.125402 celery-5.4.0rc1/celery/app/
--rw-r--r--   0 nusnus     (501) staff       (20)     2430 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/app/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    23236 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/app/amqp.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1445 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/app/annotations.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2506 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/app/autoretry.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2702 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/app/backends.py
--rw-r--r--   0 nusnus     (501) staff       (20)    50532 2023-12-25 21:13:51.000000 celery-5.4.0rc1/celery/app/base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6673 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/app/builtins.py
--rw-r--r--   0 nusnus     (501) staff       (20)    29171 2023-10-10 19:45:26.000000 celery-5.4.0rc1/celery/app/control.py
--rw-r--r--   0 nusnus     (501) staff       (20)    15081 2023-11-23 09:45:25.000000 celery-5.4.0rc1/celery/app/defaults.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1326 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/app/events.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9067 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/app/log.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2001 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/app/registry.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4527 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/app/routes.py
--rw-r--r--   0 nusnus     (501) staff       (20)    43794 2023-11-19 15:09:26.000000 celery-5.4.0rc1/celery/app/task.py
--rw-r--r--   0 nusnus     (501) staff       (20)    27551 2024-01-17 12:16:30.000000 celery-5.4.0rc1/celery/app/trace.py
--rw-r--r--   0 nusnus     (501) staff       (20)    13160 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/app/utils.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.125928 celery-5.4.0rc1/celery/apps/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/celery/apps/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5724 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/apps/beat.py
--rw-r--r--   0 nusnus     (501) staff       (20)    16360 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/apps/multi.py
--rw-r--r--   0 nusnus     (501) staff       (20)    13208 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/apps/worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.128460 celery-5.4.0rc1/celery/backends/
--rw-r--r--   0 nusnus     (501) staff       (20)       23 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/backends/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5937 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/backends/arangodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10309 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/backends/asynchronous.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5127 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/backends/azureblockblob.py
--rw-r--r--   0 nusnus     (501) staff       (20)    43989 2024-01-14 19:31:27.000000 celery-5.4.0rc1/celery/backends/base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4831 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/backends/cache.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9006 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/backends/cassandra.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3816 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/backends/consul.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6777 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/backends/cosmosdbsql.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3393 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/backends/couchbase.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2935 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/backends/couchdb.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.129028 celery-5.4.0rc1/celery/backends/database/
--rw-r--r--   0 nusnus     (501) staff       (20)     7751 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/backends/database/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3394 2024-01-14 19:31:27.000000 celery-5.4.0rc1/celery/backends/database/models.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3011 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/backends/database/session.py
--rw-r--r--   0 nusnus     (501) staff       (20)    17179 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/backends/dynamodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9583 2024-01-14 19:31:27.000000 celery-5.4.0rc1/celery/backends/elasticsearch.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3776 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/backends/filesystem.py
--rw-r--r--   0 nusnus     (501) staff       (20)    11438 2023-12-25 21:13:51.000000 celery-5.4.0rc1/celery/backends/mongodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)    26389 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/backends/redis.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12077 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/backends/rpc.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2752 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/backends/s3.py
--rw-r--r--   0 nusnus     (501) staff       (20)    24455 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/beat.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.131526 celery-5.4.0rc1/celery/bin/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/bin/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10023 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/bin/amqp.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8525 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/bin/base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2592 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/bin/beat.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2370 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/bin/call.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7440 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/bin/celery.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7058 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/bin/control.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2794 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/bin/events.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5796 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/bin/graph.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1058 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/bin/list.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4267 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/bin/logtool.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2108 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/bin/migrate.py
--rw-r--r--   0 nusnus     (501) staff       (20)    15374 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/bin/multi.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2608 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/bin/purge.py
--rw-r--r--   0 nusnus     (501) staff       (20)      976 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/bin/result.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4839 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/bin/shell.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3064 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/bin/upgrade.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12886 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/bin/worker.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12277 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/bootsteps.py
--rw-r--r--   0 nusnus     (501) staff       (20)    95883 2024-01-17 16:29:51.000000 celery-5.4.0rc1/celery/canvas.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.132688 celery-5.4.0rc1/celery/concurrency/
--rw-r--r--   0 nusnus     (501) staff       (20)     1457 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/concurrency/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    51471 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/concurrency/asynpool.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4706 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/concurrency/base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5126 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/concurrency/eventlet.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3387 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/concurrency/gevent.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5850 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/concurrency/prefork.py
--rw-r--r--   0 nusnus     (501) staff       (20)      754 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/concurrency/solo.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1807 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/concurrency/thread.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.133534 celery-5.4.0rc1/celery/contrib/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/celery/contrib/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5003 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/contrib/abortable.py
--rw-r--r--   0 nusnus     (501) staff       (20)    14361 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/contrib/migrate.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6754 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/contrib/pytest.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5005 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/contrib/rdb.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3391 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/contrib/sphinx.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.134276 celery-5.4.0rc1/celery/contrib/testing/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/celery/contrib/testing/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3112 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/contrib/testing/app.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8605 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/contrib/testing/manager.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4182 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/contrib/testing/mocks.py
--rw-r--r--   0 nusnus     (501) staff       (20)      208 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/contrib/testing/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7064 2023-10-17 13:52:33.000000 celery-5.4.0rc1/celery/contrib/testing/worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.135290 celery-5.4.0rc1/celery/events/
--rw-r--r--   0 nusnus     (501) staff       (20)      477 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/events/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    17961 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/events/cursesmon.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8987 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/events/dispatcher.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3116 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/events/dumper.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1736 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/events/event.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4998 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/events/receiver.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3294 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/events/snapshot.py
--rw-r--r--   0 nusnus     (501) staff       (20)    25648 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/events/state.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9086 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/exceptions.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.135558 celery-5.4.0rc1/celery/fixups/
--rw-r--r--   0 nusnus     (501) staff       (20)       14 2022-08-03 16:05:58.000000 celery-5.4.0rc1/celery/fixups/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7180 2023-12-25 21:13:51.000000 celery-5.4.0rc1/celery/fixups/django.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.136078 celery-5.4.0rc1/celery/loaders/
--rw-r--r--   0 nusnus     (501) staff       (20)      490 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/loaders/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      199 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/loaders/app.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9147 2023-12-25 21:13:51.000000 celery-5.4.0rc1/celery/loaders/base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1520 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/loaders/default.py
--rw-r--r--   0 nusnus     (501) staff       (20)    16087 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/local.py
--rw-r--r--   0 nusnus     (501) staff       (20)    25289 2023-09-25 15:17:42.000000 celery-5.4.0rc1/celery/platforms.py
--rw-r--r--   0 nusnus     (501) staff       (20)    35612 2023-10-10 19:45:26.000000 celery-5.4.0rc1/celery/result.py
--rw-r--r--   0 nusnus     (501) staff       (20)    32003 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/schedules.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.136752 celery-5.4.0rc1/celery/security/
--rw-r--r--   0 nusnus     (501) staff       (20)     2363 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/security/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4026 2023-12-25 21:13:51.000000 celery-5.4.0rc1/celery/security/certificate.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1189 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/security/key.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4248 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/security/serialization.py
--rw-r--r--   0 nusnus     (501) staff       (20)      845 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/security/utils.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4384 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/signals.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3324 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/states.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.139896 celery-5.4.0rc1/celery/utils/
--rw-r--r--   0 nusnus     (501) staff       (20)      935 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/utils/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2874 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/utils/abstract.py
--rw-r--r--   0 nusnus     (501) staff       (20)    25432 2023-10-17 13:52:33.000000 celery-5.4.0rc1/celery/utils/collections.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4709 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/utils/debug.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3620 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/utils/deprecated.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.140193 celery-5.4.0rc1/celery/utils/dispatch/
--rw-r--r--   0 nusnus     (501) staff       (20)       74 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/utils/dispatch/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    13603 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/utils/dispatch/signal.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12017 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/utils/functional.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9041 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/utils/graph.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5126 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/utils/imports.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2916 2024-01-06 18:35:01.000000 celery-5.4.0rc1/celery/utils/iso8601.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8757 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/utils/log.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3163 2023-12-06 12:13:34.000000 celery-5.4.0rc1/celery/utils/nodenames.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4215 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/utils/objects.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9020 2023-10-17 13:52:33.000000 celery-5.4.0rc1/celery/utils/saferepr.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8209 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/utils/serialization.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.140470 celery-5.4.0rc1/celery/utils/static/
--rw-r--r--   0 nusnus     (501) staff       (20)      299 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/utils/static/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2556 2022-08-03 16:05:58.000000 celery-5.4.0rc1/celery/utils/static/celery_128.png
--rw-r--r--   0 nusnus     (501) staff       (20)     1264 2024-01-06 18:35:01.000000 celery-5.4.0rc1/celery/utils/sysinfo.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5135 2024-01-07 22:36:19.000000 celery-5.4.0rc1/celery/utils/term.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5844 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/utils/text.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9552 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/utils/threads.py
--rw-r--r--   0 nusnus     (501) staff       (20)    15039 2024-01-14 19:31:27.000000 celery-5.4.0rc1/celery/utils/time.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4813 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/utils/timer2.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.141832 celery-5.4.0rc1/celery/worker/
--rw-r--r--   0 nusnus     (501) staff       (20)       95 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/worker/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4593 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/worker/autoscale.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7497 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/worker/components.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.143132 celery-5.4.0rc1/celery/worker/consumer/
--rw-r--r--   0 nusnus     (501) staff       (20)      391 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/worker/consumer/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      525 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/worker/consumer/agent.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1026 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/worker/consumer/connection.py
--rw-r--r--   0 nusnus     (501) staff       (20)    29091 2023-11-23 09:45:25.000000 celery-5.4.0rc1/celery/worker/consumer/consumer.py
--rw-r--r--   0 nusnus     (501) staff       (20)      946 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/worker/consumer/control.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2054 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/worker/consumer/events.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6863 2023-11-14 10:15:09.000000 celery-5.4.0rc1/celery/worker/consumer/gossip.py
--rw-r--r--   0 nusnus     (501) staff       (20)      930 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/worker/consumer/heart.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2519 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/worker/consumer/mingle.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1960 2023-06-21 21:46:53.000000 celery-5.4.0rc1/celery/worker/consumer/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)    19882 2023-11-19 15:09:26.000000 celery-5.4.0rc1/celery/worker/control.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2107 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/worker/heartbeat.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4433 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/worker/loops.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3630 2022-12-29 15:36:27.000000 celery-5.4.0rc1/celery/worker/pidbox.py
--rw-r--r--   0 nusnus     (501) staff       (20)    27229 2023-06-26 13:41:34.000000 celery-5.4.0rc1/celery/worker/request.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8583 2023-06-26 13:41:34.000000 celery-5.4.0rc1/celery/worker/state.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7324 2023-09-21 12:52:33.000000 celery-5.4.0rc1/celery/worker/strategy.py
--rw-r--r--   0 nusnus     (501) staff       (20)    14488 2023-12-25 21:13:51.000000 celery-5.4.0rc1/celery/worker/worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.215245 celery-5.4.0rc1/celery.egg-info/
--rw-r--r--   0 nusnus     (501) staff       (20)    21172 2024-01-17 17:52:21.000000 celery-5.4.0rc1/celery.egg-info/PKG-INFO
--rw-r--r--   0 nusnus     (501) staff       (20)    22465 2024-01-17 17:52:21.000000 celery-5.4.0rc1/celery.egg-info/SOURCES.txt
--rw-r--r--   0 nusnus     (501) staff       (20)        1 2024-01-17 17:52:21.000000 celery-5.4.0rc1/celery.egg-info/dependency_links.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       48 2024-01-17 17:52:21.000000 celery-5.4.0rc1/celery.egg-info/entry_points.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     1872 2024-01-17 17:52:21.000000 celery-5.4.0rc1/celery.egg-info/requires.txt
--rw-r--r--   0 nusnus     (501) staff       (20)        7 2024-01-17 17:52:21.000000 celery-5.4.0rc1/celery.egg-info/top_level.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.144952 celery-5.4.0rc1/docs/
--rw-r--r--   0 nusnus     (501) staff       (20)     6148 2023-11-19 14:46:03.000000 celery-5.4.0rc1/docs/.DS_Store
--rw-r--r--   0 nusnus     (501) staff       (20)     5293 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/AUTHORS.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     8111 2024-01-17 17:29:30.000000 celery-5.4.0rc1/docs/Makefile
--rw-r--r--   0 nusnus     (501) staff       (20)      494 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/THANKS
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.145085 celery-5.4.0rc1/docs/_ext/
--rw-r--r--   0 nusnus     (501) staff       (20)     5164 2022-12-29 15:36:27.000000 celery-5.4.0rc1/docs/_ext/celerydocs.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.145211 celery-5.4.0rc1/docs/_static/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/_static/.keep
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.145301 celery-5.4.0rc1/docs/_templates/
--rw-r--r--   0 nusnus     (501) staff       (20)      486 2022-12-29 15:36:27.000000 celery-5.4.0rc1/docs/_templates/sidebardonations.html
--rw-r--r--   0 nusnus     (501) staff       (20)       30 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/changelog.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      981 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/community.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     2597 2023-09-21 12:52:33.000000 celery-5.4.0rc1/docs/conf.py
--rw-r--r--   0 nusnus     (501) staff       (20)       83 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/configuration.html
--rw-r--r--   0 nusnus     (501) staff       (20)       33 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/contributing.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      931 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/copyright.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.145539 celery-5.4.0rc1/docs/django/
--rw-r--r--   0 nusnus     (501) staff       (20)     7942 2023-09-21 12:52:33.000000 celery-5.4.0rc1/docs/django/first-steps-with-django.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      137 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/django/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    29852 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/faq.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.146218 celery-5.4.0rc1/docs/getting-started/
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.146737 celery-5.4.0rc1/docs/getting-started/backends-and-brokers/
--rw-r--r--   0 nusnus     (501) staff       (20)     3905 2023-11-19 15:09:26.000000 celery-5.4.0rc1/docs/getting-started/backends-and-brokers/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     5010 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/getting-started/backends-and-brokers/rabbitmq.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     8384 2023-11-23 11:53:28.000000 celery-5.4.0rc1/docs/getting-started/backends-and-brokers/redis.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    10843 2023-12-11 00:08:34.000000 celery-5.4.0rc1/docs/getting-started/backends-and-brokers/sqs.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    14995 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/getting-started/first-steps-with-celery.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-12-29 15:36:27.000000 celery-5.4.0rc1/docs/getting-started/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    10903 2023-09-21 12:52:33.000000 celery-5.4.0rc1/docs/getting-started/introduction.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    22874 2023-11-14 10:15:09.000000 celery-5.4.0rc1/docs/getting-started/next-steps.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      132 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/getting-started/resources.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     4448 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/glossary.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.150767 celery-5.4.0rc1/docs/history/
--rw-r--r--   0 nusnus     (501) staff       (20)    58104 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/history/changelog-1.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    34009 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/history/changelog-2.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    23550 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/changelog-2.1.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    33558 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/history/changelog-2.2.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    11200 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/history/changelog-2.3.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    13012 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/history/changelog-2.4.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     5414 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/changelog-2.5.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    49344 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/history/changelog-3.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    52336 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/history/changelog-3.1.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     6432 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/changelog-4.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     8950 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/changelog-4.1.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    13593 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/changelog-4.2.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    17251 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/changelog-4.3.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    24332 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/changelog-4.4.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     5720 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/history/changelog-5.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     5592 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/history/changelog-5.1.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      692 2024-01-17 17:41:20.000000 celery-5.4.0rc1/docs/history/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    16026 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/whatsnew-2.5.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    30892 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/whatsnew-3.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    44129 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/whatsnew-3.1.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    76466 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/history/whatsnew-4.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     8244 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/whatsnew-4.1.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    35711 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/whatsnew-4.2.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    16865 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/whatsnew-4.3.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     6999 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/whatsnew-4.4.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    10957 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/history/whatsnew-5.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    14128 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/history/whatsnew-5.1.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    11263 2024-01-17 17:41:20.000000 celery-5.4.0rc1/docs/history/whatsnew-5.3.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.152335 celery-5.4.0rc1/docs/images/
--rw-r--r--   0 nusnus     (501) staff       (20)    14168 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/images/celery-banner-small.png
--rw-r--r--   0 nusnus     (501) staff       (20)    14038 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/images/celery-banner.png
--rw-r--r--   0 nusnus     (501) staff       (20)     2556 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/images/celery_128.png
--rw-r--r--   0 nusnus     (501) staff       (20)     8658 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/images/celery_512.png
--rw-r--r--   0 nusnus     (501) staff       (20)    77397 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/images/celeryevshotsm.jpg
--rw-r--r--   0 nusnus     (501) staff       (20)    88879 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/images/dashboard.png
--rw-r--r--   0 nusnus     (501) staff       (20)     4286 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/images/favicon.ico
--rw-r--r--   0 nusnus     (501) staff       (20)   146412 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/images/monitor.png
--rw-r--r--   0 nusnus     (501) staff       (20)    35894 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/images/result_graph.png
--rw-r--r--   0 nusnus     (501) staff       (20)    99783 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/images/worker_graph_full.png
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.152772 celery-5.4.0rc1/docs/includes/
--rw-r--r--   0 nusnus     (501) staff       (20)     4023 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/includes/installation.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     6421 2024-01-17 17:47:15.000000 celery-5.4.0rc1/docs/includes/introduction.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     1375 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/includes/resources.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     1596 2024-01-17 17:41:20.000000 celery-5.4.0rc1/docs/index.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.153510 celery-5.4.0rc1/docs/internals/
--rw-r--r--   0 nusnus     (501) staff       (20)     5985 2022-12-29 15:36:27.000000 celery-5.4.0rc1/docs/internals/app-overview.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     5696 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/internals/deprecation.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     8586 2023-02-01 20:37:32.000000 celery-5.4.0rc1/docs/internals/guide.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      206 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     9898 2022-12-29 15:36:27.000000 celery-5.4.0rc1/docs/internals/protocol.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.161900 celery-5.4.0rc1/docs/internals/reference/
--rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery._state.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      257 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.app.annotations.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      224 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.app.routes.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.app.trace.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.arangodb.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.asynchronous.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      293 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.azureblockblob.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      243 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.base.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.cache.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      278 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.cassandra.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      253 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.consul.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      284 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.cosmosdbsql.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      270 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.couchbase.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      262 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.couchdb.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      276 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.database.models.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      293 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.database.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      283 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.database.session.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      265 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.dynamodb.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      280 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.elasticsearch.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      269 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.filesystem.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.mongodb.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      254 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.redis.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      242 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.rpc.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      206 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      245 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.backends.s3.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      270 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.concurrency.base.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      310 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.concurrency.eventlet.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      304 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.concurrency.gevent.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      307 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.concurrency.prefork.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      229 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.concurrency.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      310 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.concurrency.solo.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      304 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.concurrency.thread.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      260 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.events.cursesmon.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      251 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.events.dumper.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      257 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.events.snapshot.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      231 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.platforms.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      272 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.security.certificate.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      248 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.security.key.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      278 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.security.serialization.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      254 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.security.utils.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.abstract.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      252 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.collections.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      260 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.deprecated.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      252 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.dispatch.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      295 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.dispatch.signal.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      282 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.functional.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      245 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.graph.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      273 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.imports.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.iso8601.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.log.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      257 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.nodenames.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.objects.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      195 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.saferepr.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      273 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.serialization.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.sysinfo.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.term.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.text.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      251 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.threads.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      258 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.time.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      224 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.utils.timer2.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.worker.autoscale.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      259 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.worker.components.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      260 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.worker.control.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      266 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.worker.heartbeat.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      236 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.worker.loops.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/reference/celery.worker.pidbox.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     1960 2022-12-29 15:36:27.000000 celery-5.4.0rc1/docs/internals/reference/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     1452 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/internals/worker.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     7675 2022-12-29 15:36:27.000000 celery-5.4.0rc1/docs/make.bat
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.172098 celery-5.4.0rc1/docs/reference/
--rw-r--r--   0 nusnus     (501) staff       (20)     1379 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.app.amqp.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      237 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.app.autoretry.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      234 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.app.backends.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      268 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.app.builtins.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      265 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.app.control.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      290 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.app.defaults.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      222 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.app.events.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      213 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.app.log.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      228 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.app.registry.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      288 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.app.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.app.task.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      219 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.app.utils.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      253 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.apps.beat.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      236 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.apps.multi.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.apps.worker.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      220 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.beat.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      189 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/reference/celery.bin.amqp.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      216 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.base.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      254 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.beat.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      258 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.call.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      242 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.celery.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.control.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.events.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.graph.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      258 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.list.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.logtool.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.migrate.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      249 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.multi.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.purge.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.result.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.shell.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.upgrade.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      242 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bin.worker.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.bootsteps.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      290 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.contrib.abortable.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      230 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.contrib.migrate.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      273 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.contrib.pytest.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.contrib.rdb.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      184 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.contrib.sphinx.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      288 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.contrib.testing.app.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      300 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.contrib.testing.manager.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.contrib.testing.mocks.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      297 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.contrib.testing.worker.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      304 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.events.dispatcher.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.events.event.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      303 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.events.receiver.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      194 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.events.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.events.state.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      222 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.exceptions.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      227 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.loaders.app.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      250 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.loaders.base.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      255 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.loaders.default.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      237 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.loaders.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      204 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.result.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     3497 2022-12-29 15:36:27.000000 celery-5.4.0rc1/docs/reference/celery.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.schedules.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      200 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.security.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      257 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.signals.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      106 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.states.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      871 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.utils.debug.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      291 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.consumer.agent.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      306 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.consumer.connection.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      300 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.consumer.consumer.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      297 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.consumer.control.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.consumer.events.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.consumer.gossip.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      291 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.consumer.heart.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.consumer.mingle.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      273 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.consumer.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      291 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.consumer.tasks.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      244 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.request.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      236 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.state.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      245 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.strategy.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/reference/celery.worker.worker.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      285 2023-09-21 12:52:33.000000 celery-5.4.0rc1/docs/reference/cli.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     1952 2022-12-29 15:36:27.000000 celery-5.4.0rc1/docs/reference/index.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.172452 celery-5.4.0rc1/docs/sec/
--rw-r--r--   0 nusnus     (501) staff       (20)     2921 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/sec/CELERYSA-0001.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     2656 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/sec/CELERYSA-0002.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     1551 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/sec/CELERYSA-0003.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     4879 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/spelling_wordlist.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.172572 celery-5.4.0rc1/docs/templates/
--rw-r--r--   0 nusnus     (501) staff       (20)     1186 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/templates/readme.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.173227 celery-5.4.0rc1/docs/tutorials/
--rw-r--r--   0 nusnus     (501) staff       (20)       86 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/tutorials/daemonizing.html
--rw-r--r--   0 nusnus     (501) staff       (20)       91 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/tutorials/debugging.html
--rw-r--r--   0 nusnus     (501) staff       (20)      121 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/tutorials/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     2766 2022-12-29 15:36:27.000000 celery-5.4.0rc1/docs/tutorials/task-cookbook.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.176225 celery-5.4.0rc1/docs/userguide/
--rw-r--r--   0 nusnus     (501) staff       (20)    14779 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/userguide/application.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    25087 2023-09-21 12:52:33.000000 celery-5.4.0rc1/docs/userguide/calling.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    38116 2024-01-17 16:29:51.000000 celery-5.4.0rc1/docs/userguide/canvas.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.176892 celery-5.4.0rc1/docs/userguide/concurrency/
--rw-r--r--   0 nusnus     (501) staff       (20)     2665 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/userguide/concurrency/eventlet.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     2872 2023-09-21 12:52:33.000000 celery-5.4.0rc1/docs/userguide/concurrency/gevent.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     1561 2024-01-08 03:58:18.000000 celery-5.4.0rc1/docs/userguide/concurrency/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)   100612 2023-11-23 09:45:25.000000 celery-5.4.0rc1/docs/userguide/configuration.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    17699 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/userguide/daemonizing.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     3131 2022-12-29 15:36:27.000000 celery-5.4.0rc1/docs/userguide/debugging.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    30057 2022-12-29 15:36:27.000000 celery-5.4.0rc1/docs/userguide/extending.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      372 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/userguide/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    21759 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/userguide/monitoring.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     8437 2022-12-29 15:36:27.000000 celery-5.4.0rc1/docs/userguide/optimizing.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    20946 2024-01-06 18:35:01.000000 celery-5.4.0rc1/docs/userguide/periodic-tasks.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    24323 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/userguide/routing.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     8693 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/userguide/security.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    18107 2023-11-14 10:15:09.000000 celery-5.4.0rc1/docs/userguide/signals.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      345 2022-08-03 16:05:58.000000 celery-5.4.0rc1/docs/userguide/sphinx.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    64549 2023-09-21 12:52:33.000000 celery-5.4.0rc1/docs/userguide/tasks.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    11146 2023-06-21 21:46:53.000000 celery-5.4.0rc1/docs/userguide/testing.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    35007 2023-11-23 09:45:25.000000 celery-5.4.0rc1/docs/userguide/workers.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.177229 celery-5.4.0rc1/examples/
--rw-r--r--   0 nusnus     (501) staff       (20)     6148 2023-04-12 11:27:42.000000 celery-5.4.0rc1/examples/.DS_Store
--rw-r--r--   0 nusnus     (501) staff       (20)      303 2022-08-03 16:05:58.000000 celery-5.4.0rc1/examples/README.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.177349 celery-5.4.0rc1/examples/app/
--rw-r--r--   0 nusnus     (501) staff       (20)      822 2024-01-10 10:18:05.000000 celery-5.4.0rc1/examples/app/myapp.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.178053 celery-5.4.0rc1/examples/celery_http_gateway/
--rw-r--r--   0 nusnus     (501) staff       (20)     1382 2022-08-03 16:05:58.000000 celery-5.4.0rc1/examples/celery_http_gateway/README.rst
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/examples/celery_http_gateway/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      385 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/celery_http_gateway/manage.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3001 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/celery_http_gateway/settings.py
--rw-r--r--   0 nusnus     (501) staff       (20)       88 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/celery_http_gateway/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)      678 2023-06-21 21:46:53.000000 celery-5.4.0rc1/examples/celery_http_gateway/urls.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.178442 celery-5.4.0rc1/examples/django/
--rw-r--r--   0 nusnus     (501) staff       (20)     1546 2023-06-21 21:46:53.000000 celery-5.4.0rc1/examples/django/README.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.178928 celery-5.4.0rc1/examples/django/demoapp/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/examples/django/demoapp/__init__.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.179185 celery-5.4.0rc1/examples/django/demoapp/migrations/
--rw-r--r--   0 nusnus     (501) staff       (20)      486 2022-08-03 16:05:58.000000 celery-5.4.0rc1/examples/django/demoapp/migrations/0001_initial.py
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/examples/django/demoapp/migrations/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      103 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/django/demoapp/models.py
--rw-r--r--   0 nusnus     (501) staff       (20)      437 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/django/demoapp/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)       26 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/django/demoapp/views.py
--rwxr-xr-x   0 nusnus     (501) staff       (20)      248 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/django/manage.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.179976 celery-5.4.0rc1/examples/django/proj/
--rw-r--r--   0 nusnus     (501) staff       (20)      174 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/django/proj/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      659 2023-06-21 21:46:53.000000 celery-5.4.0rc1/examples/django/proj/celery.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3639 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/django/proj/settings.py
--rw-r--r--   0 nusnus     (501) staff       (20)      556 2023-02-01 17:22:50.000000 celery-5.4.0rc1/examples/django/proj/urls.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1132 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/django/proj/wsgi.py
--rw-r--r--   0 nusnus     (501) staff       (20)       47 2023-06-21 21:46:53.000000 celery-5.4.0rc1/examples/django/requirements.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.180633 celery-5.4.0rc1/examples/eventlet/
--rw-r--r--   0 nusnus     (501) staff       (20)     1449 2023-06-21 21:46:53.000000 celery-5.4.0rc1/examples/eventlet/README.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     1673 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/eventlet/bulk_task_producer.py
--rw-r--r--   0 nusnus     (501) staff       (20)      312 2023-06-21 21:46:53.000000 celery-5.4.0rc1/examples/eventlet/celeryconfig.py
--rw-r--r--   0 nusnus     (501) staff       (20)      306 2023-06-21 21:46:53.000000 celery-5.4.0rc1/examples/eventlet/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2009 2023-06-21 21:46:53.000000 celery-5.4.0rc1/examples/eventlet/webcrawler.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.181006 celery-5.4.0rc1/examples/gevent/
--rw-r--r--   0 nusnus     (501) staff       (20)     1303 2023-09-21 12:52:33.000000 celery-5.4.0rc1/examples/gevent/README.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      255 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/gevent/celeryconfig.py
--rw-r--r--   0 nusnus     (501) staff       (20)      325 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/gevent/tasks.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.181120 celery-5.4.0rc1/examples/next-steps/
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.181441 celery-5.4.0rc1/examples/next-steps/proj/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/examples/next-steps/proj/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/next-steps/proj/celery.py
--rw-r--r--   0 nusnus     (501) staff       (20)      167 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/next-steps/proj/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1224 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/next-steps/setup.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.181555 celery-5.4.0rc1/examples/periodic-tasks/
--rw-r--r--   0 nusnus     (501) staff       (20)     1518 2023-06-21 21:46:53.000000 celery-5.4.0rc1/examples/periodic-tasks/myapp.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.181671 celery-5.4.0rc1/examples/resultgraph/
--rw-r--r--   0 nusnus     (501) staff       (20)     2860 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/resultgraph/tasks.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.181788 celery-5.4.0rc1/examples/security/
--rw-r--r--   0 nusnus     (501) staff       (20)     1058 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/security/mysecureapp.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.182021 celery-5.4.0rc1/examples/security/ssl/
--rw-r--r--   0 nusnus     (501) staff       (20)     3243 2022-08-03 16:05:58.000000 celery-5.4.0rc1/examples/security/ssl/worker.key
--rw-r--r--   0 nusnus     (501) staff       (20)     1923 2022-08-03 16:05:58.000000 celery-5.4.0rc1/examples/security/ssl/worker.pem
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.182745 celery-5.4.0rc1/examples/stamping/
--rw-r--r--   0 nusnus     (501) staff       (20)      103 2023-06-21 21:46:53.000000 celery-5.4.0rc1/examples/stamping/config.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1358 2023-06-21 21:46:53.000000 celery-5.4.0rc1/examples/stamping/examples.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1806 2023-06-24 09:59:42.000000 celery-5.4.0rc1/examples/stamping/myapp.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2548 2023-06-21 21:46:53.000000 celery-5.4.0rc1/examples/stamping/revoke_example.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3311 2023-06-24 09:59:42.000000 celery-5.4.0rc1/examples/stamping/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2410 2023-06-21 21:46:53.000000 celery-5.4.0rc1/examples/stamping/visitors.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.182869 celery-5.4.0rc1/examples/tutorial/
--rw-r--r--   0 nusnus     (501) staff       (20)      158 2022-12-29 15:36:27.000000 celery-5.4.0rc1/examples/tutorial/tasks.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.117783 celery-5.4.0rc1/extra/
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.182992 celery-5.4.0rc1/extra/bash-completion/
--rw-r--r--   0 nusnus     (501) staff       (20)      636 2022-12-29 15:36:27.000000 celery-5.4.0rc1/extra/bash-completion/celery.bash
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.183257 celery-5.4.0rc1/extra/generic-init.d/
--rwxr-xr-x   0 nusnus     (501) staff       (20)     9068 2023-06-21 21:46:53.000000 celery-5.4.0rc1/extra/generic-init.d/celerybeat
--rwxr-xr-x   0 nusnus     (501) staff       (20)    10813 2023-06-21 21:46:53.000000 celery-5.4.0rc1/extra/generic-init.d/celeryd
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.183508 celery-5.4.0rc1/extra/macOS/
--rw-r--r--   0 nusnus     (501) staff       (20)      751 2022-08-03 16:05:58.000000 celery-5.4.0rc1/extra/macOS/org.celeryq.beat.plist
--rw-r--r--   0 nusnus     (501) staff       (20)      757 2022-08-03 16:05:58.000000 celery-5.4.0rc1/extra/macOS/org.celeryq.worker.plist
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.184011 celery-5.4.0rc1/extra/supervisord/
--rw-r--r--   0 nusnus     (501) staff       (20)      134 2022-08-03 16:05:58.000000 celery-5.4.0rc1/extra/supervisord/celery.sh
--rw-r--r--   0 nusnus     (501) staff       (20)      699 2022-12-29 15:36:27.000000 celery-5.4.0rc1/extra/supervisord/celerybeat.conf
--rw-r--r--   0 nusnus     (501) staff       (20)      949 2022-12-29 15:36:27.000000 celery-5.4.0rc1/extra/supervisord/celeryd.conf
--rw-r--r--   0 nusnus     (501) staff       (20)      982 2023-06-21 21:46:53.000000 celery-5.4.0rc1/extra/supervisord/supervisord.conf
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.184571 celery-5.4.0rc1/extra/systemd/
--rw-r--r--   0 nusnus     (501) staff       (20)      506 2023-06-21 21:46:53.000000 celery-5.4.0rc1/extra/systemd/celery.conf
--rw-r--r--   0 nusnus     (501) staff       (20)      740 2022-12-29 15:36:27.000000 celery-5.4.0rc1/extra/systemd/celery.service
--rw-r--r--   0 nusnus     (501) staff       (20)       78 2022-08-03 16:05:58.000000 celery-5.4.0rc1/extra/systemd/celery.tmpfiles
--rw-r--r--   0 nusnus     (501) staff       (20)      395 2022-12-29 15:36:27.000000 celery-5.4.0rc1/extra/systemd/celerybeat.service
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.184690 celery-5.4.0rc1/extra/zsh-completion/
--rw-r--r--   0 nusnus     (501) staff       (20)     6244 2022-08-03 16:05:58.000000 celery-5.4.0rc1/extra/zsh-completion/celery.zsh
--rw-r--r--   0 nusnus     (501) staff       (20)     1216 2023-06-21 21:46:53.000000 celery-5.4.0rc1/pyproject.toml
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.185938 celery-5.4.0rc1/requirements/
--rw-r--r--   0 nusnus     (501) staff       (20)     1368 2023-09-21 12:52:33.000000 celery-5.4.0rc1/requirements/README.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      273 2023-11-19 15:09:26.000000 celery-5.4.0rc1/requirements/default.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.186052 celery-5.4.0rc1/requirements/deps/
--rw-r--r--   0 nusnus     (501) staff       (20)       10 2022-08-03 16:05:58.000000 celery-5.4.0rc1/requirements/deps/mock.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      151 2024-01-08 18:07:11.000000 celery-5.4.0rc1/requirements/dev.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      180 2024-01-08 18:07:11.000000 celery-5.4.0rc1/requirements/docs.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.190446 celery-5.4.0rc1/requirements/extras/
--rw-r--r--   0 nusnus     (501) staff       (20)       16 2023-09-21 12:52:33.000000 celery-5.4.0rc1/requirements/extras/arangodb.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       21 2023-12-03 15:14:31.000000 celery-5.4.0rc1/requirements/extras/auth.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       28 2023-06-21 21:46:53.000000 celery-5.4.0rc1/requirements/extras/azureblockblob.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      111 2022-08-03 16:05:58.000000 celery-5.4.0rc1/requirements/extras/brotli.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       28 2023-06-21 21:46:53.000000 celery-5.4.0rc1/requirements/extras/cassandra.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       22 2023-06-21 21:46:53.000000 celery-5.4.0rc1/requirements/extras/consul.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       20 2023-06-21 21:46:53.000000 celery-5.4.0rc1/requirements/extras/cosmosdbsql.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      119 2023-11-05 11:35:58.000000 celery-5.4.0rc1/requirements/extras/couchbase.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       18 2023-06-21 21:46:53.000000 celery-5.4.0rc1/requirements/extras/couchdb.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       15 2023-06-21 21:46:53.000000 celery-5.4.0rc1/requirements/extras/django.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       16 2023-09-21 12:52:33.000000 celery-5.4.0rc1/requirements/extras/dynamodb.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       48 2024-01-09 01:41:21.000000 celery-5.4.0rc1/requirements/extras/elasticsearch.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       40 2022-12-29 15:36:27.000000 celery-5.4.0rc1/requirements/extras/eventlet.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       14 2022-12-29 15:36:27.000000 celery-5.4.0rc1/requirements/extras/gevent.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       44 2023-09-21 12:52:33.000000 celery-5.4.0rc1/requirements/extras/librabbitmq.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       45 2023-06-21 21:46:53.000000 celery-5.4.0rc1/requirements/extras/memcache.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       20 2023-06-21 21:46:53.000000 celery-5.4.0rc1/requirements/extras/mongodb.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       15 2023-10-10 19:45:26.000000 celery-5.4.0rc1/requirements/extras/msgpack.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       23 2024-01-12 18:18:24.000000 celery-5.4.0rc1/requirements/extras/pymemcache.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       37 2023-09-21 12:52:33.000000 celery-5.4.0rc1/requirements/extras/pyro.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       23 2024-01-14 21:12:59.000000 celery-5.4.0rc1/requirements/extras/pytest.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       28 2023-09-21 12:52:33.000000 celery-5.4.0rc1/requirements/extras/redis.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       16 2023-09-21 12:52:33.000000 celery-5.4.0rc1/requirements/extras/s3.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       27 2022-08-03 16:05:58.000000 celery-5.4.0rc1/requirements/extras/slmq.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       53 2023-10-12 19:13:02.000000 celery-5.4.0rc1/requirements/extras/solar.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       27 2022-12-29 15:36:27.000000 celery-5.4.0rc1/requirements/extras/sphinxautobuild.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       24 2023-06-26 13:41:34.000000 celery-5.4.0rc1/requirements/extras/sqlalchemy.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      139 2023-09-21 12:52:33.000000 celery-5.4.0rc1/requirements/extras/sqs.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       73 2022-08-03 16:05:58.000000 celery-5.4.0rc1/requirements/extras/tblib.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       39 2022-08-03 16:05:58.000000 celery-5.4.0rc1/requirements/extras/thread.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       13 2022-08-03 16:05:58.000000 celery-5.4.0rc1/requirements/extras/yaml.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       14 2023-06-21 21:46:53.000000 celery-5.4.0rc1/requirements/extras/zeromq.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       13 2022-08-03 16:05:58.000000 celery-5.4.0rc1/requirements/extras/zookeeper.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       18 2023-11-14 10:15:09.000000 celery-5.4.0rc1/requirements/extras/zstd.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      212 2023-09-21 12:52:33.000000 celery-5.4.0rc1/requirements/pkgutils.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       19 2022-08-03 16:05:58.000000 celery-5.4.0rc1/requirements/security.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      175 2023-06-26 13:41:34.000000 celery-5.4.0rc1/requirements/test-ci-base.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      613 2023-11-14 10:15:09.000000 celery-5.4.0rc1/requirements/test-ci-default.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      160 2023-06-21 21:46:53.000000 celery-5.4.0rc1/requirements/test-integration.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       17 2022-08-03 16:05:58.000000 celery-5.4.0rc1/requirements/test-pypy3.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      337 2024-01-14 21:12:59.000000 celery-5.4.0rc1/requirements/test.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      486 2024-01-17 17:52:21.219001 celery-5.4.0rc1/setup.cfg
--rwxr-xr-x   0 nusnus     (501) staff       (20)     4640 2024-01-03 00:42:06.000000 celery-5.4.0rc1/setup.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.190753 celery-5.4.0rc1/t/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2023-09-25 19:52:57.000000 celery-5.4.0rc1/t/__init__.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.190937 celery-5.4.0rc1/t/benchmarks/
--rw-r--r--   0 nusnus     (501) staff       (20)     2816 2023-09-21 12:52:33.000000 celery-5.4.0rc1/t/benchmarks/bench_worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.193039 celery-5.4.0rc1/t/integration/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2023-09-25 17:14:49.000000 celery-5.4.0rc1/t/integration/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2304 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/integration/conftest.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12850 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/integration/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1120 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/integration/test_backend.py
--rw-r--r--   0 nusnus     (501) staff       (20)   135101 2024-01-17 16:29:51.000000 celery-5.4.0rc1/t/integration/test_canvas.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7815 2023-12-25 21:13:51.000000 celery-5.4.0rc1/t/integration/test_inspect.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1352 2023-11-23 07:26:02.000000 celery-5.4.0rc1/t/integration/test_loader.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3477 2023-12-25 21:13:51.000000 celery-5.4.0rc1/t/integration/test_security.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1651 2023-11-14 10:15:09.000000 celery-5.4.0rc1/t/integration/test_serialization.py
--rw-r--r--   0 nusnus     (501) staff       (20)      150 2023-11-14 10:15:09.000000 celery-5.4.0rc1/t/integration/test_serialization_config.py
--rw-r--r--   0 nusnus     (501) staff       (20)    22815 2024-01-07 22:36:19.000000 celery-5.4.0rc1/t/integration/test_tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)      688 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/integration/test_worker.py
--rw-r--r--   0 nusnus     (501) staff       (20)      293 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/integration/test_worker_config.py
--rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/skip.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.193481 celery-5.4.0rc1/t/smoke/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1514 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/conftest.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.193940 celery-5.4.0rc1/t/smoke/operations/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/operations/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1504 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/operations/task_termination.py
--rw-r--r--   0 nusnus     (501) staff       (20)      929 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/operations/worker_kill.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1008 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/operations/worker_restart.py
--rw-r--r--   0 nusnus     (501) staff       (20)      781 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/signals.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1653 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tasks.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.194908 celery-5.4.0rc1/t/smoke/tests/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/__init__.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.195264 celery-5.4.0rc1/t/smoke/tests/failover/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/failover/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2451 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/failover/test_broker_failover.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1918 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/failover/test_worker_failover.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.196113 celery-5.4.0rc1/t/smoke/tests/stamping/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/stamping/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1215 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/stamping/conftest.py
--rw-r--r--   0 nusnus     (501) staff       (20)      411 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/stamping/signals.py
--rw-r--r--   0 nusnus     (501) staff       (20)      708 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/stamping/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5915 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/stamping/test_hybrid_cluster.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2209 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/stamping/test_revoke.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1457 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/stamping/test_visitor.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.196355 celery-5.4.0rc1/t/smoke/tests/stamping/workers/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/stamping/workers/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1491 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/stamping/workers/legacy.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3208 2024-01-17 16:29:51.000000 celery-5.4.0rc1/t/smoke/tests/test_canvas.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5695 2024-01-17 12:16:30.000000 celery-5.4.0rc1/t/smoke/tests/test_consumer.py
--rw-r--r--   0 nusnus     (501) staff       (20)      688 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/test_control.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1847 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/test_signals.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4514 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/test_tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2015 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/test_thread_safe.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1676 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/tests/test_worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.196941 celery-5.4.0rc1/t/smoke/workers/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/workers/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1389 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/workers/alt.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1594 2024-01-15 12:58:48.000000 celery-5.4.0rc1/t/smoke/workers/dev.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1422 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/workers/latest.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1506 2024-01-14 21:12:59.000000 celery-5.4.0rc1/t/smoke/workers/other.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.197326 celery-5.4.0rc1/t/unit/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/__init__.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.200048 celery-5.4.0rc1/t/unit/app/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/app/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    13805 2023-12-25 21:13:51.000000 celery-5.4.0rc1/t/unit/app/test_amqp.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1338 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/app/test_annotations.py
--rw-r--r--   0 nusnus     (501) staff       (20)    41944 2023-12-25 21:13:51.000000 celery-5.4.0rc1/t/unit/app/test_app.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4542 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/app/test_backends.py
--rw-r--r--   0 nusnus     (501) staff       (20)    30235 2024-01-14 19:31:27.000000 celery-5.4.0rc1/t/unit/app/test_beat.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5528 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/app/test_builtins.py
--rw-r--r--   0 nusnus     (501) staff       (20)      356 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/app/test_celery.py
--rw-r--r--   0 nusnus     (501) staff       (20)    19105 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/app/test_control.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1608 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/app/test_defaults.py
--rw-r--r--   0 nusnus     (501) staff       (20)      829 2023-12-25 21:13:51.000000 celery-5.4.0rc1/t/unit/app/test_exceptions.py
--rw-r--r--   0 nusnus     (501) staff       (20)    11599 2023-11-23 07:26:02.000000 celery-5.4.0rc1/t/unit/app/test_loaders.py
--rw-r--r--   0 nusnus     (501) staff       (20)    11820 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/app/test_log.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1891 2023-09-21 12:52:33.000000 celery-5.4.0rc1/t/unit/app/test_preload_cli.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2349 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/app/test_registry.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8026 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/app/test_routes.py
--rw-r--r--   0 nusnus     (501) staff       (20)    37899 2023-12-25 21:13:51.000000 celery-5.4.0rc1/t/unit/app/test_schedules.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1790 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/app/test_utils.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.200271 celery-5.4.0rc1/t/unit/apps/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/apps/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    16234 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/apps/test_multi.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.203098 celery-5.4.0rc1/t/unit/backends/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/backends/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8246 2023-12-25 21:13:51.000000 celery-5.4.0rc1/t/unit/backends/test_arangodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6874 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/backends/test_asynchronous.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6794 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/backends/test_azureblockblob.py
--rw-r--r--   0 nusnus     (501) staff       (20)    46922 2023-09-21 12:52:33.000000 celery-5.4.0rc1/t/unit/backends/test_base.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10318 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/backends/test_cache.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8669 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/backends/test_cassandra.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1448 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/backends/test_consul.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4994 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/backends/test_cosmosdbsql.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4846 2023-11-05 12:10:53.000000 celery-5.4.0rc1/t/unit/backends/test_couchbase.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3971 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/backends/test_couchdb.py
--rw-r--r--   0 nusnus     (501) staff       (20)    15087 2023-09-02 13:17:27.000000 celery-5.4.0rc1/t/unit/backends/test_database.py
--rw-r--r--   0 nusnus     (501) staff       (20)    19214 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/backends/test_dynamodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)    37379 2024-01-14 19:31:27.000000 celery-5.4.0rc1/t/unit/backends/test_elasticsearch.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4435 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/backends/test_filesystem.py
--rw-r--r--   0 nusnus     (501) staff       (20)    29399 2024-01-14 19:31:27.000000 celery-5.4.0rc1/t/unit/backends/test_mongodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)    50595 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/backends/test_redis.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3692 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/backends/test_rpc.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6654 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/backends/test_s3.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.203661 celery-5.4.0rc1/t/unit/bin/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/bin/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)       18 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/bin/celery.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.204266 celery-5.4.0rc1/t/unit/bin/proj/
--rw-r--r--   0 nusnus     (501) staff       (20)       64 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/bin/proj/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      121 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/bin/proj/app.py
--rw-r--r--   0 nusnus     (501) staff       (20)       22 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/bin/proj/app2.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1524 2023-09-21 12:52:33.000000 celery-5.4.0rc1/t/unit/bin/proj/pyramid_celery_app.py
--rw-r--r--   0 nusnus     (501) staff       (20)      109 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/bin/proj/scheduler.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1116 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/bin/test_beat.py
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/bin/test_multi.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1089 2023-09-21 12:52:33.000000 celery-5.4.0rc1/t/unit/bin/test_worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.205219 celery-5.4.0rc1/t/unit/concurrency/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/concurrency/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5687 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/concurrency/test_concurrency.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4721 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/concurrency/test_eventlet.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3146 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/concurrency/test_gevent.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1837 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/concurrency/test_pool.py
--rw-r--r--   0 nusnus     (501) staff       (20)    16398 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/concurrency/test_prefork.py
--rw-r--r--   0 nusnus     (501) staff       (20)      848 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/concurrency/test_solo.py
--rw-r--r--   0 nusnus     (501) staff       (20)      728 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/concurrency/test_thread.py
--rw-r--r--   0 nusnus     (501) staff       (20)    23214 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/conftest.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.206131 celery-5.4.0rc1/t/unit/contrib/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/contrib/__init__.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.206878 celery-5.4.0rc1/t/unit/contrib/proj/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/contrib/proj/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      183 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/contrib/proj/conf.py
--rw-r--r--   0 nusnus     (501) staff       (20)       93 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/contrib/proj/contents.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      249 2023-02-01 17:22:50.000000 celery-5.4.0rc1/t/unit/contrib/proj/foo.py
--rw-r--r--   0 nusnus     (501) staff       (20)      113 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/contrib/proj/xyzzy.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1394 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/contrib/test_abortable.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10615 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/contrib/test_migrate.py
--rw-r--r--   0 nusnus     (501) staff       (20)      785 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/contrib/test_pytest.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3146 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/contrib/test_rdb.py
--rw-r--r--   0 nusnus     (501) staff       (20)      731 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/contrib/test_sphinx.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1474 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/contrib/test_worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.207496 celery-5.4.0rc1/t/unit/events/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/events/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2304 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/events/test_cursesmon.py
--rw-r--r--   0 nusnus     (501) staff       (20)    11372 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/events/test_events.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3359 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/events/test_snapshot.py
--rw-r--r--   0 nusnus     (501) staff       (20)    22261 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/events/test_state.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.207773 celery-5.4.0rc1/t/unit/fixups/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/fixups/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    11015 2023-09-21 12:52:33.000000 celery-5.4.0rc1/t/unit/fixups/test_django.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.208570 celery-5.4.0rc1/t/unit/security/
--rw-r--r--   0 nusnus     (501) staff       (20)     7344 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/security/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      109 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/security/case.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3369 2023-12-25 21:13:51.000000 celery-5.4.0rc1/t/unit/security/test_certificate.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1570 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/security/test_key.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6219 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/security/test_security.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2224 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/security/test_serialization.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.210244 celery-5.4.0rc1/t/unit/tasks/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/tasks/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    69239 2024-01-17 16:29:51.000000 celery-5.4.0rc1/t/unit/tasks/test_canvas.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12308 2023-09-02 13:17:27.000000 celery-5.4.0rc1/t/unit/tasks/test_chord.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3134 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/tasks/test_context.py
--rw-r--r--   0 nusnus     (501) staff       (20)    35464 2023-11-14 10:15:09.000000 celery-5.4.0rc1/t/unit/tasks/test_result.py
--rw-r--r--   0 nusnus     (501) staff       (20)    55282 2023-12-11 00:09:28.000000 celery-5.4.0rc1/t/unit/tasks/test_stamping.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1085 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/tasks/test_states.py
--rw-r--r--   0 nusnus     (501) staff       (20)    58927 2023-10-10 19:45:26.000000 celery-5.4.0rc1/t/unit/tasks/test_tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)    21991 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/tasks/test_trace.py
--rw-r--r--   0 nusnus     (501) staff       (20)       78 2022-08-17 13:45:35.000000 celery-5.4.0rc1/t/unit/tasks/unit_tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)      989 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/test_canvas.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.213429 celery-5.4.0rc1/t/unit/utils/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/utils/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    13188 2023-09-21 12:52:33.000000 celery-5.4.0rc1/t/unit/utils/test_collections.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2357 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/utils/test_debug.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1739 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/utils/test_deprecated.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5233 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/utils/test_dispatcher.py
--rw-r--r--   0 nusnus     (501) staff       (20)    13576 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/utils/test_functional.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1935 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/utils/test_graph.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4064 2023-09-21 12:52:33.000000 celery-5.4.0rc1/t/unit/utils/test_imports.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8515 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/utils/test_local.py
--rw-r--r--   0 nusnus     (501) staff       (20)      202 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/utils/test_nodenames.py
--rw-r--r--   0 nusnus     (501) staff       (20)      172 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/utils/test_objects.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1386 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/utils/test_pickle.py
--rw-r--r--   0 nusnus     (501) staff       (20)    32949 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/utils/test_platforms.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5555 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/utils/test_saferepr.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3256 2023-12-25 21:13:51.000000 celery-5.4.0rc1/t/unit/utils/test_serialization.py
--rw-r--r--   0 nusnus     (501) staff       (20)      751 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/utils/test_sysinfo.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2261 2024-01-07 22:36:19.000000 celery-5.4.0rc1/t/unit/utils/test_term.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1935 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/utils/test_text.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2427 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/utils/test_threads.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12135 2024-01-14 19:31:27.000000 celery-5.4.0rc1/t/unit/utils/test_time.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3215 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/utils/test_timer2.py
--rw-r--r--   0 nusnus     (501) staff       (20)      624 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/utils/test_utils.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-01-17 17:52:21.215047 celery-5.4.0rc1/t/unit/worker/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc1/t/unit/worker/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7574 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/worker/test_autoscale.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9415 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/worker/test_bootsteps.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2461 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/worker/test_components.py
--rw-r--r--   0 nusnus     (501) staff       (20)    31296 2023-11-23 09:45:25.000000 celery-5.4.0rc1/t/unit/worker/test_consumer.py
--rw-r--r--   0 nusnus     (501) staff       (20)    28334 2023-06-26 13:41:34.000000 celery-5.4.0rc1/t/unit/worker/test_control.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2384 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/worker/test_heartbeat.py
--rw-r--r--   0 nusnus     (501) staff       (20)    18256 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/worker/test_loops.py
--rw-r--r--   0 nusnus     (501) staff       (20)    48168 2023-12-25 21:13:51.000000 celery-5.4.0rc1/t/unit/worker/test_request.py
--rw-r--r--   0 nusnus     (501) staff       (20)      238 2022-12-29 15:36:27.000000 celery-5.4.0rc1/t/unit/worker/test_revoke.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6339 2023-06-26 13:41:34.000000 celery-5.4.0rc1/t/unit/worker/test_state.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12171 2023-09-21 12:52:33.000000 celery-5.4.0rc1/t/unit/worker/test_strategy.py
--rw-r--r--   0 nusnus     (501) staff       (20)    39912 2023-06-21 21:46:53.000000 celery-5.4.0rc1/t/unit/worker/test_worker.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.308153 celery-5.4.0rc2/
+-rw-r--r--   0 nusnus     (501) staff       (20)     8316 2024-03-11 10:08:15.000000 celery-5.4.0rc2/CONTRIBUTORS.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)    38288 2024-03-27 15:12:17.000000 celery-5.4.0rc2/Changelog.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     2717 2023-09-21 12:52:33.000000 celery-5.4.0rc2/LICENSE
+-rw-r--r--   0 nusnus     (501) staff       (20)      709 2022-08-03 16:05:58.000000 celery-5.4.0rc2/MANIFEST.in
+-rw-r--r--   0 nusnus     (501) staff       (20)    21333 2024-03-27 15:13:31.307569 celery-5.4.0rc2/PKG-INFO
+-rw-r--r--   0 nusnus     (501) staff       (20)    16182 2024-03-27 15:12:52.000000 celery-5.4.0rc2/README.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)       84 2022-08-03 16:05:58.000000 celery-5.4.0rc2/TODO
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.132482 celery-5.4.0rc2/celery/
+-rw-r--r--   0 nusnus     (501) staff       (20)     5950 2024-03-27 15:12:52.000000 celery-5.4.0rc2/celery/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      409 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/__main__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5029 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/_state.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.135556 celery-5.4.0rc2/celery/app/
+-rw-r--r--   0 nusnus     (501) staff       (20)     2430 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/app/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    23236 2023-09-21 12:52:33.000000 celery-5.4.0rc2/celery/app/amqp.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1445 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/app/annotations.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2506 2023-09-21 12:52:33.000000 celery-5.4.0rc2/celery/app/autoretry.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2746 2024-03-11 13:40:32.000000 celery-5.4.0rc2/celery/app/backends.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    50584 2024-03-11 10:08:15.000000 celery-5.4.0rc2/celery/app/base.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6673 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/app/builtins.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    29171 2023-10-10 19:45:26.000000 celery-5.4.0rc2/celery/app/control.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    15266 2024-03-11 13:40:32.000000 celery-5.4.0rc2/celery/app/defaults.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1326 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/app/events.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9067 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/app/log.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2001 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/app/registry.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4527 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/app/routes.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    43794 2023-11-19 15:09:26.000000 celery-5.4.0rc2/celery/app/task.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    27551 2024-03-11 10:08:15.000000 celery-5.4.0rc2/celery/app/trace.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    13160 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/app/utils.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.136208 celery-5.4.0rc2/celery/apps/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/celery/apps/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5724 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/apps/beat.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    16360 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/apps/multi.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    13291 2024-03-24 18:19:04.000000 celery-5.4.0rc2/celery/apps/worker.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.139913 celery-5.4.0rc2/celery/backends/
+-rw-r--r--   0 nusnus     (501) staff       (20)       23 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/backends/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5937 2023-09-21 12:52:33.000000 celery-5.4.0rc2/celery/backends/arangodb.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    10309 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/backends/asynchronous.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5127 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/backends/azureblockblob.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    43982 2024-03-11 10:08:15.000000 celery-5.4.0rc2/celery/backends/base.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4831 2023-09-21 12:52:33.000000 celery-5.4.0rc2/celery/backends/cache.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9006 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/backends/cassandra.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3816 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/backends/consul.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6777 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/backends/cosmosdbsql.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3393 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/backends/couchbase.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2935 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/backends/couchdb.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.140373 celery-5.4.0rc2/celery/backends/database/
+-rw-r--r--   0 nusnus     (501) staff       (20)     7751 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/backends/database/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3394 2024-03-11 10:08:15.000000 celery-5.4.0rc2/celery/backends/database/models.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3011 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/backends/database/session.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    19348 2024-03-11 10:08:15.000000 celery-5.4.0rc2/celery/backends/dynamodb.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9583 2024-03-11 10:08:15.000000 celery-5.4.0rc2/celery/backends/elasticsearch.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3777 2024-03-20 15:46:18.000000 celery-5.4.0rc2/celery/backends/filesystem.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4716 2024-03-11 13:40:32.000000 celery-5.4.0rc2/celery/backends/gcs.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    11438 2024-01-29 20:44:38.000000 celery-5.4.0rc2/celery/backends/mongodb.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    26389 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/backends/redis.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    12077 2024-03-20 15:46:18.000000 celery-5.4.0rc2/celery/backends/rpc.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2752 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/backends/s3.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    24521 2024-03-11 10:08:15.000000 celery-5.4.0rc2/celery/beat.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.143150 celery-5.4.0rc2/celery/bin/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/bin/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    10023 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/bin/amqp.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9173 2024-03-11 10:08:15.000000 celery-5.4.0rc2/celery/bin/base.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2592 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/bin/beat.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2370 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/bin/call.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7440 2023-09-21 12:52:33.000000 celery-5.4.0rc2/celery/bin/celery.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8645 2024-03-11 10:08:15.000000 celery-5.4.0rc2/celery/bin/control.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2794 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/bin/events.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5796 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/bin/graph.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1058 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/bin/list.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4267 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/bin/logtool.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2108 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/bin/migrate.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    15374 2023-09-21 12:52:33.000000 celery-5.4.0rc2/celery/bin/multi.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2608 2023-09-21 12:52:33.000000 celery-5.4.0rc2/celery/bin/purge.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      976 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/bin/result.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4839 2023-09-21 12:52:33.000000 celery-5.4.0rc2/celery/bin/shell.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3064 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/bin/upgrade.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    12886 2023-09-21 12:52:33.000000 celery-5.4.0rc2/celery/bin/worker.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    12277 2024-03-27 11:52:49.000000 celery-5.4.0rc2/celery/bootsteps.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    96756 2024-03-20 15:46:18.000000 celery-5.4.0rc2/celery/canvas.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.144437 celery-5.4.0rc2/celery/concurrency/
+-rw-r--r--   0 nusnus     (501) staff       (20)     1457 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/concurrency/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    51466 2024-03-20 15:46:18.000000 celery-5.4.0rc2/celery/concurrency/asynpool.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4706 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/concurrency/base.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5126 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/concurrency/eventlet.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3387 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/concurrency/gevent.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5850 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/concurrency/prefork.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      754 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/concurrency/solo.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1807 2023-09-21 12:52:33.000000 celery-5.4.0rc2/celery/concurrency/thread.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.145479 celery-5.4.0rc2/celery/contrib/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/celery/contrib/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5003 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/contrib/abortable.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.145743 celery-5.4.0rc2/celery/contrib/django/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-03-11 10:08:15.000000 celery-5.4.0rc2/celery/contrib/django/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      725 2024-03-11 10:08:15.000000 celery-5.4.0rc2/celery/contrib/django/task.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    14361 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/contrib/migrate.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6754 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/contrib/pytest.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5005 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/contrib/rdb.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3391 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/contrib/sphinx.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.146999 celery-5.4.0rc2/celery/contrib/testing/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/celery/contrib/testing/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3112 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/contrib/testing/app.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8605 2023-09-21 12:52:33.000000 celery-5.4.0rc2/celery/contrib/testing/manager.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4182 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/contrib/testing/mocks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      208 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/contrib/testing/tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7064 2023-10-17 13:52:33.000000 celery-5.4.0rc2/celery/contrib/testing/worker.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.148441 celery-5.4.0rc2/celery/events/
+-rw-r--r--   0 nusnus     (501) staff       (20)      477 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/events/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    17961 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/events/cursesmon.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8987 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/events/dispatcher.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3116 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/events/dumper.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1736 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/events/event.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4998 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/events/receiver.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3294 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/events/snapshot.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    25648 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/events/state.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9086 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/exceptions.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.148779 celery-5.4.0rc2/celery/fixups/
+-rw-r--r--   0 nusnus     (501) staff       (20)       14 2022-08-03 16:05:58.000000 celery-5.4.0rc2/celery/fixups/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7300 2024-03-11 10:08:15.000000 celery-5.4.0rc2/celery/fixups/django.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.149568 celery-5.4.0rc2/celery/loaders/
+-rw-r--r--   0 nusnus     (501) staff       (20)      490 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/loaders/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      199 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/loaders/app.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9147 2024-01-29 20:44:38.000000 celery-5.4.0rc2/celery/loaders/base.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1520 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/loaders/default.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    16087 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/local.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    25289 2023-09-25 15:17:42.000000 celery-5.4.0rc2/celery/platforms.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    35612 2023-10-10 19:45:26.000000 celery-5.4.0rc2/celery/result.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    32003 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/schedules.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.150257 celery-5.4.0rc2/celery/security/
+-rw-r--r--   0 nusnus     (501) staff       (20)     2363 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/security/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4026 2024-01-29 20:44:38.000000 celery-5.4.0rc2/celery/security/certificate.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1189 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/security/key.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4248 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/security/serialization.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      845 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/security/utils.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4384 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/signals.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3324 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/states.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.153460 celery-5.4.0rc2/celery/utils/
+-rw-r--r--   0 nusnus     (501) staff       (20)      935 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/utils/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2874 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/utils/abstract.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    25432 2023-10-17 13:52:33.000000 celery-5.4.0rc2/celery/utils/collections.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4709 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/utils/debug.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3620 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/utils/deprecated.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.153737 celery-5.4.0rc2/celery/utils/dispatch/
+-rw-r--r--   0 nusnus     (501) staff       (20)       74 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/utils/dispatch/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    13603 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/utils/dispatch/signal.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    12017 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/utils/functional.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9041 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/utils/graph.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5126 2023-09-21 12:52:33.000000 celery-5.4.0rc2/celery/utils/imports.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2916 2024-01-29 20:44:38.000000 celery-5.4.0rc2/celery/utils/iso8601.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8757 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/utils/log.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3163 2024-01-29 20:44:38.000000 celery-5.4.0rc2/celery/utils/nodenames.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4215 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/utils/objects.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9020 2023-10-17 13:52:33.000000 celery-5.4.0rc2/celery/utils/saferepr.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8209 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/utils/serialization.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.154091 celery-5.4.0rc2/celery/utils/static/
+-rw-r--r--   0 nusnus     (501) staff       (20)      299 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/utils/static/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2556 2022-08-03 16:05:58.000000 celery-5.4.0rc2/celery/utils/static/celery_128.png
+-rw-r--r--   0 nusnus     (501) staff       (20)     1264 2024-01-29 20:44:38.000000 celery-5.4.0rc2/celery/utils/sysinfo.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5135 2024-01-29 20:44:38.000000 celery-5.4.0rc2/celery/utils/term.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5844 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/utils/text.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9552 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/utils/threads.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    15039 2024-03-11 10:08:15.000000 celery-5.4.0rc2/celery/utils/time.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4813 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/utils/timer2.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.155746 celery-5.4.0rc2/celery/worker/
+-rw-r--r--   0 nusnus     (501) staff       (20)       95 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/worker/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4593 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/worker/autoscale.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7497 2024-03-27 11:52:49.000000 celery-5.4.0rc2/celery/worker/components.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.157412 celery-5.4.0rc2/celery/worker/consumer/
+-rw-r--r--   0 nusnus     (501) staff       (20)      391 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/worker/consumer/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      525 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/worker/consumer/agent.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1026 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/worker/consumer/connection.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    29091 2024-03-27 11:52:49.000000 celery-5.4.0rc2/celery/worker/consumer/consumer.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      946 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/worker/consumer/control.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2054 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/worker/consumer/events.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6863 2023-11-14 10:15:09.000000 celery-5.4.0rc2/celery/worker/consumer/gossip.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      930 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/worker/consumer/heart.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2519 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/worker/consumer/mingle.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1960 2023-06-21 21:46:53.000000 celery-5.4.0rc2/celery/worker/consumer/tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    19882 2023-11-19 15:09:26.000000 celery-5.4.0rc2/celery/worker/control.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2107 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/worker/heartbeat.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4433 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/worker/loops.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3630 2022-12-29 15:36:27.000000 celery-5.4.0rc2/celery/worker/pidbox.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    27229 2023-06-26 13:41:34.000000 celery-5.4.0rc2/celery/worker/request.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8583 2023-06-26 13:41:34.000000 celery-5.4.0rc2/celery/worker/state.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7324 2023-09-21 12:52:33.000000 celery-5.4.0rc2/celery/worker/strategy.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    14488 2024-03-27 11:52:49.000000 celery-5.4.0rc2/celery/worker/worker.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.302947 celery-5.4.0rc2/celery.egg-info/
+-rw-r--r--   0 nusnus     (501) staff       (20)    21333 2024-03-27 15:13:31.000000 celery-5.4.0rc2/celery.egg-info/PKG-INFO
+-rw-r--r--   0 nusnus     (501) staff       (20)    22931 2024-03-27 15:13:31.000000 celery-5.4.0rc2/celery.egg-info/SOURCES.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)        1 2024-03-27 15:13:31.000000 celery-5.4.0rc2/celery.egg-info/dependency_links.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       48 2024-03-27 15:13:31.000000 celery-5.4.0rc2/celery.egg-info/entry_points.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)     1914 2024-03-27 15:13:31.000000 celery-5.4.0rc2/celery.egg-info/requires.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)        7 2024-03-27 15:13:31.000000 celery-5.4.0rc2/celery.egg-info/top_level.txt
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.161435 celery-5.4.0rc2/docs/
+-rw-r--r--   0 nusnus     (501) staff       (20)     6148 2024-02-25 18:37:34.000000 celery-5.4.0rc2/docs/.DS_Store
+-rw-r--r--   0 nusnus     (501) staff       (20)     5293 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/AUTHORS.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)     8111 2024-01-18 00:07:31.000000 celery-5.4.0rc2/docs/Makefile
+-rw-r--r--   0 nusnus     (501) staff       (20)      494 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/THANKS
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.161735 celery-5.4.0rc2/docs/_ext/
+-rw-r--r--   0 nusnus     (501) staff       (20)     5164 2022-12-29 15:36:27.000000 celery-5.4.0rc2/docs/_ext/celerydocs.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.162169 celery-5.4.0rc2/docs/_static/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/_static/.keep
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.162281 celery-5.4.0rc2/docs/_templates/
+-rw-r--r--   0 nusnus     (501) staff       (20)      486 2022-12-29 15:36:27.000000 celery-5.4.0rc2/docs/_templates/sidebardonations.html
+-rw-r--r--   0 nusnus     (501) staff       (20)       30 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/changelog.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      981 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/community.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     2616 2024-03-11 10:08:15.000000 celery-5.4.0rc2/docs/conf.py
+-rw-r--r--   0 nusnus     (501) staff       (20)       83 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/configuration.html
+-rw-r--r--   0 nusnus     (501) staff       (20)       33 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/contributing.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      931 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/copyright.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.162860 celery-5.4.0rc2/docs/django/
+-rw-r--r--   0 nusnus     (501) staff       (20)    10126 2024-03-11 10:08:15.000000 celery-5.4.0rc2/docs/django/first-steps-with-django.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      137 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/django/index.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    29852 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/faq.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.164214 celery-5.4.0rc2/docs/getting-started/
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.165173 celery-5.4.0rc2/docs/getting-started/backends-and-brokers/
+-rw-r--r--   0 nusnus     (501) staff       (20)     3905 2023-11-19 15:09:26.000000 celery-5.4.0rc2/docs/getting-started/backends-and-brokers/index.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     5010 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/getting-started/backends-and-brokers/rabbitmq.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     8384 2024-01-29 20:44:38.000000 celery-5.4.0rc2/docs/getting-started/backends-and-brokers/redis.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    10845 2024-03-11 10:08:15.000000 celery-5.4.0rc2/docs/getting-started/backends-and-brokers/sqs.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    14995 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/getting-started/first-steps-with-celery.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-12-29 15:36:27.000000 celery-5.4.0rc2/docs/getting-started/index.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    10938 2024-03-11 13:40:32.000000 celery-5.4.0rc2/docs/getting-started/introduction.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    22874 2023-11-14 10:15:09.000000 celery-5.4.0rc2/docs/getting-started/next-steps.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      132 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/getting-started/resources.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     4448 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/glossary.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.179865 celery-5.4.0rc2/docs/history/
+-rw-r--r--   0 nusnus     (501) staff       (20)    58104 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/history/changelog-1.0.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    34009 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/history/changelog-2.0.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    23550 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/changelog-2.1.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    33558 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/history/changelog-2.2.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    11200 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/history/changelog-2.3.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    13012 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/history/changelog-2.4.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     5414 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/changelog-2.5.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    49344 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/history/changelog-3.0.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    52336 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/history/changelog-3.1.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     6432 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/changelog-4.0.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     8950 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/changelog-4.1.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    13593 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/changelog-4.2.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    17251 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/changelog-4.3.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    24332 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/changelog-4.4.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     5720 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/history/changelog-5.0.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     5592 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/history/changelog-5.1.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      692 2024-03-11 10:08:15.000000 celery-5.4.0rc2/docs/history/index.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    16026 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/whatsnew-2.5.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    30892 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/whatsnew-3.0.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    44129 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/whatsnew-3.1.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    76466 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/history/whatsnew-4.0.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     8244 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/whatsnew-4.1.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    35711 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/whatsnew-4.2.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    16865 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/whatsnew-4.3.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     6999 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/whatsnew-4.4.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    10957 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/history/whatsnew-5.0.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    14128 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/history/whatsnew-5.1.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    11263 2024-03-11 10:08:15.000000 celery-5.4.0rc2/docs/history/whatsnew-5.3.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.183012 celery-5.4.0rc2/docs/images/
+-rw-r--r--   0 nusnus     (501) staff       (20)    14168 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/images/celery-banner-small.png
+-rw-r--r--   0 nusnus     (501) staff       (20)    14038 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/images/celery-banner.png
+-rw-r--r--   0 nusnus     (501) staff       (20)     2556 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/images/celery_128.png
+-rw-r--r--   0 nusnus     (501) staff       (20)     8658 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/images/celery_512.png
+-rw-r--r--   0 nusnus     (501) staff       (20)    77397 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/images/celeryevshotsm.jpg
+-rw-r--r--   0 nusnus     (501) staff       (20)    88879 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/images/dashboard.png
+-rw-r--r--   0 nusnus     (501) staff       (20)     4286 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/images/favicon.ico
+-rw-r--r--   0 nusnus     (501) staff       (20)   146412 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/images/monitor.png
+-rw-r--r--   0 nusnus     (501) staff       (20)    35894 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/images/result_graph.png
+-rw-r--r--   0 nusnus     (501) staff       (20)    99783 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/images/worker_graph_full.png
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.183994 celery-5.4.0rc2/docs/includes/
+-rw-r--r--   0 nusnus     (501) staff       (20)     4120 2024-03-11 13:40:32.000000 celery-5.4.0rc2/docs/includes/installation.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)     6421 2024-03-27 15:12:52.000000 celery-5.4.0rc2/docs/includes/introduction.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)     1375 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/includes/resources.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)     1596 2024-03-11 10:08:15.000000 celery-5.4.0rc2/docs/index.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.185423 celery-5.4.0rc2/docs/internals/
+-rw-r--r--   0 nusnus     (501) staff       (20)     5985 2022-12-29 15:36:27.000000 celery-5.4.0rc2/docs/internals/app-overview.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     5696 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/internals/deprecation.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     8586 2023-02-01 20:37:32.000000 celery-5.4.0rc2/docs/internals/guide.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      206 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/index.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     9898 2022-12-29 15:36:27.000000 celery-5.4.0rc2/docs/internals/protocol.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.197698 celery-5.4.0rc2/docs/internals/reference/
+-rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery._state.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      257 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.app.annotations.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      224 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.app.routes.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.app.trace.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.arangodb.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.asynchronous.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      293 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.azureblockblob.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      243 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.base.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.cache.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      278 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.cassandra.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      253 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.consul.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      284 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.cosmosdbsql.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      270 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.couchbase.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      262 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.couchdb.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      276 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.database.models.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      293 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.database.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      283 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.database.session.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      265 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.dynamodb.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      280 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.elasticsearch.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      269 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.filesystem.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      248 2024-03-11 13:40:32.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.gcs.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.mongodb.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      254 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.redis.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      242 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.rpc.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      206 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      245 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.backends.s3.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      270 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.concurrency.base.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      310 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.concurrency.eventlet.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      304 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.concurrency.gevent.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      307 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.concurrency.prefork.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      229 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.concurrency.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      310 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.concurrency.solo.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      304 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.concurrency.thread.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      260 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.events.cursesmon.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      251 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.events.dumper.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      257 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.events.snapshot.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      231 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.platforms.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      272 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.security.certificate.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      248 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.security.key.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      278 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.security.serialization.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      254 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.security.utils.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.abstract.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      252 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.collections.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      260 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.deprecated.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      252 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.dispatch.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      295 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.dispatch.signal.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      282 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.functional.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      245 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.graph.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      273 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.imports.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.iso8601.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.log.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      257 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.nodenames.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.objects.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      195 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.saferepr.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      273 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.serialization.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.sysinfo.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.term.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.text.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      251 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.threads.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      258 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.time.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      224 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.utils.timer2.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.worker.autoscale.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      259 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.worker.components.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      260 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.worker.control.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      266 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.worker.heartbeat.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      236 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.worker.loops.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/reference/celery.worker.pidbox.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     1984 2024-03-11 13:40:32.000000 celery-5.4.0rc2/docs/internals/reference/index.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     1452 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/internals/worker.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     7675 2022-12-29 15:36:27.000000 celery-5.4.0rc2/docs/make.bat
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.211152 celery-5.4.0rc2/docs/reference/
+-rw-r--r--   0 nusnus     (501) staff       (20)     1379 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.app.amqp.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      237 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.app.autoretry.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      234 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.app.backends.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      268 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.app.builtins.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      265 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.app.control.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      290 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.app.defaults.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      222 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.app.events.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      213 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.app.log.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      228 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.app.registry.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      288 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.app.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.app.task.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      219 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.app.utils.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      253 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.apps.beat.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      236 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.apps.multi.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.apps.worker.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      220 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.beat.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      189 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/reference/celery.bin.amqp.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      216 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.base.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      254 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.beat.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      258 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.call.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      242 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.celery.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.control.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.events.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.graph.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      258 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.list.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.logtool.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.migrate.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      249 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.multi.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.purge.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.result.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.shell.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.upgrade.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      242 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bin.worker.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.bootsteps.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      290 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.contrib.abortable.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      310 2024-03-11 10:08:15.000000 celery-5.4.0rc2/docs/reference/celery.contrib.django.task.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      230 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.contrib.migrate.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      273 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.contrib.pytest.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.contrib.rdb.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      184 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.contrib.sphinx.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      288 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.contrib.testing.app.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      300 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.contrib.testing.manager.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.contrib.testing.mocks.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      297 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.contrib.testing.worker.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      304 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.events.dispatcher.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.events.event.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      303 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.events.receiver.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      194 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.events.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.events.state.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      222 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.exceptions.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      227 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.loaders.app.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      250 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.loaders.base.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      255 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.loaders.default.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      237 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.loaders.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      204 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.result.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     3497 2022-12-29 15:36:27.000000 celery-5.4.0rc2/docs/reference/celery.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.schedules.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      200 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.security.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      257 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.signals.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      106 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.states.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      871 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.utils.debug.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      291 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.consumer.agent.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      306 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.consumer.connection.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      300 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.consumer.consumer.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      297 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.consumer.control.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.consumer.events.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.consumer.gossip.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      291 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.consumer.heart.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.consumer.mingle.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      273 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.consumer.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      291 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.consumer.tasks.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      244 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.request.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      236 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.state.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      245 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.strategy.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/reference/celery.worker.worker.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      285 2023-09-21 12:52:33.000000 celery-5.4.0rc2/docs/reference/cli.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     1983 2024-03-11 10:08:15.000000 celery-5.4.0rc2/docs/reference/index.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.211787 celery-5.4.0rc2/docs/sec/
+-rw-r--r--   0 nusnus     (501) staff       (20)     2921 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/sec/CELERYSA-0001.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)     2656 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/sec/CELERYSA-0002.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)     1551 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/sec/CELERYSA-0003.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)     4879 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/spelling_wordlist.txt
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.211979 celery-5.4.0rc2/docs/templates/
+-rw-r--r--   0 nusnus     (501) staff       (20)     1186 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/templates/readme.txt
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.212867 celery-5.4.0rc2/docs/tutorials/
+-rw-r--r--   0 nusnus     (501) staff       (20)       86 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/tutorials/daemonizing.html
+-rw-r--r--   0 nusnus     (501) staff       (20)       91 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/tutorials/debugging.html
+-rw-r--r--   0 nusnus     (501) staff       (20)      121 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/tutorials/index.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     2766 2022-12-29 15:36:27.000000 celery-5.4.0rc2/docs/tutorials/task-cookbook.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.220465 celery-5.4.0rc2/docs/userguide/
+-rw-r--r--   0 nusnus     (501) staff       (20)    14779 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/userguide/application.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    25087 2023-09-21 12:52:33.000000 celery-5.4.0rc2/docs/userguide/calling.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    38136 2024-03-11 10:08:15.000000 celery-5.4.0rc2/docs/userguide/canvas.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.221497 celery-5.4.0rc2/docs/userguide/concurrency/
+-rw-r--r--   0 nusnus     (501) staff       (20)     2665 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/userguide/concurrency/eventlet.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     2872 2023-09-21 12:52:33.000000 celery-5.4.0rc2/docs/userguide/concurrency/gevent.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     1561 2024-01-29 20:44:38.000000 celery-5.4.0rc2/docs/userguide/concurrency/index.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)   106529 2024-03-11 13:40:32.000000 celery-5.4.0rc2/docs/userguide/configuration.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    17699 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/userguide/daemonizing.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     3131 2022-12-29 15:36:27.000000 celery-5.4.0rc2/docs/userguide/debugging.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    30057 2022-12-29 15:36:27.000000 celery-5.4.0rc2/docs/userguide/extending.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      372 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/userguide/index.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    21759 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/userguide/monitoring.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     8437 2022-12-29 15:36:27.000000 celery-5.4.0rc2/docs/userguide/optimizing.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    20946 2024-01-29 20:44:38.000000 celery-5.4.0rc2/docs/userguide/periodic-tasks.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    24323 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/userguide/routing.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     8693 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/userguide/security.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    18107 2023-11-14 10:15:09.000000 celery-5.4.0rc2/docs/userguide/signals.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      345 2022-08-03 16:05:58.000000 celery-5.4.0rc2/docs/userguide/sphinx.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    64549 2023-09-21 12:52:33.000000 celery-5.4.0rc2/docs/userguide/tasks.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    11146 2023-06-21 21:46:53.000000 celery-5.4.0rc2/docs/userguide/testing.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)    35007 2024-01-29 20:44:38.000000 celery-5.4.0rc2/docs/userguide/workers.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.222089 celery-5.4.0rc2/examples/
+-rw-r--r--   0 nusnus     (501) staff       (20)     6148 2023-04-12 11:27:42.000000 celery-5.4.0rc2/examples/.DS_Store
+-rw-r--r--   0 nusnus     (501) staff       (20)      303 2022-08-03 16:05:58.000000 celery-5.4.0rc2/examples/README.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.222338 celery-5.4.0rc2/examples/app/
+-rw-r--r--   0 nusnus     (501) staff       (20)      822 2024-03-27 11:52:49.000000 celery-5.4.0rc2/examples/app/myapp.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.223650 celery-5.4.0rc2/examples/celery_http_gateway/
+-rw-r--r--   0 nusnus     (501) staff       (20)     1382 2022-08-03 16:05:58.000000 celery-5.4.0rc2/examples/celery_http_gateway/README.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/examples/celery_http_gateway/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      385 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/celery_http_gateway/manage.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3001 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/celery_http_gateway/settings.py
+-rw-r--r--   0 nusnus     (501) staff       (20)       88 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/celery_http_gateway/tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      678 2023-06-21 21:46:53.000000 celery-5.4.0rc2/examples/celery_http_gateway/urls.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.224325 celery-5.4.0rc2/examples/django/
+-rw-r--r--   0 nusnus     (501) staff       (20)     1754 2024-03-11 10:08:15.000000 celery-5.4.0rc2/examples/django/README.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.225010 celery-5.4.0rc2/examples/django/demoapp/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/examples/django/demoapp/__init__.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.227604 celery-5.4.0rc2/examples/django/demoapp/migrations/
+-rw-r--r--   0 nusnus     (501) staff       (20)      486 2022-08-03 16:05:58.000000 celery-5.4.0rc2/examples/django/demoapp/migrations/0001_initial.py
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/examples/django/demoapp/migrations/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      103 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/django/demoapp/models.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      437 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/django/demoapp/tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)       26 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/django/demoapp/views.py
+-rwxr-xr-x   0 nusnus     (501) staff       (20)      248 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/django/manage.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.230338 celery-5.4.0rc2/examples/django/proj/
+-rw-r--r--   0 nusnus     (501) staff       (20)      174 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/django/proj/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      659 2023-06-21 21:46:53.000000 celery-5.4.0rc2/examples/django/proj/celery.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3639 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/django/proj/settings.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      556 2023-02-01 17:22:50.000000 celery-5.4.0rc2/examples/django/proj/urls.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1132 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/django/proj/wsgi.py
+-rw-r--r--   0 nusnus     (501) staff       (20)       47 2023-06-21 21:46:53.000000 celery-5.4.0rc2/examples/django/requirements.txt
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.231439 celery-5.4.0rc2/examples/eventlet/
+-rw-r--r--   0 nusnus     (501) staff       (20)     1449 2023-06-21 21:46:53.000000 celery-5.4.0rc2/examples/eventlet/README.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     1673 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/eventlet/bulk_task_producer.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      312 2023-06-21 21:46:53.000000 celery-5.4.0rc2/examples/eventlet/celeryconfig.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      306 2023-06-21 21:46:53.000000 celery-5.4.0rc2/examples/eventlet/tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2009 2023-06-21 21:46:53.000000 celery-5.4.0rc2/examples/eventlet/webcrawler.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.232107 celery-5.4.0rc2/examples/gevent/
+-rw-r--r--   0 nusnus     (501) staff       (20)     1303 2023-09-21 12:52:33.000000 celery-5.4.0rc2/examples/gevent/README.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      255 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/gevent/celeryconfig.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      325 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/gevent/tasks.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.232274 celery-5.4.0rc2/examples/next-steps/
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.232749 celery-5.4.0rc2/examples/next-steps/proj/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/examples/next-steps/proj/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/next-steps/proj/celery.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      167 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/next-steps/proj/tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1224 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/next-steps/setup.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.232915 celery-5.4.0rc2/examples/periodic-tasks/
+-rw-r--r--   0 nusnus     (501) staff       (20)     1518 2023-06-21 21:46:53.000000 celery-5.4.0rc2/examples/periodic-tasks/myapp.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.233091 celery-5.4.0rc2/examples/resultgraph/
+-rw-r--r--   0 nusnus     (501) staff       (20)     2860 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/resultgraph/tasks.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.233282 celery-5.4.0rc2/examples/security/
+-rw-r--r--   0 nusnus     (501) staff       (20)     1058 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/security/mysecureapp.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.233722 celery-5.4.0rc2/examples/security/ssl/
+-rw-r--r--   0 nusnus     (501) staff       (20)     3243 2022-08-03 16:05:58.000000 celery-5.4.0rc2/examples/security/ssl/worker.key
+-rw-r--r--   0 nusnus     (501) staff       (20)     1923 2022-08-03 16:05:58.000000 celery-5.4.0rc2/examples/security/ssl/worker.pem
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.235182 celery-5.4.0rc2/examples/stamping/
+-rw-r--r--   0 nusnus     (501) staff       (20)      103 2023-06-21 21:46:53.000000 celery-5.4.0rc2/examples/stamping/config.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1358 2023-06-21 21:46:53.000000 celery-5.4.0rc2/examples/stamping/examples.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1806 2023-06-24 09:59:42.000000 celery-5.4.0rc2/examples/stamping/myapp.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2548 2023-06-21 21:46:53.000000 celery-5.4.0rc2/examples/stamping/revoke_example.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3311 2023-06-24 09:59:42.000000 celery-5.4.0rc2/examples/stamping/tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2410 2023-06-21 21:46:53.000000 celery-5.4.0rc2/examples/stamping/visitors.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.235401 celery-5.4.0rc2/examples/tutorial/
+-rw-r--r--   0 nusnus     (501) staff       (20)      158 2022-12-29 15:36:27.000000 celery-5.4.0rc2/examples/tutorial/tasks.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.125584 celery-5.4.0rc2/extra/
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.235554 celery-5.4.0rc2/extra/bash-completion/
+-rw-r--r--   0 nusnus     (501) staff       (20)      636 2022-12-29 15:36:27.000000 celery-5.4.0rc2/extra/bash-completion/celery.bash
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.235921 celery-5.4.0rc2/extra/generic-init.d/
+-rwxr-xr-x   0 nusnus     (501) staff       (20)     9068 2023-06-21 21:46:53.000000 celery-5.4.0rc2/extra/generic-init.d/celerybeat
+-rwxr-xr-x   0 nusnus     (501) staff       (20)    10813 2023-06-21 21:46:53.000000 celery-5.4.0rc2/extra/generic-init.d/celeryd
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.236354 celery-5.4.0rc2/extra/macOS/
+-rw-r--r--   0 nusnus     (501) staff       (20)      751 2022-08-03 16:05:58.000000 celery-5.4.0rc2/extra/macOS/org.celeryq.beat.plist
+-rw-r--r--   0 nusnus     (501) staff       (20)      757 2022-08-03 16:05:58.000000 celery-5.4.0rc2/extra/macOS/org.celeryq.worker.plist
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.237291 celery-5.4.0rc2/extra/supervisord/
+-rw-r--r--   0 nusnus     (501) staff       (20)      134 2022-08-03 16:05:58.000000 celery-5.4.0rc2/extra/supervisord/celery.sh
+-rw-r--r--   0 nusnus     (501) staff       (20)      699 2022-12-29 15:36:27.000000 celery-5.4.0rc2/extra/supervisord/celerybeat.conf
+-rw-r--r--   0 nusnus     (501) staff       (20)      949 2022-12-29 15:36:27.000000 celery-5.4.0rc2/extra/supervisord/celeryd.conf
+-rw-r--r--   0 nusnus     (501) staff       (20)      982 2023-06-21 21:46:53.000000 celery-5.4.0rc2/extra/supervisord/supervisord.conf
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.238073 celery-5.4.0rc2/extra/systemd/
+-rw-r--r--   0 nusnus     (501) staff       (20)      506 2023-06-21 21:46:53.000000 celery-5.4.0rc2/extra/systemd/celery.conf
+-rw-r--r--   0 nusnus     (501) staff       (20)      740 2022-12-29 15:36:27.000000 celery-5.4.0rc2/extra/systemd/celery.service
+-rw-r--r--   0 nusnus     (501) staff       (20)       78 2022-08-03 16:05:58.000000 celery-5.4.0rc2/extra/systemd/celery.tmpfiles
+-rw-r--r--   0 nusnus     (501) staff       (20)      395 2022-12-29 15:36:27.000000 celery-5.4.0rc2/extra/systemd/celerybeat.service
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.238233 celery-5.4.0rc2/extra/zsh-completion/
+-rw-r--r--   0 nusnus     (501) staff       (20)     6244 2022-08-03 16:05:58.000000 celery-5.4.0rc2/extra/zsh-completion/celery.zsh
+-rw-r--r--   0 nusnus     (501) staff       (20)     1216 2023-06-21 21:46:53.000000 celery-5.4.0rc2/pyproject.toml
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.240628 celery-5.4.0rc2/requirements/
+-rw-r--r--   0 nusnus     (501) staff       (20)     1368 2024-03-11 10:09:31.000000 celery-5.4.0rc2/requirements/README.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      273 2023-11-19 15:09:26.000000 celery-5.4.0rc2/requirements/default.txt
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.240755 celery-5.4.0rc2/requirements/deps/
+-rw-r--r--   0 nusnus     (501) staff       (20)       10 2022-08-03 16:05:58.000000 celery-5.4.0rc2/requirements/deps/mock.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      151 2024-03-11 10:08:15.000000 celery-5.4.0rc2/requirements/dev.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      180 2024-03-11 10:08:15.000000 celery-5.4.0rc2/requirements/docs.txt
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.245778 celery-5.4.0rc2/requirements/extras/
+-rw-r--r--   0 nusnus     (501) staff       (20)       16 2023-09-21 12:52:33.000000 celery-5.4.0rc2/requirements/extras/arangodb.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       21 2024-03-11 10:08:15.000000 celery-5.4.0rc2/requirements/extras/auth.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       28 2023-06-21 21:46:53.000000 celery-5.4.0rc2/requirements/extras/azureblockblob.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      111 2022-08-03 16:05:58.000000 celery-5.4.0rc2/requirements/extras/brotli.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       28 2023-06-21 21:46:53.000000 celery-5.4.0rc2/requirements/extras/cassandra.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       22 2023-06-21 21:46:53.000000 celery-5.4.0rc2/requirements/extras/consul.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       20 2023-06-21 21:46:53.000000 celery-5.4.0rc2/requirements/extras/cosmosdbsql.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      119 2023-11-05 11:35:58.000000 celery-5.4.0rc2/requirements/extras/couchbase.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       18 2023-06-21 21:46:53.000000 celery-5.4.0rc2/requirements/extras/couchdb.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       15 2023-06-21 21:46:53.000000 celery-5.4.0rc2/requirements/extras/django.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       16 2023-09-21 12:52:33.000000 celery-5.4.0rc2/requirements/extras/dynamodb.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       48 2024-03-11 10:08:15.000000 celery-5.4.0rc2/requirements/extras/elasticsearch.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       40 2022-12-29 15:36:27.000000 celery-5.4.0rc2/requirements/extras/eventlet.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       29 2024-03-11 13:40:32.000000 celery-5.4.0rc2/requirements/extras/gcs.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       14 2022-12-29 15:36:27.000000 celery-5.4.0rc2/requirements/extras/gevent.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       44 2023-09-21 12:52:33.000000 celery-5.4.0rc2/requirements/extras/librabbitmq.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       45 2023-06-21 21:46:53.000000 celery-5.4.0rc2/requirements/extras/memcache.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       20 2023-06-21 21:46:53.000000 celery-5.4.0rc2/requirements/extras/mongodb.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       15 2024-03-11 11:02:58.000000 celery-5.4.0rc2/requirements/extras/msgpack.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       23 2024-03-11 10:08:15.000000 celery-5.4.0rc2/requirements/extras/pymemcache.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       37 2023-09-21 12:52:33.000000 celery-5.4.0rc2/requirements/extras/pyro.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       29 2024-03-27 14:48:28.000000 celery-5.4.0rc2/requirements/extras/pytest.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       28 2024-01-17 23:27:42.000000 celery-5.4.0rc2/requirements/extras/redis.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       16 2023-09-21 12:52:33.000000 celery-5.4.0rc2/requirements/extras/s3.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       27 2022-08-03 16:05:58.000000 celery-5.4.0rc2/requirements/extras/slmq.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       53 2023-10-12 19:13:02.000000 celery-5.4.0rc2/requirements/extras/solar.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       27 2022-12-29 15:36:27.000000 celery-5.4.0rc2/requirements/extras/sphinxautobuild.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       24 2023-06-26 13:41:34.000000 celery-5.4.0rc2/requirements/extras/sqlalchemy.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      139 2024-03-11 10:08:15.000000 celery-5.4.0rc2/requirements/extras/sqs.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       73 2022-08-03 16:05:58.000000 celery-5.4.0rc2/requirements/extras/tblib.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       39 2022-08-03 16:05:58.000000 celery-5.4.0rc2/requirements/extras/thread.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       13 2022-08-03 16:05:58.000000 celery-5.4.0rc2/requirements/extras/yaml.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       14 2023-06-21 21:46:53.000000 celery-5.4.0rc2/requirements/extras/zeromq.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       13 2022-08-03 16:05:58.000000 celery-5.4.0rc2/requirements/extras/zookeeper.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       18 2023-11-14 10:15:09.000000 celery-5.4.0rc2/requirements/extras/zstd.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      212 2023-09-21 12:52:33.000000 celery-5.4.0rc2/requirements/pkgutils.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       19 2022-08-03 16:05:58.000000 celery-5.4.0rc2/requirements/security.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      175 2024-03-26 11:51:30.000000 celery-5.4.0rc2/requirements/test-ci-base.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      613 2023-11-14 10:15:09.000000 celery-5.4.0rc2/requirements/test-ci-default.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      160 2023-06-21 21:46:53.000000 celery-5.4.0rc2/requirements/test-integration.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       17 2022-08-03 16:05:58.000000 celery-5.4.0rc2/requirements/test-pypy3.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      440 2024-03-27 14:48:28.000000 celery-5.4.0rc2/requirements/test.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      486 2024-03-27 15:13:31.308627 celery-5.4.0rc2/setup.cfg
+-rwxr-xr-x   0 nusnus     (501) staff       (20)     4651 2024-03-11 13:40:32.000000 celery-5.4.0rc2/setup.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.246054 celery-5.4.0rc2/t/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2023-09-25 19:52:57.000000 celery-5.4.0rc2/t/__init__.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.246295 celery-5.4.0rc2/t/benchmarks/
+-rw-r--r--   0 nusnus     (501) staff       (20)     2816 2023-09-21 12:52:33.000000 celery-5.4.0rc2/t/benchmarks/bench_worker.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.251690 celery-5.4.0rc2/t/integration/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2023-09-25 17:14:49.000000 celery-5.4.0rc2/t/integration/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2304 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/integration/conftest.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    12850 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/integration/tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1120 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/integration/test_backend.py
+-rw-r--r--   0 nusnus     (501) staff       (20)   137940 2024-03-11 11:02:58.000000 celery-5.4.0rc2/t/integration/test_canvas.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7815 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/integration/test_inspect.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1352 2023-11-23 07:26:02.000000 celery-5.4.0rc2/t/integration/test_loader.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3477 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/integration/test_security.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1651 2023-11-14 10:15:09.000000 celery-5.4.0rc2/t/integration/test_serialization.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      150 2023-11-14 10:15:09.000000 celery-5.4.0rc2/t/integration/test_serialization_config.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    22815 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/integration/test_tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      688 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/integration/test_worker.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      293 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/integration/test_worker_config.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/skip.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.252598 celery-5.4.0rc2/t/smoke/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1514 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/smoke/conftest.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.253612 celery-5.4.0rc2/t/smoke/operations/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/operations/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1504 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/smoke/operations/task_termination.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      929 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/operations/worker_kill.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1008 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/operations/worker_restart.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      781 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/signals.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1653 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/smoke/tasks.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.255974 celery-5.4.0rc2/t/smoke/tests/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/tests/__init__.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.256624 celery-5.4.0rc2/t/smoke/tests/failover/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/tests/failover/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2451 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/tests/failover/test_broker_failover.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1918 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/smoke/tests/failover/test_worker_failover.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.257928 celery-5.4.0rc2/t/smoke/tests/stamping/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/tests/stamping/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1215 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/smoke/tests/stamping/conftest.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      411 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/tests/stamping/signals.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      708 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/tests/stamping/tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5915 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/tests/stamping/test_hybrid_cluster.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2209 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/tests/stamping/test_revoke.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1457 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/tests/stamping/test_visitor.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.258252 celery-5.4.0rc2/t/smoke/tests/stamping/workers/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/tests/stamping/workers/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1491 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/tests/stamping/workers/legacy.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3208 2024-03-14 14:30:11.000000 celery-5.4.0rc2/t/smoke/tests/test_canvas.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5993 2024-03-11 19:54:33.000000 celery-5.4.0rc2/t/smoke/tests/test_consumer.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      688 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/tests/test_control.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1847 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/tests/test_signals.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4514 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/smoke/tests/test_tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2015 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/smoke/tests/test_thread_safe.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1676 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/smoke/tests/test_worker.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.259138 celery-5.4.0rc2/t/smoke/workers/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/workers/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1389 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/workers/alt.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1594 2024-03-14 17:25:52.000000 celery-5.4.0rc2/t/smoke/workers/dev.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1422 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/workers/latest.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1506 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/smoke/workers/other.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.259971 celery-5.4.0rc2/t/unit/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/__init__.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.265495 celery-5.4.0rc2/t/unit/app/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/app/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    13805 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/unit/app/test_amqp.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1338 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/app/test_annotations.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    41944 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/unit/app/test_app.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4540 2024-03-20 15:46:18.000000 celery-5.4.0rc2/t/unit/app/test_backends.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    31660 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/app/test_beat.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5528 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/app/test_builtins.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      356 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/app/test_celery.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    19105 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/app/test_control.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1608 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/app/test_defaults.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      829 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/unit/app/test_exceptions.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    11599 2023-11-23 07:26:02.000000 celery-5.4.0rc2/t/unit/app/test_loaders.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    11820 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/app/test_log.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1678 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/app/test_preload_cli.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2349 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/app/test_registry.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8026 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/app/test_routes.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    37899 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/unit/app/test_schedules.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1790 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/app/test_utils.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.265807 celery-5.4.0rc2/t/unit/apps/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/apps/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    16234 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/apps/test_multi.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.271714 celery-5.4.0rc2/t/unit/backends/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/backends/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8246 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/unit/backends/test_arangodb.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6874 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/backends/test_asynchronous.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6794 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/backends/test_azureblockblob.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    46922 2023-09-21 12:52:33.000000 celery-5.4.0rc2/t/unit/backends/test_base.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    10318 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/backends/test_cache.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8669 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/backends/test_cassandra.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1448 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/backends/test_consul.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4994 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/backends/test_cosmosdbsql.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4846 2023-11-05 12:10:53.000000 celery-5.4.0rc2/t/unit/backends/test_couchbase.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3971 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/backends/test_couchdb.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    15087 2023-09-02 13:17:27.000000 celery-5.4.0rc2/t/unit/backends/test_database.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    22513 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/backends/test_dynamodb.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    37379 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/backends/test_elasticsearch.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4435 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/backends/test_filesystem.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5728 2024-03-11 13:40:32.000000 celery-5.4.0rc2/t/unit/backends/test_gcs.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    29399 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/backends/test_mongodb.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    50596 2024-03-20 15:46:18.000000 celery-5.4.0rc2/t/unit/backends/test_redis.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3692 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/backends/test_rpc.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6731 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/backends/test_s3.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.273381 celery-5.4.0rc2/t/unit/bin/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/bin/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)       18 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/bin/celery.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.275545 celery-5.4.0rc2/t/unit/bin/proj/
+-rw-r--r--   0 nusnus     (501) staff       (20)       64 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/bin/proj/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      121 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/bin/proj/app.py
+-rw-r--r--   0 nusnus     (501) staff       (20)       22 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/bin/proj/app2.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      572 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/bin/proj/app_with_custom_cmds.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      118 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/bin/proj/daemon.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      564 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/bin/proj/daemon_config.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1524 2023-09-21 12:52:33.000000 celery-5.4.0rc2/t/unit/bin/proj/pyramid_celery_app.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      109 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/bin/proj/scheduler.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1116 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/bin/test_beat.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2721 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/bin/test_control.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      722 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/bin/test_daemonization.py
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/bin/test_multi.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1089 2023-09-21 12:52:33.000000 celery-5.4.0rc2/t/unit/bin/test_worker.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.277058 celery-5.4.0rc2/t/unit/concurrency/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/concurrency/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5687 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/concurrency/test_concurrency.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4721 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/concurrency/test_eventlet.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3146 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/concurrency/test_gevent.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1837 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/concurrency/test_pool.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    16398 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/concurrency/test_prefork.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      848 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/concurrency/test_solo.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      728 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/concurrency/test_thread.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    23215 2024-03-20 15:46:18.000000 celery-5.4.0rc2/t/unit/conftest.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.278619 celery-5.4.0rc2/t/unit/contrib/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/contrib/__init__.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.279024 celery-5.4.0rc2/t/unit/contrib/django/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/contrib/django/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      874 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/contrib/django/test_task.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.279981 celery-5.4.0rc2/t/unit/contrib/proj/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/contrib/proj/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      183 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/contrib/proj/conf.py
+-rw-r--r--   0 nusnus     (501) staff       (20)       93 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/contrib/proj/contents.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      249 2023-02-01 17:22:50.000000 celery-5.4.0rc2/t/unit/contrib/proj/foo.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      113 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/contrib/proj/xyzzy.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1394 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/contrib/test_abortable.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    10615 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/contrib/test_migrate.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      785 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/contrib/test_pytest.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3146 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/contrib/test_rdb.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      731 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/contrib/test_sphinx.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1466 2024-03-20 15:46:18.000000 celery-5.4.0rc2/t/unit/contrib/test_worker.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.280992 celery-5.4.0rc2/t/unit/events/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/events/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2304 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/events/test_cursesmon.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    11372 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/events/test_events.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3359 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/events/test_snapshot.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    22261 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/events/test_state.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.281307 celery-5.4.0rc2/t/unit/fixups/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/fixups/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    11901 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/fixups/test_django.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.282743 celery-5.4.0rc2/t/unit/security/
+-rw-r--r--   0 nusnus     (501) staff       (20)     7344 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/security/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      109 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/security/case.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3369 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/unit/security/test_certificate.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1570 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/security/test_key.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6219 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/security/test_security.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2224 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/security/test_serialization.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.286896 celery-5.4.0rc2/t/unit/tasks/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/tasks/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    71351 2024-03-11 11:02:58.000000 celery-5.4.0rc2/t/unit/tasks/test_canvas.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    12308 2023-09-02 13:17:27.000000 celery-5.4.0rc2/t/unit/tasks/test_chord.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3134 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/tasks/test_context.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    35464 2023-11-14 10:15:09.000000 celery-5.4.0rc2/t/unit/tasks/test_result.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    55282 2023-12-11 00:09:28.000000 celery-5.4.0rc2/t/unit/tasks/test_stamping.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1085 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/tasks/test_states.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    58927 2023-10-10 19:45:26.000000 celery-5.4.0rc2/t/unit/tasks/test_tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    21991 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/tasks/test_trace.py
+-rw-r--r--   0 nusnus     (501) staff       (20)       78 2022-08-17 13:45:35.000000 celery-5.4.0rc2/t/unit/tasks/unit_tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      989 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/test_canvas.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.294791 celery-5.4.0rc2/t/unit/utils/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/utils/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    13188 2023-09-21 12:52:33.000000 celery-5.4.0rc2/t/unit/utils/test_collections.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2357 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/utils/test_debug.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1739 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/utils/test_deprecated.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5233 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/utils/test_dispatcher.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    13576 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/utils/test_functional.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1935 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/utils/test_graph.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4064 2023-09-21 12:52:33.000000 celery-5.4.0rc2/t/unit/utils/test_imports.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8515 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/utils/test_local.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      202 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/utils/test_nodenames.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      172 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/utils/test_objects.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1386 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/utils/test_pickle.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    32949 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/utils/test_platforms.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5555 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/utils/test_saferepr.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3256 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/unit/utils/test_serialization.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      751 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/utils/test_sysinfo.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2261 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/unit/utils/test_term.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1935 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/utils/test_text.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2427 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/utils/test_threads.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    12135 2024-03-11 10:08:15.000000 celery-5.4.0rc2/t/unit/utils/test_time.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3215 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/utils/test_timer2.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      624 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/utils/test_utils.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 15:13:31.302439 celery-5.4.0rc2/t/unit/worker/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.4.0rc2/t/unit/worker/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7574 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/worker/test_autoscale.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9415 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/worker/test_bootsteps.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2461 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/worker/test_components.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    31296 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/unit/worker/test_consumer.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    28334 2023-06-26 13:41:34.000000 celery-5.4.0rc2/t/unit/worker/test_control.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2384 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/worker/test_heartbeat.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    18256 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/worker/test_loops.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    48168 2024-01-29 20:44:38.000000 celery-5.4.0rc2/t/unit/worker/test_request.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      238 2022-12-29 15:36:27.000000 celery-5.4.0rc2/t/unit/worker/test_revoke.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6339 2023-06-26 13:41:34.000000 celery-5.4.0rc2/t/unit/worker/test_state.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    12171 2023-09-21 12:52:33.000000 celery-5.4.0rc2/t/unit/worker/test_strategy.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    39912 2023-06-21 21:46:53.000000 celery-5.4.0rc2/t/unit/worker/test_worker.py
```

### Comparing `celery-5.4.0rc1/CONTRIBUTORS.txt` & `celery-5.4.0rc2/CONTRIBUTORS.txt`

 * *Files 2% similar despite different names*

```diff
@@ -291,8 +291,9 @@
 Tizian Seehaus, 2022/02/09
 Oleh Romanovskyi, 2022/06/09
 Tomer Nosrati, 2022/07/17
 JoonHwan Kim, 2022/08/01
 Kaustav Banerjee, 2022/11/10
 Austin Snoeyink 2022/12/06
 Jeremy Z. Othieno 2023/07/27
-Tomer Nosrati, 2022/17/07
+Tomer Nosrati, 2022/17/07
+Andy Zickler, 2024/01/18
```

### Comparing `celery-5.4.0rc1/Changelog.rst` & `celery-5.4.0rc2/Changelog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,71 @@
  Change history
 ================
 
 This document contains change notes for bugfix & new features
 in the main branch & 5.3.x series, please see :ref:`whatsnew-5.3` for
 an overview of what's new in Celery 5.3.
 
+.. _version-5.4.0rc2:
+
+5.4.0rc2
+========
+
+:release-date: 2024-03-27
+:release-by: Tomer Nosrati
+
+- feat(daemon): allows daemonization options to be fetched from app settings (#8553)
+- Fixed version documentation tag from #8553 in configuration.rst (#8802)
+- Upgraded Sphinx from v5.3.0 to v7.x.x (#8803)
+- Update elasticsearch requirement from <=8.11.1 to <=8.12.0 (#8810)
+- Update elastic-transport requirement from <=8.11.0 to <=8.12.0 (#8811)
+- Update cryptography to 42.0.0 (#8814)
+- Catch UnicodeDecodeError when opening corrupt beat-schedule.db (#8806)
+- Update cryptography to 42.0.1 (#8817)
+- Limit moto to <5.0.0 until the breaking issues are fixed (#8820)
+- Enable efficient `chord` when using dynamicdb as backend store (#8783)
+- Add a Task class specialised for Django (#8491)
+- Sync kombu versions in requirements and setup.cfg (#8825)
+- chore(ci): Enhance CI with `workflow_dispatch` for targeted debugging and testing (#8826)
+- Update cryptography to 42.0.2 (#8827)
+- Docfix: pip install celery[sqs] -> pip install "celery[sqs]" (#8829)
+- Bump pre-commit/action from 3.0.0 to 3.0.1 (#8835)
+- Support moto 5.0 (#8838)
+- Another fix for `link_error` signatures being `dict`s instead of `Signature`s (#8841)
+- Bump codecov/codecov-action from 3 to 4 (#8831)
+- Upgrade from pytest-celery v1.0.0b1 -> v1.0.0b2 (#8843)
+- Bump pytest from 7.4.4 to 8.0.0 (#8823)
+- Update pre-commit to 3.6.1 (#8839)
+- Update cryptography to 42.0.3 (#8854)
+- Bump pytest from 8.0.0 to 8.0.1 (#8855)
+- Update cryptography to 42.0.4 (#8864)
+- Update pytest to 8.0.2 (#8870)
+- Update cryptography to 42.0.5 (#8869)
+- Update elasticsearch requirement from <=8.12.0 to <=8.12.1 (#8867)
+- Eliminate consecutive chords generated by group | task upgrade (#8663)
+- Make custom remote control commands available in CLI (#8489)
+- Add Google Cloud Storage (GCS) backend (#8868)
+- Bump msgpack from 1.0.7 to 1.0.8 (#8885)
+- Update pytest to 8.1.0 (#8886)
+- Bump pytest-timeout from 2.2.0 to 2.3.1 (#8894)
+- Bump pytest-subtests from 0.11.0 to 0.12.1 (#8896)
+- Bump mypy from 1.8.0 to 1.9.0 (#8898)
+- Update pytest to 8.1.1 (#8901)
+- Update contributing guide to use ssh upstream url (#8881)
+- Fix recursive result parents on group in middle of chain (#8903)
+- Bump pytest-celery to 1.0.0b4 (#8899)
+- Adjusted smoke tests CI time limit (#8907)
+- Update pytest-rerunfailures to 14.0 (#8910)
+- Use the "all" extra for pytest-celery (#8911)
+- Fix typos and grammar (#8915)
+- Bump pytest-celery to 1.0.0rc1 (#8918)
+- Print safe_say() to stdout for non-error flows (#8919)
+- Update pytest-cov to 5.0.0 (#8924)
+- Bump pytest-celery to 1.0.0rc2 (#8928)
+
 .. _version-5.4.0rc1:
 
 5.4.0rc1
 ========
 
 :release-date: 2024-01-17 7:00 P.M GMT+2
 :release-by: Tomer Nosrati
```

### Comparing `celery-5.4.0rc1/LICENSE` & `celery-5.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/MANIFEST.in` & `celery-5.4.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/PKG-INFO` & `celery-5.4.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery
-Version: 5.4.0rc1
+Version: 5.4.0rc2
 Summary: Distributed Task Queue.
 Home-page: https://docs.celeryq.dev/
 Author: Ask Solem
 Author-email: auvipy@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.celeryq.dev/en/stable/
 Project-URL: Changelog, https://docs.celeryq.dev/en/stable/changelog.html
@@ -37,88 +37,90 @@
 Requires-Dist: click-didyoumean>=0.3.0
 Requires-Dist: click-repl>=0.2.0
 Requires-Dist: click-plugins>=1.1.1
 Requires-Dist: importlib-metadata>=3.6; python_version < "3.8"
 Requires-Dist: backports.zoneinfo>=0.2.1; python_version < "3.9"
 Requires-Dist: tzdata>=2022.7
 Requires-Dist: python-dateutil>=2.8.2
-Provides-Extra: cosmosdbsql
-Requires-Dist: pydocumentdb==2.3.5; extra == "cosmosdbsql"
-Provides-Extra: couchdb
-Requires-Dist: pycouchdb==1.14.2; extra == "couchdb"
-Provides-Extra: s3
-Requires-Dist: boto3>=1.26.143; extra == "s3"
-Provides-Extra: pyro
-Requires-Dist: pyro4==4.82; python_version < "3.11" and extra == "pyro"
-Provides-Extra: memcache
-Requires-Dist: pylibmc==1.6.3; platform_system != "Windows" and extra == "memcache"
-Provides-Extra: elasticsearch
-Requires-Dist: elasticsearch<=8.11.1; extra == "elasticsearch"
-Requires-Dist: elastic-transport<=8.11.0; extra == "elasticsearch"
 Provides-Extra: eventlet
 Requires-Dist: eventlet>=0.32.0; python_version < "3.10" and extra == "eventlet"
-Provides-Extra: pytest
-Requires-Dist: pytest-celery==1.0.0b1; extra == "pytest"
-Provides-Extra: pymemcache
-Requires-Dist: python-memcached>=1.61; extra == "pymemcache"
-Provides-Extra: auth
-Requires-Dist: cryptography==41.0.7; extra == "auth"
+Provides-Extra: gevent
+Requires-Dist: gevent>=1.5.0; extra == "gevent"
+Provides-Extra: dynamodb
+Requires-Dist: boto3>=1.26.143; extra == "dynamodb"
 Provides-Extra: zstd
 Requires-Dist: zstandard==0.22.0; extra == "zstd"
-Provides-Extra: redis
-Requires-Dist: redis!=4.5.5,<6.0.0,>=4.5.2; extra == "redis"
-Provides-Extra: django
-Requires-Dist: Django>=2.2.28; extra == "django"
-Provides-Extra: slmq
-Requires-Dist: softlayer_messaging>=1.0.3; extra == "slmq"
-Provides-Extra: mongodb
-Requires-Dist: pymongo[srv]>=4.0.2; extra == "mongodb"
-Provides-Extra: sqs
-Requires-Dist: boto3>=1.26.143; extra == "sqs"
-Requires-Dist: pycurl>=7.43.0.5; (sys_platform != "win32" and platform_python_implementation == "CPython") and extra == "sqs"
-Requires-Dist: urllib3>=1.26.16; extra == "sqs"
-Requires-Dist: kombu[sqs]>=5.3.0; extra == "sqs"
-Provides-Extra: consul
-Requires-Dist: python-consul2==0.1.5; extra == "consul"
+Provides-Extra: yaml
+Requires-Dist: PyYAML>=3.10; extra == "yaml"
 Provides-Extra: zookeeper
 Requires-Dist: kazoo>=1.3.1; extra == "zookeeper"
-Provides-Extra: msgpack
-Requires-Dist: msgpack==1.0.7; extra == "msgpack"
-Provides-Extra: gevent
-Requires-Dist: gevent>=1.5.0; extra == "gevent"
-Provides-Extra: arangodb
-Requires-Dist: pyArango>=2.0.2; extra == "arangodb"
-Provides-Extra: sqlalchemy
-Requires-Dist: sqlalchemy<2.1,>=1.4.48; extra == "sqlalchemy"
-Provides-Extra: azureblockblob
-Requires-Dist: azure-storage-blob>=12.15.0; extra == "azureblockblob"
 Provides-Extra: cassandra
 Requires-Dist: cassandra-driver<4,>=3.25.0; extra == "cassandra"
+Provides-Extra: sqlalchemy
+Requires-Dist: sqlalchemy<2.1,>=1.4.48; extra == "sqlalchemy"
+Provides-Extra: gcs
+Requires-Dist: google-cloud-storage>=2.10.0; extra == "gcs"
+Provides-Extra: pymemcache
+Requires-Dist: python-memcached>=1.61; extra == "pymemcache"
+Provides-Extra: django
+Requires-Dist: Django>=2.2.28; extra == "django"
+Provides-Extra: s3
+Requires-Dist: boto3>=1.26.143; extra == "s3"
+Provides-Extra: cosmosdbsql
+Requires-Dist: pydocumentdb==2.3.5; extra == "cosmosdbsql"
 Provides-Extra: couchbase
 Requires-Dist: couchbase>=3.0.0; (platform_python_implementation != "PyPy" and (platform_system != "Windows" or python_version < "3.10")) and extra == "couchbase"
+Provides-Extra: tblib
+Requires-Dist: tblib>=1.5.0; python_version >= "3.8.0" and extra == "tblib"
+Requires-Dist: tblib>=1.3.0; python_version < "3.8.0" and extra == "tblib"
+Provides-Extra: couchdb
+Requires-Dist: pycouchdb==1.14.2; extra == "couchdb"
+Provides-Extra: msgpack
+Requires-Dist: msgpack==1.0.8; extra == "msgpack"
+Provides-Extra: sqs
+Requires-Dist: boto3>=1.26.143; extra == "sqs"
+Requires-Dist: pycurl>=7.43.0.5; (sys_platform != "win32" and platform_python_implementation == "CPython") and extra == "sqs"
+Requires-Dist: urllib3>=1.26.16; extra == "sqs"
+Requires-Dist: kombu[sqs]>=5.3.4; extra == "sqs"
+Provides-Extra: slmq
+Requires-Dist: softlayer_messaging>=1.0.3; extra == "slmq"
 Provides-Extra: librabbitmq
 Requires-Dist: librabbitmq>=2.0.0; python_version < "3.11" and extra == "librabbitmq"
-Provides-Extra: yaml
-Requires-Dist: PyYAML>=3.10; extra == "yaml"
 Provides-Extra: brotli
 Requires-Dist: brotlipy>=0.7.0; platform_python_implementation == "PyPy" and extra == "brotli"
 Requires-Dist: brotli>=1.0.0; platform_python_implementation == "CPython" and extra == "brotli"
-Provides-Extra: tblib
-Requires-Dist: tblib>=1.5.0; python_version >= "3.8.0" and extra == "tblib"
-Requires-Dist: tblib>=1.3.0; python_version < "3.8.0" and extra == "tblib"
+Provides-Extra: azureblockblob
+Requires-Dist: azure-storage-blob>=12.15.0; extra == "azureblockblob"
+Provides-Extra: consul
+Requires-Dist: python-consul2==0.1.5; extra == "consul"
+Provides-Extra: elasticsearch
+Requires-Dist: elasticsearch<=8.12.1; extra == "elasticsearch"
+Requires-Dist: elastic-transport<=8.12.0; extra == "elasticsearch"
+Provides-Extra: memcache
+Requires-Dist: pylibmc==1.6.3; platform_system != "Windows" and extra == "memcache"
+Provides-Extra: redis
+Requires-Dist: redis!=4.5.5,<6.0.0,>=4.5.2; extra == "redis"
 Provides-Extra: solar
 Requires-Dist: ephem==4.1.5; platform_python_implementation != "PyPy" and extra == "solar"
-Provides-Extra: dynamodb
-Requires-Dist: boto3>=1.26.143; extra == "dynamodb"
+Provides-Extra: mongodb
+Requires-Dist: pymongo[srv]>=4.0.2; extra == "mongodb"
+Provides-Extra: arangodb
+Requires-Dist: pyArango>=2.0.2; extra == "arangodb"
+Provides-Extra: pytest
+Requires-Dist: pytest-celery[all]==1.0.0rc2; extra == "pytest"
+Provides-Extra: pyro
+Requires-Dist: pyro4==4.82; python_version < "3.11" and extra == "pyro"
+Provides-Extra: auth
+Requires-Dist: cryptography==42.0.5; extra == "auth"
 
 .. image:: https://docs.celeryq.dev/en/latest/_images/celery-banner-small.png
 
 |build-status| |coverage| |license| |wheel| |semgrep| |pyversion| |pyimp| |ocbackerbadge| |ocsponsorbadge|
 
-:Version: 5.4.0rc1 (opalescent)
+:Version: 5.4.0rc2 (opalescent)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 Donations
@@ -425,14 +427,17 @@
 
 :``celery[azureblockblob]``:
     for using Azure Storage as a result backend (using ``azure-storage``)
 
 :``celery[s3]``:
     for using S3 Storage as a result backend.
 
+:``celery[gcs]``:
+    for using Google Cloud Storage as a result backend.
+
 :``celery[couchbase]``:
     for using Couchbase as a result backend.
 
 :``celery[arangodb]``:
     for using ArangoDB as a result backend.
 
 :``celery[elasticsearch]``:
```

### Comparing `celery-5.4.0rc1/README.rst` & `celery-5.4.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .. image:: https://docs.celeryq.dev/en/latest/_images/celery-banner-small.png
 
 |build-status| |coverage| |license| |wheel| |semgrep| |pyversion| |pyimp| |ocbackerbadge| |ocsponsorbadge|
 
-:Version: 5.4.0rc1 (opalescent)
+:Version: 5.4.0rc2 (opalescent)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 Donations
@@ -313,14 +313,17 @@
 
 :``celery[azureblockblob]``:
     for using Azure Storage as a result backend (using ``azure-storage``)
 
 :``celery[s3]``:
     for using S3 Storage as a result backend.
 
+:``celery[gcs]``:
+    for using Google Cloud Storage as a result backend.
+
 :``celery[couchbase]``:
     for using Couchbase as a result backend.
 
 :``celery[arangodb]``:
     for using ArangoDB as a result backend.
 
 :``celery[elasticsearch]``:
```

### Comparing `celery-5.4.0rc1/celery/__init__.py` & `celery-5.4.0rc2/celery/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from collections import namedtuple
 
 # Lazy loading
 from . import local
 
 SERIES = 'opalescent'
 
-__version__ = '5.4.0rc1'
+__version__ = '5.4.0rc2'
 __author__ = 'Ask Solem'
 __contact__ = 'auvipy@gmail.com'
 __homepage__ = 'https://docs.celeryq.dev/'
 __docformat__ = 'restructuredtext'
 __keywords__ = 'task job queue distributed messaging actor'
 
 # -eof meta-
```

### Comparing `celery-5.4.0rc1/celery/_state.py` & `celery-5.4.0rc2/celery/_state.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/app/__init__.py` & `celery-5.4.0rc2/celery/app/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/app/amqp.py` & `celery-5.4.0rc2/celery/app/amqp.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/app/annotations.py` & `celery-5.4.0rc2/celery/app/annotations.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/app/autoretry.py` & `celery-5.4.0rc2/celery/app/autoretry.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/app/backends.py` & `celery-5.4.0rc2/celery/app/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     'file': 'celery.backends.filesystem:FilesystemBackend',
     'disabled': 'celery.backends.base:DisabledBackend',
     'consul': 'celery.backends.consul:ConsulBackend',
     'dynamodb': 'celery.backends.dynamodb:DynamoDBBackend',
     'azureblockblob': 'celery.backends.azureblockblob:AzureBlockBlobBackend',
     'arangodb': 'celery.backends.arangodb:ArangoDbBackend',
     's3': 'celery.backends.s3:S3Backend',
+    'gs': 'celery.backends.gcs:GCSBackend',
 }
 
 
 def by_name(backend=None, loader=None,
             extension_namespace='celery.result_backends'):
     """Get backend class by name/alias."""
     backend = backend or 'disabled'
```

### Comparing `celery-5.4.0rc1/celery/app/base.py` & `celery-5.4.0rc2/celery/app/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,14 +236,15 @@
         self.clock = LamportClock()
         self.main = main
         self.amqp_cls = amqp or self.amqp_cls
         self.events_cls = events or self.events_cls
         self.loader_cls = loader or self._get_default_loader()
         self.log_cls = log or self.log_cls
         self.control_cls = control or self.control_cls
+        self._custom_task_cls_used = bool(task_cls)
         self.task_cls = task_cls or self.task_cls
         self.set_as_current = set_as_current
         self.registry_cls = symbol_by_name(self.registry_cls)
         self.user_options = defaultdict(set)
         self.steps = defaultdict(set)
         self.autofinalize = autofinalize
         self.namespace = namespace
```

### Comparing `celery-5.4.0rc1/celery/app/builtins.py` & `celery-5.4.0rc2/celery/app/builtins.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/app/control.py` & `celery-5.4.0rc2/celery/app/control.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/app/defaults.py` & `celery-5.4.0rc2/celery/app/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,20 @@
         retry_initial_backoff_sec=Option(2, type='int'),
         retry_increment_base=Option(2, type='int'),
         retry_max_attempts=Option(3, type='int'),
         base_path=Option('', type='string'),
         connection_timeout=Option(20, type='int'),
         read_timeout=Option(120, type='int'),
     ),
+    gcs=Namespace(
+        bucket=Option(type='string'),
+        project=Option(type='string'),
+        base_path=Option('', type='string'),
+        ttl=Option(0, type='float'),
+    ),
     control=Namespace(
         queue_ttl=Option(300.0, type='float'),
         queue_expires=Option(10.0, type='float'),
         exchange=Option('celery', type='string'),
     ),
     couchbase=Namespace(
         __old__=old_ns('celery_couchbase'),
```

### Comparing `celery-5.4.0rc1/celery/app/events.py` & `celery-5.4.0rc2/celery/app/events.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/app/log.py` & `celery-5.4.0rc2/celery/app/log.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/app/registry.py` & `celery-5.4.0rc2/celery/app/registry.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/app/routes.py` & `celery-5.4.0rc2/celery/app/routes.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/app/task.py` & `celery-5.4.0rc2/celery/app/task.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/app/trace.py` & `celery-5.4.0rc2/celery/app/trace.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/app/utils.py` & `celery-5.4.0rc2/celery/app/utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/apps/beat.py` & `celery-5.4.0rc2/celery/apps/beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/apps/multi.py` & `celery-5.4.0rc2/celery/apps/multi.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/apps/worker.py` & `celery-5.4.0rc2/celery/apps/worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,16 +73,16 @@
 
 def active_thread_count():
     from threading import enumerate
     return sum(1 for t in enumerate()
                if not t.name.startswith('Dummy-'))
 
 
-def safe_say(msg):
-    print(f'\n{msg}', file=sys.__stderr__, flush=True)
+def safe_say(msg, f=sys.__stderr__):
+    print(f'\n{msg}', file=f, flush=True)
 
 
 class Worker(WorkController):
     """Worker as a program."""
 
     def on_before_init(self, quiet=False, **kwargs):
         self.quiet = quiet
@@ -282,15 +282,15 @@
                       callback=None, exitcode=EX_OK):
     def _handle_request(*args):
         with in_sighandler():
             from celery.worker import state
             if current_process()._name == 'MainProcess':
                 if callback:
                     callback(worker)
-                safe_say(f'worker: {how} shutdown (MainProcess)')
+                safe_say(f'worker: {how} shutdown (MainProcess)', sys.__stdout__)
                 signals.worker_shutting_down.send(
                     sender=worker.hostname, sig=sig, how=how,
                     exitcode=exitcode,
                 )
             setattr(state, {'Warm': 'should_stop',
                             'Cold': 'should_terminate'}[how], exitcode)
     _handle_request.__name__ = str(f'worker_{how}')
@@ -313,15 +313,16 @@
     )
 else:  # pragma: no cover
     install_worker_term_handler = \
         install_worker_term_hard_handler = lambda *a, **kw: None
 
 
 def on_SIGINT(worker):
-    safe_say('worker: Hitting Ctrl+C again will terminate all running tasks!')
+    safe_say('worker: Hitting Ctrl+C again will terminate all running tasks!',
+             sys.__stdout__)
     install_worker_term_hard_handler(worker, sig='SIGINT')
 
 
 if not is_jython:  # pragma: no cover
     install_worker_int_handler = partial(
         _shutdown_handler, sig='SIGINT', callback=on_SIGINT,
         exitcode=EX_FAILURE,
@@ -339,15 +340,16 @@
 
 
 def install_worker_restart_handler(worker, sig='SIGHUP'):
 
     def restart_worker_sig_handler(*args):
         """Signal handler restarting the current python program."""
         set_in_sighandler(True)
-        safe_say(f"Restarting celery worker ({' '.join(sys.argv)})")
+        safe_say(f"Restarting celery worker ({' '.join(sys.argv)})",
+                 sys.__stdout__)
         import atexit
         atexit.register(_reload_current_worker)
         from celery.worker import state
         state.should_stop = EX_OK
     platforms.signals[sig] = restart_worker_sig_handler
```

### Comparing `celery-5.4.0rc1/celery/backends/arangodb.py` & `celery-5.4.0rc2/celery/backends/arangodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/asynchronous.py` & `celery-5.4.0rc2/celery/backends/asynchronous.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/azureblockblob.py` & `celery-5.4.0rc2/celery/backends/azureblockblob.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/base.py` & `celery-5.4.0rc2/celery/backends/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1076,15 +1076,15 @@
                     logger.exception('Chord %r raised: %r', gid, exc)
                     self.chord_error_from_stack(
                         callback,
                         ChordError(f'Callback error: {exc!r}'),
                     )
             finally:
                 deps.delete()
-                self.client.delete(key)
+                self.delete(key)
         else:
             self.expire(key, self.expires)
 
 
 class KeyValueStoreBackend(BaseKeyValueStoreBackend, SyncBackendMixin):
     """Result backend base class for key/value stores."""
```

### Comparing `celery-5.4.0rc1/celery/backends/cache.py` & `celery-5.4.0rc2/celery/backends/cache.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/cassandra.py` & `celery-5.4.0rc2/celery/backends/cassandra.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/consul.py` & `celery-5.4.0rc2/celery/backends/consul.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/cosmosdbsql.py` & `celery-5.4.0rc2/celery/backends/cosmosdbsql.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/couchbase.py` & `celery-5.4.0rc2/celery/backends/couchbase.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/couchdb.py` & `celery-5.4.0rc2/celery/backends/couchdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/database/__init__.py` & `celery-5.4.0rc2/celery/backends/database/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/database/models.py` & `celery-5.4.0rc2/celery/backends/database/models.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/database/session.py` & `celery-5.4.0rc2/celery/backends/database/session.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/dynamodb.py` & `celery-5.4.0rc2/celery/backends/dynamodb.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """AWS DynamoDB result store backend."""
 from collections import namedtuple
 from time import sleep, time
+from typing import Any, Dict
 
 from kombu.utils.url import _parse_url as parse_url
 
 from celery.exceptions import ImproperlyConfigured
 from celery.utils.log import get_logger
 
 from .base import KeyValueStoreBackend
@@ -50,19 +51,23 @@
     #: Item time-to-live in seconds (`default`)
     time_to_live_seconds = None
 
     # DynamoDB supports Time to Live as an auto-expiry mechanism.
     supports_autoexpire = True
 
     _key_field = DynamoDBAttribute(name='id', data_type='S')
+    # Each record has either a value field or count field
     _value_field = DynamoDBAttribute(name='result', data_type='B')
+    _count_filed = DynamoDBAttribute(name="chord_count", data_type='N')
     _timestamp_field = DynamoDBAttribute(name='timestamp', data_type='N')
     _ttl_field = DynamoDBAttribute(name='ttl', data_type='N')
     _available_fields = None
 
+    implements_incr = True
+
     def __init__(self, url=None, table_name=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.url = url
         self.table_name = table_name or self.table_name
 
         if not boto3:
@@ -455,14 +460,48 @@
                 self._ttl_field.name: {
                     self._ttl_field.data_type:
                         str(int(timestamp + self.time_to_live_seconds))
                 }
             })
         return put_request
 
+    def _prepare_init_count_request(self, key: str) -> Dict[str, Any]:
+        """Construct the counter initialization request parameters"""
+        timestamp = time()
+        return {
+            'TableName': self.table_name,
+            'Item': {
+                self._key_field.name: {
+                    self._key_field.data_type: key
+                },
+                self._count_filed.name: {
+                    self._count_filed.data_type: "0"
+                },
+                self._timestamp_field.name: {
+                    self._timestamp_field.data_type: str(timestamp)
+                }
+            }
+        }
+
+    def _prepare_inc_count_request(self, key: str) -> Dict[str, Any]:
+        """Construct the counter increment request parameters"""
+        return {
+            'TableName': self.table_name,
+            'Key': {
+                self._key_field.name: {
+                    self._key_field.data_type: key
+                }
+            },
+            'UpdateExpression': f"set {self._count_filed.name} = {self._count_filed.name} + :num",
+            "ExpressionAttributeValues": {
+                ":num": {"N": "1"},
+            },
+            "ReturnValues" : "UPDATED_NEW",
+        }
+
     def _item_to_dict(self, raw_response):
         """Convert get_item() response to field-value pairs."""
         if 'Item' not in raw_response:
             return {}
         return {
             field.name: raw_response['Item'][field.name][field.data_type]
             for field in self._available_fields
@@ -487,7 +526,22 @@
     def mget(self, keys):
         return [self.get(key) for key in keys]
 
     def delete(self, key):
         key = str(key)
         request_parameters = self._prepare_get_request(key)
         self.client.delete_item(**request_parameters)
+
+    def incr(self, key: bytes) -> int:
+        """Atomically increase the chord_count and return the new count"""
+        key = str(key)
+        request_parameters = self._prepare_inc_count_request(key)
+        item_response = self.client.update_item(**request_parameters)
+        new_count: str = item_response["Attributes"][self._count_filed.name][self._count_filed.data_type]
+        return int(new_count)
+
+    def _apply_chord_incr(self, header_result_args, body, **kwargs):
+        chord_key = self.get_key_for_chord(header_result_args[0])
+        init_count_request = self._prepare_init_count_request(str(chord_key))
+        self.client.put_item(**init_count_request)
+        return super()._apply_chord_incr(
+            header_result_args, body, **kwargs)
```

### Comparing `celery-5.4.0rc1/celery/backends/elasticsearch.py` & `celery-5.4.0rc2/celery/backends/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/filesystem.py` & `celery-5.4.0rc2/celery/backends/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         # We need the path and separator as bytes objects
         self.path = path.encode(encoding)
         self.sep = sep.encode(encoding)
 
         self.open = open
         self.unlink = unlink
 
-        # Lets verify that we've everything setup right
+        # Let's verify that we've everything setup right
         self._do_directory_test(b'.fs-backend-' + uuid().encode(encoding))
 
     def __reduce__(self, args=(), kwargs=None):
         kwargs = {} if not kwargs else kwargs
         return super().__reduce__(args, {**kwargs, 'url': self.url})
 
     def _find_path(self, url):
```

### Comparing `celery-5.4.0rc1/celery/backends/mongodb.py` & `celery-5.4.0rc2/celery/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/redis.py` & `celery-5.4.0rc2/celery/backends/redis.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/backends/rpc.py` & `celery-5.4.0rc2/celery/backends/rpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
             'result': self.encode_result(result, state),
             'traceback': traceback,
             'children': self.current_task_children(request),
         }
 
     def on_out_of_band_result(self, task_id, message):
         # Callback called when a reply for a task is received,
-        # but we have no idea what do do with it.
+        # but we have no idea what to do with it.
         # Since the result is not pending, we put it in a separate
         # buffer: probably it will become pending later.
         if self.result_consumer:
             self.result_consumer.on_out_of_band_result(message)
         self._out_of_band[task_id] = message
 
     def get_task_meta(self, task_id, backlog_limit=1000):
```

### Comparing `celery-5.4.0rc1/celery/backends/s3.py` & `celery-5.4.0rc2/celery/backends/s3.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/beat.py` & `celery-5.4.0rc2/celery/beat.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,19 +564,19 @@
         debug('Current schedule:\n' + '\n'.join(
             repr(entry) for entry in entries.values()))
 
     def _create_schedule(self):
         for _ in (1, 2):
             try:
                 self._store['entries']
-            except KeyError:
+            except (KeyError, UnicodeDecodeError, TypeError):
                 # new schedule db
                 try:
                     self._store['entries'] = {}
-                except KeyError as exc:
+                except (KeyError, UnicodeDecodeError, TypeError) as exc:
                     self._store = self._destroy_open_corrupted_schedule(exc)
                     continue
             else:
                 if '__version__' not in self._store:
                     warning('DB Reset: Account for new __version__ field')
                     self._store.clear()   # remove schedule at 2.2.2 upgrade.
                 elif 'tz' not in self._store:
```

### Comparing `celery-5.4.0rc1/celery/bin/amqp.py` & `celery-5.4.0rc2/celery/bin/amqp.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/base.py` & `celery-5.4.0rc2/celery/bin/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Click customizations for Celery."""
 import json
 import numbers
 from collections import OrderedDict
 from functools import update_wrapper
 from pprint import pformat
+from typing import Any
 
 import click
-from click import ParamType
+from click import Context, ParamType
 from kombu.utils.objects import cached_property
 
 from celery._state import get_current_app
 from celery.signals import user_preload_options
 from celery.utils import text
 from celery.utils.log import mlevel
 from celery.utils.time import maybe_iso8601
@@ -166,27 +167,44 @@
                     opts.setdefault('Options', []).append(rv)
 
         for name, opts_group in opts.items():
             with formatter.section(name):
                 formatter.write_dl(opts_group)
 
 
+class DaemonOption(CeleryOption):
+    """Common daemonization option"""
+    def __init__(self, *args, **kwargs):
+        super().__init__(args,
+                         help_group=kwargs.pop("help_group", "Daemonization Options"),
+                         callback=kwargs.pop("callback", self.daemon_setting),
+                         **kwargs)
+
+    def daemon_setting(self, ctx: Context, opt: CeleryOption, value: Any) -> Any:
+        """
+        Try to fetch deamonization option from applications settings.
+        Use the daemon command name as prefix (eg. `worker` -> `worker_pidfile`)
+        """
+        return value or getattr(ctx.obj.app.conf, f"{ctx.command.name}_{self.name}", None)
+
+
 class CeleryDaemonCommand(CeleryCommand):
     """Daemon commands."""
 
     def __init__(self, *args, **kwargs):
         """Initialize a Celery command with common daemon options."""
         super().__init__(*args, **kwargs)
-        self.params.append(CeleryOption(('-f', '--logfile'), help_group="Daemonization Options",
-                           help="Log destination; defaults to stderr"))
-        self.params.append(CeleryOption(('--pidfile',), help_group="Daemonization Options"))
-        self.params.append(CeleryOption(('--uid',), help_group="Daemonization Options"))
-        self.params.append(CeleryOption(('--gid',), help_group="Daemonization Options"))
-        self.params.append(CeleryOption(('--umask',), help_group="Daemonization Options"))
-        self.params.append(CeleryOption(('--executable',), help_group="Daemonization Options"))
+        self.params.extend((
+            DaemonOption("--logfile", "-f", help="Log destination; defaults to stderr"),
+            DaemonOption("--pidfile", help="PID file path; defaults to no PID file"),
+            DaemonOption("--uid", help="Drops privileges to this user ID"),
+            DaemonOption("--gid", help="Drops privileges to this group ID"),
+            DaemonOption("--umask", help="Create files and directories with this umask"),
+            DaemonOption("--executable", help="Override path to the Python executable"),
+        ))
 
 
 class CommaSeparatedList(ParamType):
     """Comma separated list argument."""
 
     name = "comma separated list"
```

### Comparing `celery-5.4.0rc1/celery/bin/beat.py` & `celery-5.4.0rc2/celery/bin/beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/call.py` & `celery-5.4.0rc2/celery/bin/call.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/celery.py` & `celery-5.4.0rc2/celery/bin/celery.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/control.py` & `celery-5.4.0rc2/celery/bin/control.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """The ``celery control``, ``. inspect`` and ``. status`` programs."""
 from functools import partial
+from typing import Literal
 
 import click
 from kombu.utils.json import dumps
 
 from celery.bin.base import COMMA_SEPARATED_LIST, CeleryCommand, CeleryOption, handle_preload_options
 from celery.exceptions import CeleryCommandException
 from celery.platforms import EX_UNAVAILABLE
@@ -35,26 +36,77 @@
                         method, meta.signature))
             else:
                 yield name, typ(arg) if typ is not None else arg
     finally:
         args[:] = args[i:]
 
 
-def _compile_arguments(action, args):
-    meta = Panel.meta[action]
+def _compile_arguments(command, args):
+    meta = Panel.meta[command]
     arguments = {}
     if meta.args:
         arguments.update({
-            k: v for k, v in _consume_arguments(meta, action, args)
+            k: v for k, v in _consume_arguments(meta, command, args)
         })
     if meta.variadic:
         arguments.update({meta.variadic: args})
     return arguments
 
 
+_RemoteControlType = Literal['inspect', 'control']
+
+
+def _verify_command_name(type_: _RemoteControlType, command: str) -> None:
+    choices = _get_commands_of_type(type_)
+
+    if command not in choices:
+        command_listing = ", ".join(choices)
+        raise click.UsageError(
+            message=f'Command {command} not recognized. Available {type_} commands: {command_listing}',
+        )
+
+
+def _list_option(type_: _RemoteControlType):
+    def callback(ctx: click.Context, param, value) -> None:
+        if not value:
+            return
+        choices = _get_commands_of_type(type_)
+
+        formatter = click.HelpFormatter()
+
+        with formatter.section(f'{type_.capitalize()} Commands'):
+            command_list = []
+            for command_name, info in choices.items():
+                if info.signature:
+                    command_preview = f'{command_name} {info.signature}'
+                else:
+                    command_preview = command_name
+                command_list.append((command_preview, info.help))
+            formatter.write_dl(command_list)
+        ctx.obj.echo(formatter.getvalue(), nl=False)
+        ctx.exit()
+
+    return click.option(
+        '--list',
+        is_flag=True,
+        help=f'List available {type_} commands and exit.',
+        expose_value=False,
+        is_eager=True,
+        callback=callback,
+    )
+
+
+def _get_commands_of_type(type_: _RemoteControlType) -> dict:
+    command_name_info_pairs = [
+        (name, info) for name, info in Panel.meta.items()
+        if info.type == type_ and info.visible
+    ]
+    return dict(sorted(command_name_info_pairs))
+
+
 @click.command(cls=CeleryCommand)
 @click.option('-t',
               '--timeout',
               cls=CeleryOption,
               type=float,
               default=1.0,
               help_group='Remote Control Options',
@@ -92,18 +144,16 @@
     if not kwargs.get('quiet', False):
         ctx.obj.echo('\n{} {} online.'.format(
             nodecount, text.pluralize(nodecount, 'node')))
 
 
 @click.command(cls=CeleryCommand,
                context_settings={'allow_extra_args': True})
-@click.argument("action", type=click.Choice([
-    name for name, info in Panel.meta.items()
-    if info.type == 'inspect' and info.visible
-]))
+@click.argument('command')
+@_list_option('inspect')
 @click.option('-t',
               '--timeout',
               cls=CeleryOption,
               type=float,
               default=1.0,
               help_group='Remote Control Options',
               help='Timeout in seconds waiting for reply.')
@@ -117,27 +167,27 @@
               '--json',
               cls=CeleryOption,
               is_flag=True,
               help_group='Remote Control Options',
               help='Use json as output format.')
 @click.pass_context
 @handle_preload_options
-def inspect(ctx, action, timeout, destination, json, **kwargs):
-    """Inspect the worker at runtime.
+def inspect(ctx, command, timeout, destination, json, **kwargs):
+    """Inspect the workers by sending them the COMMAND inspect command.
 
     Availability: RabbitMQ (AMQP) and Redis transports.
     """
+    _verify_command_name('inspect', command)
     callback = None if json else partial(_say_remote_command_reply, ctx,
                                          show_reply=True)
-    arguments = _compile_arguments(action, ctx.args)
+    arguments = _compile_arguments(command, ctx.args)
     inspect = ctx.obj.app.control.inspect(timeout=timeout,
                                           destination=destination,
                                           callback=callback)
-    replies = inspect._request(action,
-                               **arguments)
+    replies = inspect._request(command, **arguments)
 
     if not replies:
         raise CeleryCommandException(
             message='No nodes replied within time constraint',
             exit_code=EX_UNAVAILABLE
         )
 
@@ -149,18 +199,16 @@
     if not ctx.obj.quiet:
         ctx.obj.echo('\n{} {} online.'.format(
             nodecount, text.pluralize(nodecount, 'node')))
 
 
 @click.command(cls=CeleryCommand,
                context_settings={'allow_extra_args': True})
-@click.argument("action", type=click.Choice([
-    name for name, info in Panel.meta.items()
-    if info.type == 'control' and info.visible
-]))
+@click.argument('command')
+@_list_option('control')
 @click.option('-t',
               '--timeout',
               cls=CeleryOption,
               type=float,
               default=1.0,
               help_group='Remote Control Options',
               help='Timeout in seconds waiting for reply.')
@@ -174,24 +222,25 @@
               '--json',
               cls=CeleryOption,
               is_flag=True,
               help_group='Remote Control Options',
               help='Use json as output format.')
 @click.pass_context
 @handle_preload_options
-def control(ctx, action, timeout, destination, json):
-    """Workers remote control.
+def control(ctx, command, timeout, destination, json):
+    """Send the COMMAND control command to the workers.
 
     Availability: RabbitMQ (AMQP), Redis, and MongoDB transports.
     """
+    _verify_command_name('control', command)
     callback = None if json else partial(_say_remote_command_reply, ctx,
                                          show_reply=True)
     args = ctx.args
-    arguments = _compile_arguments(action, args)
-    replies = ctx.obj.app.control.broadcast(action, timeout=timeout,
+    arguments = _compile_arguments(command, args)
+    replies = ctx.obj.app.control.broadcast(command, timeout=timeout,
                                             destination=destination,
                                             callback=callback,
                                             reply=True,
                                             arguments=arguments)
 
     if not replies:
         raise CeleryCommandException(
```

### Comparing `celery-5.4.0rc1/celery/bin/events.py` & `celery-5.4.0rc2/celery/bin/events.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/graph.py` & `celery-5.4.0rc2/celery/bin/graph.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/list.py` & `celery-5.4.0rc2/celery/bin/list.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/logtool.py` & `celery-5.4.0rc2/celery/bin/logtool.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/migrate.py` & `celery-5.4.0rc2/celery/bin/migrate.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/multi.py` & `celery-5.4.0rc2/celery/bin/multi.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/purge.py` & `celery-5.4.0rc2/celery/bin/purge.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/result.py` & `celery-5.4.0rc2/celery/bin/result.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/shell.py` & `celery-5.4.0rc2/celery/bin/shell.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/upgrade.py` & `celery-5.4.0rc2/celery/bin/upgrade.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bin/worker.py` & `celery-5.4.0rc2/celery/bin/worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/bootsteps.py` & `celery-5.4.0rc2/celery/bootsteps.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/canvas.py` & `celery-5.4.0rc2/celery/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,15 +392,15 @@
             return
         # For callbacks: extra args are prepended to the stored args.
         if args or kwargs or options:
             args, kwargs, options = self._merge(args, kwargs, options)
         else:
             args, kwargs, options = self.args, self.kwargs, self.options
         # pylint: disable=too-many-function-args
-        #   Borks on this, as it's a property
+        #   Works on this, as it's a property
         return _apply(args, kwargs, **options)
 
     def _merge(self, args=None, kwargs=None, options=None, force=False):
         """Merge partial args/kwargs/options with existing ones.
 
         If the signature is immutable and ``force`` is False, the existing
         args/kwargs will be returned as-is and only the options will be merged.
@@ -511,15 +511,15 @@
         if group_id and "group_id" not in opts:
             opts['group_id'] = group_id
         if chord:
             opts['chord'] = chord
         if group_index is not None:
             opts['group_index'] = group_index
         # pylint: disable=too-many-function-args
-        #   Borks on this, as it's a property.
+        #   Works on this, as it's a property.
         return self.AsyncResult(tid)
 
     _freeze = freeze
 
     def replace(self, args=None, kwargs=None, options=None):
         """Replace the args, kwargs or options set for this signature.
 
@@ -954,14 +954,16 @@
         if self.tasks:
             return self.apply_async(args, kwargs)
 
     def __or__(self, other):
         if isinstance(other, group):
             # unroll group with one member
             other = maybe_unroll_group(other)
+            if not isinstance(other, group):
+                return self.__or__(other)
             # chain | group() -> chain
             tasks = self.unchain_tasks()
             if not tasks:
                 # If the chain is empty, return the group
                 return other
             if isinstance(tasks[-1], chord):
                 # CHAIN [last item is chord] | GROUP -> chain with chord body.
@@ -977,14 +979,21 @@
                 self.unchain_tasks(), other.unchain_tasks()), app=self._app)
         elif isinstance(other, Signature):
             if self.tasks and isinstance(self.tasks[-1], group):
                 # CHAIN [last item is group] | TASK -> chord
                 sig = self.clone()
                 sig.tasks[-1] = chord(
                     sig.tasks[-1], other, app=self._app)
+                # In the scenario where the second-to-last item in a chain is a chord,
+                # it leads to a situation where two consecutive chords are formed.
+                # In such cases, a further upgrade can be considered.
+                # This would involve chaining the body of the second-to-last chord with the last chord."
+                if len(sig.tasks) > 1 and isinstance(sig.tasks[-2], chord):
+                    sig.tasks[-2].body = sig.tasks[-2].body | sig.tasks[-1]
+                    sig.tasks = sig.tasks[:-1]
                 return sig
             elif self.tasks and isinstance(self.tasks[-1], chord):
                 # CHAIN [last item is chord] -> chain with chord body.
                 sig = self.clone()
                 sig.tasks[-1].body = sig.tasks[-1].body | other
                 return sig
             else:
@@ -1212,14 +1221,20 @@
                     # of multiple tasks.
                     # We therefore, have to construct the chord without it.
                     # Issues #5467, #3585.
                     task = chord(
                         task, body=prev_task,
                         root_id=root_id, app=app,
                     )
+                if tasks:
+                    prev_task = tasks[-1]
+                    prev_res = results[-1]
+                else:
+                    prev_task = None
+                    prev_res = None
 
             if is_last_task:
                 # chain(task_id=id) means task id is set for the last task
                 # in the chain.  If the chord is part of a chord/group
                 # then that chord/group must synchronize based on the
                 # last task in the chain, so we only set the group_id and
                 # chord callback for the last task.
@@ -1669,14 +1684,16 @@
         # Any child task might error so we need to ensure that they are all
         # capable of calling the linked error signature. This opens the
         # possibility that the task is called more than once but that's better
         # than it not being called at all.
         #
         # We return a concretised tuple of the signatures actually applied to
         # each child task signature, of which there might be none!
+        sig = maybe_signature(sig)
+
         return tuple(child_task.link_error(sig.clone(immutable=True)) for child_task in self.tasks)
 
     def _prepared(self, tasks, partial_args, group_id, root_id, app,
                   CallableSignature=abstract.CallableSignature,
                   from_dict=Signature.from_dict,
                   isinstance=isinstance, tuple=tuple):
         """Recursively unroll the group into a generator of its tasks.
```

### Comparing `celery-5.4.0rc1/celery/concurrency/__init__.py` & `celery-5.4.0rc2/celery/concurrency/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/concurrency/asynpool.py` & `celery-5.4.0rc2/celery/concurrency/asynpool.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
                                     hub_method, *args, **kwargs):
     """Apply hub method to fds in iter, remove from list if failure.
 
     Some file descriptors may become stale through OS reasons
     or possibly other reasons, so safely manage our lists of FDs.
     :param fds_iter: the file descriptors to iterate and apply hub_method
     :param source_data: data source to remove FD if it renders OSError
-    :param hub_method: the method to call with with each fd and kwargs
+    :param hub_method: the method to call with each fd and kwargs
     :*args to pass through to the hub_method;
     with a special syntax string '*fd*' represents a substitution
     for the current fd object in the iteration (for some callers).
     :**kwargs to pass through to the hub method (no substitutions needed)
     """
     def _meta_fd_argument_maker():
         # uses the current iterations value for fd
```

### Comparing `celery-5.4.0rc1/celery/concurrency/base.py` & `celery-5.4.0rc2/celery/concurrency/base.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/concurrency/eventlet.py` & `celery-5.4.0rc2/celery/concurrency/eventlet.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/concurrency/gevent.py` & `celery-5.4.0rc2/celery/concurrency/gevent.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/concurrency/prefork.py` & `celery-5.4.0rc2/celery/concurrency/prefork.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/concurrency/solo.py` & `celery-5.4.0rc2/celery/concurrency/solo.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/concurrency/thread.py` & `celery-5.4.0rc2/celery/concurrency/thread.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/contrib/abortable.py` & `celery-5.4.0rc2/celery/contrib/abortable.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/contrib/migrate.py` & `celery-5.4.0rc2/celery/contrib/migrate.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/contrib/pytest.py` & `celery-5.4.0rc2/celery/contrib/pytest.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/contrib/rdb.py` & `celery-5.4.0rc2/celery/contrib/rdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/contrib/sphinx.py` & `celery-5.4.0rc2/celery/contrib/sphinx.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/contrib/testing/app.py` & `celery-5.4.0rc2/celery/contrib/testing/app.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/contrib/testing/manager.py` & `celery-5.4.0rc2/celery/contrib/testing/manager.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/contrib/testing/mocks.py` & `celery-5.4.0rc2/celery/contrib/testing/mocks.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/contrib/testing/worker.py` & `celery-5.4.0rc2/celery/contrib/testing/worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/events/cursesmon.py` & `celery-5.4.0rc2/celery/events/cursesmon.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/events/dispatcher.py` & `celery-5.4.0rc2/celery/events/dispatcher.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/events/dumper.py` & `celery-5.4.0rc2/celery/events/dumper.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/events/event.py` & `celery-5.4.0rc2/celery/events/event.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/events/receiver.py` & `celery-5.4.0rc2/celery/events/receiver.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/events/snapshot.py` & `celery-5.4.0rc2/celery/events/snapshot.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/events/state.py` & `celery-5.4.0rc2/celery/events/state.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/exceptions.py` & `celery-5.4.0rc2/celery/exceptions.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/fixups/django.py` & `celery-5.4.0rc2/celery/fixups/django.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,17 @@
         # The project directory has precedence over system modules,
         # so we prepend it to the path.
         sys.path.insert(0, os.getcwd())
 
         self._settings = symbol_by_name('django.conf:settings')
         self.app.loader.now = self.now
 
+        if not self.app._custom_task_cls_used:
+            self.app.task_cls = 'celery.contrib.django.task:DjangoTask'
+
         signals.import_modules.connect(self.on_import_modules)
         signals.worker_init.connect(self.on_worker_init)
         return self
 
     @property
     def worker_fixup(self) -> "DjangoWorkerFixup":
         if self._worker_fixup is None:
```

### Comparing `celery-5.4.0rc1/celery/loaders/base.py` & `celery-5.4.0rc2/celery/loaders/base.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/loaders/default.py` & `celery-5.4.0rc2/celery/loaders/default.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/local.py` & `celery-5.4.0rc2/celery/local.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/platforms.py` & `celery-5.4.0rc2/celery/platforms.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/result.py` & `celery-5.4.0rc2/celery/result.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/schedules.py` & `celery-5.4.0rc2/celery/schedules.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/security/__init__.py` & `celery-5.4.0rc2/celery/security/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/security/certificate.py` & `celery-5.4.0rc2/celery/security/certificate.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/security/key.py` & `celery-5.4.0rc2/celery/security/key.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/security/serialization.py` & `celery-5.4.0rc2/celery/security/serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/security/utils.py` & `celery-5.4.0rc2/celery/security/utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/signals.py` & `celery-5.4.0rc2/celery/signals.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/states.py` & `celery-5.4.0rc2/celery/states.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/__init__.py` & `celery-5.4.0rc2/celery/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/abstract.py` & `celery-5.4.0rc2/celery/utils/abstract.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/collections.py` & `celery-5.4.0rc2/celery/utils/collections.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/debug.py` & `celery-5.4.0rc2/celery/utils/debug.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/deprecated.py` & `celery-5.4.0rc2/celery/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/dispatch/signal.py` & `celery-5.4.0rc2/celery/utils/dispatch/signal.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/functional.py` & `celery-5.4.0rc2/celery/utils/functional.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/graph.py` & `celery-5.4.0rc2/celery/utils/graph.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/imports.py` & `celery-5.4.0rc2/celery/utils/imports.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/iso8601.py` & `celery-5.4.0rc2/celery/utils/iso8601.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/log.py` & `celery-5.4.0rc2/celery/utils/log.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/nodenames.py` & `celery-5.4.0rc2/celery/utils/nodenames.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/objects.py` & `celery-5.4.0rc2/celery/utils/objects.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/saferepr.py` & `celery-5.4.0rc2/celery/utils/saferepr.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/serialization.py` & `celery-5.4.0rc2/celery/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/static/celery_128.png` & `celery-5.4.0rc2/celery/utils/static/celery_128.png`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/sysinfo.py` & `celery-5.4.0rc2/celery/utils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/term.py` & `celery-5.4.0rc2/celery/utils/term.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/text.py` & `celery-5.4.0rc2/celery/utils/text.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/threads.py` & `celery-5.4.0rc2/celery/utils/threads.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/time.py` & `celery-5.4.0rc2/celery/utils/time.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/utils/timer2.py` & `celery-5.4.0rc2/celery/utils/timer2.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/autoscale.py` & `celery-5.4.0rc2/celery/worker/autoscale.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/components.py` & `celery-5.4.0rc2/celery/worker/components.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/consumer/agent.py` & `celery-5.4.0rc2/celery/worker/consumer/agent.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/consumer/connection.py` & `celery-5.4.0rc2/celery/worker/consumer/connection.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/consumer/consumer.py` & `celery-5.4.0rc2/celery/worker/consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/consumer/control.py` & `celery-5.4.0rc2/celery/worker/consumer/control.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/consumer/events.py` & `celery-5.4.0rc2/celery/worker/consumer/events.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/consumer/gossip.py` & `celery-5.4.0rc2/celery/worker/consumer/gossip.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/consumer/heart.py` & `celery-5.4.0rc2/celery/worker/consumer/heart.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/consumer/mingle.py` & `celery-5.4.0rc2/celery/worker/consumer/mingle.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/consumer/tasks.py` & `celery-5.4.0rc2/celery/worker/consumer/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/control.py` & `celery-5.4.0rc2/celery/worker/control.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/heartbeat.py` & `celery-5.4.0rc2/celery/worker/heartbeat.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/loops.py` & `celery-5.4.0rc2/celery/worker/loops.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/pidbox.py` & `celery-5.4.0rc2/celery/worker/pidbox.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/request.py` & `celery-5.4.0rc2/celery/worker/request.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/state.py` & `celery-5.4.0rc2/celery/worker/state.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/strategy.py` & `celery-5.4.0rc2/celery/worker/strategy.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery/worker/worker.py` & `celery-5.4.0rc2/celery/worker/worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/celery.egg-info/PKG-INFO` & `celery-5.4.0rc2/celery.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery
-Version: 5.4.0rc1
+Version: 5.4.0rc2
 Summary: Distributed Task Queue.
 Home-page: https://docs.celeryq.dev/
 Author: Ask Solem
 Author-email: auvipy@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.celeryq.dev/en/stable/
 Project-URL: Changelog, https://docs.celeryq.dev/en/stable/changelog.html
@@ -37,88 +37,90 @@
 Requires-Dist: click-didyoumean>=0.3.0
 Requires-Dist: click-repl>=0.2.0
 Requires-Dist: click-plugins>=1.1.1
 Requires-Dist: importlib-metadata>=3.6; python_version < "3.8"
 Requires-Dist: backports.zoneinfo>=0.2.1; python_version < "3.9"
 Requires-Dist: tzdata>=2022.7
 Requires-Dist: python-dateutil>=2.8.2
-Provides-Extra: cosmosdbsql
-Requires-Dist: pydocumentdb==2.3.5; extra == "cosmosdbsql"
-Provides-Extra: couchdb
-Requires-Dist: pycouchdb==1.14.2; extra == "couchdb"
-Provides-Extra: s3
-Requires-Dist: boto3>=1.26.143; extra == "s3"
-Provides-Extra: pyro
-Requires-Dist: pyro4==4.82; python_version < "3.11" and extra == "pyro"
-Provides-Extra: memcache
-Requires-Dist: pylibmc==1.6.3; platform_system != "Windows" and extra == "memcache"
-Provides-Extra: elasticsearch
-Requires-Dist: elasticsearch<=8.11.1; extra == "elasticsearch"
-Requires-Dist: elastic-transport<=8.11.0; extra == "elasticsearch"
 Provides-Extra: eventlet
 Requires-Dist: eventlet>=0.32.0; python_version < "3.10" and extra == "eventlet"
-Provides-Extra: pytest
-Requires-Dist: pytest-celery==1.0.0b1; extra == "pytest"
-Provides-Extra: pymemcache
-Requires-Dist: python-memcached>=1.61; extra == "pymemcache"
-Provides-Extra: auth
-Requires-Dist: cryptography==41.0.7; extra == "auth"
+Provides-Extra: gevent
+Requires-Dist: gevent>=1.5.0; extra == "gevent"
+Provides-Extra: dynamodb
+Requires-Dist: boto3>=1.26.143; extra == "dynamodb"
 Provides-Extra: zstd
 Requires-Dist: zstandard==0.22.0; extra == "zstd"
-Provides-Extra: redis
-Requires-Dist: redis!=4.5.5,<6.0.0,>=4.5.2; extra == "redis"
-Provides-Extra: django
-Requires-Dist: Django>=2.2.28; extra == "django"
-Provides-Extra: slmq
-Requires-Dist: softlayer_messaging>=1.0.3; extra == "slmq"
-Provides-Extra: mongodb
-Requires-Dist: pymongo[srv]>=4.0.2; extra == "mongodb"
-Provides-Extra: sqs
-Requires-Dist: boto3>=1.26.143; extra == "sqs"
-Requires-Dist: pycurl>=7.43.0.5; (sys_platform != "win32" and platform_python_implementation == "CPython") and extra == "sqs"
-Requires-Dist: urllib3>=1.26.16; extra == "sqs"
-Requires-Dist: kombu[sqs]>=5.3.0; extra == "sqs"
-Provides-Extra: consul
-Requires-Dist: python-consul2==0.1.5; extra == "consul"
+Provides-Extra: yaml
+Requires-Dist: PyYAML>=3.10; extra == "yaml"
 Provides-Extra: zookeeper
 Requires-Dist: kazoo>=1.3.1; extra == "zookeeper"
-Provides-Extra: msgpack
-Requires-Dist: msgpack==1.0.7; extra == "msgpack"
-Provides-Extra: gevent
-Requires-Dist: gevent>=1.5.0; extra == "gevent"
-Provides-Extra: arangodb
-Requires-Dist: pyArango>=2.0.2; extra == "arangodb"
-Provides-Extra: sqlalchemy
-Requires-Dist: sqlalchemy<2.1,>=1.4.48; extra == "sqlalchemy"
-Provides-Extra: azureblockblob
-Requires-Dist: azure-storage-blob>=12.15.0; extra == "azureblockblob"
 Provides-Extra: cassandra
 Requires-Dist: cassandra-driver<4,>=3.25.0; extra == "cassandra"
+Provides-Extra: sqlalchemy
+Requires-Dist: sqlalchemy<2.1,>=1.4.48; extra == "sqlalchemy"
+Provides-Extra: gcs
+Requires-Dist: google-cloud-storage>=2.10.0; extra == "gcs"
+Provides-Extra: pymemcache
+Requires-Dist: python-memcached>=1.61; extra == "pymemcache"
+Provides-Extra: django
+Requires-Dist: Django>=2.2.28; extra == "django"
+Provides-Extra: s3
+Requires-Dist: boto3>=1.26.143; extra == "s3"
+Provides-Extra: cosmosdbsql
+Requires-Dist: pydocumentdb==2.3.5; extra == "cosmosdbsql"
 Provides-Extra: couchbase
 Requires-Dist: couchbase>=3.0.0; (platform_python_implementation != "PyPy" and (platform_system != "Windows" or python_version < "3.10")) and extra == "couchbase"
+Provides-Extra: tblib
+Requires-Dist: tblib>=1.5.0; python_version >= "3.8.0" and extra == "tblib"
+Requires-Dist: tblib>=1.3.0; python_version < "3.8.0" and extra == "tblib"
+Provides-Extra: couchdb
+Requires-Dist: pycouchdb==1.14.2; extra == "couchdb"
+Provides-Extra: msgpack
+Requires-Dist: msgpack==1.0.8; extra == "msgpack"
+Provides-Extra: sqs
+Requires-Dist: boto3>=1.26.143; extra == "sqs"
+Requires-Dist: pycurl>=7.43.0.5; (sys_platform != "win32" and platform_python_implementation == "CPython") and extra == "sqs"
+Requires-Dist: urllib3>=1.26.16; extra == "sqs"
+Requires-Dist: kombu[sqs]>=5.3.4; extra == "sqs"
+Provides-Extra: slmq
+Requires-Dist: softlayer_messaging>=1.0.3; extra == "slmq"
 Provides-Extra: librabbitmq
 Requires-Dist: librabbitmq>=2.0.0; python_version < "3.11" and extra == "librabbitmq"
-Provides-Extra: yaml
-Requires-Dist: PyYAML>=3.10; extra == "yaml"
 Provides-Extra: brotli
 Requires-Dist: brotlipy>=0.7.0; platform_python_implementation == "PyPy" and extra == "brotli"
 Requires-Dist: brotli>=1.0.0; platform_python_implementation == "CPython" and extra == "brotli"
-Provides-Extra: tblib
-Requires-Dist: tblib>=1.5.0; python_version >= "3.8.0" and extra == "tblib"
-Requires-Dist: tblib>=1.3.0; python_version < "3.8.0" and extra == "tblib"
+Provides-Extra: azureblockblob
+Requires-Dist: azure-storage-blob>=12.15.0; extra == "azureblockblob"
+Provides-Extra: consul
+Requires-Dist: python-consul2==0.1.5; extra == "consul"
+Provides-Extra: elasticsearch
+Requires-Dist: elasticsearch<=8.12.1; extra == "elasticsearch"
+Requires-Dist: elastic-transport<=8.12.0; extra == "elasticsearch"
+Provides-Extra: memcache
+Requires-Dist: pylibmc==1.6.3; platform_system != "Windows" and extra == "memcache"
+Provides-Extra: redis
+Requires-Dist: redis!=4.5.5,<6.0.0,>=4.5.2; extra == "redis"
 Provides-Extra: solar
 Requires-Dist: ephem==4.1.5; platform_python_implementation != "PyPy" and extra == "solar"
-Provides-Extra: dynamodb
-Requires-Dist: boto3>=1.26.143; extra == "dynamodb"
+Provides-Extra: mongodb
+Requires-Dist: pymongo[srv]>=4.0.2; extra == "mongodb"
+Provides-Extra: arangodb
+Requires-Dist: pyArango>=2.0.2; extra == "arangodb"
+Provides-Extra: pytest
+Requires-Dist: pytest-celery[all]==1.0.0rc2; extra == "pytest"
+Provides-Extra: pyro
+Requires-Dist: pyro4==4.82; python_version < "3.11" and extra == "pyro"
+Provides-Extra: auth
+Requires-Dist: cryptography==42.0.5; extra == "auth"
 
 .. image:: https://docs.celeryq.dev/en/latest/_images/celery-banner-small.png
 
 |build-status| |coverage| |license| |wheel| |semgrep| |pyversion| |pyimp| |ocbackerbadge| |ocsponsorbadge|
 
-:Version: 5.4.0rc1 (opalescent)
+:Version: 5.4.0rc2 (opalescent)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 Donations
@@ -425,14 +427,17 @@
 
 :``celery[azureblockblob]``:
     for using Azure Storage as a result backend (using ``azure-storage``)
 
 :``celery[s3]``:
     for using S3 Storage as a result backend.
 
+:``celery[gcs]``:
+    for using Google Cloud Storage as a result backend.
+
 :``celery[couchbase]``:
     for using Couchbase as a result backend.
 
 :``celery[arangodb]``:
     for using ArangoDB as a result backend.
 
 :``celery[elasticsearch]``:
```

### Comparing `celery-5.4.0rc1/celery.egg-info/SOURCES.txt` & `celery-5.4.0rc2/celery.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 celery/backends/consul.py
 celery/backends/cosmosdbsql.py
 celery/backends/couchbase.py
 celery/backends/couchdb.py
 celery/backends/dynamodb.py
 celery/backends/elasticsearch.py
 celery/backends/filesystem.py
+celery/backends/gcs.py
 celery/backends/mongodb.py
 celery/backends/redis.py
 celery/backends/rpc.py
 celery/backends/s3.py
 celery/backends/database/__init__.py
 celery/backends/database/models.py
 celery/backends/database/session.py
@@ -95,14 +96,16 @@
 celery/concurrency/thread.py
 celery/contrib/__init__.py
 celery/contrib/abortable.py
 celery/contrib/migrate.py
 celery/contrib/pytest.py
 celery/contrib/rdb.py
 celery/contrib/sphinx.py
+celery/contrib/django/__init__.py
+celery/contrib/django/task.py
 celery/contrib/testing/__init__.py
 celery/contrib/testing/app.py
 celery/contrib/testing/manager.py
 celery/contrib/testing/mocks.py
 celery/contrib/testing/tasks.py
 celery/contrib/testing/worker.py
 celery/events/__init__.py
@@ -261,14 +264,15 @@
 docs/internals/reference/celery.backends.couchdb.rst
 docs/internals/reference/celery.backends.database.models.rst
 docs/internals/reference/celery.backends.database.rst
 docs/internals/reference/celery.backends.database.session.rst
 docs/internals/reference/celery.backends.dynamodb.rst
 docs/internals/reference/celery.backends.elasticsearch.rst
 docs/internals/reference/celery.backends.filesystem.rst
+docs/internals/reference/celery.backends.gcs.rst
 docs/internals/reference/celery.backends.mongodb.rst
 docs/internals/reference/celery.backends.redis.rst
 docs/internals/reference/celery.backends.rpc.rst
 docs/internals/reference/celery.backends.rst
 docs/internals/reference/celery.backends.s3.rst
 docs/internals/reference/celery.concurrency.base.rst
 docs/internals/reference/celery.concurrency.eventlet.rst
@@ -344,14 +348,15 @@
 docs/reference/celery.bin.purge.rst
 docs/reference/celery.bin.result.rst
 docs/reference/celery.bin.shell.rst
 docs/reference/celery.bin.upgrade.rst
 docs/reference/celery.bin.worker.rst
 docs/reference/celery.bootsteps.rst
 docs/reference/celery.contrib.abortable.rst
+docs/reference/celery.contrib.django.task.rst
 docs/reference/celery.contrib.migrate.rst
 docs/reference/celery.contrib.pytest.rst
 docs/reference/celery.contrib.rdb.rst
 docs/reference/celery.contrib.sphinx.rst
 docs/reference/celery.contrib.testing.app.rst
 docs/reference/celery.contrib.testing.manager.rst
 docs/reference/celery.contrib.testing.mocks.rst
@@ -501,14 +506,15 @@
 requirements/extras/cosmosdbsql.txt
 requirements/extras/couchbase.txt
 requirements/extras/couchdb.txt
 requirements/extras/django.txt
 requirements/extras/dynamodb.txt
 requirements/extras/elasticsearch.txt
 requirements/extras/eventlet.txt
+requirements/extras/gcs.txt
 requirements/extras/gevent.txt
 requirements/extras/librabbitmq.txt
 requirements/extras/memcache.txt
 requirements/extras/mongodb.txt
 requirements/extras/msgpack.txt
 requirements/extras/pymemcache.txt
 requirements/extras/pyro.txt
@@ -609,26 +615,32 @@
 t/unit/backends/test_cosmosdbsql.py
 t/unit/backends/test_couchbase.py
 t/unit/backends/test_couchdb.py
 t/unit/backends/test_database.py
 t/unit/backends/test_dynamodb.py
 t/unit/backends/test_elasticsearch.py
 t/unit/backends/test_filesystem.py
+t/unit/backends/test_gcs.py
 t/unit/backends/test_mongodb.py
 t/unit/backends/test_redis.py
 t/unit/backends/test_rpc.py
 t/unit/backends/test_s3.py
 t/unit/bin/__init__.py
 t/unit/bin/celery.py
 t/unit/bin/test_beat.py
+t/unit/bin/test_control.py
+t/unit/bin/test_daemonization.py
 t/unit/bin/test_multi.py
 t/unit/bin/test_worker.py
 t/unit/bin/proj/__init__.py
 t/unit/bin/proj/app.py
 t/unit/bin/proj/app2.py
+t/unit/bin/proj/app_with_custom_cmds.py
+t/unit/bin/proj/daemon.py
+t/unit/bin/proj/daemon_config.py
 t/unit/bin/proj/pyramid_celery_app.py
 t/unit/bin/proj/scheduler.py
 t/unit/concurrency/__init__.py
 t/unit/concurrency/test_concurrency.py
 t/unit/concurrency/test_eventlet.py
 t/unit/concurrency/test_gevent.py
 t/unit/concurrency/test_pool.py
@@ -638,14 +650,16 @@
 t/unit/contrib/__init__.py
 t/unit/contrib/test_abortable.py
 t/unit/contrib/test_migrate.py
 t/unit/contrib/test_pytest.py
 t/unit/contrib/test_rdb.py
 t/unit/contrib/test_sphinx.py
 t/unit/contrib/test_worker.py
+t/unit/contrib/django/__init__.py
+t/unit/contrib/django/test_task.py
 t/unit/contrib/proj/__init__.py
 t/unit/contrib/proj/conf.py
 t/unit/contrib/proj/contents.rst
 t/unit/contrib/proj/foo.py
 t/unit/contrib/proj/xyzzy.py
 t/unit/events/__init__.py
 t/unit/events/test_cursesmon.py
```

### Comparing `celery-5.4.0rc1/celery.egg-info/requires.txt` & `celery-5.4.0rc2/celery.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 [:python_version < "3.9"]
 backports.zoneinfo>=0.2.1
 
 [arangodb]
 pyArango>=2.0.2
 
 [auth]
-cryptography==41.0.7
+cryptography==42.0.5
 
 [azureblockblob]
 azure-storage-blob>=12.15.0
 
 [brotli]
 
 [brotli:platform_python_implementation == "CPython"]
@@ -51,22 +51,25 @@
 [django]
 Django>=2.2.28
 
 [dynamodb]
 boto3>=1.26.143
 
 [elasticsearch]
-elasticsearch<=8.11.1
-elastic-transport<=8.11.0
+elasticsearch<=8.12.1
+elastic-transport<=8.12.0
 
 [eventlet]
 
 [eventlet:python_version < "3.10"]
 eventlet>=0.32.0
 
+[gcs]
+google-cloud-storage>=2.10.0
+
 [gevent]
 gevent>=1.5.0
 
 [librabbitmq]
 
 [librabbitmq:python_version < "3.11"]
 librabbitmq>=2.0.0
@@ -76,26 +79,26 @@
 [memcache:platform_system != "Windows"]
 pylibmc==1.6.3
 
 [mongodb]
 pymongo[srv]>=4.0.2
 
 [msgpack]
-msgpack==1.0.7
+msgpack==1.0.8
 
 [pymemcache]
 python-memcached>=1.61
 
 [pyro]
 
 [pyro:python_version < "3.11"]
 pyro4==4.82
 
 [pytest]
-pytest-celery==1.0.0b1
+pytest-celery[all]==1.0.0rc2
 
 [redis]
 redis!=4.5.5,<6.0.0,>=4.5.2
 
 [s3]
 boto3>=1.26.143
 
@@ -109,15 +112,15 @@
 
 [sqlalchemy]
 sqlalchemy<2.1,>=1.4.48
 
 [sqs]
 boto3>=1.26.143
 urllib3>=1.26.16
-kombu[sqs]>=5.3.0
+kombu[sqs]>=5.3.4
 
 [sqs:sys_platform != "win32" and platform_python_implementation == "CPython"]
 pycurl>=7.43.0.5
 
 [tblib]
 
 [tblib:python_version < "3.8.0"]
```

### Comparing `celery-5.4.0rc1/docs/.DS_Store` & `celery-5.4.0rc2/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/AUTHORS.txt` & `celery-5.4.0rc2/docs/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/Makefile` & `celery-5.4.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/_ext/celerydocs.py` & `celery-5.4.0rc2/docs/_ext/celerydocs.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/community.rst` & `celery-5.4.0rc2/docs/community.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/conf.py` & `celery-5.4.0rc2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         'celery.utils.encoding',
         r'celery.utils.static.*',
     ],
     linkcheck_ignore=[
         r'^http://localhost'
     ],
     autodoc_mock_imports=[
-        'riak'
+        'riak',
+        'django',
     ]
 ))
 
 settings = {}
 ignored_settings = {
     # Deprecated broker settings (replaced by broker_url)
     'broker_host',
```

### Comparing `celery-5.4.0rc1/docs/copyright.rst` & `celery-5.4.0rc2/docs/copyright.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/django/first-steps-with-django.rst` & `celery-5.4.0rc2/docs/django/first-steps-with-django.rst`

 * *Files 14% similar despite different names*

```diff
@@ -149,14 +149,72 @@
 
 
 .. seealso::
 
     You can find the full source code for the Django example project at:
     https://github.com/celery/celery/tree/main/examples/django/
 
+Trigger tasks at the end of the database transaction
+----------------------------------------------------
+
+A common pitfall with Django is triggering a task immediately and not wait until
+the end of the database transaction, which means that the Celery task may run
+before all changes are persisted to the database. For example:
+
+.. code-block:: python
+
+    # views.py
+    def create_user(request):
+        # Note: simplified example, use a form to validate input
+        user = User.objects.create(username=request.POST['username'])
+        send_email.delay(user.pk)
+        return HttpResponse('User created')
+
+    # task.py
+    @shared_task
+    def send_email(user_pk):
+        user = User.objects.get(pk=user_pk)
+        # send email ...
+
+In this case, the ``send_email`` task could start before the view has committed
+the transaction to the database, and therefore the task may not be able to find
+the user.
+
+A common solution is to use Django's `on_commit`_ hook to trigger the task
+after the transaction has been committed:
+
+.. _on_commit: https://docs.djangoproject.com/en/stable/topics/db/transactions/#django.db.transaction.on_commit
+
+.. code-block:: diff
+
+    - send_email.delay(user.pk)
+    + transaction.on_commit(lambda: send_email.delay(user.pk))
+
+.. versionadded:: 5.4
+
+Since this is such a common pattern, Celery 5.4 introduced a handy shortcut for this,
+using a :class:`~celery.contrib.django.task.DjangoTask`. Instead of calling
+:meth:`~celery.app.task.Task.delay`, you should call
+:meth:`~celery.contrib.django.task.DjangoTask.delay_on_commit`:
+
+.. code-block:: diff
+
+    - send_email.delay(user.pk)
+    + send_email.delay_on_commit(user.pk)
+
+
+This API takes care of wrapping the call into the `on_commit`_ hook for you.
+In rare cases where you want to trigger a task without waiting, the existing
+:meth:`~celery.app.task.Task.delay` API is still available.
+
+This task class should be used automatically if you've follow the setup steps above.
+However, if your app :ref:`uses a custom task base class <task-custom-classes>`,
+you'll need inherit from :class:`~celery.contrib.django.task.DjangoTask` instead of
+:class:`~celery.app.task.Task` to get this behaviour.
+
 Extensions
 ==========
 
 .. _django-celery-results:
 
 ``django-celery-results`` - Using the Django ORM/Cache as a result backend
 --------------------------------------------------------------------------
```

### Comparing `celery-5.4.0rc1/docs/faq.rst` & `celery-5.4.0rc2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/getting-started/backends-and-brokers/index.rst` & `celery-5.4.0rc2/docs/getting-started/backends-and-brokers/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/getting-started/backends-and-brokers/rabbitmq.rst` & `celery-5.4.0rc2/docs/getting-started/backends-and-brokers/rabbitmq.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/getting-started/backends-and-brokers/redis.rst` & `celery-5.4.0rc2/docs/getting-started/backends-and-brokers/redis.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/getting-started/backends-and-brokers/sqs.rst` & `celery-5.4.0rc2/docs/getting-started/backends-and-brokers/sqs.rst`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 For the Amazon SQS support you have to install additional dependencies.
 You can install both Celery and these dependencies in one go using
 the ``celery[sqs]`` :ref:`bundle <bundles>`:
 
 .. code-block:: console
 
-    $ pip install celery[sqs]
+    $ pip install "celery[sqs]"
 
 .. _broker-sqs-configuration:
 
 Configuration
 =============
 
 You have to specify SQS in the broker URL::
```

### Comparing `celery-5.4.0rc1/docs/getting-started/first-steps-with-celery.rst` & `celery-5.4.0rc2/docs/getting-started/first-steps-with-celery.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/getting-started/introduction.rst` & `celery-5.4.0rc2/docs/getting-started/introduction.rst`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
             - AMQP, Redis
             - Memcached,
             - SQLAlchemy, Django ORM
             - Apache Cassandra, Elasticsearch, Riak
             - MongoDB, CouchDB, Couchbase, ArangoDB
             - Amazon DynamoDB, Amazon S3
             - Microsoft Azure Block Blob, Microsoft Azure Cosmos DB
+            - Google Cloud Storage
             - File system
 
         - **Serialization**
 
             - *pickle*, *json*, *yaml*, *msgpack*.
             - *zlib*, *bzip2* compression.
             - Cryptographic message signing.
```

### Comparing `celery-5.4.0rc1/docs/getting-started/next-steps.rst` & `celery-5.4.0rc2/docs/getting-started/next-steps.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/glossary.rst` & `celery-5.4.0rc2/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-1.0.rst` & `celery-5.4.0rc2/docs/history/changelog-1.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-2.0.rst` & `celery-5.4.0rc2/docs/history/changelog-2.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-2.1.rst` & `celery-5.4.0rc2/docs/history/changelog-2.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-2.2.rst` & `celery-5.4.0rc2/docs/history/changelog-2.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-2.3.rst` & `celery-5.4.0rc2/docs/history/changelog-2.3.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-2.4.rst` & `celery-5.4.0rc2/docs/history/changelog-2.4.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-2.5.rst` & `celery-5.4.0rc2/docs/history/changelog-2.5.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-3.0.rst` & `celery-5.4.0rc2/docs/history/changelog-3.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-3.1.rst` & `celery-5.4.0rc2/docs/history/changelog-3.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-4.0.rst` & `celery-5.4.0rc2/docs/history/changelog-4.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-4.1.rst` & `celery-5.4.0rc2/docs/history/changelog-4.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-4.2.rst` & `celery-5.4.0rc2/docs/history/changelog-4.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-4.3.rst` & `celery-5.4.0rc2/docs/history/changelog-4.3.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-4.4.rst` & `celery-5.4.0rc2/docs/history/changelog-4.4.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-5.0.rst` & `celery-5.4.0rc2/docs/history/changelog-5.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/changelog-5.1.rst` & `celery-5.4.0rc2/docs/history/changelog-5.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/index.rst` & `celery-5.4.0rc2/docs/history/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/whatsnew-2.5.rst` & `celery-5.4.0rc2/docs/history/whatsnew-2.5.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/whatsnew-3.0.rst` & `celery-5.4.0rc2/docs/history/whatsnew-3.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/whatsnew-3.1.rst` & `celery-5.4.0rc2/docs/history/whatsnew-3.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/whatsnew-4.0.rst` & `celery-5.4.0rc2/docs/history/whatsnew-4.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/whatsnew-4.1.rst` & `celery-5.4.0rc2/docs/history/whatsnew-4.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/whatsnew-4.2.rst` & `celery-5.4.0rc2/docs/history/whatsnew-4.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/whatsnew-4.3.rst` & `celery-5.4.0rc2/docs/history/whatsnew-4.3.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/whatsnew-4.4.rst` & `celery-5.4.0rc2/docs/history/whatsnew-4.4.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/whatsnew-5.0.rst` & `celery-5.4.0rc2/docs/history/whatsnew-5.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/whatsnew-5.1.rst` & `celery-5.4.0rc2/docs/history/whatsnew-5.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/history/whatsnew-5.3.rst` & `celery-5.4.0rc2/docs/history/whatsnew-5.3.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/images/celery-banner-small.png` & `celery-5.4.0rc2/docs/images/celery-banner-small.png`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/images/celery-banner.png` & `celery-5.4.0rc2/docs/images/celery-banner.png`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/images/celery_128.png` & `celery-5.4.0rc2/docs/images/celery_128.png`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/images/celery_512.png` & `celery-5.4.0rc2/docs/images/celery_512.png`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/images/celeryevshotsm.jpg` & `celery-5.4.0rc2/docs/images/celeryevshotsm.jpg`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/images/dashboard.png` & `celery-5.4.0rc2/docs/images/dashboard.png`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/images/favicon.ico` & `celery-5.4.0rc2/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/images/monitor.png` & `celery-5.4.0rc2/docs/images/monitor.png`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/images/result_graph.png` & `celery-5.4.0rc2/docs/images/result_graph.png`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/images/worker_graph_full.png` & `celery-5.4.0rc2/docs/images/worker_graph_full.png`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/includes/installation.txt` & `celery-5.4.0rc2/docs/includes/installation.txt`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,18 @@
 
 :``celery[django]``:
     specifies the lowest version possible for Django support.
 
     You should probably not use this in your requirements, it's here
     for informational purposes only.
 
+:``celery[gcs]``:
+    for using the Google Cloud Storage as a result backend (*experimental*).
+
+
 
 .. _celery-installing-from-source:
 
 Downloading and installing from source
 --------------------------------------
 
 Download the latest version of Celery from PyPI:
```

### Comparing `celery-5.4.0rc1/docs/includes/introduction.txt` & `celery-5.4.0rc2/docs/includes/introduction.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-:Version: 5.4.0rc1 (opalescent)
+:Version: 5.4.0rc2 (opalescent)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 --
```

### Comparing `celery-5.4.0rc1/docs/includes/resources.txt` & `celery-5.4.0rc2/docs/includes/resources.txt`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/index.rst` & `celery-5.4.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/internals/app-overview.rst` & `celery-5.4.0rc2/docs/internals/app-overview.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/internals/deprecation.rst` & `celery-5.4.0rc2/docs/internals/deprecation.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/internals/guide.rst` & `celery-5.4.0rc2/docs/internals/guide.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/internals/protocol.rst` & `celery-5.4.0rc2/docs/internals/protocol.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/internals/reference/index.rst` & `celery-5.4.0rc2/docs/internals/reference/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     celery.backends.cassandra
     celery.backends.couchbase
     celery.backends.arangodb
     celery.backends.dynamodb
     celery.backends.filesystem
     celery.backends.cosmosdbsql
     celery.backends.s3
+    celery.backends.gcs
     celery.app.trace
     celery.app.annotations
     celery.app.routes
     celery.security.certificate
     celery.security.key
     celery.security.serialization
     celery.security.utils
```

### Comparing `celery-5.4.0rc1/docs/internals/worker.rst` & `celery-5.4.0rc2/docs/internals/worker.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/make.bat` & `celery-5.4.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/reference/celery.app.amqp.rst` & `celery-5.4.0rc2/docs/reference/celery.app.amqp.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/reference/celery.rst` & `celery-5.4.0rc2/docs/reference/celery.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/reference/celery.utils.debug.rst` & `celery-5.4.0rc2/docs/reference/celery.utils.debug.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/reference/index.rst` & `celery-5.4.0rc2/docs/reference/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     celery.exceptions
     celery.loaders
     celery.loaders.app
     celery.loaders.default
     celery.loaders.base
     celery.states
     celery.contrib.abortable
+    celery.contrib.django.task
     celery.contrib.migrate
     celery.contrib.pytest
     celery.contrib.sphinx
     celery.contrib.testing.worker
     celery.contrib.testing.app
     celery.contrib.testing.manager
     celery.contrib.testing.mocks
```

### Comparing `celery-5.4.0rc1/docs/sec/CELERYSA-0001.txt` & `celery-5.4.0rc2/docs/sec/CELERYSA-0001.txt`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/sec/CELERYSA-0002.txt` & `celery-5.4.0rc2/docs/sec/CELERYSA-0002.txt`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/sec/CELERYSA-0003.txt` & `celery-5.4.0rc2/docs/sec/CELERYSA-0003.txt`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/spelling_wordlist.txt` & `celery-5.4.0rc2/docs/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/templates/readme.txt` & `celery-5.4.0rc2/docs/templates/readme.txt`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/tutorials/task-cookbook.rst` & `celery-5.4.0rc2/docs/tutorials/task-cookbook.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/application.rst` & `celery-5.4.0rc2/docs/userguide/application.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/calling.rst` & `celery-5.4.0rc2/docs/userguide/calling.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/canvas.rst` & `celery-5.4.0rc2/docs/userguide/canvas.rst`

 * *Files 0% similar despite different names*

```diff
@@ -996,19 +996,19 @@
     @app.task(bind=True)
     def unlock_chord(self, group, callback, interval=1, max_retries=None):
         if group.ready():
             return maybe_signature(callback).delay(group.join())
         raise self.retry(countdown=interval, max_retries=max_retries)
 
 
-This is used by all result backends except Redis and Memcached: they
+This is used by all result backends except Redis, Memcached and DynamoDB: they
 increment a counter after each task in the header, then applies the callback
 when the counter exceeds the number of tasks in the set.
 
-The Redis and Memcached approach is a much better solution, but not easily
+The Redis, Memcached and DynamoDB approach is a much better solution, but not easily
 implemented in other backends (suggestions welcome!).
 
 .. note::
 
    Chords don't properly work with Redis before version 2.2; you'll need to
    upgrade to at least redis-server 2.2 to use them.
```

### Comparing `celery-5.4.0rc1/docs/userguide/concurrency/eventlet.rst` & `celery-5.4.0rc2/docs/userguide/concurrency/eventlet.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/concurrency/gevent.rst` & `celery-5.4.0rc2/docs/userguide/concurrency/gevent.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/concurrency/index.rst` & `celery-5.4.0rc2/docs/userguide/concurrency/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/configuration.rst` & `celery-5.4.0rc2/docs/userguide/configuration.rst`

 * *Files 3% similar despite different names*

```diff
@@ -727,14 +727,18 @@
     Use the `AzureBlockBlob`_ PaaS store to store the results
     See :ref:`conf-azureblockblob-result-backend`.
 
 * ``s3``
     Use the `S3`_ to store the results
     See :ref:`conf-s3-result-backend`.
 
+* ``gcs``
+    Use the `GCS`_ to store the results
+    See :ref:`conf-gcs-result-backend`.
+
 .. warning:
 
     While the AMQP result backend is very efficient, you must make sure
     you only receive the same result once. See :doc:`userguide/calling`).
 
 .. _`SQLAlchemy`: http://sqlalchemy.org
 .. _`Memcached`: http://memcached.org
@@ -746,14 +750,15 @@
 .. _`CouchDB`: http://www.couchdb.com/
 .. _`CosmosDB`: https://azure.microsoft.com/en-us/services/cosmos-db/
 .. _`Couchbase`: https://www.couchbase.com/
 .. _`ArangoDB`: https://www.arangodb.com/
 .. _`Consul`: https://consul.io/
 .. _`AzureBlockBlob`: https://azure.microsoft.com/en-us/services/storage/blobs/
 .. _`S3`: https://aws.amazon.com/s3/
+.. _`GCS`: https://cloud.google.com/storage/
 
 
 .. setting:: result_backend_always_retry
 
 ``result_backend_always_retry``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -1794,14 +1799,104 @@
 ``azureblockblob_read_timeout``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Default: 120.
 
 Timeout in seconds for reading of an azure block blob.
 
+.. _conf-gcs-result-backend:
+
+GCS backend settings
+--------------------
+
+.. note::
+
+    This gcs backend driver requires :pypi:`google-cloud-storage`.
+
+    To install, use :command:`gcs`:
+
+    .. code-block:: console
+
+        $ pip install celery[gcs]
+
+    See :ref:`bundles` for information on combining multiple extension
+    requirements.
+
+GCS could be configured via the URL provided in :setting:`result_backend`, for example::
+
+    result_backend = 'gcs://mybucket/some-prefix?project=myproject&ttl=600'
+
+This backend requires the following configuration directives to be set:
+
+.. setting:: gcs_bucket
+
+``gcs_bucket``
+~~~~~~~~~~~~~~
+
+Default: None.
+
+The gcs bucket name. For example::
+
+    gcs_bucket = 'bucket_name'
+
+.. setting:: gcs_project
+
+``gcs_project``
+~~~~~~~~~~~~~~~
+
+Default: None.
+
+The gcs project name. For example::
+
+    gcs_project = 'test-project'
+
+.. setting:: gcs_base_path
+
+``gcs_base_path``
+~~~~~~~~~~~~~~~~~
+
+Default: None.
+
+A base path in the gcs bucket to use to store all result keys. For example::
+
+    gcs_base_path = '/prefix'
+
+``gcs_ttl``
+~~~~~~~~~~~
+
+Default: 0.
+
+The time to live in seconds for the results blobs.
+Requires a GCS bucket with "Delete" Object Lifecycle Management action enabled.
+Use it to automatically delete results from Cloud Storage Buckets.
+
+For example to auto remove results after 24 hours::
+
+    gcs_ttl = 86400
+
+``gcs_threadpool_maxsize``
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Default: 10.
+
+Threadpool size for GCS operations. Same value defines the connection pool size.
+Allows to control the number of concurrent operations. For example::
+
+    gcs_threadpool_maxsize = 20
+
+Example configuration
+~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    gcs_bucket = 'mybucket'
+    gcs_project = 'myproject'
+    gcs_base_path = '/celery_result_backend'
+    gcs_ttl = 86400
+
 .. _conf-elasticsearch-result-backend:
 
 Elasticsearch backend settings
 ------------------------------
 
 To use `Elasticsearch`_ as the result backend you simply need to
 configure the :setting:`result_backend` setting with the correct URL.
@@ -2817,15 +2912,15 @@
 
 Maximum number of retries before we give up re-establishing a connection
 to the AMQP broker.
 
 If this is set to :const:`None`, we'll retry forever.
 
 ``broker_channel_error_retry``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. versionadded:: 5.3
 
 Default: Disabled.
 
 Automatically try to re-establish the connection to the AMQP broker
 if any invalid response has been returned.
@@ -2980,15 +3075,15 @@
 Default: Enabled.
 
 The ``worker_enable_prefetch_count_reduction`` setting governs the restoration behavior of the
 prefetch count to its maximum allowable value following a connection loss to the message
 broker. By default, this setting is enabled.
 
 Upon a connection loss, Celery will attempt to reconnect to the broker automatically,
-provided the :setting:`broker_connection_retry_on_startup` or :setting:`broker_connection_retry` 
+provided the :setting:`broker_connection_retry_on_startup` or :setting:`broker_connection_retry`
 is not set to False. During the period of lost connection, the message broker does not keep track
 of the number of tasks already fetched. Therefore, to manage the task load effectively and prevent
 overloading, Celery reduces the prefetch count based on the number of tasks that are
 currently running.
 
 The prefetch count is the number of messages that a worker will fetch from the broker at
 a time. The reduced prefetch count helps ensure that tasks are not fetched excessively
@@ -3215,14 +3310,81 @@
 Message serialization format used when sending event messages.
 
 .. seealso::
 
     :ref:`calling-serializers`.
 
 
+.. setting:: events_logfile
+
+``events_logfile``
+~~~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional file path for :program:`celery events` to log into (defaults to `stdout`).
+
+.. setting:: events_pidfile
+
+``events_pidfile``
+~~~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional file path for :program:`celery events` to create/store its PID file (default to no PID file created).
+
+.. setting:: events_uid
+
+``events_uid``
+~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional user ID to use when events :program:`celery events` drops its privileges (defaults to no UID change).
+
+.. setting:: events_gid
+
+``events_gid``
+~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional group ID to use when :program:`celery events` daemon drops its privileges (defaults to no GID change).
+
+.. setting:: events_umask
+
+``events_umask``
+~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional `umask` to use when :program:`celery events` creates files (log, pid...) when daemonizing.
+
+.. setting:: events_executable
+
+``events_executable``
+~~~~~~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional `python` executable path for :program:`celery events` to use when deaemonizing (defaults to :data:`sys.executable`).
+
+
 .. _conf-control:
 
 Remote Control Commands
 -----------------------
 
 .. note::
 
@@ -3483,14 +3645,80 @@
 ~~~~~~~~~~~~~~~~
 
 Default: ``"kombu.asynchronous.hub.timer:Timer"``.
 
 Name of the ETA scheduler class used by the worker.
 Default is or set by the pool implementation.
 
+.. setting:: worker_logfile
+
+``worker_logfile``
+~~~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional file path for :program:`celery worker` to log into (defaults to `stdout`).
+
+.. setting:: worker_pidfile
+
+``worker_pidfile``
+~~~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional file path for :program:`celery worker` to create/store its PID file (defaults to no PID file created).
+
+.. setting:: worker_uid
+
+``worker_uid``
+~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional user ID to use when :program:`celery worker` daemon drops its privileges (defaults to no UID change).
+
+.. setting:: worker_gid
+
+``worker_gid``
+~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional group ID to use when :program:`celery worker` daemon drops its privileges (defaults to no GID change).
+
+.. setting:: worker_umask
+
+``worker_umask``
+~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional `umask` to use when :program:`celery worker` creates files (log, pid...) when daemonizing.
+
+.. setting:: worker_executable
+
+``worker_executable``
+~~~~~~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional `python` executable path for :program:`celery worker` to use when deaemonizing (defaults to :data:`sys.executable`).
+
 .. _conf-celerybeat:
 
 Beat Settings (:program:`celery beat`)
 --------------------------------------
 
 .. setting:: beat_schedule
 
@@ -3569,7 +3797,73 @@
 .. versionadded:: 5.3
 
 Default: None.
 
 When using cron, the number of seconds :mod:`~celery.bin.beat` can look back
 when deciding whether a cron schedule is due. When set to `None`, cronjobs that
 are past due will always run immediately.
+
+.. setting:: beat_logfile
+
+``beat_logfile``
+~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional file path for :program:`celery beat` to log into (defaults to `stdout`).
+
+.. setting:: beat_pidfile
+
+``beat_pidfile``
+~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional file path for :program:`celery beat` to create/store it PID file (defaults to no PID file created).
+
+.. setting:: beat_uid
+
+``beat_uid``
+~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional user ID to use when beat :program:`celery beat` drops its privileges (defaults to no UID change).
+
+.. setting:: beat_gid
+
+``beat_gid``
+~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional group ID to use when :program:`celery beat` daemon drops its privileges (defaults to no GID change).
+
+.. setting:: beat_umask
+
+``beat_umask``
+~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional `umask` to use when :program:`celery beat` creates files (log, pid...) when daemonizing.
+
+.. setting:: beat_executable
+
+``beat_executable``
+~~~~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.4
+
+Default: :const:`None`
+
+An optional `python` executable path for :program:`celery beat` to use when deaemonizing (defaults to :data:`sys.executable`).
```

### Comparing `celery-5.4.0rc1/docs/userguide/daemonizing.rst` & `celery-5.4.0rc2/docs/userguide/daemonizing.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/debugging.rst` & `celery-5.4.0rc2/docs/userguide/debugging.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/extending.rst` & `celery-5.4.0rc2/docs/userguide/extending.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/monitoring.rst` & `celery-5.4.0rc2/docs/userguide/monitoring.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/optimizing.rst` & `celery-5.4.0rc2/docs/userguide/optimizing.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/periodic-tasks.rst` & `celery-5.4.0rc2/docs/userguide/periodic-tasks.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/routing.rst` & `celery-5.4.0rc2/docs/userguide/routing.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/security.rst` & `celery-5.4.0rc2/docs/userguide/security.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/signals.rst` & `celery-5.4.0rc2/docs/userguide/signals.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/tasks.rst` & `celery-5.4.0rc2/docs/userguide/tasks.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/testing.rst` & `celery-5.4.0rc2/docs/userguide/testing.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/docs/userguide/workers.rst` & `celery-5.4.0rc2/docs/userguide/workers.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/.DS_Store` & `celery-5.4.0rc2/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/app/myapp.py` & `celery-5.4.0rc2/examples/app/myapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/celery_http_gateway/README.rst` & `celery-5.4.0rc2/examples/celery_http_gateway/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/celery_http_gateway/settings.py` & `celery-5.4.0rc2/examples/celery_http_gateway/settings.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/celery_http_gateway/urls.py` & `celery-5.4.0rc2/examples/celery_http_gateway/urls.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/django/README.rst` & `celery-5.4.0rc2/examples/django/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -51,10 +51,16 @@
 Running a task
 ===================
 
 .. code-block:: console
 
     $ python ./manage.py shell
     >>> from demoapp.tasks import add, mul, xsum
-    >>> res = add.delay(2,3)
+    >>> res = add.delay_on_commit(2, 3)
     >>> res.get()
     5
+
+.. note::
+
+    The ``delay_on_commit`` method is only available when using Django,
+    and was added in Celery 5.4. If you are using an older version of Celery,
+    you can use ``delay`` instead.
```

### Comparing `celery-5.4.0rc1/examples/django/proj/celery.py` & `celery-5.4.0rc2/examples/django/proj/celery.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/django/proj/settings.py` & `celery-5.4.0rc2/examples/django/proj/settings.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/django/proj/urls.py` & `celery-5.4.0rc2/examples/django/proj/urls.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/django/proj/wsgi.py` & `celery-5.4.0rc2/examples/django/proj/wsgi.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/eventlet/README.rst` & `celery-5.4.0rc2/examples/eventlet/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/eventlet/bulk_task_producer.py` & `celery-5.4.0rc2/examples/eventlet/bulk_task_producer.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/eventlet/webcrawler.py` & `celery-5.4.0rc2/examples/eventlet/webcrawler.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/gevent/README.rst` & `celery-5.4.0rc2/examples/gevent/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/next-steps/setup.py` & `celery-5.4.0rc2/examples/next-steps/setup.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/periodic-tasks/myapp.py` & `celery-5.4.0rc2/examples/periodic-tasks/myapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/resultgraph/tasks.py` & `celery-5.4.0rc2/examples/resultgraph/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/security/mysecureapp.py` & `celery-5.4.0rc2/examples/security/mysecureapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/security/ssl/worker.key` & `celery-5.4.0rc2/examples/security/ssl/worker.key`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/security/ssl/worker.pem` & `celery-5.4.0rc2/examples/security/ssl/worker.pem`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/stamping/examples.py` & `celery-5.4.0rc2/examples/stamping/examples.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/stamping/myapp.py` & `celery-5.4.0rc2/examples/stamping/myapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/stamping/revoke_example.py` & `celery-5.4.0rc2/examples/stamping/revoke_example.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/stamping/tasks.py` & `celery-5.4.0rc2/examples/stamping/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/examples/stamping/visitors.py` & `celery-5.4.0rc2/examples/stamping/visitors.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/extra/bash-completion/celery.bash` & `celery-5.4.0rc2/extra/bash-completion/celery.bash`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/extra/generic-init.d/celerybeat` & `celery-5.4.0rc2/extra/generic-init.d/celerybeat`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/extra/generic-init.d/celeryd` & `celery-5.4.0rc2/extra/generic-init.d/celeryd`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/extra/macOS/org.celeryq.beat.plist` & `celery-5.4.0rc2/extra/macOS/org.celeryq.beat.plist`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/extra/macOS/org.celeryq.worker.plist` & `celery-5.4.0rc2/extra/macOS/org.celeryq.worker.plist`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/extra/supervisord/celerybeat.conf` & `celery-5.4.0rc2/extra/supervisord/celerybeat.conf`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/extra/supervisord/celeryd.conf` & `celery-5.4.0rc2/extra/supervisord/celeryd.conf`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/extra/supervisord/supervisord.conf` & `celery-5.4.0rc2/extra/supervisord/supervisord.conf`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/extra/systemd/celery.service` & `celery-5.4.0rc2/extra/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/extra/zsh-completion/celery.zsh` & `celery-5.4.0rc2/extra/zsh-completion/celery.zsh`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/pyproject.toml` & `celery-5.4.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/requirements/README.rst` & `celery-5.4.0rc2/requirements/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/requirements/test-ci-default.txt` & `celery-5.4.0rc2/requirements/test-ci-default.txt`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/setup.py` & `celery-5.4.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     'couchbase',
     'couchdb',
     'django',
     'dynamodb',
     'elasticsearch',
     'eventlet',
     'gevent',
+    'gcs',
     'librabbitmq',
     'memcache',
     'mongodb',
     'msgpack',
     'pymemcache',
     'pyro',
     'pytest',
```

### Comparing `celery-5.4.0rc1/t/benchmarks/bench_worker.py` & `celery-5.4.0rc2/t/benchmarks/bench_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/integration/conftest.py` & `celery-5.4.0rc2/t/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/integration/tasks.py` & `celery-5.4.0rc2/t/integration/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/integration/test_backend.py` & `celery-5.4.0rc2/t/integration/test_backend.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/integration/test_canvas.py` & `celery-5.4.0rc2/t/integration/test_canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1033,14 +1033,85 @@
     def test_freezing_chain_sets_id_of_last_task(self, manager):
         last_task = add.s(2).set(task_id='42')
         c = add.s(4) | last_task
         assert c.id is None
         c.freeze(last_task.id)
         assert c.id == last_task.id
 
+    @pytest.mark.parametrize(
+        "group_last_task",
+        [False, True],
+    )
+    def test_chaining_upgraded_chords_mixed_canvas_protocol_2(
+            self, manager, subtests, group_last_task):
+        """ This test is built to reproduce the github issue https://github.com/celery/celery/issues/8662
+
+        The issue describes a canvas where a chain of groups are executed multiple times instead of once.
+        This test is built to reproduce the issue and to verify that the issue is fixed.
+        """
+        try:
+            manager.app.backend.ensure_chords_allowed()
+        except NotImplementedError as e:
+            raise pytest.skip(e.args[0])
+
+        if not manager.app.conf.result_backend.startswith('redis'):
+            raise pytest.skip('Requires redis result backend.')
+
+        redis_connection = get_redis_connection()
+        redis_key = 'echo_chamber'
+
+        c = chain(
+            group([
+                redis_echo.si('1', redis_key=redis_key),
+                redis_echo.si('2', redis_key=redis_key)
+            ]),
+            group([
+                redis_echo.si('3', redis_key=redis_key),
+                redis_echo.si('4', redis_key=redis_key),
+                redis_echo.si('5', redis_key=redis_key)
+            ]),
+            group([
+                redis_echo.si('6', redis_key=redis_key),
+                redis_echo.si('7', redis_key=redis_key),
+                redis_echo.si('8', redis_key=redis_key),
+                redis_echo.si('9', redis_key=redis_key)
+            ]),
+            redis_echo.si('Done', redis_key='Done') if not group_last_task else
+            group(redis_echo.si('Done', redis_key='Done')),
+        )
+
+        with subtests.test(msg='Run the chain and wait for completion'):
+            redis_connection.delete(redis_key, 'Done')
+            c.delay().get(timeout=TIMEOUT)
+            await_redis_list_message_length(1, redis_key='Done', timeout=10)
+
+        with subtests.test(msg='All tasks are executed once'):
+            actual = [
+                sig.decode('utf-8')
+                for sig in redis_connection.lrange(redis_key, 0, -1)
+            ]
+            expected = [str(i) for i in range(1, 10)]
+            with subtests.test(msg='All tasks are executed once'):
+                assert sorted(actual) == sorted(expected)
+
+        # Cleanup
+        redis_connection.delete(redis_key, 'Done')
+
+    def test_group_in_center_of_chain(self, manager):
+        try:
+            manager.app.backend.ensure_chords_allowed()
+        except NotImplementedError as e:
+            raise pytest.skip(e.args[0])
+
+        t1 = chain(tsum.s(), group(add.s(8), add.s(16)), tsum.s() | add.s(32))
+        t2 = chord([tsum, tsum], t1)
+        t3 = chord([add.s(0, 1)], t2)
+        res = t3.apply_async()  # should not raise
+        assert res.get(timeout=TIMEOUT) == 60
+
 
 class test_result_set:
 
     @flaky
     def test_result_set(self, manager):
         assert_ping(manager)
```

### Comparing `celery-5.4.0rc1/t/integration/test_inspect.py` & `celery-5.4.0rc2/t/integration/test_inspect.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/integration/test_loader.py` & `celery-5.4.0rc2/t/integration/test_loader.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/integration/test_security.py` & `celery-5.4.0rc2/t/integration/test_security.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/integration/test_serialization.py` & `celery-5.4.0rc2/t/integration/test_serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/integration/test_tasks.py` & `celery-5.4.0rc2/t/integration/test_tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/integration/test_worker.py` & `celery-5.4.0rc2/t/integration/test_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/conftest.py` & `celery-5.4.0rc2/t/smoke/conftest.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/operations/task_termination.py` & `celery-5.4.0rc2/t/smoke/operations/task_termination.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/operations/worker_kill.py` & `celery-5.4.0rc2/t/smoke/operations/worker_kill.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/operations/worker_restart.py` & `celery-5.4.0rc2/t/smoke/operations/worker_restart.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/signals.py` & `celery-5.4.0rc2/t/smoke/signals.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tasks.py` & `celery-5.4.0rc2/t/smoke/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/failover/test_broker_failover.py` & `celery-5.4.0rc2/t/smoke/tests/failover/test_broker_failover.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/failover/test_worker_failover.py` & `celery-5.4.0rc2/t/smoke/tests/failover/test_worker_failover.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/stamping/conftest.py` & `celery-5.4.0rc2/t/smoke/tests/stamping/conftest.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/stamping/tasks.py` & `celery-5.4.0rc2/t/smoke/tests/stamping/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/stamping/test_hybrid_cluster.py` & `celery-5.4.0rc2/t/smoke/tests/stamping/test_hybrid_cluster.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/stamping/test_revoke.py` & `celery-5.4.0rc2/t/smoke/tests/stamping/test_revoke.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/stamping/test_visitor.py` & `celery-5.4.0rc2/t/smoke/tests/stamping/test_visitor.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/stamping/workers/legacy.py` & `celery-5.4.0rc2/t/smoke/tests/stamping/workers/legacy.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/test_canvas.py` & `celery-5.4.0rc2/t/smoke/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/test_consumer.py` & `celery-5.4.0rc2/t/smoke/tests/test_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,17 @@
             app = default_worker_app
             app.conf.worker_prefetch_multiplier = 2
             app.conf.worker_cancel_long_running_tasks_on_connection_loss = True
             app.conf.task_acks_late = True
             return app
 
         def test_max_prefetch_passed_on_broker_restart(self, celery_setup: CeleryTestSetup):
+            if isinstance(celery_setup.broker, RedisTestBroker):
+                pytest.xfail("Real Bug: Broker does not fetch messages after restart")
+
             sig = group(long_running_task.s(420) for _ in range(WORKER_CONCURRENCY))
             sig.apply_async(queue=celery_setup.worker.worker_queue)
             celery_setup.broker.restart()
             noop.s().apply_async(queue=celery_setup.worker.worker_queue)
             celery_setup.worker.assert_log_exists("Task t.smoke.tasks.noop")
 
 
@@ -88,14 +91,17 @@
         app.conf.worker_prefetch_multiplier = 1
         app.conf.worker_enable_prefetch_count_reduction = False
         app.conf.worker_cancel_long_running_tasks_on_connection_loss = True
         app.conf.task_acks_late = True
         return app
 
     def test_max_prefetch_not_passed_on_broker_restart(self, celery_setup: CeleryTestSetup):
+        if isinstance(celery_setup.broker, RedisTestBroker):
+            pytest.xfail("Real Bug: Broker does not fetch messages after restart")
+
         sig = group(long_running_task.s(10) for _ in range(WORKER_CONCURRENCY))
         r = sig.apply_async(queue=celery_setup.worker.worker_queue)
         celery_setup.broker.restart()
         noop.s().apply_async(queue=celery_setup.worker.worker_queue)
         assert "Task t.smoke.tasks.noop" not in celery_setup.worker.logs()
         r.get(timeout=RESULT_TIMEOUT)
         assert "Task t.smoke.tasks.noop" in celery_setup.worker.logs()
```

### Comparing `celery-5.4.0rc1/t/smoke/tests/test_control.py` & `celery-5.4.0rc2/t/smoke/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/test_signals.py` & `celery-5.4.0rc2/t/smoke/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/test_tasks.py` & `celery-5.4.0rc2/t/smoke/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/test_thread_safe.py` & `celery-5.4.0rc2/t/smoke/tests/test_thread_safe.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/tests/test_worker.py` & `celery-5.4.0rc2/t/smoke/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/workers/alt.py` & `celery-5.4.0rc2/t/smoke/workers/alt.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/workers/dev.py` & `celery-5.4.0rc2/t/smoke/workers/dev.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/workers/latest.py` & `celery-5.4.0rc2/t/smoke/workers/latest.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/smoke/workers/other.py` & `celery-5.4.0rc2/t/smoke/workers/other.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/app/test_amqp.py` & `celery-5.4.0rc2/t/unit/app/test_amqp.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/app/test_annotations.py` & `celery-5.4.0rc2/t/unit/app/test_annotations.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/app/test_app.py` & `celery-5.4.0rc2/t/unit/app/test_app.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/app/test_backends.py` & `celery-5.4.0rc2/t/unit/app/test_backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 def embed_worker(app,
                  concurrency=1,
                  pool='threading', **kwargs):
     """
     Helper embedded worker for testing.
 
     It's based on a :func:`celery.contrib.testing.worker.start_worker`,
-    but doesn't modifies logging settings and additionally shutdown
+    but doesn't modify logging settings and additionally shutdown
     worker pool.
     """
     # prepare application for worker
     app.finalize()
     app.set_current()
 
     worker = contrib_embed_worker.TestWorkController(
```

### Comparing `celery-5.4.0rc1/t/unit/app/test_beat.py` & `celery-5.4.0rc2/t/unit/app/test_beat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import errno
 import sys
 from datetime import datetime, timedelta, timezone
 from pickle import dumps, loads
-from unittest.mock import Mock, call, patch
+from unittest.mock import MagicMock, Mock, call, patch
 
 import pytest
 
 from celery import __version__, beat, uuid
 from celery.beat import BeatLazyFunc, event_t
 from celery.schedules import crontab, schedule
 from celery.utils.objects import Bunch
@@ -665,14 +665,46 @@
         err.errno = errno.ENOENT
         remove.side_effect = err
         s._remove_db()
         err.errno = errno.EPERM
         with pytest.raises(OSError):
             s._remove_db()
 
+    def test_create_schedule_corrupted(self):
+        """
+        Test that any decoding errors that might happen when opening beat-schedule.db are caught
+        """
+        s = create_persistent_scheduler()[0](app=self.app,
+                                             schedule_filename='schedule')
+        s._store = MagicMock()
+        s._destroy_open_corrupted_schedule = Mock()
+        s._destroy_open_corrupted_schedule.return_value = MagicMock()
+
+        # self._store['entries'] will throw a KeyError
+        s._store.__getitem__.side_effect = KeyError()
+        # then, when _create_schedule tries to reset _store['entries'], throw another error
+        expected_error = UnicodeDecodeError("ascii", b"ordinal not in range(128)", 0, 0, "")
+        s._store.__setitem__.side_effect = expected_error
+
+        s._create_schedule()
+        s._destroy_open_corrupted_schedule.assert_called_with(expected_error)
+
+    def test_create_schedule_missing_entries(self):
+        """
+        Test that if _create_schedule can't find the key "entries" in _store it will recreate it
+        """
+        s = create_persistent_scheduler()[0](app=self.app, schedule_filename="schedule")
+        s._store = MagicMock()
+
+        # self._store['entries'] will throw a KeyError
+        s._store.__getitem__.side_effect = TypeError()
+
+        s._create_schedule()
+        s._store.__setitem__.assert_called_with("entries", {})
+
     def test_setup_schedule(self):
         s = create_persistent_scheduler()[0](app=self.app,
                                              schedule_filename='schedule')
         opens = s.persistence.open = Mock()
         s._remove_db = Mock()
 
         def effect(*args, **kwargs):
```

### Comparing `celery-5.4.0rc1/t/unit/app/test_builtins.py` & `celery-5.4.0rc2/t/unit/app/test_builtins.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/app/test_control.py` & `celery-5.4.0rc2/t/unit/app/test_control.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/app/test_defaults.py` & `celery-5.4.0rc2/t/unit/app/test_defaults.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/app/test_exceptions.py` & `celery-5.4.0rc2/t/unit/app/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/app/test_loaders.py` & `celery-5.4.0rc2/t/unit/app/test_loaders.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/app/test_log.py` & `celery-5.4.0rc2/t/unit/app/test_log.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/app/test_registry.py` & `celery-5.4.0rc2/t/unit/app/test_registry.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/app/test_routes.py` & `celery-5.4.0rc2/t/unit/app/test_routes.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/app/test_schedules.py` & `celery-5.4.0rc2/t/unit/app/test_schedules.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/app/test_utils.py` & `celery-5.4.0rc2/t/unit/app/test_utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/apps/test_multi.py` & `celery-5.4.0rc2/t/unit/apps/test_multi.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_arangodb.py` & `celery-5.4.0rc2/t/unit/backends/test_arangodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_asynchronous.py` & `celery-5.4.0rc2/t/unit/backends/test_asynchronous.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_azureblockblob.py` & `celery-5.4.0rc2/t/unit/backends/test_azureblockblob.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_base.py` & `celery-5.4.0rc2/t/unit/backends/test_base.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_cache.py` & `celery-5.4.0rc2/t/unit/backends/test_cache.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_cassandra.py` & `celery-5.4.0rc2/t/unit/backends/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_consul.py` & `celery-5.4.0rc2/t/unit/backends/test_consul.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_cosmosdbsql.py` & `celery-5.4.0rc2/t/unit/backends/test_cosmosdbsql.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_couchbase.py` & `celery-5.4.0rc2/t/unit/backends/test_couchbase.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_couchdb.py` & `celery-5.4.0rc2/t/unit/backends/test_couchdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_database.py` & `celery-5.4.0rc2/t/unit/backends/test_database.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_dynamodb.py` & `celery-5.4.0rc2/t/unit/backends/test_dynamodb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from decimal import Decimal
-from unittest.mock import MagicMock, Mock, patch, sentinel
+from unittest.mock import ANY, MagicMock, Mock, call, patch, sentinel
 
 import pytest
 
-from celery import states
+from celery import states, uuid
 from celery.backends import dynamodb as module
 from celery.backends.dynamodb import DynamoDBBackend
 from celery.exceptions import ImproperlyConfigured
 
 pytest.importorskip('boto3')
 
 
@@ -422,14 +422,42 @@
                 }
             }
         }
         with patch('celery.backends.dynamodb.time', self._mock_time):
             result = self.backend._prepare_put_request('abcdef', 'val')
         assert result == expected
 
+    def test_prepare_init_count_request(self):
+        expected = {
+            'TableName': 'celery',
+            'Item': {
+                'id': {'S': 'abcdef'},
+                'chord_count': {'N': '0'},
+                'timestamp': {
+                    'N': str(Decimal(self._static_timestamp))
+                },
+            }
+        }
+        with patch('celery.backends.dynamodb.time', self._mock_time):
+            result = self.backend._prepare_init_count_request('abcdef')
+        assert result == expected
+
+    def test_prepare_inc_count_request(self):
+        expected = {
+            'TableName': 'celery',
+            'Key': {
+                'id': {'S': 'abcdef'},
+            },
+            'UpdateExpression': 'set chord_count = chord_count + :num',
+            'ExpressionAttributeValues': {":num": {"N": "1"}},
+            'ReturnValues': 'UPDATED_NEW',
+        }
+        result = self.backend._prepare_inc_count_request('abcdef')
+        assert result == expected
+
     def test_item_to_dict(self):
         boto_response = {
             'Item': {
                 'id': {
                     'S': sentinel.key
                 },
                 'result': {
@@ -513,14 +541,47 @@
         # should return None
         assert self.backend.delete('1f3fab') is None
         self.backend.client.delete_item.assert_called_once_with(
             Key={'id': {'S': '1f3fab'}},
             TableName='celery'
         )
 
+    def test_inc(self):
+        mocked_incr_response = {
+            'Attributes': {
+                'chord_count': {
+                    'N': '1'
+                }
+            },
+            'ResponseMetadata': {
+                'RequestId': '16d31c72-51f6-4538-9415-499f1135dc59',
+                'HTTPStatusCode': 200,
+                'HTTPHeaders': {
+                    'date': 'Wed, 10 Jan 2024 17:53:41 GMT',
+                    'x-amzn-requestid': '16d31c72-51f6-4538-9415-499f1135dc59',
+                    'content-type': 'application/x-amz-json-1.0',
+                    'x-amz-crc32': '3438282865',
+                    'content-length': '40',
+                    'server': 'Jetty(11.0.17)'
+                },
+                'RetryAttempts': 0
+            }
+        }
+        self.backend._client = MagicMock()
+        self.backend._client.update_item = MagicMock(return_value=mocked_incr_response)
+
+        assert self.backend.incr('1f3fab') == 1
+        self.backend.client.update_item.assert_called_once_with(
+            Key={'id': {'S': '1f3fab'}},
+            TableName='celery',
+            UpdateExpression='set chord_count = chord_count + :num',
+            ExpressionAttributeValues={":num": {"N": "1"}},
+            ReturnValues='UPDATED_NEW',
+        )
+
     def test_backend_by_url(self, url='dynamodb://'):
         from celery.app import backends
         from celery.backends.dynamodb import DynamoDBBackend
         backend, url_ = backends.by_url(url, self.app.loader)
         assert backend is DynamoDBBackend
         assert url_ == url
 
@@ -533,7 +594,37 @@
         )
         assert self.backend.aws_region == 'us-east-1'
         assert self.backend.table_name == 'celery_results'
         assert self.backend.read_capacity_units == 10
         assert self.backend.write_capacity_units == 20
         assert self.backend.time_to_live_seconds == 600
         assert self.backend.endpoint_url is None
+
+    def test_apply_chord(self, unlock="celery.chord_unlock"):
+        self.app.tasks[unlock] = Mock()
+        chord_uuid = uuid()
+        header_result_args = (
+            chord_uuid,
+            [self.app.AsyncResult(x) for x in range(3)],
+        )
+        self.backend._client = MagicMock()
+        self.backend.apply_chord(header_result_args, None)
+        assert self.backend._client.put_item.call_args_list == [
+            call(
+                TableName="celery",
+                Item={
+                    "id": {"S": f"b'chord-unlock-{chord_uuid}'"},
+                    "chord_count": {"N": "0"},
+                    "timestamp": {"N": ANY},
+                },
+            ),
+            call(
+                TableName="celery",
+                Item={
+                    "id": {"S": f"b'celery-taskset-meta-{chord_uuid}'"},
+                    "result": {
+                        "B": ANY,
+                    },
+                    "timestamp": {"N": ANY},
+                },
+            ),
+        ]
```

### Comparing `celery-5.4.0rc1/t/unit/backends/test_elasticsearch.py` & `celery-5.4.0rc2/t/unit/backends/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_filesystem.py` & `celery-5.4.0rc2/t/unit/backends/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_mongodb.py` & `celery-5.4.0rc2/t/unit/backends/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_redis.py` & `celery-5.4.0rc2/t/unit/backends/test_redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1167,15 +1167,15 @@
                 assert self.b.client.zadd.call_count == 1
                 self.b.client.zadd.reset_mock()
         # Confirm that neither `zrange` not `lrange` were called
         self.b.client.zrange.assert_not_called()
         self.b.client.lrange.assert_not_called()
         # Confirm that the `GroupResult.restore` mock was called
         complex_header_result.assert_called_once_with(request.group)
-        # Confirm the the callback was called with the `join()`ed group result
+        # Confirm that the callback was called with the `join()`ed group result
         if supports_native_join:
             expected_join = mock_result_obj.join_native
         else:
             expected_join = mock_result_obj.join
         callback.delay.assert_called_once_with(expected_join())
```

### Comparing `celery-5.4.0rc1/t/unit/backends/test_rpc.py` & `celery-5.4.0rc2/t/unit/backends/test_rpc.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/backends/test_s3.py` & `celery-5.4.0rc2/t/unit/backends/test_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from unittest.mock import patch
 
 import boto3
 import pytest
 from botocore.exceptions import ClientError
-from moto import mock_s3
+
+try:
+    from moto import mock_aws
+except ImportError:
+    from moto import mock_s3 as mock_aws
 
 from celery import states
 from celery.backends.s3 import S3Backend
 from celery.exceptions import ImproperlyConfigured
 
 
 class test_S3Backend:
@@ -80,42 +84,42 @@
         self.app.conf.s3_endpoint_url = endpoint_url
 
         S3Backend(app=self.app)
         mock_boto3.Session().resource.assert_called_once_with(
             's3', endpoint_url=endpoint_url)
 
     @pytest.mark.parametrize("key", ['uuid', b'uuid'])
-    @mock_s3
+    @mock_aws
     def test_set_and_get_a_key(self, key):
         self._mock_s3_resource()
 
         self.app.conf.s3_access_key_id = 'somekeyid'
         self.app.conf.s3_secret_access_key = 'somesecret'
         self.app.conf.s3_bucket = 'bucket'
 
         s3_backend = S3Backend(app=self.app)
         s3_backend._set_with_state(key, 'another_status', states.SUCCESS)
 
         assert s3_backend.get(key) == 'another_status'
 
-    @mock_s3
+    @mock_aws
     def test_set_and_get_a_result(self):
         self._mock_s3_resource()
 
         self.app.conf.result_serializer = 'pickle'
         self.app.conf.s3_access_key_id = 'somekeyid'
         self.app.conf.s3_secret_access_key = 'somesecret'
         self.app.conf.s3_bucket = 'bucket'
 
         s3_backend = S3Backend(app=self.app)
         s3_backend.store_result('foo', 'baar', 'STARTED')
         value = s3_backend.get_result('foo')
         assert value == 'baar'
 
-    @mock_s3
+    @mock_aws
     def test_get_a_missing_key(self):
         self._mock_s3_resource()
 
         self.app.conf.s3_access_key_id = 'somekeyid'
         self.app.conf.s3_secret_access_key = 'somesecret'
         self.app.conf.s3_bucket = 'bucket'
 
@@ -137,15 +141,15 @@
 
         s3_backend = S3Backend(app=self.app)
 
         with pytest.raises(ClientError):
             s3_backend.get('uuidddd')
 
     @pytest.mark.parametrize("key", ['uuid', b'uuid'])
-    @mock_s3
+    @mock_aws
     def test_delete_a_key(self, key):
         self._mock_s3_resource()
 
         self.app.conf.s3_access_key_id = 'somekeyid'
         self.app.conf.s3_secret_access_key = 'somesecret'
         self.app.conf.s3_bucket = 'bucket'
 
@@ -153,15 +157,15 @@
         s3_backend._set_with_state(key, 'another_status', states.SUCCESS)
         assert s3_backend.get(key) == 'another_status'
 
         s3_backend.delete(key)
 
         assert s3_backend.get(key) is None
 
-    @mock_s3
+    @mock_aws
     def test_with_a_non_existing_bucket(self):
         self._mock_s3_resource()
 
         self.app.conf.s3_access_key_id = 'somekeyid'
         self.app.conf.s3_secret_access_key = 'somesecret'
         self.app.conf.s3_bucket = 'bucket_not_exists'
```

### Comparing `celery-5.4.0rc1/t/unit/bin/proj/pyramid_celery_app.py` & `celery-5.4.0rc2/t/unit/bin/proj/pyramid_celery_app.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/bin/test_beat.py` & `celery-5.4.0rc2/t/unit/bin/test_beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/bin/test_worker.py` & `celery-5.4.0rc2/t/unit/bin/test_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/concurrency/test_concurrency.py` & `celery-5.4.0rc2/t/unit/concurrency/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/concurrency/test_eventlet.py` & `celery-5.4.0rc2/t/unit/concurrency/test_eventlet.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/concurrency/test_gevent.py` & `celery-5.4.0rc2/t/unit/concurrency/test_gevent.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/concurrency/test_pool.py` & `celery-5.4.0rc2/t/unit/concurrency/test_pool.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/concurrency/test_prefork.py` & `celery-5.4.0rc2/t/unit/concurrency/test_prefork.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/concurrency/test_solo.py` & `celery-5.4.0rc2/t/unit/concurrency/test_solo.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/concurrency/test_thread.py` & `celery-5.4.0rc2/t/unit/concurrency/test_thread.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/conftest.py` & `celery-5.4.0rc2/t/unit/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             if isinstance(backend.client, DummyClient):
                 backend.client.cache.clear()
             backend._cache.clear()
 
 
 @contextmanager
 def assert_signal_called(signal, **expected):
-    """Context that verifes signal is called before exiting."""
+    """Context that verifies signal is called before exiting."""
     handler = Mock()
 
     def on_call(**kwargs):
         return handler(**kwargs)
 
     signal.connect(on_call)
     try:
```

### Comparing `celery-5.4.0rc1/t/unit/contrib/test_abortable.py` & `celery-5.4.0rc2/t/unit/contrib/test_abortable.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/contrib/test_migrate.py` & `celery-5.4.0rc2/t/unit/contrib/test_migrate.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/contrib/test_pytest.py` & `celery-5.4.0rc2/t/unit/contrib/test_pytest.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/contrib/test_rdb.py` & `celery-5.4.0rc2/t/unit/contrib/test_rdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/contrib/test_sphinx.py` & `celery-5.4.0rc2/t/unit/contrib/test_sphinx.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/contrib/test_worker.py` & `celery-5.4.0rc2/t/unit/contrib/test_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.error_task = error_task
 
         self.app.config_from_object({
             'worker_hijack_root_logger': False,
         })
 
         # to avoid changing the root logger level to ERROR,
-        # we have we have to set both app.log.loglevel start_worker arg to 0
+        # we have to set both app.log.loglevel start_worker arg to 0
         # (see celery.app.log.setup_logging_subsystem)
         self.app.log.loglevel = 0
 
     def test_start_worker(self):
         with start_worker(app=self.app, loglevel=0):
             result = self.add.s(1, 2).apply_async()
             val = result.get(timeout=5)
```

### Comparing `celery-5.4.0rc1/t/unit/events/test_cursesmon.py` & `celery-5.4.0rc2/t/unit/events/test_cursesmon.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/events/test_events.py` & `celery-5.4.0rc2/t/unit/events/test_events.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/events/test_snapshot.py` & `celery-5.4.0rc2/t/unit/events/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/events/test_state.py` & `celery-5.4.0rc2/t/unit/events/test_state.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/fixups/test_django.py` & `celery-5.4.0rc2/t/unit/fixups/test_django.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,26 +83,50 @@
             _maybe_close_fd(Mock())
             _maybe_close_fd(object())
 
     def test_init(self):
         with self.fixup_context(self.app) as (f, importmod, sym):
             assert f
 
-    def test_install(self, patching):
+    @pytest.mark.patched_module(
+        'django',
+        'django.db',
+        'django.db.transaction',
+    )
+    def test_install(self, patching, module):
         self.app.loader = Mock()
         self.cw = patching('os.getcwd')
         self.p = patching('sys.path')
         self.sigs = patching('celery.fixups.django.signals')
         with self.fixup_context(self.app) as (f, _, _):
             self.cw.return_value = '/opt/vandelay'
             f.install()
             self.sigs.worker_init.connect.assert_called_with(f.on_worker_init)
             assert self.app.loader.now == f.now
+
+            # Specialized Task class is used
+            assert self.app.task_cls == 'celery.contrib.django.task:DjangoTask'
+            from celery.contrib.django.task import DjangoTask
+            assert issubclass(f.app.Task, DjangoTask)
+            assert hasattr(f.app.Task, 'delay_on_commit')
+            assert hasattr(f.app.Task, 'apply_async_on_commit')
+
             self.p.insert.assert_called_with(0, '/opt/vandelay')
 
+    def test_install_custom_user_task(self, patching):
+        patching('celery.fixups.django.signals')
+
+        self.app.task_cls = 'myapp.celery.tasks:Task'
+        self.app._custom_task_cls_used = True
+
+        with self.fixup_context(self.app) as (f, _, _):
+            f.install()
+            # Specialized Task class is NOT used
+            assert self.app.task_cls == 'myapp.celery.tasks:Task'
+
     def test_now(self):
         with self.fixup_context(self.app) as (f, _, _):
             assert f.now(utc=True)
             f._now.assert_not_called()
             assert f.now(utc=False)
             f._now.assert_called()
```

### Comparing `celery-5.4.0rc1/t/unit/security/__init__.py` & `celery-5.4.0rc2/t/unit/security/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/security/test_certificate.py` & `celery-5.4.0rc2/t/unit/security/test_certificate.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/security/test_key.py` & `celery-5.4.0rc2/t/unit/security/test_key.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/security/test_security.py` & `celery-5.4.0rc2/t/unit/security/test_security.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/security/test_serialization.py` & `celery-5.4.0rc2/t/unit/security/test_serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/tasks/test_canvas.py` & `celery-5.4.0rc2/t/unit/tasks/test_canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -567,14 +567,44 @@
         c = chord([signature('header')], group(signature('body')))
         c = chain(c)
         t = signature('t')
         new_chain = c | t  # t should be chained with the body of c[0] and create a new chord
         assert isinstance(new_chain, _chain)
         assert isinstance(new_chain.tasks[0].body, chord)
 
+    @pytest.mark.parametrize(
+        "group_last_task",
+        [False, True],
+    )
+    def test_chain_of_chord_upgrade_on_chaining__protocol_2(
+            self, group_last_task):
+        c = chain(
+            group([self.add.s(i, i) for i in range(5)], app=self.app),
+            group([self.add.s(i, i) for i in range(10, 15)], app=self.app),
+            group([self.add.s(i, i) for i in range(20, 25)], app=self.app),
+            self.add.s(30) if not group_last_task else group(self.add.s(30),
+                                                             app=self.app))
+        assert isinstance(c, _chain)
+        assert len(
+            c.tasks
+        ) == 1, "Consecutive chords should be further upgraded to a single chord."
+        assert isinstance(c.tasks[0], chord)
+
+    def test_chain_of_chord_upgrade_on_chaining__protocol_3(self):
+        c = chain(
+            chain([self.add.s(i, i) for i in range(5)]),
+            group([self.add.s(i, i) for i in range(10, 15)], app=self.app),
+            chord([signature('header')], signature('body'), app=self.app),
+            group([self.add.s(i, i) for i in range(20, 25)], app=self.app))
+        assert isinstance(c, _chain)
+        assert isinstance(
+            c.tasks[-1], chord
+        ), "Chord followed by a group should be upgraded to a single chord with chained body."
+        assert len(c.tasks) == 6
+
     def test_apply_options(self):
 
         class static(Signature):
 
             def clone(self, *args, **kwargs):
                 return self
 
@@ -785,14 +815,20 @@
         assert 'link' not in flat_chain.tasks[0].options
         assert signature(flat_chain.tasks[0].options['link_error'][0]) == signature('link_ab')
         assert flat_chain.tasks[1].name == 'b'
         assert 'link' in flat_chain.tasks[1].options, "b is missing the link from inner_chain.options['link'][0]"
         assert signature(flat_chain.tasks[1].options['link'][0]) == signature('link_b')
         assert signature(flat_chain.tasks[1].options['link_error'][0]) == signature('link_ab')
 
+    def test_group_in_center_of_chain(self):
+        t1 = chain(self.add.si(1, 1), group(self.add.si(1, 1), self.add.si(1, 1)),
+                   self.add.si(1, 1) | self.add.si(1, 1))
+        t2 = chord([self.add.si(1, 1), self.add.si(1, 1)], t1)
+        t2.freeze()  # should not raise
+
 
 class test_group(CanvasCase):
     def test_repr(self):
         x = group([self.add.s(2, 2), self.add.s(4, 4)])
         assert repr(x)
 
     def test_repr_empty_group(self):
@@ -865,14 +901,24 @@
         sig = Mock(name='sig')
         g1.link_error(sig)
         # We expect that all group children will be given the errback to ensure
         # it gets called
         for child_sig in g1.tasks:
             child_sig.link_error.assert_called_with(sig.clone(immutable=True))
 
+    def test_link_error_with_dict_sig(self):
+        g1 = group(Mock(name='t1'), Mock(name='t2'), app=self.app)
+        errback = signature('tcb')
+        errback_dict = dict(errback)
+        g1.link_error(errback_dict)
+        # We expect that all group children will be given the errback to ensure
+        # it gets called
+        for child_sig in g1.tasks:
+            child_sig.link_error.assert_called_with(errback.clone(immutable=True))
+
     def test_apply_empty(self):
         x = group(app=self.app)
         x.apply()
         res = x.apply_async()
         assert res
         assert not res.results
```

### Comparing `celery-5.4.0rc1/t/unit/tasks/test_chord.py` & `celery-5.4.0rc2/t/unit/tasks/test_chord.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/tasks/test_context.py` & `celery-5.4.0rc2/t/unit/tasks/test_context.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/tasks/test_result.py` & `celery-5.4.0rc2/t/unit/tasks/test_result.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/tasks/test_stamping.py` & `celery-5.4.0rc2/t/unit/tasks/test_stamping.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/tasks/test_states.py` & `celery-5.4.0rc2/t/unit/tasks/test_states.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/tasks/test_tasks.py` & `celery-5.4.0rc2/t/unit/tasks/test_tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/tasks/test_trace.py` & `celery-5.4.0rc2/t/unit/tasks/test_trace.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/test_canvas.py` & `celery-5.4.0rc2/t/unit/test_canvas.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_collections.py` & `celery-5.4.0rc2/t/unit/utils/test_collections.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_debug.py` & `celery-5.4.0rc2/t/unit/utils/test_debug.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_deprecated.py` & `celery-5.4.0rc2/t/unit/utils/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_dispatcher.py` & `celery-5.4.0rc2/t/unit/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_functional.py` & `celery-5.4.0rc2/t/unit/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_graph.py` & `celery-5.4.0rc2/t/unit/utils/test_graph.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_imports.py` & `celery-5.4.0rc2/t/unit/utils/test_imports.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_local.py` & `celery-5.4.0rc2/t/unit/utils/test_local.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_pickle.py` & `celery-5.4.0rc2/t/unit/utils/test_pickle.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_platforms.py` & `celery-5.4.0rc2/t/unit/utils/test_platforms.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_saferepr.py` & `celery-5.4.0rc2/t/unit/utils/test_saferepr.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_serialization.py` & `celery-5.4.0rc2/t/unit/utils/test_serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_sysinfo.py` & `celery-5.4.0rc2/t/unit/utils/test_sysinfo.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_term.py` & `celery-5.4.0rc2/t/unit/utils/test_term.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_text.py` & `celery-5.4.0rc2/t/unit/utils/test_text.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_threads.py` & `celery-5.4.0rc2/t/unit/utils/test_threads.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_time.py` & `celery-5.4.0rc2/t/unit/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_timer2.py` & `celery-5.4.0rc2/t/unit/utils/test_timer2.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/utils/test_utils.py` & `celery-5.4.0rc2/t/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/worker/test_autoscale.py` & `celery-5.4.0rc2/t/unit/worker/test_autoscale.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/worker/test_bootsteps.py` & `celery-5.4.0rc2/t/unit/worker/test_bootsteps.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/worker/test_components.py` & `celery-5.4.0rc2/t/unit/worker/test_components.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/worker/test_consumer.py` & `celery-5.4.0rc2/t/unit/worker/test_consumer.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/worker/test_control.py` & `celery-5.4.0rc2/t/unit/worker/test_control.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/worker/test_heartbeat.py` & `celery-5.4.0rc2/t/unit/worker/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/worker/test_loops.py` & `celery-5.4.0rc2/t/unit/worker/test_loops.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/worker/test_request.py` & `celery-5.4.0rc2/t/unit/worker/test_request.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/worker/test_state.py` & `celery-5.4.0rc2/t/unit/worker/test_state.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/worker/test_strategy.py` & `celery-5.4.0rc2/t/unit/worker/test_strategy.py`

 * *Files identical despite different names*

### Comparing `celery-5.4.0rc1/t/unit/worker/test_worker.py` & `celery-5.4.0rc2/t/unit/worker/test_worker.py`

 * *Files identical despite different names*

