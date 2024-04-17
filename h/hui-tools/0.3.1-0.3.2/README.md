# Comparing `tmp/hui-tools-0.3.1.tar.gz` & `tmp/hui-tools-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hui-tools-0.3.1.tar", last modified: Thu Mar 28 16:02:11 2024, max compression
+gzip compressed data, was "hui-tools-0.3.2.tar", last modified: Wed Apr 17 04:02:55 2024, max compression
```

## Comparing `hui-tools-0.3.1.tar` & `hui-tools-0.3.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.180499 hui-tools-0.3.1/
--rw-r--r--   0 liuminhui   (501) staff       (20)    11357 2023-07-29 10:14:17.000000 hui-tools-0.3.1/LICENSE
--rw-r--r--   0 liuminhui   (501) staff       (20)    17636 2024-03-28 16:02:11.180194 hui-tools-0.3.1/PKG-INFO
--rw-r--r--   0 liuminhui   (501) staff       (20)    15797 2024-03-28 16:00:11.000000 hui-tools-0.3.1/README.md
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.172219 hui-tools-0.3.1/hui_tools.egg-info/
--rw-r--r--   0 liuminhui   (501) staff       (20)    17636 2024-03-28 16:02:11.000000 hui-tools-0.3.1/hui_tools.egg-info/PKG-INFO
--rw-r--r--   0 liuminhui   (501) staff       (20)     1520 2024-03-28 16:02:11.000000 hui-tools-0.3.1/hui_tools.egg-info/SOURCES.txt
--rw-r--r--   0 liuminhui   (501) staff       (20)        1 2024-03-28 16:02:11.000000 hui-tools-0.3.1/hui_tools.egg-info/dependency_links.txt
--rw-r--r--   0 liuminhui   (501) staff       (20)      532 2024-03-28 16:02:11.000000 hui-tools-0.3.1/hui_tools.egg-info/requires.txt
--rw-r--r--   0 liuminhui   (501) staff       (20)       15 2024-03-28 16:02:11.000000 hui-tools-0.3.1/hui_tools.egg-info/top_level.txt
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.172368 hui-tools-0.3.1/py_tools/
--rw-r--r--   0 liuminhui   (501) staff       (20)        1 2023-09-04 08:25:07.000000 hui-tools-0.3.1/py_tools/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.173002 hui-tools-0.3.1/py_tools/chatbot/
--rw-r--r--   0 liuminhui   (501) staff       (20)      128 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/chatbot/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)    11243 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/chatbot/app_server.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     5238 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/chatbot/chatbot.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     2385 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/chatbot/factory.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.173138 hui-tools-0.3.1/py_tools/connections/
--rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/connections/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.173403 hui-tools-0.3.1/py_tools/connections/db/
--rw-r--r--   0 liuminhui   (501) staff       (20)      182 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/connections/db/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.174120 hui-tools-0.3.1/py_tools/connections/db/mysql/
--rw-r--r--   0 liuminhui   (501) staff       (20)      215 2024-03-28 15:06:17.000000 hui-tools-0.3.1/py_tools/connections/db/mysql/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)    18946 2024-03-28 15:59:27.000000 hui-tools-0.3.1/py_tools/connections/db/mysql/client.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1706 2024-03-28 01:23:21.000000 hui-tools-0.3.1/py_tools/connections/db/mysql/orm_model.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1452 2024-03-28 01:23:21.000000 hui-tools-0.3.1/py_tools/connections/db/redis_client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.174436 hui-tools-0.3.1/py_tools/connections/http/
--rw-r--r--   0 liuminhui   (501) staff       (20)      158 2023-08-10 03:40:34.000000 hui-tools-0.3.1/py_tools/connections/http/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     8809 2023-09-28 06:51:00.000000 hui-tools-0.3.1/py_tools/connections/http/client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.174917 hui-tools-0.3.1/py_tools/connections/mq/
--rw-r--r--   0 liuminhui   (501) staff       (20)      185 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/connections/mq/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      184 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/connections/mq/kafka_client.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      187 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/connections/mq/rabbitmq_client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.175192 hui-tools-0.3.1/py_tools/connections/oss/
--rw-r--r--   0 liuminhui   (501) staff       (20)      173 2024-03-28 01:23:21.000000 hui-tools-0.3.1/py_tools/connections/oss/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1955 2024-03-28 01:23:21.000000 hui-tools-0.3.1/py_tools/connections/oss/minio_client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.175347 hui-tools-0.3.1/py_tools/constants/
--rw-r--r--   0 liuminhui   (501) staff       (20)      171 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/constants/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.175631 hui-tools-0.3.1/py_tools/data_models/
--rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/data_models/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      270 2023-09-09 16:15:14.000000 hui-tools-0.3.1/py_tools/data_models/time.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.176094 hui-tools-0.3.1/py_tools/decorators/
--rw-r--r--   0 liuminhui   (501) staff       (20)      213 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/decorators/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     6380 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/decorators/base.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     4395 2023-09-09 16:15:14.000000 hui-tools-0.3.1/py_tools/decorators/cache.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.177201 hui-tools-0.3.1/py_tools/enums/
--rw-r--r--   0 liuminhui   (501) staff       (20)      334 2023-09-09 16:15:14.000000 hui-tools-0.3.1/py_tools/enums/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1699 2023-09-09 15:54:57.000000 hui-tools-0.3.1/py_tools/enums/base.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1234 2023-09-09 16:15:14.000000 hui-tools-0.3.1/py_tools/enums/error.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/enums/feishu.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      452 2023-09-09 16:15:14.000000 hui-tools-0.3.1/py_tools/enums/http.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      403 2023-09-09 15:58:16.000000 hui-tools-0.3.1/py_tools/enums/pub_biz.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-09-09 06:12:03.000000 hui-tools-0.3.1/py_tools/enums/time.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.177450 hui-tools-0.3.1/py_tools/exceptions/
--rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/exceptions/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1141 2023-09-09 16:15:14.000000 hui-tools-0.3.1/py_tools/exceptions/base.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.177576 hui-tools-0.3.1/py_tools/logging/
--rw-r--r--   0 liuminhui   (501) staff       (20)       26 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/logging/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.177824 hui-tools-0.3.1/py_tools/meta_cls/
--rw-r--r--   0 liuminhui   (501) staff       (20)       35 2023-09-04 07:12:03.000000 hui-tools-0.3.1/py_tools/meta_cls/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      963 2023-09-09 06:35:40.000000 hui-tools-0.3.1/py_tools/meta_cls/base.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.178702 hui-tools-0.3.1/py_tools/utils/
--rw-r--r--   0 liuminhui   (501) staff       (20)      166 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/utils/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/utils/base.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     5992 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/utils/excel.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      182 2023-09-09 16:15:14.000000 hui-tools-0.3.1/py_tools/utils/func.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.3.1/py_tools/utils/mask.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      179 2023-09-09 16:16:35.000000 hui-tools-0.3.1/py_tools/utils/serializer.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     6859 2023-09-09 06:33:24.000000 hui-tools-0.3.1/py_tools/utils/time.py
--rw-r--r--   0 liuminhui   (501) staff       (20)       38 2024-03-28 16:02:11.180547 hui-tools-0.3.1/setup.cfg
--rw-r--r--   0 liuminhui   (501) staff       (20)     2289 2024-03-28 16:00:59.000000 hui-tools-0.3.1/setup.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-03-28 16:02:11.178853 hui-tools-0.3.1/tests/
--rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.3.1/tests/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.911946 hui-tools-0.3.2/
+-rw-r--r--   0 liuminhui   (501) staff       (20)    11357 2023-07-29 10:14:17.000000 hui-tools-0.3.2/LICENSE
+-rw-r--r--   0 liuminhui   (501) staff       (20)    17648 2024-04-17 04:02:55.911662 hui-tools-0.3.2/PKG-INFO
+-rw-r--r--   0 liuminhui   (501) staff       (20)    15809 2024-04-15 11:39:36.000000 hui-tools-0.3.2/README.md
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.899506 hui-tools-0.3.2/hui_tools.egg-info/
+-rw-r--r--   0 liuminhui   (501) staff       (20)    17648 2024-04-17 04:02:55.000000 hui-tools-0.3.2/hui_tools.egg-info/PKG-INFO
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1520 2024-04-17 04:02:55.000000 hui-tools-0.3.2/hui_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)        1 2024-04-17 04:02:55.000000 hui-tools-0.3.2/hui_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)      532 2024-04-17 04:02:55.000000 hui-tools-0.3.2/hui_tools.egg-info/requires.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)       15 2024-04-17 04:02:55.000000 hui-tools-0.3.2/hui_tools.egg-info/top_level.txt
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.899645 hui-tools-0.3.2/py_tools/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        1 2023-09-04 08:25:07.000000 hui-tools-0.3.2/py_tools/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.900761 hui-tools-0.3.2/py_tools/chatbot/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      128 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/chatbot/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)    11243 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/chatbot/app_server.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     5238 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/chatbot/chatbot.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2385 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/chatbot/factory.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.900947 hui-tools-0.3.2/py_tools/connections/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/connections/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.901289 hui-tools-0.3.2/py_tools/connections/db/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      182 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/connections/db/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.902084 hui-tools-0.3.2/py_tools/connections/db/mysql/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      215 2024-03-28 15:06:17.000000 hui-tools-0.3.2/py_tools/connections/db/mysql/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)    20121 2024-04-17 03:58:06.000000 hui-tools-0.3.2/py_tools/connections/db/mysql/client.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1722 2024-04-17 03:58:06.000000 hui-tools-0.3.2/py_tools/connections/db/mysql/orm_model.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1452 2024-03-28 01:23:21.000000 hui-tools-0.3.2/py_tools/connections/db/redis_client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.902784 hui-tools-0.3.2/py_tools/connections/http/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      158 2023-08-10 03:40:34.000000 hui-tools-0.3.2/py_tools/connections/http/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     8809 2023-09-28 06:51:00.000000 hui-tools-0.3.2/py_tools/connections/http/client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.903524 hui-tools-0.3.2/py_tools/connections/mq/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      185 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/connections/mq/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      184 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/connections/mq/kafka_client.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      187 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/connections/mq/rabbitmq_client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.903913 hui-tools-0.3.2/py_tools/connections/oss/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      173 2024-03-28 01:23:21.000000 hui-tools-0.3.2/py_tools/connections/oss/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1955 2024-03-28 01:23:21.000000 hui-tools-0.3.2/py_tools/connections/oss/minio_client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.904133 hui-tools-0.3.2/py_tools/constants/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      171 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/constants/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.904430 hui-tools-0.3.2/py_tools/data_models/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/data_models/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      270 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/data_models/time.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.905002 hui-tools-0.3.2/py_tools/decorators/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      213 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/decorators/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     6380 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/decorators/base.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     4395 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/decorators/cache.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.906771 hui-tools-0.3.2/py_tools/enums/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      334 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/enums/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1699 2023-09-09 15:54:57.000000 hui-tools-0.3.2/py_tools/enums/base.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1234 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/enums/error.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/enums/feishu.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      452 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/enums/http.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      403 2023-09-09 15:58:16.000000 hui-tools-0.3.2/py_tools/enums/pub_biz.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-09-09 06:12:03.000000 hui-tools-0.3.2/py_tools/enums/time.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.907146 hui-tools-0.3.2/py_tools/exceptions/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/exceptions/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1141 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/exceptions/base.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.907367 hui-tools-0.3.2/py_tools/logging/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       26 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/logging/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.907787 hui-tools-0.3.2/py_tools/meta_cls/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       35 2023-09-04 07:12:03.000000 hui-tools-0.3.2/py_tools/meta_cls/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      963 2023-09-09 06:35:40.000000 hui-tools-0.3.2/py_tools/meta_cls/base.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.909807 hui-tools-0.3.2/py_tools/utils/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      166 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/utils/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/utils/base.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     5992 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/utils/excel.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      182 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/utils/func.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/utils/mask.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      179 2023-09-09 16:16:35.000000 hui-tools-0.3.2/py_tools/utils/serializer.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     6859 2023-09-09 06:33:24.000000 hui-tools-0.3.2/py_tools/utils/time.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)       38 2024-04-17 04:02:55.912003 hui-tools-0.3.2/setup.cfg
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2289 2024-04-17 04:02:44.000000 hui-tools-0.3.2/setup.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.910281 hui-tools-0.3.2/tests/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.3.2/tests/__init__.py
```

### Comparing `hui-tools-0.3.1/LICENSE` & `hui-tools-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/PKG-INFO` & `hui-tools-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hui-tools
-Version: 0.3.1
+Version: 0.3.2
 Home-page: https://github.com/HuiDBK/py-tools
 Author: hui
 Author-email: huidbk@163.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -28,26 +28,26 @@
 Requires-Dist: requests==2.31.0; extra == "http-client"
 Provides-Extra: time-tools
 Requires-Dist: python-dateutil==2.8.2; extra == "time-tools"
 Provides-Extra: excel-tools
 Requires-Dist: pandas==1.3.5; extra == "excel-tools"
 Requires-Dist: openpyxl==3.0.10; extra == "excel-tools"
 Provides-Extra: all
-Requires-Dist: httpx==0.24.1; extra == "all"
-Requires-Dist: requests==2.31.0; extra == "all"
-Requires-Dist: minio==7.1.17; extra == "all"
 Requires-Dist: sqlalchemy[asyncio]==2.0.20; extra == "all"
+Requires-Dist: requests==2.31.0; extra == "all"
 Requires-Dist: pydantic<3,>=2.1.1; extra == "all"
-Requires-Dist: aiomysql==0.2.0; extra == "all"
-Requires-Dist: cacheout==0.14.1; extra == "all"
-Requires-Dist: openpyxl==3.0.10; extra == "all"
-Requires-Dist: python-dateutil==2.8.2; extra == "all"
 Requires-Dist: pandas==1.3.5; extra == "all"
-Requires-Dist: loguru<0.8,>=0.7.0; extra == "all"
+Requires-Dist: httpx==0.24.1; extra == "all"
+Requires-Dist: openpyxl==3.0.10; extra == "all"
+Requires-Dist: cacheout==0.14.1; extra == "all"
+Requires-Dist: minio==7.1.17; extra == "all"
 Requires-Dist: redis>=4.5.4; extra == "all"
+Requires-Dist: loguru<0.8,>=0.7.0; extra == "all"
+Requires-Dist: aiomysql==0.2.0; extra == "all"
+Requires-Dist: python-dateutil==2.8.2; extra == "all"
 
 # Py-Tools
 
 > Py-Tools 是一个实用的 Python 工具集和可复用组件库，旨在简化常见任务，提高 Python 项目的开发效率。
 > 
 > 设计细节请移步到掘金查看：https://juejin.cn/column/7131286129713610766
 
@@ -323,18 +323,20 @@
         # 返回影响的记录数
         return cursor_result.rowcount
 ```
 
 
 部分使用demo，详情请到 demo/connections/sqlalchemy_demo/demo.py 文件查阅
 ```python
+import uuid
+
 async def create_and_transaction_demo():
     async with UserFileManager.transaction() as session:
-        await UserFileManager().bulk_insert(
-            add_rows=[{"filename": "aaa", "oss_key": uuid.uuid4().hex}], session=session
+        await UserFileManager().bulk_add(
+            table_objs=[{"filename": "aaa", "oss_key": uuid.uuid4().hex}], session=session
         )
         user_file_obj = UserFileTable(filename="eee", oss_key=uuid.uuid4().hex)
         file_id = await UserFileManager().add(table_obj=user_file_obj, session=session)
         print("file_id", file_id)
 
         ret: UserFileTable = await UserFileManager().query_by_id(2, session=session)
         print("query_by_id", ret)
```

### Comparing `hui-tools-0.3.1/README.md` & `hui-tools-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -276,18 +276,20 @@
         # 返回影响的记录数
         return cursor_result.rowcount
 ```
 
 
 部分使用demo，详情请到 demo/connections/sqlalchemy_demo/demo.py 文件查阅
 ```python
+import uuid
+
 async def create_and_transaction_demo():
     async with UserFileManager.transaction() as session:
-        await UserFileManager().bulk_insert(
-            add_rows=[{"filename": "aaa", "oss_key": uuid.uuid4().hex}], session=session
+        await UserFileManager().bulk_add(
+            table_objs=[{"filename": "aaa", "oss_key": uuid.uuid4().hex}], session=session
         )
         user_file_obj = UserFileTable(filename="eee", oss_key=uuid.uuid4().hex)
         file_id = await UserFileManager().add(table_obj=user_file_obj, session=session)
         print("file_id", file_id)
 
         ret: UserFileTable = await UserFileManager().query_by_id(2, session=session)
         print("query_by_id", ret)
```

### Comparing `hui-tools-0.3.1/hui_tools.egg-info/PKG-INFO` & `hui-tools-0.3.2/hui_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hui-tools
-Version: 0.3.1
+Version: 0.3.2
 Home-page: https://github.com/HuiDBK/py-tools
 Author: hui
 Author-email: huidbk@163.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -28,26 +28,26 @@
 Requires-Dist: requests==2.31.0; extra == "http-client"
 Provides-Extra: time-tools
 Requires-Dist: python-dateutil==2.8.2; extra == "time-tools"
 Provides-Extra: excel-tools
 Requires-Dist: pandas==1.3.5; extra == "excel-tools"
 Requires-Dist: openpyxl==3.0.10; extra == "excel-tools"
 Provides-Extra: all
-Requires-Dist: httpx==0.24.1; extra == "all"
-Requires-Dist: requests==2.31.0; extra == "all"
-Requires-Dist: minio==7.1.17; extra == "all"
 Requires-Dist: sqlalchemy[asyncio]==2.0.20; extra == "all"
+Requires-Dist: requests==2.31.0; extra == "all"
 Requires-Dist: pydantic<3,>=2.1.1; extra == "all"
-Requires-Dist: aiomysql==0.2.0; extra == "all"
-Requires-Dist: cacheout==0.14.1; extra == "all"
-Requires-Dist: openpyxl==3.0.10; extra == "all"
-Requires-Dist: python-dateutil==2.8.2; extra == "all"
 Requires-Dist: pandas==1.3.5; extra == "all"
-Requires-Dist: loguru<0.8,>=0.7.0; extra == "all"
+Requires-Dist: httpx==0.24.1; extra == "all"
+Requires-Dist: openpyxl==3.0.10; extra == "all"
+Requires-Dist: cacheout==0.14.1; extra == "all"
+Requires-Dist: minio==7.1.17; extra == "all"
 Requires-Dist: redis>=4.5.4; extra == "all"
+Requires-Dist: loguru<0.8,>=0.7.0; extra == "all"
+Requires-Dist: aiomysql==0.2.0; extra == "all"
+Requires-Dist: python-dateutil==2.8.2; extra == "all"
 
 # Py-Tools
 
 > Py-Tools 是一个实用的 Python 工具集和可复用组件库，旨在简化常见任务，提高 Python 项目的开发效率。
 > 
 > 设计细节请移步到掘金查看：https://juejin.cn/column/7131286129713610766
 
@@ -323,18 +323,20 @@
         # 返回影响的记录数
         return cursor_result.rowcount
 ```
 
 
 部分使用demo，详情请到 demo/connections/sqlalchemy_demo/demo.py 文件查阅
 ```python
+import uuid
+
 async def create_and_transaction_demo():
     async with UserFileManager.transaction() as session:
-        await UserFileManager().bulk_insert(
-            add_rows=[{"filename": "aaa", "oss_key": uuid.uuid4().hex}], session=session
+        await UserFileManager().bulk_add(
+            table_objs=[{"filename": "aaa", "oss_key": uuid.uuid4().hex}], session=session
         )
         user_file_obj = UserFileTable(filename="eee", oss_key=uuid.uuid4().hex)
         file_id = await UserFileManager().add(table_obj=user_file_obj, session=session)
         print("file_id", file_id)
 
         ret: UserFileTable = await UserFileManager().query_by_id(2, session=session)
         print("query_by_id", ret)
```

### Comparing `hui-tools-0.3.1/hui_tools.egg-info/SOURCES.txt` & `hui-tools-0.3.2/hui_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/hui_tools.egg-info/requires.txt` & `hui-tools-0.3.2/hui_tools.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 loguru<0.8,>=0.7.0
 pydantic<3,>=2.1.1
 
 [all]
-httpx==0.24.1
-requests==2.31.0
-minio==7.1.17
 sqlalchemy[asyncio]==2.0.20
+requests==2.31.0
 pydantic<3,>=2.1.1
-aiomysql==0.2.0
-cacheout==0.14.1
-openpyxl==3.0.10
-python-dateutil==2.8.2
 pandas==1.3.5
-loguru<0.8,>=0.7.0
+httpx==0.24.1
+openpyxl==3.0.10
+cacheout==0.14.1
+minio==7.1.17
 redis>=4.5.4
+loguru<0.8,>=0.7.0
+aiomysql==0.2.0
+python-dateutil==2.8.2
 
 [chatbot]
 requests==2.31.0
 cacheout==0.14.1
 
 [db-orm]
 sqlalchemy[asyncio]==2.0.20
```

### Comparing `hui-tools-0.3.1/py_tools/chatbot/app_server.py` & `hui-tools-0.3.2/py_tools/chatbot/app_server.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/chatbot/chatbot.py` & `hui-tools-0.3.2/py_tools/chatbot/chatbot.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/chatbot/factory.py` & `hui-tools-0.3.2/py_tools/chatbot/factory.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/connections/db/mysql/client.py` & `hui-tools-0.3.2/py_tools/connections/db/mysql/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 # @Desc: { 数据库连接客户端模块 }
 # @Date: 2023/08/17 23:57
 import asyncio
 import functools
 import logging
 from contextlib import asynccontextmanager
 from datetime import datetime
-from typing import Type, Any, Union, List, TypeVar
+from typing import Any, AsyncIterator, List, Type, TypeVar, Union
+
 from loguru import logger
-from sqlalchemy import update, delete, insert, text, select, func, column, Result
+from sqlalchemy import Result, column, delete, func, select, text, update
+from sqlalchemy.ext.asyncio import AsyncConnection, AsyncEngine, AsyncSession, async_sessionmaker, create_async_engine
 
 from py_tools.connections.db.mysql import BaseOrmTable
 from py_tools.meta_cls import SingletonMetaCls
-from sqlalchemy.ext.asyncio import create_async_engine, async_sessionmaker, AsyncEngine, AsyncSession
 
-T_BaseOrmTable = TypeVar('T_BaseOrmTable', bound=BaseOrmTable)
+T_BaseOrmTable = TypeVar("T_BaseOrmTable", bound=BaseOrmTable)
 T_Hints = TypeVar("T_Hints")  # 用于修复被装饰的函数参数提示，让IDE有类型提示
 
 
 def with_session(method) -> T_Hints:
     """
     兼容事务
     Args:
@@ -45,24 +46,24 @@
     return wrapper
 
 
 class SQLAlchemyManager(metaclass=SingletonMetaCls):
     DB_URL_TEMPLATE = "{protocol}://{user}:{password}@{host}:{port}/{db}"
 
     def __init__(
-            self,
-            host: str = "localhost",
-            port: int = 3306,
-            user: str = "",
-            password: str = "",
-            db_name: str = "",
-            pool_size: int = 30,
-            pool_pre_ping: bool = True,
-            pool_recycle: int = 600,
-            log: Union[logging.Logger] = None
+        self,
+        host: str = "localhost",
+        port: int = 3306,
+        user: str = "",
+        password: str = "",
+        db_name: str = "",
+        pool_size: int = 30,
+        pool_pre_ping: bool = True,
+        pool_recycle: int = 600,
+        log: Union[logging.Logger] = None,
     ):
         self.host = host
         self.port = port
         self.user = user
         self.password = password
         self.db_name = db_name
         self.pool_size = pool_size
@@ -71,43 +72,46 @@
         self.log = log or logger
 
         self.db_engine: AsyncEngine = None
         self.async_session_maker: async_sessionmaker = None
 
     def get_db_url(self, protocol: str = "mysql+aiomysql"):
         db_url = self.DB_URL_TEMPLATE.format(
-            protocol=protocol,
-            user=self.user,
-            password=self.password,
-            host=self.host,
-            port=self.port,
-            db=self.db_name
+            protocol=protocol, user=self.user, password=self.password, host=self.host, port=self.port, db=self.db_name
         )
         return db_url
 
-    def init_mysql_engine(self, protocol: str = "mysql+aiomysql"):
+    def init_db_engine(self, protocol: str):
         """
-        初始化mysql引擎
+        初始化db引擎
         Args:
             protocol: 驱动协议类型
 
         Returns:
             self.db_engine
         """
         db_url = self.get_db_url(protocol=protocol)
-        self.log.info(f"init_mysql_engine => {db_url}")
+        self.log.info(f"init_db_engine => {db_url}")
         self.db_engine = create_async_engine(
-            url=db_url,
-            pool_size=self.pool_size,
-            pool_pre_ping=self.pool_pre_ping,
-            pool_recycle=self.pool_recycle
+            url=db_url, pool_size=self.pool_size, pool_pre_ping=self.pool_pre_ping, pool_recycle=self.pool_recycle
         )
         self.async_session_maker = async_sessionmaker(bind=self.db_engine, expire_on_commit=False)
         return self.db_engine
 
+    def init_mysql_engine(self, protocol: str = "mysql+aiomysql"):
+        """
+        初始化mysql引擎
+        Args:
+            protocol: 驱动协议类型
+
+        Returns:
+            self.db_engine
+        """
+        return self.init_db_engine(protocol=protocol)
+
 
 class DBManager(metaclass=SingletonMetaCls):
     DB_CLIENT: SQLAlchemyManager = None
     orm_table: Type[BaseOrmTable] = None
 
     @classmethod
     def init_db_client(cls, db_client: SQLAlchemyManager):
@@ -117,23 +121,31 @@
     @classmethod
     @asynccontextmanager
     async def transaction(cls):
         """事务上下文管理器"""
         async with cls.DB_CLIENT.async_session_maker.begin() as session:
             yield session
 
+    @classmethod
+    @asynccontextmanager
+    async def connection(cls) -> AsyncIterator[AsyncConnection]:
+        """数据库引擎连接上下文管理器"""
+        async with cls.DB_CLIENT.db_engine.begin() as conn:
+            yield conn
+
     @with_session
     async def bulk_delete_by_ids(
-            self,
-            pk_ids: list,
-            orm_table: Type[BaseOrmTable] = None,
-            logic_del: bool = False,
-            logic_field: str = "deleted_at",
-            logic_del_set_value: Any = None,
-            session: AsyncSession = None
+        self,
+        pk_ids: list,
+        *,
+        orm_table: Type[BaseOrmTable] = None,
+        logic_del: bool = False,
+        logic_field: str = "deleted_at",
+        logic_del_set_value: Any = None,
+        session: AsyncSession = None,
     ):
         """
         根据主键id批量删除
         Args:
             pk_ids: 主键id列表
             orm_table: orm表映射类
             logic_del: 逻辑删除，默认 False 物理删除 True 逻辑删除
@@ -147,26 +159,27 @@
         conds = [orm_table.id.in_(pk_ids)]
         return await self.delete(
             conds=conds,
             orm_table=orm_table,
             logic_del=logic_del,
             logic_field=logic_field,
             logic_del_set_value=logic_del_set_value,
-            session=session
+            session=session,
         )
 
     @with_session
     async def delete_by_id(
-            self,
-            pk_id: int,
-            orm_table: Type[BaseOrmTable] = None,
-            logic_del: bool = False,
-            logic_field: str = "deleted_at",
-            logic_del_set_value: Any = None,
-            session: AsyncSession = None
+        self,
+        pk_id: int,
+        *,
+        orm_table: Type[BaseOrmTable] = None,
+        logic_del: bool = False,
+        logic_field: str = "deleted_at",
+        logic_del_set_value: Any = None,
+        session: AsyncSession = None,
     ):
         """
         根据主键id删除
         Args:
             pk_id: 主键id
             orm_table: orm表映射类
             logic_del: 逻辑删除，默认 False 物理删除 True 逻辑删除
@@ -180,31 +193,32 @@
         conds = [orm_table.id == pk_id]
         return await self.delete(
             conds=conds,
             orm_table=orm_table,
             logic_del=logic_del,
             logic_field=logic_field,
             logic_del_set_value=logic_del_set_value,
-            session=session
+            session=session,
         )
 
     @with_session
     async def delete(
-            self,
-            conds: list = None,
-            orm_table: Type[BaseOrmTable] = None,
-            logic_del: bool = False,
-            logic_field: str = "deleted_at",
-            logic_del_set_value: Any = None,
-            session: AsyncSession = None,
+        self,
+        *,
+        conds: list = None,
+        orm_table: Type[BaseOrmTable] = None,
+        logic_del: bool = False,
+        logic_field: str = "deleted_at",
+        logic_del_set_value: Any = None,
+        session: AsyncSession = None,
     ):
         """
         通用删除
         Args:
-            conds: 条件列表, eg. [UserTable.id == 1]
+            conds: 条件列表, e.g. [UserTable.id == 1]
             orm_table: orm表映射类
             logic_del: 逻辑删除，默认 False 物理删除 True 逻辑删除
             logic_field: 逻辑删除字段 默认 deleted_at
             logic_del_set_value: 逻辑删除字段设置的值
             session: 数据库会话对象，如果为 None，则通过装饰器在方法内部开启新的事务
 
         Returns: 删除的记录数
@@ -222,69 +236,74 @@
 
         cursor_result = await session.execute(delete_stmt)
 
         # 返回影响的记录数
         return cursor_result.rowcount
 
     @with_session
-    async def bulk_insert(
-            self,
-            add_rows: List[dict],
-            orm_table: Type[BaseOrmTable] = None,
-            session: AsyncSession = None,
-    ) -> Union[int, Any]:
+    async def bulk_add(
+        self,
+        table_objs: List[Union[T_BaseOrmTable, dict]],
+        *,
+        orm_table: Type[BaseOrmTable] = None,
+        flush: bool = False,
+        session: AsyncSession = None,
+    ) -> List[T_BaseOrmTable]:
         """
         批量插入
         Args:
+            table_objs: orm映射类实例列表
+                e.g. [UserTable(username="hui", age=18), ...] or [{"username": "hui", "age": 18}, ...]
             orm_table: orm表映射类
-            add_rows: 批量添加的数据集, eg. [{"username": "hui", "age": 18}, ...]
+            flush: 刷新对象状态，默认不刷新
             session: 数据库会话对象，如果为 None，则通过装饰器在方法内部开启新的事务
 
         Returns:
-            成功插入的影响行数
+            成功插入的对象列表
         """
         orm_table = orm_table or self.orm_table
-        sql = insert(orm_table).values(add_rows)
-        result = await session.execute(sql)
-        return result.rowcount
+        if all(isinstance(table_obj, dict) for table_obj in table_objs):
+            # 字典列表转成orm映射类实例列表处理
+            table_objs = [orm_table(**table_obj) for table_obj in table_objs]
 
-    @with_session
-    async def bulk_add(self, table_objs: List[T_BaseOrmTable], session: AsyncSession = None) -> int:
-        """
-        批量插入
-        Args:
-            table_objs: orm映射类实例列表, eg. [UserTable(username="hui", age=18), ...]
-            session: 数据库会话对象，如果为 None，则通过装饰器在方法内部开启新的事务
-
-        Returns:
-            成功插入的影响行数
-        """
         session.add_all(table_objs)
-        return len(table_objs)
+        if flush:
+            await session.flush(table_objs)
+
+        return table_objs
 
     @with_session
-    async def add(self, table_obj: T_BaseOrmTable, session: AsyncSession = None) -> int:
+    async def add(
+        self, table_obj: [T_BaseOrmTable, dict], *, orm_table: Type[BaseOrmTable] = None, session: AsyncSession = None
+    ) -> int:
         """
         插入一条数据
         Args:
-            table_obj: orm映射类实例对象, eg. UserTable(username="hui", age=18)
+            table_obj: orm映射类实例对象, eg. UserTable(username="hui", age=18) or {"username": "hui", "age": 18}
+            orm_table: orm表映射类
             session: 数据库会话对象，如果为 None，则通过装饰器在方法内部开启新的事务
 
         Returns: 新增的id
             table_obj.id
         """
+        orm_table = orm_table or self.orm_table
+        if isinstance(table_obj, dict):
+            table_obj = orm_table(**table_obj)
+
         session.add(table_obj)
+        await session.flush(objects=[table_obj])  # 刷新对象状态，获取新增的id
         return table_obj.id
 
     @with_session
     async def query_by_id(
-            self,
-            pk_id: int,
-            orm_table: Type[BaseOrmTable] = None,
-            session: AsyncSession = None,
+        self,
+        pk_id: int,
+        *,
+        orm_table: Type[BaseOrmTable] = None,
+        session: AsyncSession = None,
     ) -> Union[T_BaseOrmTable, None]:
         """
         根据主键id查询
         Args:
             pk_id: 主键id
             orm_table: orm表映射类
             session: 数据库会话对象，如果为 None，则通过装饰器在方法内部开启新的事务
@@ -294,22 +313,23 @@
         """
         orm_table = orm_table or self.orm_table
         ret = await session.get(orm_table, pk_id)
         return ret
 
     @with_session
     async def _query(
-            self,
-            cols: list = None,
-            orm_table: BaseOrmTable = None,
-            conds: list = None,
-            orders: list = None,
-            limit: int = None,
-            offset: int = 0,
-            session: AsyncSession = None,
+        self,
+        *,
+        cols: list = None,
+        orm_table: BaseOrmTable = None,
+        conds: list = None,
+        orders: list = None,
+        limit: int = None,
+        offset: int = 0,
+        session: AsyncSession = None,
     ) -> Result[Any]:
         """
         通用查询
         Args:
             cols: 查询的列表字段
             orm_table: orm表映射类
             conds: 查询的条件列表
@@ -341,33 +361,34 @@
 
         # 执行查询
         cursor_result = await session.execute(query_sql)
         return cursor_result
 
     @with_session
     async def query_one(
-            self,
-            cols: list = None,
-            orm_table: Type[BaseOrmTable] = None,
-            conds: list = None,
-            orders: list = None,
-            flat: bool = False,
-            session: AsyncSession = None,
+        self,
+        *,
+        cols: list = None,
+        orm_table: Type[BaseOrmTable] = None,
+        conds: list = None,
+        orders: list = None,
+        flat: bool = False,
+        session: AsyncSession = None,
     ) -> Union[dict, T_BaseOrmTable, Any]:
         """
         查询单行
         Args:
             cols: 查询的列表字段
             orm_table: orm表映射类
             conds: 查询的条件列表
             orders: 排序列表
             flat: 单字段时扁平化处理
             session: 数据库会话对象，如果为 None，则通过装饰器在方法内部开启新的事务
 
-        Notes:
+        Examples:
             # 指定列名
             ret = await UserManager().query_one(cols=["username", "age"], conds=[UserTable.id == 1])
             sql => select username, age from user where id=1
             ret => {"username": "hui", "age": 18}
 
             # 指定列名，单字段扁平化处理
             ret = await UserManager().query_one(cols=["username"], conds=[UserTable.id == 1])
@@ -400,23 +421,24 @@
         else:
             # 未指定列名查询默认全部字段，返回的是表实例对象 BaseOrmTable()
             # eg: select id, username, age from user where id=1 => UserTable(id=1, username="hui", age=18)
             return cursor_result.scalar_one()
 
     @with_session
     async def query_all(
-            self,
-            cols: list = None,
-            orm_table: BaseOrmTable = None,
-            conds: list = None,
-            orders: list = None,
-            flat: bool = False,
-            limit: int = None,
-            offset: int = None,
-            session: AsyncSession = None,
+        self,
+        *,
+        cols: list = None,
+        orm_table: BaseOrmTable = None,
+        conds: list = None,
+        orders: list = None,
+        flat: bool = False,
+        limit: int = None,
+        offset: int = None,
+        session: AsyncSession = None,
     ) -> Union[List[dict], List[T_BaseOrmTable], Any]:
         """
         查询多行
         Args:
             cols: 查询的列表字段
             orm_table: orm表映射类
             conds: 查询的条件列表
@@ -440,22 +462,22 @@
         else:
             # 未指定列名查询默认全部字段，返回的是表实例对象 [BaseOrmTable()]
             # eg: select id, username, age from user
             # [User(id=1, username="hui", age=18), User(id=2, username="dbk", age=18)
             return cursor_result.scalars().all()
 
     async def list_page(
-            self,
-            cols: list = None,
-            orm_table: BaseOrmTable = None,
-            conds: list = None,
-            orders: list = None,
-            curr_page: int = 1,
-            page_size: int = 20,
-            session: AsyncSession = None,
+        self,
+        cols: list = None,
+        orm_table: BaseOrmTable = None,
+        conds: list = None,
+        orders: list = None,
+        curr_page: int = 1,
+        page_size: int = 20,
+        session: AsyncSession = None,
     ):
         """
         单表通用分页查询
         Args:
             cols: 查询的列表字段
             orm_table: orm表映射类
             conds: 查询的条件列表
@@ -469,31 +491,29 @@
         conds = conds or []
         orders = orders or [column("id")]
         orm_table = orm_table or self.orm_table
 
         limit = page_size
         offset = (curr_page - 1) * page_size
         total_count, data_list = await asyncio.gather(
-            self.query_one(
-                cols=[func.count()], orm_table=orm_table, conds=conds, orders=orders, flat=True, session=session
-            ),
+            self.query_one(cols=[func.count()], orm_table=orm_table, conds=conds, orders=orders, flat=True, session=session),
             self.query_all(
                 cols=cols, orm_table=orm_table, conds=conds, orders=orders, limit=limit, offset=offset, session=session
             ),
         )
 
         return total_count, data_list
 
     @with_session
     async def update(
-            self,
-            values: dict,
-            orm_table: Type[BaseOrmTable] = None,
-            conds: list = None,
-            session: AsyncSession = None,
+        self,
+        values: dict,
+        orm_table: Type[BaseOrmTable] = None,
+        conds: list = None,
+        session: AsyncSession = None,
     ):
         """
         更新数据
         Args:
             values: 要更新的字段和对应的值，字典格式，例如 {"field1": value1, "field2": value2, ...}
             orm_table: ORM表映射类
             conds: 更新条件列表，每个条件为一个表达式，例如 [UserTable.username == "hui", ...]
@@ -508,20 +528,41 @@
         if not values:
             return
         sql = update(orm_table).where(*conds).values(**values)
         cursor_result = await session.execute(sql)
         return cursor_result.rowcount
 
     @with_session
+    async def update_or_add(
+        self,
+        table_obj: [T_BaseOrmTable, dict],
+        *,
+        orm_table: Type[BaseOrmTable] = None,
+        session: AsyncSession = None,
+        **kwargs,
+    ):
+        """
+        指定对象更新or添加数据
+        Args:
+            table_obj: 映射类实例对象 or dict，
+                e.g. UserTable(username="hui", age=18) or {"username": "hui", "v": 18, ...}
+            orm_table: ORM表映射类
+            session: 数据库会话对象，如果为 None，则在方法内部开启新的事务
+
+        Returns:
+        """
+        orm_table = orm_table or self.orm_table
+        if isinstance(table_obj, dict):
+            table_obj = orm_table(**table_obj)
+
+        return await session.merge(table_obj, **kwargs)
+
+    @with_session
     async def run_sql(
-            self,
-            sql: str,
-            params: dict = None,
-            query_one: bool = False,
-            session: AsyncSession = None
+        self, sql: str, *, params: dict = None, query_one: bool = False, session: AsyncSession = None
     ) -> Union[dict, List[dict]]:
         """
         执行并提交单条sql
         Args:
             sql: sql语句
             params: sql参数, eg. {":id_val": 10, ":name_val": "hui"}
             query_one: 是否查询单条，默认False查询多条
```

### Comparing `hui-tools-0.3.1/py_tools/connections/db/mysql/orm_model.py` & `hui-tools-0.3.2/py_tools/connections/db/mysql/orm_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 # @Author: Hui
 # @Desc: { 模块描述 }
 # @Date: 2023/08/17 23:55
 from datetime import datetime
-from sqlalchemy import func
+
 from sqlalchemy.ext.asyncio import AsyncAttrs
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column
 
 
 class BaseOrmTable(AsyncAttrs, DeclarativeBase):
     """SQLAlchemy Base ORM Model"""
 
     __abstract__ = True
 
     id: Mapped[int] = mapped_column(primary_key=True, comment="主键ID")
 
+    def __repr__(self):
+        return str(self.to_dict())
+
     def to_dict(self, alias_dict: dict = None, exclude_none=True) -> dict:
         """
         数据库模型转成字典
         Args:
             alias_dict: 字段别名字典
                 eg: {"id": "user_id"}, 把id名称替换成 user_id
             exclude_none: 默认排查None值
         Returns: dict
         """
         alias_dict = alias_dict or {}
         if exclude_none:
             return {
                 alias_dict.get(c.name, c.name): getattr(self, c.name)
-                for c in self.__table__.columns if getattr(self, c.name) is not None
-            }
-        else:
-            return {
-                alias_dict.get(c.name, c.name): getattr(self, c.name, None)
                 for c in self.__table__.columns
+                if getattr(self, c.name) is not None
             }
+        else:
+            return {alias_dict.get(c.name, c.name): getattr(self, c.name, None) for c in self.__table__.columns}
 
 
 class TimestampColumns(AsyncAttrs, DeclarativeBase):
     """时间戳相关列"""
+
     __abstract__ = True
 
-    created_at: Mapped[datetime] = mapped_column(default=func.now, comment="创建时间")
+    created_at: Mapped[datetime] = mapped_column(default=datetime.now, comment="创建时间")
 
-    updated_at: Mapped[datetime] = mapped_column(default=func.now, onupdate=func.now, comment="更新时间")
+    updated_at: Mapped[datetime] = mapped_column(default=datetime.now, onupdate=datetime.now, comment="更新时间")
 
     deleted_at: Mapped[datetime] = mapped_column(nullable=True, comment="删除时间")
 
 
 class BaseOrmTableWithTS(BaseOrmTable, TimestampColumns):
     __abstract__ = True
```

### Comparing `hui-tools-0.3.1/py_tools/connections/db/redis_client.py` & `hui-tools-0.3.2/py_tools/connections/db/redis_client.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/connections/http/client.py` & `hui-tools-0.3.2/py_tools/connections/http/client.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/connections/oss/minio_client.py` & `hui-tools-0.3.2/py_tools/connections/oss/minio_client.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/decorators/base.py` & `hui-tools-0.3.2/py_tools/decorators/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/decorators/cache.py` & `hui-tools-0.3.2/py_tools/decorators/cache.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/enums/base.py` & `hui-tools-0.3.2/py_tools/enums/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/enums/error.py` & `hui-tools-0.3.2/py_tools/enums/error.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/enums/feishu.py` & `hui-tools-0.3.2/py_tools/enums/feishu.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/enums/time.py` & `hui-tools-0.3.2/py_tools/enums/time.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/exceptions/base.py` & `hui-tools-0.3.2/py_tools/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/meta_cls/base.py` & `hui-tools-0.3.2/py_tools/meta_cls/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/utils/excel.py` & `hui-tools-0.3.2/py_tools/utils/excel.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/py_tools/utils/time.py` & `hui-tools-0.3.2/py_tools/utils/time.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.1/setup.py` & `hui-tools-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from functools import reduce
 
 from setuptools import find_packages, setup
 
 
 class PKGManager:
     name = "hui-tools"
-    version = "0.3.1"
+    version = "0.3.2"
     author = "hui"
     author_email = "huidbk@163.com"
 
     @classmethod
     def get_pkg_desc(cls):
         """获取包描述"""
         with open("README.md", "r") as f:
```

