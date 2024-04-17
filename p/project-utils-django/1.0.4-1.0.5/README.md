# Comparing `tmp/project-utils-django-1.0.4.tar.gz` & `tmp/project-utils-django-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project-utils-django-1.0.4.tar", last modified: Wed Apr 17 01:29:50 2024, max compression
+gzip compressed data, was "project-utils-django-1.0.5.tar", last modified: Wed Apr 17 01:41:21 2024, max compression
```

## Comparing `project-utils-django-1.0.4.tar` & `project-utils-django-1.0.5.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.180374 project-utils-django-1.0.4/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 07:03:44.000000 project-utils-django-1.0.4/LICENSE
--rw-r--r--   0 mylx2014   (501) staff       (20)     1876 2024-04-17 01:29:50.180105 project-utils-django-1.0.4/PKG-INFO
--rw-r--r--   0 mylx2014   (501) staff       (20)     1289 2023-11-24 01:16:34.000000 project-utils-django-1.0.4/README.md
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.160186 project-utils-django-1.0.4/project_utils/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.4/project_utils/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.160797 project-utils-django-1.0.4/project_utils/collection/
--rw-r--r--   0 mylx2014   (501) staff       (20)      140 2023-10-14 01:51:03.000000 project-utils-django-1.0.4/project_utils/collection/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      596 2023-10-13 02:35:45.000000 project-utils-django-1.0.4/project_utils/collection/list_util.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.161537 project-utils-django-1.0.4/project_utils/config/
--rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 01:51:03.000000 project-utils-django-1.0.4/project_utils/config/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.162966 project-utils-django-1.0.4/project_utils/config/addr_config/
--rw-r--r--   0 mylx2014   (501) staff       (20)      652 2023-10-14 01:51:03.000000 project-utils-django-1.0.4/project_utils/config/addr_config/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      739 2023-11-24 01:16:34.000000 project-utils-django-1.0.4/project_utils/config/addr_config/base_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)       86 2023-10-14 01:51:03.000000 project-utils-django-1.0.4/project_utils/config/addr_config/hbase_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      777 2023-10-14 01:51:03.000000 project-utils-django-1.0.4/project_utils/config/addr_config/kafka_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      695 2023-10-14 01:51:03.000000 project-utils-django-1.0.4/project_utils/config/addr_config/mysql_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      825 2023-11-24 01:16:34.000000 project-utils-django-1.0.4/project_utils/config/addr_config/redis_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1039 2023-10-14 01:51:03.000000 project-utils-django-1.0.4/project_utils/config/base_config.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.163480 project-utils-django-1.0.4/project_utils/config/path_config/
--rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 01:51:03.000000 project-utils-django-1.0.4/project_utils/config/path_config/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      970 2023-10-13 02:35:45.000000 project-utils-django-1.0.4/project_utils/config/path_config/path_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1977 2023-10-14 01:51:03.000000 project-utils-django-1.0.4/project_utils/config/template.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.163679 project-utils-django-1.0.4/project_utils/db/
--rw-r--r--   0 mylx2014   (501) staff       (20)      164 2023-10-14 01:57:29.000000 project-utils-django-1.0.4/project_utils/db/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.164903 project-utils-django-1.0.4/project_utils/db/mysql/
--rw-r--r--   0 mylx2014   (501) staff       (20)      257 2023-10-14 01:57:29.000000 project-utils-django-1.0.4/project_utils/db/mysql/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3484 2023-11-28 08:48:43.000000 project-utils-django-1.0.4/project_utils/db/mysql/_collection.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2291 2023-12-15 01:39:50.000000 project-utils-django-1.0.4/project_utils/db/mysql/_pool.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      832 2023-11-24 01:16:34.000000 project-utils-django-1.0.4/project_utils/db/mysql/_result.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      107 2023-10-13 02:35:45.000000 project-utils-django-1.0.4/project_utils/db/mysql/_types.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.165650 project-utils-django-1.0.4/project_utils/exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      811 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      148 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/exception/collection_exception.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      144 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/exception/config_exception.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.165955 project-utils-django-1.0.4/project_utils/exception/db_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      141 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/exception/db_exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      118 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/exception/db_exception/mysql_exception.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      507 2023-10-13 02:35:45.000000 project-utils-django-1.0.4/project_utils/exception/my_base_exception.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.166095 project-utils-django-1.0.4/project_utils/exception/web_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/exception/web_exception/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.166366 project-utils-django-1.0.4/project_utils/exception/web_exception/django_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      125 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/exception/web_exception/django_exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      127 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/exception/web_exception/django_exception/model_exception.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.166665 project-utils-django-1.0.4/project_utils/exception/web_exception/django_exception/view_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      275 2023-10-18 02:20:38.000000 project-utils-django-1.0.4/project_utils/exception/web_exception/django_exception/view_exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      120 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/exception/web_exception/django_exception/view_exception/response_exception.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1255 2023-10-13 02:35:45.000000 project-utils-django-1.0.4/project_utils/io.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.166915 project-utils-django-1.0.4/project_utils/os/
--rw-r--r--   0 mylx2014   (501) staff       (20)       98 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/os/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      760 2023-10-13 02:35:45.000000 project-utils-django-1.0.4/project_utils/os/dir.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2029 2024-01-16 07:43:03.000000 project-utils-django-1.0.4/project_utils/time.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.167037 project-utils-django-1.0.4/project_utils/web/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.4/project_utils/web/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.167119 project-utils-django-1.0.4/project_utils/web/aiohttp/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.4/project_utils/web/aiohttp/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.167332 project-utils-django-1.0.4/project_utils/web/django/
--rw-r--r--   0 mylx2014   (501) staff       (20)      463 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/web/django/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.167625 project-utils-django-1.0.4/project_utils/web/django/celery/
--rw-r--r--   0 mylx2014   (501) staff       (20)       84 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/web/django/celery/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.167878 project-utils-django-1.0.4/project_utils/web/django/celery/_conf/
--rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/web/django/celery/_conf/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1061 2023-11-24 01:16:34.000000 project-utils-django-1.0.4/project_utils/web/django/celery/_conf/_celery_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      334 2023-10-18 01:14:46.000000 project-utils-django-1.0.4/project_utils/web/django/celery/create_app.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.168158 project-utils-django-1.0.4/project_utils/web/django/conf/
--rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/web/django/conf/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2145 2023-11-24 01:16:34.000000 project-utils-django-1.0.4/project_utils/web/django/conf/_django_config.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.168484 project-utils-django-1.0.4/project_utils/web/django/middle/
--rw-r--r--   0 mylx2014   (501) staff       (20)      124 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/web/django/middle/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1161 2023-11-24 01:16:34.000000 project-utils-django-1.0.4/project_utils/web/django/middle/_base_middle.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.169725 project-utils-django-1.0.4/project_utils/web/django/model/
--rw-r--r--   0 mylx2014   (501) staff       (20)      434 2024-01-15 14:04:29.000000 project-utils-django-1.0.4/project_utils/web/django/model/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      106 2023-12-10 05:49:34.000000 project-utils-django-1.0.4/project_utils/web/django/model/_base_meta.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1511 2024-01-15 14:04:29.000000 project-utils-django-1.0.4/project_utils/web/django/model/_base_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      487 2023-12-08 06:57:16.000000 project-utils-django-1.0.4/project_utils/web/django/model/_id_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      461 2024-01-15 14:04:29.000000 project-utils-django-1.0.4/project_utils/web/django/model/_model_type.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.170138 project-utils-django-1.0.4/project_utils/web/django/pagination/
--rw-r--r--   0 mylx2014   (501) staff       (20)      197 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/web/django/pagination/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1011 2023-11-24 01:16:34.000000 project-utils-django-1.0.4/project_utils/web/django/pagination/_base_pagination.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.170555 project-utils-django-1.0.4/project_utils/web/django/request/
--rw-r--r--   0 mylx2014   (501) staff       (20)      102 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/web/django/request/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1379 2023-11-24 01:16:34.000000 project-utils-django-1.0.4/project_utils/web/django/request/_request.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.171206 project-utils-django-1.0.4/project_utils/web/django/response/
--rw-r--r--   0 mylx2014   (501) staff       (20)      153 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/web/django/response/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1291 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/web/django/response/_response_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      213 2023-11-24 01:16:34.000000 project-utils-django-1.0.4/project_utils/web/django/response/_response_types.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.171679 project-utils-django-1.0.4/project_utils/web/django/serializer/
--rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/web/django/serializer/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      284 2023-10-13 02:35:45.000000 project-utils-django-1.0.4/project_utils/web/django/serializer/_base_meta.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      418 2023-10-14 02:37:02.000000 project-utils-django-1.0.4/project_utils/web/django/serializer/_base_serializer.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.172055 project-utils-django-1.0.4/project_utils/web/django/swagger/
--rw-r--r--   0 mylx2014   (501) staff       (20)      499 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.173273 project-utils-django-1.0.4/project_utils/web/django/swagger/_params/
--rw-r--r--   0 mylx2014   (501) staff       (20)      675 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/_params/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/_params/_base.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1025 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/_params/_form.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1164 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/_params/_params.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      978 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/_params/_query.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2065 2023-12-10 07:17:18.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/_params/_response.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      412 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/_params/_types.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      268 2023-12-10 07:15:26.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/_urls.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.174053 project-utils-django-1.0.4/project_utils/web/django/swagger/config/
--rw-r--r--   0 mylx2014   (501) staff       (20)       69 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/config/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      488 2023-12-10 07:15:01.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/config/_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1274 2023-12-10 07:15:01.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/config/_swagger.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.174545 project-utils-django-1.0.4/project_utils/web/django/swagger/document/
--rw-r--r--   0 mylx2014   (501) staff       (20)      256 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/document/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1169 2023-12-10 07:15:01.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/document/_document.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      273 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/swagger/document/_types.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      678 2023-11-24 01:16:34.000000 project-utils-django-1.0.4/project_utils/web/django/utils.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.175487 project-utils-django-1.0.4/project_utils/web/django/view/
--rw-r--r--   0 mylx2014   (501) staff       (20)      478 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/view/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/view/_async_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2086 2023-12-10 15:11:23.000000 project-utils-django-1.0.4/project_utils/web/django/view/_base.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.175976 project-utils-django-1.0.4/project_utils/web/django/view/_base_api/
--rw-r--r--   0 mylx2014   (501) staff       (20)       57 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/view/_base_api/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3277 2023-12-10 15:07:50.000000 project-utils-django-1.0.4/project_utils/web/django/view/_base_api/api.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      908 2023-12-10 15:07:50.000000 project-utils-django-1.0.4/project_utils/web/django/view/_base_api/api_util.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.176743 project-utils-django-1.0.4/project_utils/web/django/view/_rest_api/
--rw-r--r--   0 mylx2014   (501) staff       (20)      296 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/view/_rest_api/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1921 2023-12-10 15:07:50.000000 project-utils-django-1.0.4/project_utils/web/django/view/_rest_api/api.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      480 2023-12-10 15:08:55.000000 project-utils-django-1.0.4/project_utils/web/django/view/_rest_api/api_utils.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2020 2023-12-10 15:08:55.000000 project-utils-django-1.0.4/project_utils/web/django/view/_rest_api/async_api.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.177938 project-utils-django-1.0.4/project_utils/web/django/view/_rest_view/
--rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/view/_rest_view/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)    12607 2023-12-10 15:16:37.000000 project-utils-django-1.0.4/project_utils/web/django/view/_rest_view/_async_base_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 15:11:23.000000 project-utils-django-1.0.4/project_utils/web/django/view/_rest_view/_async_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)    12432 2023-12-10 15:11:23.000000 project-utils-django-1.0.4/project_utils/web/django/view/_rest_view/_base_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 15:11:23.000000 project-utils-django-1.0.4/project_utils/web/django/view/_rest_view/_swagger_base.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 07:27:29.000000 project-utils-django-1.0.4/project_utils/web/django/view/_swagger_base.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      750 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/view/_types.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.178700 project-utils-django-1.0.4/project_utils/web/django/view/_user_view/
--rw-r--r--   0 mylx2014   (501) staff       (20)      185 2023-12-10 07:02:32.000000 project-utils-django-1.0.4/project_utils/web/django/view/_user_view/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      239 2023-12-10 15:11:23.000000 project-utils-django-1.0.4/project_utils/web/django/view/_user_view/_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)    11333 2023-12-10 15:11:23.000000 project-utils-django-1.0.4/project_utils/web/django/view/_user_view/_view.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.178952 project-utils-django-1.0.4/project_utils/web/fastapi/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.4/project_utils/web/fastapi/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.179050 project-utils-django-1.0.4/project_utils/web/flask/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.4/project_utils/web/flask/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:29:50.179785 project-utils-django-1.0.4/project_utils_django.egg-info/
--rw-r--r--   0 mylx2014   (501) staff       (20)     1876 2024-04-17 01:29:50.000000 project-utils-django-1.0.4/project_utils_django.egg-info/PKG-INFO
--rw-r--r--   0 mylx2014   (501) staff       (20)     4854 2024-04-17 01:29:50.000000 project-utils-django-1.0.4/project_utils_django.egg-info/SOURCES.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)        1 2024-04-17 01:29:50.000000 project-utils-django-1.0.4/project_utils_django.egg-info/dependency_links.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)       83 2024-04-17 01:29:50.000000 project-utils-django-1.0.4/project_utils_django.egg-info/requires.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)       14 2024-04-17 01:29:50.000000 project-utils-django-1.0.4/project_utils_django.egg-info/top_level.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)       38 2024-04-17 01:29:50.180409 project-utils-django-1.0.4/setup.cfg
--rw-r--r--   0 mylx2014   (501) staff       (20)      838 2024-04-17 01:29:44.000000 project-utils-django-1.0.4/setup.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.877531 project-utils-django-1.0.5/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 07:03:44.000000 project-utils-django-1.0.5/LICENSE
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1876 2024-04-17 01:41:21.877233 project-utils-django-1.0.5/PKG-INFO
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1289 2023-11-24 01:16:34.000000 project-utils-django-1.0.5/README.md
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.864327 project-utils-django-1.0.5/project_utils/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.5/project_utils/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.864531 project-utils-django-1.0.5/project_utils/collection/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      140 2023-10-14 01:51:03.000000 project-utils-django-1.0.5/project_utils/collection/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      596 2023-10-13 02:35:45.000000 project-utils-django-1.0.5/project_utils/collection/list_util.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.864845 project-utils-django-1.0.5/project_utils/config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 01:51:03.000000 project-utils-django-1.0.5/project_utils/config/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.865449 project-utils-django-1.0.5/project_utils/config/addr_config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      652 2023-10-14 01:51:03.000000 project-utils-django-1.0.5/project_utils/config/addr_config/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      739 2023-11-24 01:16:34.000000 project-utils-django-1.0.5/project_utils/config/addr_config/base_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)       86 2023-10-14 01:51:03.000000 project-utils-django-1.0.5/project_utils/config/addr_config/hbase_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      777 2023-10-14 01:51:03.000000 project-utils-django-1.0.5/project_utils/config/addr_config/kafka_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      695 2023-10-14 01:51:03.000000 project-utils-django-1.0.5/project_utils/config/addr_config/mysql_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      825 2023-11-24 01:16:34.000000 project-utils-django-1.0.5/project_utils/config/addr_config/redis_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1039 2023-10-14 01:51:03.000000 project-utils-django-1.0.5/project_utils/config/base_config.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.865659 project-utils-django-1.0.5/project_utils/config/path_config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 01:51:03.000000 project-utils-django-1.0.5/project_utils/config/path_config/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      970 2023-10-13 02:35:45.000000 project-utils-django-1.0.5/project_utils/config/path_config/path_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1977 2023-10-14 01:51:03.000000 project-utils-django-1.0.5/project_utils/config/template.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.865768 project-utils-django-1.0.5/project_utils/db/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      164 2023-10-14 01:57:29.000000 project-utils-django-1.0.5/project_utils/db/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.866264 project-utils-django-1.0.5/project_utils/db/mysql/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      257 2023-10-14 01:57:29.000000 project-utils-django-1.0.5/project_utils/db/mysql/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3484 2023-11-28 08:48:43.000000 project-utils-django-1.0.5/project_utils/db/mysql/_collection.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2291 2023-12-15 01:39:50.000000 project-utils-django-1.0.5/project_utils/db/mysql/_pool.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      832 2023-11-24 01:16:34.000000 project-utils-django-1.0.5/project_utils/db/mysql/_result.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      107 2023-10-13 02:35:45.000000 project-utils-django-1.0.5/project_utils/db/mysql/_types.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.866671 project-utils-django-1.0.5/project_utils/exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      811 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      148 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/exception/collection_exception.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      144 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/exception/config_exception.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.866870 project-utils-django-1.0.5/project_utils/exception/db_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      141 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/exception/db_exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      118 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/exception/db_exception/mysql_exception.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      507 2023-10-13 02:35:45.000000 project-utils-django-1.0.5/project_utils/exception/my_base_exception.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.866980 project-utils-django-1.0.5/project_utils/exception/web_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/exception/web_exception/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.867211 project-utils-django-1.0.5/project_utils/exception/web_exception/django_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      125 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/exception/web_exception/django_exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      127 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/exception/web_exception/django_exception/model_exception.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.867447 project-utils-django-1.0.5/project_utils/exception/web_exception/django_exception/view_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      275 2023-10-18 02:20:38.000000 project-utils-django-1.0.5/project_utils/exception/web_exception/django_exception/view_exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      120 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/exception/web_exception/django_exception/view_exception/response_exception.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1255 2023-10-13 02:35:45.000000 project-utils-django-1.0.5/project_utils/io.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.867657 project-utils-django-1.0.5/project_utils/os/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       98 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/os/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      760 2023-10-13 02:35:45.000000 project-utils-django-1.0.5/project_utils/os/dir.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2029 2024-01-16 07:43:03.000000 project-utils-django-1.0.5/project_utils/time.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.867760 project-utils-django-1.0.5/project_utils/web/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.5/project_utils/web/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.867838 project-utils-django-1.0.5/project_utils/web/aiohttp/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.5/project_utils/web/aiohttp/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.868019 project-utils-django-1.0.5/project_utils/web/django/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      463 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/web/django/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.868249 project-utils-django-1.0.5/project_utils/web/django/celery/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       84 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/web/django/celery/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.868505 project-utils-django-1.0.5/project_utils/web/django/celery/_conf/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/web/django/celery/_conf/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1061 2023-11-24 01:16:34.000000 project-utils-django-1.0.5/project_utils/web/django/celery/_conf/_celery_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      334 2023-10-18 01:14:46.000000 project-utils-django-1.0.5/project_utils/web/django/celery/create_app.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.868735 project-utils-django-1.0.5/project_utils/web/django/conf/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/web/django/conf/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2145 2023-11-24 01:16:34.000000 project-utils-django-1.0.5/project_utils/web/django/conf/_django_config.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.868974 project-utils-django-1.0.5/project_utils/web/django/middle/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      124 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/web/django/middle/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1161 2023-11-24 01:16:34.000000 project-utils-django-1.0.5/project_utils/web/django/middle/_base_middle.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.869496 project-utils-django-1.0.5/project_utils/web/django/model/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      434 2024-01-15 14:04:29.000000 project-utils-django-1.0.5/project_utils/web/django/model/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      106 2023-12-10 05:49:34.000000 project-utils-django-1.0.5/project_utils/web/django/model/_base_meta.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1511 2024-01-15 14:04:29.000000 project-utils-django-1.0.5/project_utils/web/django/model/_base_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      487 2023-12-08 06:57:16.000000 project-utils-django-1.0.5/project_utils/web/django/model/_id_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      461 2024-01-15 14:04:29.000000 project-utils-django-1.0.5/project_utils/web/django/model/_model_type.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.869713 project-utils-django-1.0.5/project_utils/web/django/pagination/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      197 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/web/django/pagination/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1011 2023-11-24 01:16:34.000000 project-utils-django-1.0.5/project_utils/web/django/pagination/_base_pagination.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.869936 project-utils-django-1.0.5/project_utils/web/django/request/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      102 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/web/django/request/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1379 2023-11-24 01:16:34.000000 project-utils-django-1.0.5/project_utils/web/django/request/_request.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.870270 project-utils-django-1.0.5/project_utils/web/django/response/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      153 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/web/django/response/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1291 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/web/django/response/_response_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      213 2023-11-24 01:16:34.000000 project-utils-django-1.0.5/project_utils/web/django/response/_response_types.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.870825 project-utils-django-1.0.5/project_utils/web/django/serializer/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/web/django/serializer/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      284 2023-10-13 02:35:45.000000 project-utils-django-1.0.5/project_utils/web/django/serializer/_base_meta.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      418 2023-10-14 02:37:02.000000 project-utils-django-1.0.5/project_utils/web/django/serializer/_base_serializer.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.871157 project-utils-django-1.0.5/project_utils/web/django/swagger/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      499 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.872172 project-utils-django-1.0.5/project_utils/web/django/swagger/_params/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      675 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/_params/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/_params/_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1025 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/_params/_form.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1164 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/_params/_params.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      978 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/_params/_query.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2065 2023-12-10 07:17:18.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/_params/_response.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      412 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/_params/_types.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      268 2023-12-10 07:15:26.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/_urls.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.872604 project-utils-django-1.0.5/project_utils/web/django/swagger/config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       69 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/config/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      488 2023-12-10 07:15:01.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/config/_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1274 2023-12-10 07:15:01.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/config/_swagger.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.873012 project-utils-django-1.0.5/project_utils/web/django/swagger/document/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      256 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/document/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1169 2023-12-10 07:15:01.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/document/_document.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      273 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/swagger/document/_types.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      678 2023-11-24 01:16:34.000000 project-utils-django-1.0.5/project_utils/web/django/utils.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.873666 project-utils-django-1.0.5/project_utils/web/django/view/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      478 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/view/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/view/_async_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2086 2023-12-10 15:11:23.000000 project-utils-django-1.0.5/project_utils/web/django/view/_base.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.874078 project-utils-django-1.0.5/project_utils/web/django/view/_base_api/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       57 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/view/_base_api/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3277 2023-12-10 15:07:50.000000 project-utils-django-1.0.5/project_utils/web/django/view/_base_api/api.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      908 2023-12-10 15:07:50.000000 project-utils-django-1.0.5/project_utils/web/django/view/_base_api/api_util.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.874800 project-utils-django-1.0.5/project_utils/web/django/view/_rest_api/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      296 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/view/_rest_api/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1921 2023-12-10 15:07:50.000000 project-utils-django-1.0.5/project_utils/web/django/view/_rest_api/api.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      480 2023-12-10 15:08:55.000000 project-utils-django-1.0.5/project_utils/web/django/view/_rest_api/api_utils.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2020 2023-12-10 15:08:55.000000 project-utils-django-1.0.5/project_utils/web/django/view/_rest_api/async_api.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.875510 project-utils-django-1.0.5/project_utils/web/django/view/_rest_view/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/view/_rest_view/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)    12607 2023-12-10 15:16:37.000000 project-utils-django-1.0.5/project_utils/web/django/view/_rest_view/_async_base_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 15:11:23.000000 project-utils-django-1.0.5/project_utils/web/django/view/_rest_view/_async_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)    12432 2023-12-10 15:11:23.000000 project-utils-django-1.0.5/project_utils/web/django/view/_rest_view/_base_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 15:11:23.000000 project-utils-django-1.0.5/project_utils/web/django/view/_rest_view/_swagger_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 07:27:29.000000 project-utils-django-1.0.5/project_utils/web/django/view/_swagger_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      750 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/view/_types.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.875866 project-utils-django-1.0.5/project_utils/web/django/view/_user_view/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      185 2023-12-10 07:02:32.000000 project-utils-django-1.0.5/project_utils/web/django/view/_user_view/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      239 2023-12-10 15:11:23.000000 project-utils-django-1.0.5/project_utils/web/django/view/_user_view/_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)    11333 2023-12-10 15:11:23.000000 project-utils-django-1.0.5/project_utils/web/django/view/_user_view/_view.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.876000 project-utils-django-1.0.5/project_utils/web/fastapi/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.5/project_utils/web/fastapi/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.876326 project-utils-django-1.0.5/project_utils/web/flask/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.5/project_utils/web/flask/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-17 01:41:21.876961 project-utils-django-1.0.5/project_utils_django.egg-info/
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1876 2024-04-17 01:41:21.000000 project-utils-django-1.0.5/project_utils_django.egg-info/PKG-INFO
+-rw-r--r--   0 mylx2014   (501) staff       (20)     4854 2024-04-17 01:41:21.000000 project-utils-django-1.0.5/project_utils_django.egg-info/SOURCES.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)        1 2024-04-17 01:41:21.000000 project-utils-django-1.0.5/project_utils_django.egg-info/dependency_links.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)       83 2024-04-17 01:41:21.000000 project-utils-django-1.0.5/project_utils_django.egg-info/requires.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)       14 2024-04-17 01:41:21.000000 project-utils-django-1.0.5/project_utils_django.egg-info/top_level.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)       38 2024-04-17 01:41:21.877573 project-utils-django-1.0.5/setup.cfg
+-rw-r--r--   0 mylx2014   (501) staff       (20)      838 2024-04-17 01:41:14.000000 project-utils-django-1.0.5/setup.py
```

### Comparing `project-utils-django-1.0.4/PKG-INFO` & `project-utils-django-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: project-utils-django
-Version: 1.0.4
+Version: 1.0.5
 Summary: python project_utils tools
 Home-page: https://gitee.com/mylx2014/project-utils-django.git
 Author: mylx2014
 Author-email: mylx2014@163.com
 License: MIT
 Keywords: python,utils,project utils,aiofiles
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django<=4.2.9
+Requires-Dist: django==4.2.9
 Requires-Dist: loguru
 Requires-Dist: dbutils
 Requires-Dist: pymysql
 Requires-Dist: djangorestframework
 Requires-Dist: drf-yasg
 Requires-Dist: asyncio
 Requires-Dist: aiofiles
```

### Comparing `project-utils-django-1.0.4/README.md` & `project-utils-django-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/collection/list_util.py` & `project-utils-django-1.0.5/project_utils/collection/list_util.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/config/addr_config/__init__.py` & `project-utils-django-1.0.5/project_utils/config/addr_config/__init__.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/config/addr_config/base_config.py` & `project-utils-django-1.0.5/project_utils/config/addr_config/base_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/config/addr_config/kafka_config.py` & `project-utils-django-1.0.5/project_utils/config/addr_config/kafka_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/config/addr_config/mysql_config.py` & `project-utils-django-1.0.5/project_utils/config/addr_config/mysql_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/config/addr_config/redis_config.py` & `project-utils-django-1.0.5/project_utils/config/addr_config/redis_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/config/base_config.py` & `project-utils-django-1.0.5/project_utils/config/base_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/config/path_config/path_config.py` & `project-utils-django-1.0.5/project_utils/config/path_config/path_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/config/template.py` & `project-utils-django-1.0.5/project_utils/config/template.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/db/mysql/_collection.py` & `project-utils-django-1.0.5/project_utils/db/mysql/_collection.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/db/mysql/_pool.py` & `project-utils-django-1.0.5/project_utils/db/mysql/_pool.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/db/mysql/_result.py` & `project-utils-django-1.0.5/project_utils/db/mysql/_result.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/exception/__init__.py` & `project-utils-django-1.0.5/project_utils/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/io.py` & `project-utils-django-1.0.5/project_utils/io.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/os/dir.py` & `project-utils-django-1.0.5/project_utils/os/dir.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/time.py` & `project-utils-django-1.0.5/project_utils/time.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/celery/_conf/_celery_config.py` & `project-utils-django-1.0.5/project_utils/web/django/celery/_conf/_celery_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/conf/_django_config.py` & `project-utils-django-1.0.5/project_utils/web/django/conf/_django_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/middle/_base_middle.py` & `project-utils-django-1.0.5/project_utils/web/django/middle/_base_middle.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/model/_base_model.py` & `project-utils-django-1.0.5/project_utils/web/django/model/_base_model.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/pagination/_base_pagination.py` & `project-utils-django-1.0.5/project_utils/web/django/pagination/_base_pagination.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/request/_request.py` & `project-utils-django-1.0.5/project_utils/web/django/request/_request.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/response/_response_model.py` & `project-utils-django-1.0.5/project_utils/web/django/response/_response_model.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/swagger/_params/__init__.py` & `project-utils-django-1.0.5/project_utils/web/django/swagger/_params/__init__.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/swagger/_params/_form.py` & `project-utils-django-1.0.5/project_utils/web/django/swagger/_params/_form.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/swagger/_params/_params.py` & `project-utils-django-1.0.5/project_utils/web/django/swagger/_params/_params.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/swagger/_params/_query.py` & `project-utils-django-1.0.5/project_utils/web/django/swagger/_params/_query.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/swagger/_params/_response.py` & `project-utils-django-1.0.5/project_utils/web/django/swagger/_params/_response.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/swagger/config/_swagger.py` & `project-utils-django-1.0.5/project_utils/web/django/swagger/config/_swagger.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/swagger/document/_document.py` & `project-utils-django-1.0.5/project_utils/web/django/swagger/document/_document.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/utils.py` & `project-utils-django-1.0.5/project_utils/web/django/utils.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/view/_async_view.py` & `project-utils-django-1.0.5/project_utils/web/django/view/_async_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/view/_base.py` & `project-utils-django-1.0.5/project_utils/web/django/view/_base.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/view/_base_api/api.py` & `project-utils-django-1.0.5/project_utils/web/django/view/_base_api/api.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/view/_base_api/api_util.py` & `project-utils-django-1.0.5/project_utils/web/django/view/_base_api/api_util.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/view/_rest_api/api.py` & `project-utils-django-1.0.5/project_utils/web/django/view/_rest_api/api.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/view/_rest_api/async_api.py` & `project-utils-django-1.0.5/project_utils/web/django/view/_rest_api/async_api.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/view/_rest_view/_async_base_view.py` & `project-utils-django-1.0.5/project_utils/web/django/view/_rest_view/_async_base_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/view/_rest_view/_async_view.py` & `project-utils-django-1.0.5/project_utils/web/django/view/_rest_view/_async_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/view/_rest_view/_base_view.py` & `project-utils-django-1.0.5/project_utils/web/django/view/_rest_view/_base_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/view/_rest_view/_swagger_base.py` & `project-utils-django-1.0.5/project_utils/web/django/view/_rest_view/_swagger_base.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/view/_swagger_base.py` & `project-utils-django-1.0.5/project_utils/web/django/view/_swagger_base.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/view/_types.py` & `project-utils-django-1.0.5/project_utils/web/django/view/_types.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils/web/django/view/_user_view/_view.py` & `project-utils-django-1.0.5/project_utils/web/django/view/_user_view/_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/project_utils_django.egg-info/PKG-INFO` & `project-utils-django-1.0.5/project_utils_django.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: project-utils-django
-Version: 1.0.4
+Version: 1.0.5
 Summary: python project_utils tools
 Home-page: https://gitee.com/mylx2014/project-utils-django.git
 Author: mylx2014
 Author-email: mylx2014@163.com
 License: MIT
 Keywords: python,utils,project utils,aiofiles
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django<=4.2.9
+Requires-Dist: django==4.2.9
 Requires-Dist: loguru
 Requires-Dist: dbutils
 Requires-Dist: pymysql
 Requires-Dist: djangorestframework
 Requires-Dist: drf-yasg
 Requires-Dist: asyncio
 Requires-Dist: aiofiles
```

### Comparing `project-utils-django-1.0.4/project_utils_django.egg-info/SOURCES.txt` & `project-utils-django-1.0.5/project_utils_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `project-utils-django-1.0.4/setup.py` & `project-utils-django-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.0.4"
+VERSION = "1.0.5"
 DESCRIPTION = "python project_utils tools"
 setup(
     name="project-utils-django",
     version=VERSION,
     author="mylx2014",
     author_email="mylx2014@163.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=open('README.md', encoding="UTF8").read(),
     packages=find_packages(),
     install_requires=[
-        "django<=4.2.9", 'loguru', 'dbutils', 'pymysql', "djangorestframework", "drf-yasg", "asyncio",
+        "django==4.2.9", 'loguru', 'dbutils', 'pymysql', "djangorestframework", "drf-yasg", "asyncio",
                       "aiofiles"],
     keywords=['python', 'utils', 'project utils', "aiofiles"],
     data_files=[],
     entry_points={},
     license="MIT",
     url="https://gitee.com/mylx2014/project-utils-django.git",
     scripts=[],
```

