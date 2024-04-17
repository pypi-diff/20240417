# Comparing `tmp/hao-3.8.6.tar.gz` & `tmp/hao-3.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hao-3.8.6.tar", last modified: Fri Mar 22 11:18:14 2024, max compression
+gzip compressed data, was "hao-3.8.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hao-3.8.6.tar` & `hao-3.8.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11357 2020-08-14 05:40:38.118171 hao-3.8.6/LICENSE
--rw-r--r--   0        0        0     4550 2024-01-24 03:43:53.608275 hao-3.8.6/README.md
--rw-r--r--   0        0        0      371 2024-03-20 10:43:38.957886 hao-3.8.6/hao/__init__.py
--rw-r--r--   0        0        0     5202 2024-02-08 23:32:22.070927 hao-3.8.6/hao/arango.py
--rw-r--r--   0        0        0     1752 2024-03-21 02:42:14.902996 hao-3.8.6/hao/args.py
--rw-r--r--   0        0        0      456 2021-10-13 03:48:38.248130 hao-3.8.6/hao/asyncs.py
--rw-r--r--   0        0        0     4287 2023-12-12 10:48:58.766747 hao-3.8.6/hao/charsets.py
--rw-r--r--   0        0        0     1886 2024-01-04 06:05:25.811022 hao-3.8.6/hao/cli.py
--rw-r--r--   0        0        0     5539 2024-01-22 09:11:37.678170 hao-3.8.6/hao/config.py
--rw-r--r--   0        0        0     1465 2021-10-13 03:48:38.248130 hao-3.8.6/hao/currencies.py
--rw-r--r--   0        0        0     9092 2024-03-21 01:47:17.438178 hao-3.8.6/hao/dates.py
--rw-r--r--   0        0        0     2450 2023-12-07 02:22:50.584468 hao-3.8.6/hao/db.py
--rw-r--r--   0        0        0     5452 2023-11-21 08:14:53.909683 hao-3.8.6/hao/decorators.py
--rw-r--r--   0        0        0     1513 2023-06-13 10:11:01.543543 hao-3.8.6/hao/dicts.py
--rw-r--r--   0        0        0    55769 2021-10-13 03:48:38.248130 hao-3.8.6/hao/english.py
--rw-r--r--   0        0        0      662 2023-03-27 03:43:21.995697 hao-3.8.6/hao/enums.py
--rw-r--r--   0        0        0     2067 2024-01-19 03:23:22.550873 hao-3.8.6/hao/envs.py
--rw-r--r--   0        0        0    11192 2023-12-07 02:22:50.584468 hao-3.8.6/hao/es.py
--rw-r--r--   0        0        0      190 2021-10-13 03:48:38.248130 hao-3.8.6/hao/exceptions.py
--rw-r--r--   0        0        0      775 2024-03-07 06:56:26.246672 hao-3.8.6/hao/exits.py
--rw-r--r--   0        0        0     3289 2023-04-04 08:33:34.689439 hao-3.8.6/hao/files.py
--rw-r--r--   0        0        0     3557 2024-01-04 07:46:49.520797 hao-3.8.6/hao/hf.py
--rw-r--r--   0        0        0      379 2023-06-29 02:10:36.407201 hao-3.8.6/hao/invoker.py
--rw-r--r--   0        0        0     1782 2023-06-13 10:11:01.543543 hao-3.8.6/hao/jsons.py
--rw-r--r--   0        0        0     4611 2023-12-07 02:22:50.584468 hao-3.8.6/hao/kafka.py
--rw-r--r--   0        0        0     3719 2023-03-27 03:43:21.995697 hao-3.8.6/hao/lists.py
--rw-r--r--   0        0        0     9040 2024-03-20 10:39:59.305419 hao-3.8.6/hao/logs.py
--rw-r--r--   0        0        0     3893 2024-02-09 02:44:21.683818 hao-3.8.6/hao/meters.py
--rw-r--r--   0        0        0     1278 2023-04-25 17:21:24.642589 hao-3.8.6/hao/modules.py
--rw-r--r--   0        0        0     9237 2023-12-07 02:22:50.584468 hao-3.8.6/hao/mongo.py
--rw-r--r--   0        0        0     5466 2023-12-10 10:09:20.530845 hao-3.8.6/hao/mysql.py
--rw-r--r--   0        0        0    10862 2024-03-06 10:18:35.715088 hao-3.8.6/hao/namespaces.py
--rw-r--r--   0        0        0     9785 2021-10-13 03:48:38.248130 hao-3.8.6/hao/nations.py
--rw-r--r--   0        0        0      295 2021-10-13 03:48:38.248130 hao-3.8.6/hao/networks.py
--rw-r--r--   0        0        0    14779 2023-04-04 08:18:53.973078 hao-3.8.6/hao/oss.py
--rw-r--r--   0        0        0     3713 2024-03-06 06:20:59.128480 hao-3.8.6/hao/paths.py
--rw-r--r--   0        0        0     5238 2024-02-14 01:02:50.223767 hao-3.8.6/hao/pg.py
--rw-r--r--   0        0        0   211235 2023-12-13 08:25:09.409744 hao-3.8.6/hao/places.py
--rw-r--r--   0        0        0     8705 2023-12-07 02:22:50.584468 hao-3.8.6/hao/rabbit.py
--rw-r--r--   0        0        0     2441 2023-12-07 02:22:50.584468 hao-3.8.6/hao/redis.py
--rw-r--r--   0        0        0     1383 2023-06-29 05:50:26.598477 hao-3.8.6/hao/regexes.py
--rw-r--r--   0        0        0     6273 2023-06-29 02:10:36.411201 hao-3.8.6/hao/s3.py
--rw-r--r--   0        0        0     1152 2022-06-03 16:02:48.521000 hao-3.8.6/hao/singleton.py
--rw-r--r--   0        0        0     1839 2023-06-13 10:11:01.543543 hao-3.8.6/hao/slacks.py
--rw-r--r--   0        0        0     1914 2024-03-21 01:47:17.438178 hao-3.8.6/hao/spinner.py
--rw-r--r--   0        0        0     3676 2024-03-20 11:19:02.953658 hao-3.8.6/hao/sqlite.py
--rw-r--r--   0        0        0     3079 2024-03-21 01:47:26.214112 hao-3.8.6/hao/stopwatch.py
--rw-r--r--   0        0        0    12052 2024-02-08 23:39:08.139407 hao-3.8.6/hao/strings.py
--rw-r--r--   0        0        0      906 2024-02-09 01:58:02.438476 hao-3.8.6/hao/threads.py
--rw-r--r--   0        0        0     1375 2023-08-03 03:04:54.324235 hao-3.8.6/hao/uuid.py
--rw-r--r--   0        0        0     1441 2023-12-10 10:14:12.527924 hao-3.8.6/hao/versions.py
--rw-r--r--   0        0        0      987 2024-03-20 08:26:15.928874 hao-3.8.6/hao/vs.py
--rw-r--r--   0        0        0     2243 2024-03-20 08:27:31.296321 hao-3.8.6/pyproject.toml
--rw-r--r--   0        0        0     6293 1970-01-01 00:00:00.000000 hao-3.8.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2020-08-14 05:40:38.118171 hao-3.8.7/LICENSE
+-rw-r--r--   0        0        0     4550 2024-01-24 03:43:53.608275 hao-3.8.7/README.md
+-rw-r--r--   0        0        0      371 2024-04-17 09:52:45.530290 hao-3.8.7/hao/__init__.py
+-rw-r--r--   0        0        0     5202 2024-02-08 23:32:22.070927 hao-3.8.7/hao/arango.py
+-rw-r--r--   0        0        0     1752 2024-03-21 02:42:14.902996 hao-3.8.7/hao/args.py
+-rw-r--r--   0        0        0      456 2021-10-13 03:48:38.248130 hao-3.8.7/hao/asyncs.py
+-rw-r--r--   0        0        0     4287 2023-12-12 10:48:58.766747 hao-3.8.7/hao/charsets.py
+-rw-r--r--   0        0        0     1886 2024-01-04 06:05:25.811022 hao-3.8.7/hao/cli.py
+-rw-r--r--   0        0        0     5539 2024-01-22 09:11:37.678170 hao-3.8.7/hao/config.py
+-rw-r--r--   0        0        0     1465 2021-10-13 03:48:38.248130 hao-3.8.7/hao/currencies.py
+-rw-r--r--   0        0        0     9092 2024-03-21 01:47:17.438178 hao-3.8.7/hao/dates.py
+-rw-r--r--   0        0        0     2450 2023-12-07 02:22:50.584468 hao-3.8.7/hao/db.py
+-rw-r--r--   0        0        0     5452 2023-11-21 08:14:53.909683 hao-3.8.7/hao/decorators.py
+-rw-r--r--   0        0        0     1513 2023-06-13 10:11:01.543543 hao-3.8.7/hao/dicts.py
+-rw-r--r--   0        0        0    55769 2021-10-13 03:48:38.248130 hao-3.8.7/hao/english.py
+-rw-r--r--   0        0        0      662 2023-03-27 03:43:21.995697 hao-3.8.7/hao/enums.py
+-rw-r--r--   0        0        0     2067 2024-01-19 03:23:22.550873 hao-3.8.7/hao/envs.py
+-rw-r--r--   0        0        0    11233 2024-04-17 09:43:38.646299 hao-3.8.7/hao/es.py
+-rw-r--r--   0        0        0      190 2021-10-13 03:48:38.248130 hao-3.8.7/hao/exceptions.py
+-rw-r--r--   0        0        0      775 2024-03-07 06:56:26.246672 hao-3.8.7/hao/exits.py
+-rw-r--r--   0        0        0     3289 2023-04-04 08:33:34.689439 hao-3.8.7/hao/files.py
+-rw-r--r--   0        0        0     3557 2024-01-04 07:46:49.520797 hao-3.8.7/hao/hf.py
+-rw-r--r--   0        0        0      379 2023-06-29 02:10:36.407201 hao-3.8.7/hao/invoker.py
+-rw-r--r--   0        0        0     1782 2023-06-13 10:11:01.543543 hao-3.8.7/hao/jsons.py
+-rw-r--r--   0        0        0     4611 2023-12-07 02:22:50.584468 hao-3.8.7/hao/kafka.py
+-rw-r--r--   0        0        0     3719 2023-03-27 03:43:21.995697 hao-3.8.7/hao/lists.py
+-rw-r--r--   0        0        0     9040 2024-03-20 10:39:59.305419 hao-3.8.7/hao/logs.py
+-rw-r--r--   0        0        0     3893 2024-02-09 02:44:21.683818 hao-3.8.7/hao/meters.py
+-rw-r--r--   0        0        0     1278 2023-04-25 17:21:24.642589 hao-3.8.7/hao/modules.py
+-rw-r--r--   0        0        0     9237 2023-12-07 02:22:50.584468 hao-3.8.7/hao/mongo.py
+-rw-r--r--   0        0        0     5466 2024-04-03 14:27:23.635069 hao-3.8.7/hao/mysql.py
+-rw-r--r--   0        0        0    10862 2024-03-06 10:18:35.715088 hao-3.8.7/hao/namespaces.py
+-rw-r--r--   0        0        0     9785 2021-10-13 03:48:38.248130 hao-3.8.7/hao/nations.py
+-rw-r--r--   0        0        0      295 2021-10-13 03:48:38.248130 hao-3.8.7/hao/networks.py
+-rw-r--r--   0        0        0    14779 2023-04-04 08:18:53.973078 hao-3.8.7/hao/oss.py
+-rw-r--r--   0        0        0     3713 2024-03-06 06:20:59.128480 hao-3.8.7/hao/paths.py
+-rw-r--r--   0        0        0     5238 2024-04-03 14:27:23.635069 hao-3.8.7/hao/pg.py
+-rw-r--r--   0        0        0   211235 2023-12-13 08:25:09.409744 hao-3.8.7/hao/places.py
+-rw-r--r--   0        0        0     8705 2023-12-07 02:22:50.584468 hao-3.8.7/hao/rabbit.py
+-rw-r--r--   0        0        0     2441 2023-12-07 02:22:50.584468 hao-3.8.7/hao/redis.py
+-rw-r--r--   0        0        0     1383 2023-06-29 05:50:26.598477 hao-3.8.7/hao/regexes.py
+-rw-r--r--   0        0        0     6273 2023-06-29 02:10:36.411201 hao-3.8.7/hao/s3.py
+-rw-r--r--   0        0        0     1152 2022-06-03 16:02:48.521000 hao-3.8.7/hao/singleton.py
+-rw-r--r--   0        0        0     1839 2023-06-13 10:11:01.543543 hao-3.8.7/hao/slacks.py
+-rw-r--r--   0        0        0     1914 2024-03-21 01:47:17.438178 hao-3.8.7/hao/spinner.py
+-rw-r--r--   0        0        0     3676 2024-03-20 11:19:02.953658 hao-3.8.7/hao/sqlite.py
+-rw-r--r--   0        0        0     3079 2024-03-21 01:47:26.214112 hao-3.8.7/hao/stopwatch.py
+-rw-r--r--   0        0        0    12052 2024-02-08 23:39:08.139407 hao-3.8.7/hao/strings.py
+-rw-r--r--   0        0        0      906 2024-02-09 01:58:02.438476 hao-3.8.7/hao/threads.py
+-rw-r--r--   0        0        0     1375 2023-08-03 03:04:54.324235 hao-3.8.7/hao/uuid.py
+-rw-r--r--   0        0        0     1441 2023-12-10 10:14:12.527924 hao-3.8.7/hao/versions.py
+-rw-r--r--   0        0        0     1095 2024-04-09 10:18:22.444119 hao-3.8.7/hao/vs.py
+-rw-r--r--   0        0        0     2243 2024-03-20 08:27:31.296321 hao-3.8.7/pyproject.toml
+-rw-r--r--   0        0        0     6293 1970-01-01 00:00:00.000000 hao-3.8.7/PKG-INFO
```

### Comparing `hao-3.8.6/LICENSE` & `hao-3.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/README.md` & `hao-3.8.7/README.md`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/arango.py` & `hao-3.8.7/hao/arango.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/args.py` & `hao-3.8.7/hao/args.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/charsets.py` & `hao-3.8.7/hao/charsets.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/cli.py` & `hao-3.8.7/hao/cli.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/config.py` & `hao-3.8.7/hao/config.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/currencies.py` & `hao-3.8.7/hao/currencies.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/dates.py` & `hao-3.8.7/hao/dates.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/db.py` & `hao-3.8.7/hao/db.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/decorators.py` & `hao-3.8.7/hao/decorators.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/dicts.py` & `hao-3.8.7/hao/dicts.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/english.py` & `hao-3.8.7/hao/english.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/enums.py` & `hao-3.8.7/hao/enums.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/envs.py` & `hao-3.8.7/hao/envs.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/es.py` & `hao-3.8.7/hao/es.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,20 +93,20 @@
 
     def __str__(self) -> str:
         return f"profile: [{self.profile}], host: {self.__conf.get('host')}, port: {self.__conf.get('port')}"
 
     def __repr__(self) -> str:
         return self.__str__()
 
-    def get_by_id(self, _id, index: str, **params):
+    def get_by_id(self, _id, index: str, params: Optional[dict] = None, **kwargs):
         assert _id is not None, '_id required'
         assert index is not None, 'index required'
 
         try:
-            return self.client.get(index=index, id=_id, params=params)
+            return self.client.get(index=index, id=_id, params=params, **kwargs)
         except NotFoundError:
             return None
 
     def find_by_id(self, _id, index: str, **params) -> list:
         query = {"query": {"term": {"_id": _id}}}
         return list(self.search(query, index, **params))
```

### Comparing `hao-3.8.6/hao/exits.py` & `hao-3.8.7/hao/exits.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/files.py` & `hao-3.8.7/hao/files.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/hf.py` & `hao-3.8.7/hao/hf.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/jsons.py` & `hao-3.8.7/hao/jsons.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/kafka.py` & `hao-3.8.7/hao/kafka.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/lists.py` & `hao-3.8.7/hao/lists.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/logs.py` & `hao-3.8.7/hao/logs.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/meters.py` & `hao-3.8.7/hao/meters.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/modules.py` & `hao-3.8.7/hao/modules.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/mongo.py` & `hao-3.8.7/hao/mongo.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/mysql.py` & `hao-3.8.7/hao/mysql.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/namespaces.py` & `hao-3.8.7/hao/namespaces.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/nations.py` & `hao-3.8.7/hao/nations.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/oss.py` & `hao-3.8.7/hao/oss.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/paths.py` & `hao-3.8.7/hao/paths.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/pg.py` & `hao-3.8.7/hao/pg.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/places.py` & `hao-3.8.7/hao/places.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/rabbit.py` & `hao-3.8.7/hao/rabbit.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/redis.py` & `hao-3.8.7/hao/redis.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/regexes.py` & `hao-3.8.7/hao/regexes.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/s3.py` & `hao-3.8.7/hao/s3.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/singleton.py` & `hao-3.8.7/hao/singleton.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/slacks.py` & `hao-3.8.7/hao/slacks.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/spinner.py` & `hao-3.8.7/hao/spinner.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/sqlite.py` & `hao-3.8.7/hao/sqlite.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/stopwatch.py` & `hao-3.8.7/hao/stopwatch.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/strings.py` & `hao-3.8.7/hao/strings.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/threads.py` & `hao-3.8.7/hao/threads.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/uuid.py` & `hao-3.8.7/hao/uuid.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/versions.py` & `hao-3.8.7/hao/versions.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/hao/vs.py` & `hao-3.8.7/hao/vs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # -*- coding: utf-8 -*-
 import json
+import logging
 import os
 import sys
 
 from . import jsons, paths
 
+LOGGER = logging.getLogger(__name__)
+
+
 def run():
     argv = sys.argv
     n_args = len(argv)
     if n_args == 1:
         print('Usage: h-code {module.name}')
         return
 
     try:
-        module_name = argv[1]
+        module_name = argv[-1]
         path_launch_json = paths.get('.vscode/launch.json')
         if not os.path.exists(path_launch_json):
             data = {'version': '0.2.0', 'configurations': []}
+            paths.make_parent_dirs(path_launch_json)
         else:
             with open(path_launch_json) as f:
                 data = json.load(f)
         data.get('configurations').append({
             "name": module_name,
             "type": "debugpy",
             "request": "launch",
```

### Comparing `hao-3.8.6/pyproject.toml` & `hao-3.8.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hao-3.8.6/PKG-INFO` & `hao-3.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hao
-Version: 3.8.6
+Version: 3.8.7
 Summary: conf, logs, namespace, etc
 Home-page: https://github.com/orctom/hao
 License: Apache-2.0
 Author: orctom
 Author-email: orctom <orctom@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

