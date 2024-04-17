# Comparing `tmp/digitalhub-core-0.3.1.tar.gz` & `tmp/digitalhub_core-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub-core-0.3.1.tar", last modified: Wed Apr 10 08:28:29 2024, max compression
+gzip compressed data, was "digitalhub_core-0.3.2.tar", last modified: Wed Apr 17 12:31:10 2024, max compression
```

## Comparing `digitalhub-core-0.3.1.tar` & `digitalhub_core-0.3.2.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.875790 digitalhub-core-0.3.1/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-core-0.3.1/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14637 2024-04-10 08:28:29.875790 digitalhub-core-0.3.1/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       84 2023-11-17 11:56:29.000000 digitalhub-core-0.3.1/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.851790 digitalhub-core-0.3.1/digitalhub_core/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1263 2024-04-10 08:00:26.000000 digitalhub-core-0.3.1/digitalhub_core/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.855790 digitalhub-core-0.3.1/digitalhub_core/client/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/client/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1948 2024-02-21 12:33:19.000000 digitalhub-core-0.3.1/digitalhub_core/client/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.855790 digitalhub-core-0.3.1/digitalhub_core/client/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub-core-0.3.1/digitalhub_core/client/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1194 2024-03-19 15:41:29.000000 digitalhub-core-0.3.1/digitalhub_core/client/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8192 2024-04-03 11:07:40.000000 digitalhub-core-0.3.1/digitalhub_core/client/objects/dhcore.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    15046 2024-04-04 07:48:11.000000 digitalhub-core-0.3.1/digitalhub_core/client/objects/local.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.855790 digitalhub-core-0.3.1/digitalhub_core/context/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/context/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub-core-0.3.1/digitalhub_core/context/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2803 2024-03-19 15:49:55.000000 digitalhub-core-0.3.1/digitalhub_core/context/context.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.859790 digitalhub-core-0.3.1/digitalhub_core/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.859790 digitalhub-core-0.3.1/digitalhub_core/entities/_base/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_base/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_base/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3099 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_base/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2581 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_base/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1785 2024-02-15 12:11:01.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_base/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2164 2024-03-11 14:15:28.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_base/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.859790 digitalhub-core-0.3.1/digitalhub_core/entities/_builders/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_builders/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3239 2024-04-10 08:00:26.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_builders/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2991 2024-04-10 08:00:26.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_builders/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3173 2024-04-10 08:00:26.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_builders/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.859790 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6563 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    13513 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1109 2024-01-31 09:13:38.000000 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-03-07 15:14:39.000000 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:14.000000 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.863790 digitalhub-core-0.3.1/digitalhub_core/entities/functions/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/functions/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6220 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/functions/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16241 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/functions/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1109 2024-01-31 09:16:01.000000 digitalhub-core-0.3.1/digitalhub_core/entities/functions/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-08 12:53:09.000000 digitalhub-core-0.3.1/digitalhub_core/entities/functions/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub-core-0.3.1/digitalhub_core/entities/functions/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.863790 digitalhub-core-0.3.1/digitalhub_core/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8627 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    21767 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      866 2024-01-31 09:16:02.000000 digitalhub-core-0.3.1/digitalhub_core/entities/projects/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub-core-0.3.1/digitalhub_core/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub-core-0.3.1/digitalhub_core/entities/projects/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      710 2024-03-07 13:44:22.000000 digitalhub-core-0.3.1/digitalhub_core/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.863790 digitalhub-core-0.3.1/digitalhub_core/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4819 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/runs/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14263 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/runs/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      825 2024-01-31 09:16:02.000000 digitalhub-core-0.3.1/digitalhub_core/entities/runs/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3620 2024-03-22 13:57:11.000000 digitalhub-core-0.3.1/digitalhub_core/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2692 2024-03-20 12:21:43.000000 digitalhub-core-0.3.1/digitalhub_core/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.867790 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6082 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8374 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1103 2024-02-06 10:40:16.000000 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.867790 digitalhub-core-0.3.1/digitalhub_core/entities/services/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:49:32.000000 digitalhub-core-0.3.1/digitalhub_core/entities/services/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6043 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/services/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6997 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/services/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1106 2024-02-06 10:49:57.000000 digitalhub-core-0.3.1/digitalhub_core/entities/services/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      368 2024-02-15 09:49:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/services/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:37.000000 digitalhub-core-0.3.1/digitalhub_core/entities/services/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.867790 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5606 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10494 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      828 2024-01-31 09:16:02.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5084 2024-03-19 10:03:54.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.871790 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6083 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     7180 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1109 2024-01-31 09:16:02.000000 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      373 2024-02-15 09:49:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.871790 digitalhub-core-0.3.1/digitalhub_core/runtimes/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub-core-0.3.1/digitalhub_core/runtimes/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3963 2024-03-01 09:41:58.000000 digitalhub-core-0.3.1/digitalhub_core/runtimes/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2233 2024-02-21 08:40:16.000000 digitalhub-core-0.3.1/digitalhub_core/runtimes/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      640 2024-02-01 10:45:50.000000 digitalhub-core-0.3.1/digitalhub_core/runtimes/registry.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.871790 digitalhub-core-0.3.1/digitalhub_core/stores/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/stores/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/stores/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.871790 digitalhub-core-0.3.1/digitalhub_core/stores/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/stores/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4587 2024-01-03 08:29:18.000000 digitalhub-core-0.3.1/digitalhub_core/stores/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4508 2024-03-12 13:41:08.000000 digitalhub-core-0.3.1/digitalhub_core/stores/objects/local.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5039 2024-03-12 13:41:08.000000 digitalhub-core-0.3.1/digitalhub_core/stores/objects/remote.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8844 2024-01-03 08:29:18.000000 digitalhub-core-0.3.1/digitalhub_core/stores/objects/s3.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8927 2024-01-03 08:29:18.000000 digitalhub-core-0.3.1/digitalhub_core/stores/objects/sql.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.871790 digitalhub-core-0.3.1/digitalhub_core/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub-core-0.3.1/digitalhub_core/utils/api.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub-core-0.3.1/digitalhub_core/utils/exceptions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub-core-0.3.1/digitalhub_core/utils/file_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5341 2024-04-09 08:40:57.000000 digitalhub-core-0.3.1/digitalhub_core/utils/generic_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2331 2024-02-15 10:46:43.000000 digitalhub-core-0.3.1/digitalhub_core/utils/import_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub-core-0.3.1/digitalhub_core/utils/io_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub-core-0.3.1/digitalhub_core/utils/logger.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      770 2024-04-08 13:33:46.000000 digitalhub-core-0.3.1/digitalhub_core/utils/uri_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.871790 digitalhub-core-0.3.1/digitalhub_core.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14637 2024-04-10 08:28:29.000000 digitalhub-core-0.3.1/digitalhub_core.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3986 2024-04-10 08:28:29.000000 digitalhub-core-0.3.1/digitalhub_core.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-10 08:28:29.000000 digitalhub-core-0.3.1/digitalhub_core.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      250 2024-04-10 08:28:29.000000 digitalhub-core-0.3.1/digitalhub_core.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-10 08:28:29.000000 digitalhub-core-0.3.1/digitalhub_core.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1727 2024-04-09 13:57:43.000000 digitalhub-core-0.3.1/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-10 08:28:29.875790 digitalhub-core-0.3.1/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.737126 digitalhub_core-0.3.2/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub_core-0.3.2/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14637 2024-04-17 12:31:10.737126 digitalhub_core-0.3.2/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       84 2023-11-17 11:56:29.000000 digitalhub_core-0.3.2/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.721126 digitalhub_core-0.3.2/digitalhub_core/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1263 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.721126 digitalhub_core-0.3.2/digitalhub_core/client/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.3.2/digitalhub_core/client/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1948 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/client/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.725126 digitalhub_core-0.3.2/digitalhub_core/client/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub_core-0.3.2/digitalhub_core/client/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1194 2024-03-19 15:41:29.000000 digitalhub_core-0.3.2/digitalhub_core/client/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8193 2024-04-16 14:02:23.000000 digitalhub_core-0.3.2/digitalhub_core/client/objects/dhcore.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    15046 2024-04-04 07:48:11.000000 digitalhub_core-0.3.2/digitalhub_core/client/objects/local.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.725126 digitalhub_core-0.3.2/digitalhub_core/context/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.3.2/digitalhub_core/context/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub_core-0.3.2/digitalhub_core/context/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2803 2024-03-19 15:49:55.000000 digitalhub_core-0.3.2/digitalhub_core/context/context.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.725126 digitalhub_core-0.3.2/digitalhub_core/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.3.2/digitalhub_core/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.725126 digitalhub_core-0.3.2/digitalhub_core/entities/_base/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.3.2/digitalhub_core/entities/_base/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub_core-0.3.2/digitalhub_core/entities/_base/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3099 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/_base/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2581 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/_base/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1785 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/_base/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2164 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/_base/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.725126 digitalhub_core-0.3.2/digitalhub_core/entities/_builders/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub_core-0.3.2/digitalhub_core/entities/_builders/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3239 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/_builders/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2991 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/_builders/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3173 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/_builders/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.725126 digitalhub_core-0.3.2/digitalhub_core/entities/artifacts/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.3.2/digitalhub_core/entities/artifacts/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6563 2024-04-16 14:28:24.000000 digitalhub_core-0.3.2/digitalhub_core/entities/artifacts/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    13513 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/artifacts/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1109 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/artifacts/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/artifacts/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/artifacts/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.729126 digitalhub_core-0.3.2/digitalhub_core/entities/functions/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.3.2/digitalhub_core/entities/functions/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6220 2024-04-16 14:28:24.000000 digitalhub_core-0.3.2/digitalhub_core/entities/functions/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16241 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/functions/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1109 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/functions/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1496 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/functions/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub_core-0.3.2/digitalhub_core/entities/functions/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.729126 digitalhub_core-0.3.2/digitalhub_core/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.3.2/digitalhub_core/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8627 2024-04-16 14:28:24.000000 digitalhub_core-0.3.2/digitalhub_core/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    21873 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      866 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/projects/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub_core-0.3.2/digitalhub_core/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub_core-0.3.2/digitalhub_core/entities/projects/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      710 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.729126 digitalhub_core-0.3.2/digitalhub_core/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.3.2/digitalhub_core/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4819 2024-04-16 14:28:24.000000 digitalhub_core-0.3.2/digitalhub_core/entities/runs/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14263 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/runs/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      825 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/runs/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3620 2024-03-22 13:57:11.000000 digitalhub_core-0.3.2/digitalhub_core/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2692 2024-03-20 12:21:43.000000 digitalhub_core-0.3.2/digitalhub_core/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.729126 digitalhub_core-0.3.2/digitalhub_core/entities/secrets/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub_core-0.3.2/digitalhub_core/entities/secrets/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6082 2024-04-16 14:28:24.000000 digitalhub_core-0.3.2/digitalhub_core/entities/secrets/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8374 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/secrets/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1103 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/secrets/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub_core-0.3.2/digitalhub_core/entities/secrets/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub_core-0.3.2/digitalhub_core/entities/secrets/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.729126 digitalhub_core-0.3.2/digitalhub_core/entities/services/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:49:32.000000 digitalhub_core-0.3.2/digitalhub_core/entities/services/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6043 2024-04-16 14:28:24.000000 digitalhub_core-0.3.2/digitalhub_core/entities/services/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6997 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/services/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1106 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/services/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      368 2024-02-15 09:49:55.000000 digitalhub_core-0.3.2/digitalhub_core/entities/services/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:37.000000 digitalhub_core-0.3.2/digitalhub_core/entities/services/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.729126 digitalhub_core-0.3.2/digitalhub_core/entities/tasks/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.3.2/digitalhub_core/entities/tasks/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5606 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/tasks/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10494 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/tasks/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      828 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/tasks/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5084 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/tasks/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub_core-0.3.2/digitalhub_core/entities/tasks/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub_core-0.3.2/digitalhub_core/entities/tasks/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.733126 digitalhub_core-0.3.2/digitalhub_core/entities/workflows/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.3.2/digitalhub_core/entities/workflows/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6083 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/workflows/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     7058 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/workflows/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1109 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/workflows/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      373 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/entities/workflows/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub_core-0.3.2/digitalhub_core/entities/workflows/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.733126 digitalhub_core-0.3.2/digitalhub_core/runtimes/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub_core-0.3.2/digitalhub_core/runtimes/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3963 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/runtimes/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2233 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/runtimes/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      640 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/runtimes/registry.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.733126 digitalhub_core-0.3.2/digitalhub_core/stores/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.3.2/digitalhub_core/stores/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-04-16 14:28:24.000000 digitalhub_core-0.3.2/digitalhub_core/stores/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.733126 digitalhub_core-0.3.2/digitalhub_core/stores/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.3.2/digitalhub_core/stores/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4587 2024-01-03 08:29:18.000000 digitalhub_core-0.3.2/digitalhub_core/stores/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4508 2024-03-12 13:41:08.000000 digitalhub_core-0.3.2/digitalhub_core/stores/objects/local.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5039 2024-03-12 13:41:08.000000 digitalhub_core-0.3.2/digitalhub_core/stores/objects/remote.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8844 2024-01-03 08:29:18.000000 digitalhub_core-0.3.2/digitalhub_core/stores/objects/s3.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8927 2024-01-03 08:29:18.000000 digitalhub_core-0.3.2/digitalhub_core/stores/objects/sql.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.733126 digitalhub_core-0.3.2/digitalhub_core/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.3.2/digitalhub_core/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub_core-0.3.2/digitalhub_core/utils/api.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub_core-0.3.2/digitalhub_core/utils/exceptions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub_core-0.3.2/digitalhub_core/utils/file_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5341 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/utils/generic_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2331 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/utils/import_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub_core-0.3.2/digitalhub_core/utils/io_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub_core-0.3.2/digitalhub_core/utils/logger.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      770 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/digitalhub_core/utils/uri_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:10.733126 digitalhub_core-0.3.2/digitalhub_core.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14637 2024-04-17 12:31:10.000000 digitalhub_core-0.3.2/digitalhub_core.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3986 2024-04-17 12:31:10.000000 digitalhub_core-0.3.2/digitalhub_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-17 12:31:10.000000 digitalhub_core-0.3.2/digitalhub_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      250 2024-04-17 12:31:10.000000 digitalhub_core-0.3.2/digitalhub_core.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-17 12:31:10.000000 digitalhub_core-0.3.2/digitalhub_core.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1727 2024-04-17 12:30:02.000000 digitalhub_core-0.3.2/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-17 12:31:10.737126 digitalhub_core-0.3.2/setup.cfg
```

### Comparing `digitalhub-core-0.3.1/LICENSE.txt` & `digitalhub_core-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/PKG-INFO` & `digitalhub_core-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub-core-0.3.1/digitalhub_core/__init__.py` & `digitalhub_core-0.3.2/digitalhub_core/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/client/builder.py` & `digitalhub_core-0.3.2/digitalhub_core/client/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/client/objects/base.py` & `digitalhub_core-0.3.2/digitalhub_core/client/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/client/objects/dhcore.py` & `digitalhub_core-0.3.2/digitalhub_core/client/objects/dhcore.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
         """
         # User for future entity ownership
         self._user = os.getenv("DIGITALHUB_CORE_USER")
 
         # Prioritize token over user/password
         token = os.getenv("DIGITALHUB_CORE_TOKEN")
         if token is not None:
-            self._auth_type = "token"
+            self._auth_type = "oauth2"
             self._access_token = token
             return
 
         password = os.getenv("DIGITALHUB_CORE_PASSWORD")
         if self._user is not None and password is not None:
             self._auth_type = "basic"
             self._password = password
```

### Comparing `digitalhub-core-0.3.1/digitalhub_core/client/objects/local.py` & `digitalhub_core-0.3.2/digitalhub_core/client/objects/local.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/context/builder.py` & `digitalhub_core-0.3.2/digitalhub_core/context/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/context/context.py` & `digitalhub_core-0.3.2/digitalhub_core/context/context.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/_base/base.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/_base/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/_base/entity.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/_base/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/_base/metadata.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/_base/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/_base/spec.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/_base/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/_base/status.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/_base/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/_builders/metadata.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/_builders/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/_builders/spec.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/_builders/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/_builders/status.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/_builders/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/crud.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/artifacts/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/entity.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/artifacts/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/metadata.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/artifacts/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/spec.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/artifacts/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/functions/crud.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/functions/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/functions/entity.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/functions/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/functions/metadata.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/functions/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/functions/spec.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/functions/spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,37 +22,33 @@
     """
     Source code struct.
     """
 
     def __init__(
         self,
         source: str | None = None,
-        handler: str | None = None,
         code: str | None = None,
         base64: str | None = None,
         lang: str | None = None,
     ) -> None:
         """
         Constructor.
 
         Parameters
         ----------
         source : str
             Source reference.
-        handler : str
-            Function entrypoint.
         code : str
             Source code (plain).
         base64 : str
             Source code (base64 encoded).
         lang : str
             Source code language (hint).
         """
         self.source = source
-        self.handler = handler
         self.code = code
         self.base64 = base64
         self.lang = lang
 
     def to_dict(self) -> dict:
         """
         Convert to dictionary.
@@ -61,16 +57,14 @@
         -------
         dict
             Dictionary representation of the object.
         """
         dict_ = {}
         if self.source is not None:
             dict_["source"] = self.source
-        if self.handler is not None:
-            dict_["handler"] = self.handler
         if self.base64 is not None:
             dict_["base64"] = self.base64
         if self.lang is not None:
             dict_["lang"] = self.lang
 
         return dict_
```

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/projects/crud.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/projects/entity.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/projects/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,20 +136,22 @@
             obj = self._refresh().to_dict()
         else:
             obj = self.to_dict()
 
         if not update:
             api = api_base_create("projects")
             new_obj = self._client.create_object(api, obj)
+            new_obj["local"] = self._client.is_local()
             self._update_attributes(new_obj)
             return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_base_update("projects", self.id)
         new_obj = self._client.update_object(api, obj)
+        new_obj["local"] = self._client.is_local()
         self._update_attributes(new_obj)
         return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file. If the objects are not embedded, the objects are
         exported as a YAML file.
```

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/projects/metadata.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/projects/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/projects/spec.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/registries.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/runs/crud.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/runs/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/runs/entity.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/runs/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/runs/metadata.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/runs/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/runs/spec.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/runs/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/runs/status.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/runs/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/secrets/crud.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/secrets/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/secrets/entity.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/secrets/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/secrets/metadata.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/secrets/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/secrets/spec.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/secrets/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/services/crud.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/services/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/services/entity.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/services/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/services/metadata.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/services/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/tasks/crud.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/tasks/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/tasks/entity.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/tasks/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/tasks/metadata.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/tasks/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/tasks/models.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/tasks/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/workflows/crud.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/workflows/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/workflows/entity.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/workflows/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,20 @@
 from pathlib import Path
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
-from digitalhub_core.entities.functions.crud import get_function
 from digitalhub_core.utils.api import api_ctx_create, api_ctx_update
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
-    from digitalhub_core.entities.runs.entity import Run
     from digitalhub_core.entities.workflows.metadata import WorkflowMetadata
     from digitalhub_core.entities.workflows.spec import WorkflowSpec
     from digitalhub_core.entities.workflows.status import WorkflowStatus
 
 
 class Workflow(Entity):
     """
```

### Comparing `digitalhub-core-0.3.1/digitalhub_core/entities/workflows/metadata.py` & `digitalhub_core-0.3.2/digitalhub_core/entities/workflows/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/runtimes/base.py` & `digitalhub_core-0.3.2/digitalhub_core/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/runtimes/builder.py` & `digitalhub_core-0.3.2/digitalhub_core/runtimes/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/runtimes/registry.py` & `digitalhub_core-0.3.2/digitalhub_core/runtimes/registry.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/stores/builder.py` & `digitalhub_core-0.3.2/digitalhub_core/stores/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/stores/objects/base.py` & `digitalhub_core-0.3.2/digitalhub_core/stores/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/stores/objects/local.py` & `digitalhub_core-0.3.2/digitalhub_core/stores/objects/local.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/stores/objects/remote.py` & `digitalhub_core-0.3.2/digitalhub_core/stores/objects/remote.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/stores/objects/s3.py` & `digitalhub_core-0.3.2/digitalhub_core/stores/objects/s3.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/stores/objects/sql.py` & `digitalhub_core-0.3.2/digitalhub_core/stores/objects/sql.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/utils/api.py` & `digitalhub_core-0.3.2/digitalhub_core/utils/api.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/utils/file_utils.py` & `digitalhub_core-0.3.2/digitalhub_core/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/utils/generic_utils.py` & `digitalhub_core-0.3.2/digitalhub_core/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/utils/import_utils.py` & `digitalhub_core-0.3.2/digitalhub_core/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/utils/io_utils.py` & `digitalhub_core-0.3.2/digitalhub_core/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core/utils/uri_utils.py` & `digitalhub_core-0.3.2/digitalhub_core/utils/uri_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/digitalhub_core.egg-info/PKG-INFO` & `digitalhub_core-0.3.2/digitalhub_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub-core-0.3.1/digitalhub_core.egg-info/SOURCES.txt` & `digitalhub_core-0.3.2/digitalhub_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.1/pyproject.toml` & `digitalhub_core-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-core"
-version = "0.3.1"
+version = "0.3.2"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -61,15 +61,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.bumpver]
-current_version = "0.3.1"
+current_version = "0.3.2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

