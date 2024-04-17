# Comparing `tmp/dbt-duckdb-1.7.3.tar.gz` & `tmp/dbt_duckdb-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-duckdb-1.7.3.tar", last modified: Thu Mar  7 18:57:26 2024, max compression
+gzip compressed data, was "dbt_duckdb-1.7.4.tar", last modified: Wed Apr 17 06:01:38 2024, max compression
```

## Comparing `dbt-duckdb-1.7.3.tar` & `dbt_duckdb-1.7.4.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:26.965383 dbt-duckdb-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23279 2024-03-07 18:57:26.965383 dbt-duckdb-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22265 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:26.957383 dbt-duckdb-1.7.3/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:26.957383 dbt-duckdb-1.7.3/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:26.957383 dbt-duckdb-1.7.3/dbt/adapters/duckdb/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:26.957383 dbt-duckdb-1.7.3/dbt/adapters/duckdb/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     9340 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/environments/buenavista.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/environments/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:26.961383 dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/glue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/gsheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/iceberg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/motherduck.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/pd_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/adapters/duckdb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:26.961383 dbt-duckdb-1.7.3/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:26.961383 dbt-duckdb-1.7.3/dbt/include/duckdb/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:26.961383 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/incremental_helper.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:26.961383 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/materializations/external.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/seed.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/snapshot_helper.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:26.961383 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/utils/external_location.sql
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/utils/lastday.sql
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/utils/splitpart.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/macros/utils/upstream.sql
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/dbt/include/duckdb/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:26.965383 dbt-duckdb-1.7.3/dbt_duckdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23279 2024-03-07 18:57:26.000000 dbt-duckdb-1.7.3/dbt_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-07 18:57:26.000000 dbt-duckdb-1.7.3/dbt_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 18:57:26.000000 dbt-duckdb-1.7.3/dbt_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-07 18:57:26.000000 dbt-duckdb-1.7.3/dbt_duckdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-07 18:57:26.000000 dbt-duckdb-1.7.3/dbt_duckdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 18:57:26.965383 dbt-duckdb-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-03-07 18:57:22.000000 dbt-duckdb-1.7.3/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.843292 dbt_duckdb-1.7.4/
+-rw-r--r--   0 jwills     (501) staff       (20)    11357 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/LICENSE
+-rw-r--r--   0 jwills     (501) staff       (20)       47 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/MANIFEST.in
+-rw-r--r--   0 jwills     (501) staff       (20)    23279 2024-04-17 06:01:38.843066 dbt_duckdb-1.7.4/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)    22265 2024-04-17 05:57:44.000000 dbt_duckdb-1.7.4/README.md
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.831895 dbt_duckdb-1.7.4/dbt/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.832136 dbt_duckdb-1.7.4/dbt/adapters/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.834522 dbt_duckdb-1.7.4/dbt/adapters/duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)      407 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)       18 2024-04-17 05:57:34.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/__version__.py
+-rw-r--r--   0 jwills     (501) staff       (20)      856 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/column.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3740 2024-04-03 05:10:12.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/connections.py
+-rw-r--r--   0 jwills     (501) staff       (20)     9883 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/credentials.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.835556 dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/
+-rw-r--r--   0 jwills     (501) staff       (20)     9673 2024-04-03 05:10:12.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2404 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/buenavista.py
+-rw-r--r--   0 jwills     (501) staff       (20)     5462 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/local.py
+-rw-r--r--   0 jwills     (501) staff       (20)    11267 2024-04-17 05:42:41.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/impl.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.838174 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/
+-rw-r--r--   0 jwills     (501) staff       (20)     5039 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1230 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/delta.py
+-rw-r--r--   0 jwills     (501) staff       (20)     4951 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/excel.py
+-rw-r--r--   0 jwills     (501) staff       (20)    12466 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/glue.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2386 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/gsheet.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1029 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/iceberg.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1703 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/motherduck.py
+-rw-r--r--   0 jwills     (501) staff       (20)      533 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/pd_utils.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1296 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/postgres.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1505 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/sqlalchemy.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3457 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/relation.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2445 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/utils.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.838305 dbt_duckdb-1.7.4/dbt/include/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.838729 dbt_duckdb-1.7.4/dbt/include/duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)       52 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)       74 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/dbt_project.yml
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.840206 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/
+-rw-r--r--   0 jwills     (501) staff       (20)     7949 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/adapters.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1465 2024-04-03 05:10:12.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/catalog.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      643 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/columns.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1429 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/incremental_helper.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.840872 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/
+-rw-r--r--   0 jwills     (501) staff       (20)     4165 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/external.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     5315 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/incremental.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     2529 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/table.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1620 2024-04-03 05:10:12.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/persist_docs.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1849 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/seed.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1359 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/snapshot_helper.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.841974 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/
+-rw-r--r--   0 jwills     (501) staff       (20)       93 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/any_value.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      174 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/dateadd.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      172 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/datediff.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      357 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/external_location.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      378 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/lastday.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      568 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/listagg.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      167 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/splitpart.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1683 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/upstream.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      174 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/sample_profiles.yml
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.842657 dbt_duckdb-1.7.4/dbt_duckdb.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)    23279 2024-04-17 06:01:38.000000 dbt_duckdb-1.7.4/dbt_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)     1982 2024-04-17 06:01:38.000000 dbt_duckdb-1.7.4/dbt_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2024-04-17 06:01:38.000000 dbt_duckdb-1.7.4/dbt_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       88 2024-04-17 06:01:38.000000 dbt_duckdb-1.7.4/dbt_duckdb.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        4 2024-04-17 06:01:38.000000 dbt_duckdb-1.7.4/dbt_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2024-04-17 06:01:38.843330 dbt_duckdb-1.7.4/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)     1899 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/setup.py
```

### Comparing `dbt-duckdb-1.7.3/LICENSE` & `dbt_duckdb-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/PKG-INFO` & `dbt_duckdb-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.7.3
+Version: 1.7.4
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-duckdb-1.7.3/README.md` & `dbt_duckdb-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/column.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/column.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/connections.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/connections.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import atexit
 import threading
 from contextlib import contextmanager
 from typing import Optional
 from typing import Tuple
-
-import agate
+from typing import TYPE_CHECKING
 
 import dbt.exceptions
 from . import environments
 from dbt.adapters.sql import SQLConnectionManager
 from dbt.contracts.connection import AdapterRequiredConfig
 from dbt.contracts.connection import AdapterResponse
 from dbt.contracts.connection import Connection
 from dbt.contracts.connection import ConnectionState
 from dbt.logger import GLOBAL_LOGGER as logger
 
+if TYPE_CHECKING:
+    import agate
+
 
 class DuckDBConnectionManager(SQLConnectionManager):
     TYPE = "duckdb"
     _LOCK = threading.RLock()
     _ENV = None
 
     def __init__(self, profile: AdapterRequiredConfig):
@@ -97,14 +99,14 @@
 
     def execute(
         self,
         sql: str,
         auto_begin: bool = False,
         fetch: bool = False,
         limit: Optional[int] = None,
-    ) -> Tuple[AdapterResponse, agate.Table]:
+    ) -> Tuple[AdapterResponse, "agate.Table"]:
         if self.disable_transactions:
             auto_begin = False
         return super().execute(sql, auto_begin, fetch, limit)
 
 
 atexit.register(DuckDBConnectionManager.close_all_connections)
```

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/credentials.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/environments/__init__.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,20 @@
 
         # Add any module paths to the Python path for the environment
         if creds.module_paths:
             for path in creds.module_paths:
                 if path not in sys.path:
                     sys.path.append(path)
 
+        major, minor, patch = [int(x) for x in duckdb.__version__.split(".")]
+        if major == 0 and (minor < 10 or (minor == 10 and patch == 0)):
+            self._supports_comments = False
+        else:
+            self._supports_comments = True
+
     @property
     def creds(self) -> DuckDBCredentials:
         return self._creds
 
     @abc.abstractmethod
     def handle(self):
         pass
@@ -105,14 +111,17 @@
     @abc.abstractmethod
     def store_relation(self, plugin_name: str, target_config: TargetConfig) -> None:
         pass
 
     def get_binding_char(self) -> str:
         return "?"
 
+    def supports_comments(self) -> bool:
+        return self._supports_comments
+
     @classmethod
     def initialize_db(
         cls, creds: DuckDBCredentials, plugins: Optional[Dict[str, BasePlugin]] = None
     ):
         config = creds.config_options or {}
         plugins = plugins or {}
         for plugin in plugins.values():
```

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/environments/buenavista.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/buenavista.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/environments/local.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/local.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/impl.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Sequence
-
-import agate
+from typing import TYPE_CHECKING
 
 from dbt.adapters.base import BaseRelation
 from dbt.adapters.base.column import Column as BaseColumn
 from dbt.adapters.base.impl import ConstraintSupport
 from dbt.adapters.base.meta import available
 from dbt.adapters.duckdb.column import DuckDBColumn
 from dbt.adapters.duckdb.connections import DuckDBConnectionManager
@@ -24,14 +23,17 @@
 from dbt.contracts.relation import RelationType
 from dbt.exceptions import DbtInternalError
 from dbt.exceptions import DbtRuntimeError
 
 TEMP_SCHEMA_NAME = "temp_schema_name"
 DEFAULT_TEMP_SCHEMA_NAME = "dbt_temp"
 
+if TYPE_CHECKING:
+    import agate
+
 
 class DuckDBAdapter(SQLAdapter):
     ConnectionManager = DuckDBConnectionManager
     Column = DuckDBColumn
     Relation = DuckDBRelation
 
     CONSTRAINT_SUPPORT = {
@@ -57,15 +59,17 @@
         self.execute("select 1 as id")
 
     @available
     def is_motherduck(self):
         return self.config.credentials.is_motherduck
 
     @available
-    def convert_datetimes_to_strs(self, table: agate.Table) -> agate.Table:
+    def convert_datetimes_to_strs(self, table: "agate.Table") -> "agate.Table":
+        import agate
+
         for column in table.columns:
             if isinstance(column.data_type, agate.DateTime):
                 table = table.compute(
                     [
                         (
                             column.name,
                             agate.Formula(agate.Text(), lambda row: str(row[column.name])),
@@ -114,14 +118,21 @@
         return self.config.credentials.external_root
 
     @available
     def get_binding_char(self):
         return DuckDBConnectionManager.env().get_binding_char()
 
     @available
+    def catalog_comment(self, prefix):
+        if DuckDBConnectionManager.env().supports_comments():
+            return f"{prefix}.comment"
+        else:
+            return "''"
+
+    @available
     def external_write_options(self, write_location: str, rendered_options: dict) -> str:
         if "format" not in rendered_options:
             ext = os.path.splitext(write_location)[1].lower()
             if ext:
                 rendered_options["format"] = ext[1:]
             elif "delimiter" in rendered_options:
                 rendered_options["format"] = "csv"
@@ -226,19 +237,31 @@
         rendering."""
         if constraint.type == ConstraintType.foreign_key:
             # DuckDB doesn't support 'foreign key' as an alias
             return f"references {constraint.expression}"
         else:
             return super().render_column_constraint(constraint)
 
+    def _clean_up_temp_relation_for_incremental(self, config):
+        if self.is_motherduck():
+            if "incremental" == config.model.get_materialization():
+                temp_relation = self.Relation(
+                    path=self.get_temp_relation_path(config.model), type=RelationType.Table
+                )
+                self.drop_relation(temp_relation)
+
     def pre_model_hook(self, config: Any) -> None:
-        """A hook for getting the temp schema name from the model config"""
+        """A hook for getting the temp schema name from the model config.
+        Cleans up the remote temporary table on MotherDuck before running
+        an incremental model.
+        """
         self._temp_schema_name = config.model.config.meta.get(
             TEMP_SCHEMA_NAME, self._temp_schema_name
         )
+        self._clean_up_temp_relation_for_incremental(config)
         super().pre_model_hook(config)
 
     @available
     def get_temp_relation_path(self, model: Any):
         """This is a workaround to enable incremental models on MotherDuck because it
         currently doesn't support remote temporary tables. Instead we use a regular
         table that is dropped at the end of the incremental macro or post-model hook.
@@ -247,20 +270,15 @@
             schema=self._temp_schema_name, database=model.database, identifier=model.identifier
         )
 
     def post_model_hook(self, config: Any, context: Any) -> None:
         """A hook for cleaning up the remote temporary table on MotherDuck if the
         incremental model materialization fails to do so.
         """
-        if self.is_motherduck():
-            if "incremental" == config.model.get_materialization():
-                temp_relation = self.Relation(
-                    path=self.get_temp_relation_path(config.model), type=RelationType.Table
-                )
-                self.drop_relation(temp_relation)
+        self._clean_up_temp_relation_for_incremental(config)
         super().post_model_hook(config, context)
 
 
 # Change `table_a/b` to `table_aaaaa/bbbbb` to avoid duckdb binding issues when relation_a/b
 # is called "table_a" or "table_b" in some of the dbt tests
 COLUMNS_EQUAL_SQL = """
 with diff_count as (
```

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/__init__.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/delta.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/delta.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/excel.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/excel.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/glue.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/glue.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/gsheet.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/gsheet.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/iceberg.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/iceberg.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/motherduck.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/motherduck.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/pd_utils.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/pd_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/postgres.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/postgres.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/plugins/sqlalchemy.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/relation.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/adapters/duckdb/utils.py` & `dbt_duckdb-1.7.4/dbt/adapters/duckdb/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/include/duckdb/macros/adapters.sql` & `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/include/duckdb/macros/catalog.sql` & `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/catalog.sql`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,45 @@
 
 {% macro duckdb__get_catalog(information_schema, schemas) -%}
   {%- call statement('catalog', fetch_result=True) -%}
+    with relations AS (
+      select
+        t.table_name
+        , t.database_name
+        , t.schema_name
+        , 'BASE TABLE' as table_type
+        , {{ adapter.catalog_comment('t') }} as table_comment
+      from duckdb_tables() t
+      WHERE t.database_name = '{{ database }}'
+      UNION ALL
+      SELECT v.view_name as table_name
+      , v.database_name
+      , v.schema_name
+      , 'VIEW' as table_type
+      , {{ adapter.catalog_comment('v') }} as table_comment
+      from duckdb_views() v
+      WHERE v.database_name = '{{ database }}'
+    )
     select
         '{{ database }}' as table_database,
-        t.table_schema,
-        t.table_name,
-        t.table_type,
-        '' as table_comment,
+        r.schema_name as table_schema,
+        r.table_name,
+        r.table_type,
+        r.table_comment,
         c.column_name,
-        c.ordinal_position as column_index,
-        c.data_type column_type,
-        '' as column_comment,
+        c.column_index as column_index,
+        c.data_type as column_type,
+        {{ adapter.catalog_comment('c') }} as column_comment,
         '' as table_owner
-    FROM information_schema.tables t JOIN information_schema.columns c ON t.table_schema = c.table_schema AND t.table_name = c.table_name
+    FROM relations r JOIN duckdb_columns() c ON r.schema_name = c.schema_name AND r.table_name = c.table_name
     WHERE (
         {%- for schema in schemas -%}
-          upper(t.table_schema) = upper('{{ schema }}'){%- if not loop.last %} or {% endif -%}
+          upper(r.schema_name) = upper('{{ schema }}'){%- if not loop.last %} or {% endif -%}
         {%- endfor -%}
     )
-    AND t.table_type IN ('BASE TABLE', 'VIEW')
     ORDER BY
-        t.table_schema,
-        t.table_name,
-        c.ordinal_position
+        r.schema_name,
+        r.table_name,
+        c.column_index
   {%- endcall -%}
   {{ return(load_result('catalog').table) }}
 {%- endmacro %}
```

### Comparing `dbt-duckdb-1.7.3/dbt/include/duckdb/macros/columns.sql` & `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/include/duckdb/macros/incremental_helper.sql` & `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/incremental_helper.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/include/duckdb/macros/materializations/external.sql` & `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/external.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/include/duckdb/macros/materializations/incremental.sql` & `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/include/duckdb/macros/materializations/table.sql` & `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/include/duckdb/macros/seed.sql` & `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/include/duckdb/macros/snapshot_helper.sql` & `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/snapshot_helper.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/include/duckdb/macros/utils/listagg.sql` & `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt/include/duckdb/macros/utils/upstream.sql` & `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/upstream.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.7.3/dbt_duckdb.egg-info/PKG-INFO` & `dbt_duckdb-1.7.4/dbt_duckdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.7.3
+Version: 1.7.4
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-duckdb-1.7.3/dbt_duckdb.egg-info/SOURCES.txt` & `dbt_duckdb-1.7.4/dbt_duckdb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 dbt/include/duckdb/__init__.py
 dbt/include/duckdb/dbt_project.yml
 dbt/include/duckdb/sample_profiles.yml
 dbt/include/duckdb/macros/adapters.sql
 dbt/include/duckdb/macros/catalog.sql
 dbt/include/duckdb/macros/columns.sql
 dbt/include/duckdb/macros/incremental_helper.sql
+dbt/include/duckdb/macros/persist_docs.sql
 dbt/include/duckdb/macros/seed.sql
 dbt/include/duckdb/macros/snapshot_helper.sql
 dbt/include/duckdb/macros/materializations/external.sql
 dbt/include/duckdb/macros/materializations/incremental.sql
 dbt/include/duckdb/macros/materializations/table.sql
 dbt/include/duckdb/macros/utils/any_value.sql
 dbt/include/duckdb/macros/utils/dateadd.sql
```

### Comparing `dbt-duckdb-1.7.3/setup.py` & `dbt_duckdb-1.7.4/setup.py`

 * *Files identical despite different names*

