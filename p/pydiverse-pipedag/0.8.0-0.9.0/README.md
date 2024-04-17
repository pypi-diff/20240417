# Comparing `tmp/pydiverse_pipedag-0.8.0.tar.gz` & `tmp/pydiverse_pipedag-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse_pipedag-0.8.0.tar", max compression
+gzip compressed data, was "pydiverse_pipedag-0.9.0.tar", max compression
```

## Comparing `pydiverse_pipedag-0.8.0.tar` & `pydiverse_pipedag-0.9.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
--rw-r--r--   0        0        0     1517 2024-04-02 08:29:11.021852 pydiverse_pipedag-0.8.0/LICENSE
--rw-r--r--   0        0        0     5483 2024-04-02 08:29:11.021852 pydiverse_pipedag-0.8.0/docs/package/README.md
--rw-r--r--   0        0        0     3912 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       13 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      515 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/__init__.py
--rw-r--r--   0        0        0      857 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/_typing.py
--rw-r--r--   0        0        0       97 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/__init__.py
--rw-r--r--   0        0        0     6613 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/blob.py
--rw-r--r--   0        0        0      393 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/__init__.py
--rw-r--r--   0        0        0     6097 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/base.py
--rw-r--r--   0        0        0    13599 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/database.py
--rw-r--r--   0        0        0     2756 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/filelock.py
--rw-r--r--   0        0        0      769 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/nolock.py
--rw-r--r--   0        0        0     3983 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/zookeeper.py
--rw-r--r--   0        0        0      233 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/__init__.py
--rw-r--r--   0        0        0    30207 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/base.py
--rw-r--r--   0        0        0      108 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/cache/__init__.py
--rw-r--r--   0        0        0     3455 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/cache/base.py
--rw-r--r--   0        0        0     6892 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/cache/parquet.py
--rw-r--r--   0        0        0     6757 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/dict.py
--rw-r--r--   0        0        0      157 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/__init__.py
--rw-r--r--   0        0        0    41260 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/ddl.py
--rw-r--r--   0        0        0      187 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
--rw-r--r--   0        0        0     4411 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
--rw-r--r--   0        0        0    10670 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
--rw-r--r--   0        0        0    12669 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
--rw-r--r--   0        0        0     5443 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
--rw-r--r--   0        0        0    29307 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/hooks.py
--rw-r--r--   0        0        0     4617 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/reflection.py
--rw-r--r--   0        0        0    64631 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/sql.py
--rw-r--r--   0        0        0       81 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/util/__init__.py
--rw-r--r--   0        0        0     8887 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/util/dtype.py
--rw-r--r--   0        0        0      433 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/context/__init__.py
--rw-r--r--   0        0        0    11531 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/context/context.py
--rw-r--r--   0        0        0    27793 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/context/run_context.py
--rw-r--r--   0        0        0      311 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/__init__.py
--rw-r--r--   0        0        0    23202 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/config.py
--rw-r--r--   0        0        0    22133 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/flow.py
--rw-r--r--   0        0        0     4294 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/result.py
--rw-r--r--   0        0        0     8035 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/stage.py
--rw-r--r--   0        0        0     8392 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/task.py
--rw-r--r--   0        0        0      135 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/debug/__init__.py
--rw-r--r--   0        0        0      368 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/__init__.py
--rw-r--r--   0        0        0      654 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/base.py
--rw-r--r--   0        0        0     3133 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/dask.py
--rw-r--r--   0        0        0     7269 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/prefect.py
--rw-r--r--   0        0        0     1388 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/sequential.py
--rw-r--r--   0        0        0     1079 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/errors/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/__init__.py
--rw-r--r--   0        0        0      620 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/cli.py
--rw-r--r--   0        0        0        0 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/commands/__init__.py
--rw-r--r--   0        0        0     1741 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/commands/clear_metadata.py
--rw-r--r--   0        0        0     2744 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/commands/delete_schemas.py
--rw-r--r--   0        0        0      182 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/__init__.py
--rw-r--r--   0        0        0     1709 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/cache.py
--rw-r--r--   0        0        0    13261 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/container.py
--rw-r--r--   0        0        0    32965 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/core.py
--rw-r--r--   0        0        0     2921 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/debug.py
--rw-r--r--   0        0        0     3837 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/details.py
--rw-r--r--   0        0        0     2074 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/metadata.py
--rw-r--r--   0        0        0    20861 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/store.py
--rw-r--r--   0        0        0      213 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/__init__.py
--rw-r--r--   0        0        0     9273 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/computation_tracing.py
--rw-r--r--   0        0        0     2061 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/deep_map.py
--rw-r--r--   0        0        0     1848 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/deep_merge.py
--rw-r--r--   0        0        0      944 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/disposable.py
--rw-r--r--   0        0        0     1129 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/hashing.py
--rw-r--r--   0        0        0     3816 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/import_.py
--rw-r--r--   0        0        0     7992 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/ipc.py
--rw-r--r--   0        0        0     4812 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/json.py
--rw-r--r--   0        0        0     1377 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/naming.py
--rw-r--r--   0        0        0     2847 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/structlog.py
--rw-r--r--   0        0        0     7365 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1517 2024-04-17 10:05:40.314924 pydiverse_pipedag-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5623 2024-04-17 10:05:40.314924 pydiverse_pipedag-0.9.0/docs/package/README.md
+-rw-r--r--   0        0        0     3912 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       13 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      629 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/__init__.py
+-rw-r--r--   0        0        0      857 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/_typing.py
+-rw-r--r--   0        0        0       97 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/__init__.py
+-rw-r--r--   0        0        0     6613 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/blob.py
+-rw-r--r--   0        0        0      393 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/__init__.py
+-rw-r--r--   0        0        0     6102 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/base.py
+-rw-r--r--   0        0        0    13646 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/database.py
+-rw-r--r--   0        0        0     2756 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/filelock.py
+-rw-r--r--   0        0        0      769 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/nolock.py
+-rw-r--r--   0        0        0     3983 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/zookeeper.py
+-rw-r--r--   0        0        0      233 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/__init__.py
+-rw-r--r--   0        0        0    30931 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/base.py
+-rw-r--r--   0        0        0      108 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/cache/__init__.py
+-rw-r--r--   0        0        0     3455 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/cache/base.py
+-rw-r--r--   0        0        0     6892 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/cache/parquet.py
+-rw-r--r--   0        0        0     6757 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/dict.py
+-rw-r--r--   0        0        0      103 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/__init__.py
+-rw-r--r--   0        0        0    41541 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/ddl.py
+-rw-r--r--   0        0        0      187 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
+-rw-r--r--   0        0        0     4411 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
+-rw-r--r--   0        0        0    10717 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
+-rw-r--r--   0        0        0    12665 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
+-rw-r--r--   0        0        0     5490 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
+-rw-r--r--   0        0        0    30118 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/hooks.py
+-rw-r--r--   0        0        0     4617 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/reflection.py
+-rw-r--r--   0        0        0    62186 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/sql.py
+-rw-r--r--   0        0        0       81 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/util/__init__.py
+-rw-r--r--   0        0        0     8887 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/util/dtype.py
+-rw-r--r--   0        0        0      433 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/context/__init__.py
+-rw-r--r--   0        0        0    12059 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/context/context.py
+-rw-r--r--   0        0        0    27776 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/context/run_context.py
+-rw-r--r--   0        0        0      408 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/__init__.py
+-rw-r--r--   0        0        0    26497 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/config.py
+-rw-r--r--   0        0        0    51959 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/flow.py
+-rw-r--r--   0        0        0     7891 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/group_node.py
+-rw-r--r--   0        0        0     4552 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/result.py
+-rw-r--r--   0        0        0     8529 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/stage.py
+-rw-r--r--   0        0        0     8768 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/task.py
+-rw-r--r--   0        0        0      135 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/debug/__init__.py
+-rw-r--r--   0        0        0      493 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/base.py
+-rw-r--r--   0        0        0     3123 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/dask.py
+-rw-r--r--   0        0        0     7269 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/prefect.py
+-rw-r--r--   0        0        0     1981 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/sequential.py
+-rw-r--r--   0        0        0     1191 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/errors/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/__init__.py
+-rw-r--r--   0        0        0      620 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/cli.py
+-rw-r--r--   0        0        0        0 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/commands/__init__.py
+-rw-r--r--   0        0        0     1741 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/commands/clear_metadata.py
+-rw-r--r--   0        0        0     2795 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/commands/delete_schemas.py
+-rw-r--r--   0        0        0      258 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/__init__.py
+-rw-r--r--   0        0        0     2735 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/cache.py
+-rw-r--r--   0        0        0    24375 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/container.py
+-rw-r--r--   0        0        0    38201 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/core.py
+-rw-r--r--   0        0        0     4453 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/debug.py
+-rw-r--r--   0        0        0     3837 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/details.py
+-rw-r--r--   0        0        0     2074 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/metadata.py
+-rw-r--r--   0        0        0    21432 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/store.py
+-rw-r--r--   0        0        0      213 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/__init__.py
+-rw-r--r--   0        0        0     9273 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/computation_tracing.py
+-rw-r--r--   0        0        0     2061 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/deep_map.py
+-rw-r--r--   0        0        0     1848 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/deep_merge.py
+-rw-r--r--   0        0        0      944 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/disposable.py
+-rw-r--r--   0        0        0     1129 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/hashing.py
+-rw-r--r--   0        0        0     3816 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/import_.py
+-rw-r--r--   0        0        0     7992 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/ipc.py
+-rw-r--r--   0        0        0     5375 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/json.py
+-rw-r--r--   0        0        0     1377 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/naming.py
+-rw-r--r--   0        0        0     2847 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/structlog.py
+-rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.9.0/PKG-INFO
```

### Comparing `pydiverse_pipedag-0.8.0/LICENSE` & `pydiverse_pipedag-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/docs/package/README.md` & `pydiverse_pipedag-0.9.0/docs/package/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,30 +37,30 @@
     return sa.select(
         sa.literal(1).label("x"),
         sa.literal(2).label("y"),
     )
 
 
 @materialize(lazy=True, input_type=sa.Table)
-def lazy_task_2(input1: sa.Table, input2: sa.Table):
+def lazy_task_2(input1: sa.sql.expression.Alias, input2: sa.sql.expression.Alias):
     query = sa.select(
         (input1.c.x * 5).label("x5"),
         input2.c.a,
     ).select_from(input1.outerjoin(input2, input2.c.x == input1.c.x))
 
     return Table(query, name="task_2_out", primary_key=["a"])
 
 
 @materialize(lazy=True, input_type=sa.Table)
-def lazy_task_3(input1: sa.Table):
+def lazy_task_3(input1: sa.sql.expression.Alias):
     return sa.text(f"SELECT * FROM {input1.original.schema}.{input1.original.name}")
 
 
 @materialize(lazy=True, input_type=sa.Table)
-def lazy_task_4(input1: sa.Table):
+def lazy_task_4(input1: sa.sql.expression.Alias):
     return sa.text(f"SELECT * FROM {input1.original.schema}.{input1.original.name}")
 
 
 @materialize(nout=2, version="1.0.0")
 def eager_inputs():
     dfA = pd.DataFrame(
         {
@@ -118,14 +118,15 @@
                 assert result.get(lazy_1, as_type=pd.DataFrame)["x"][0] == 1
 
 
 if __name__ == "__main__":
     setup_logging()  # you can setup the logging and/or structlog libraries as you wish
     main()
 ```
+For SQLAlchemy >= 2.0, you can use sa.Alias instead of sa.sql.expression.Alias.
 
 The `with tempfile.TemporaryDirectory()` is only needed to have an OS independent temporary directory available.
 You can also get rid of it like this:
 
 ```python
 def main():
     cfg = create_basic_pipedag_config(
```

### Comparing `pydiverse_pipedag-0.8.0/pyproject.toml` & `pydiverse_pipedag-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-pipedag"
-version = "0.8.0"
+version = "0.9.0"
 description = "A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files."
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/_typing.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/_typing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/blob.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/blob.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/base.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from enum import Enum
 from typing import Callable, Union
 
 import structlog
 
-from pydiverse.pipedag import Stage
+from pydiverse.pipedag.core import Stage
 from pydiverse.pipedag.errors import LockError
 from pydiverse.pipedag.util import Disposable
 
 
 class LockState(Enum):
     """Lock State
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/database.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 import sqlalchemy as sa
 
 from pydiverse.pipedag import ConfigContext, Stage
 from pydiverse.pipedag.backend.lock.base import BaseLockManager, Lockable, LockState
 from pydiverse.pipedag.backend.table.sql.ddl import (
     CreateSchema,
-    Schema,
 )
 from pydiverse.pipedag.errors import LockError
+from pydiverse.pipedag.materialize.container import Schema
 
 
 class DatabaseLockManager(BaseLockManager):
     """Lock manager based on database locking mechanisms
 
     Many databases provide some kind of locking mechanism. Depending on the specific
     database technology, this allows us to implement locking on either the schema
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/filelock.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/filelock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/nolock.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/nolock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/zookeeper.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/zookeeper.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/base.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,15 +345,22 @@
                 f" {repr(type(table.obj))} of the lazy task {task.name} does"
                 " not provide a query string. Lazy evaluation is not"
                 " possible. Assuming that the table is not cache valid."
             )
             # Assign random query string to ensure that task is not cache valid
             query_str = uuid.uuid4().hex
 
-        query_hash = stable_hash("LAZY-TABLE", query_str)
+        if table.assumed_dependencies is None:
+            query_hash = stable_hash("LAZY-TABLE", query_str)
+        else:
+            # include assumed dependencies in query hash for imperative materialize
+            dependencies = config_context.store.json_encoder.encode(
+                table.assumed_dependencies
+            )
+            query_hash = stable_hash("LAZY-TABLE", query_str, dependencies)
 
         # Store the table
         try:
             if task_cache_info.force_task_execution:
                 self.logger.info(
                     "Forced task execution due to config",
                     cache_validation=config_context.cache_validation,
@@ -697,14 +704,23 @@
         """
         Return `True` if this hook can retrieve a table from the store
         and convert it to the specified type. If `True` is returned, the
         `retrieve` method MUST be implemented for the type.
         """
 
     @classmethod
+    def retrieve_as_reference(cls, type_: type) -> bool:
+        """
+        Table hooks that retrieve `type_` as reference instead of copying the content
+        of the table should return True. This is used by imperative materialization
+        to determine whether input_type is a good default for returned references.
+        """
+        return False
+
+    @classmethod
     @abstractmethod
     def materialize(
         cls, store: TableHookResolverT, table: Table, stage_name: str
     ) -> None:
         """Materialize a table object
 
         :param store: The store which called this method
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/cache/base.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/cache/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/cache/parquet.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/cache/parquet.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/dict.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/dict.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/ddl.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/ddl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from __future__ import annotations
 
 import copy
 import re
 
 import pyparsing as pp
 import sqlalchemy as sa
-from attr import frozen
 from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.schema import DDLElement
 from sqlalchemy.sql import Select
 from sqlalchemy.sql.elements import TextClause
 
 __all__ = [
-    "Schema",
     "CreateSchema",
     "DropSchema",
     "RenameSchema",
     "DropSchemaContent",
     "CreateTableAsSelect",
     "InsertIntoSelect",
     "CreateTableWithSuffix",
@@ -38,26 +36,15 @@
     "LockTable",
     "LockSourceTable",
     "split_ddl_statement",
 ]
 
 from sqlalchemy.sql.type_api import TypeEngine
 
-
-@frozen
-class Schema:
-    name: str
-    prefix: str
-    suffix: str
-
-    def get(self):
-        return self.prefix + self.name + self.suffix
-
-    def __str__(self):
-        return self.get()
+from pydiverse.pipedag import Schema
 
 
 class CreateSchema(DDLElement):
     def __init__(self, schema: Schema, if_not_exists=False):
         self.schema = schema
         self.if_not_exists = if_not_exists
 
@@ -205,39 +192,39 @@
     ):
         self.from_name = from_name
         self.to_name = to_name
         self.schema = schema
 
 
 class DropTable(DDLElement):
-    def __init__(self, name, schema: Schema, if_exists=False, cascade=False):
+    def __init__(self, name, schema: Schema | str, if_exists=False, cascade=False):
         self.name = name
         self.schema = schema
         self.if_exists = if_exists
         self.cascade = cascade  # True: remove dependent views in postgres
 
 
 class DropView(DDLElement):
     """
     Attention: For mssql, this statement must be prefixed with
                a 'USE <database>' statement.
     """
 
-    def __init__(self, name, schema: Schema, if_exists=False):
+    def __init__(self, name, schema: Schema | str, if_exists=False):
         self.name = name
         self.schema = schema
         self.if_exists = if_exists
 
 
 class DropAlias(DDLElement):
     """
     This is used for dialect=ibm_sa_db
     """
 
-    def __init__(self, name, schema: Schema, if_exists=False, *, engine=None):
+    def __init__(self, name, schema: Schema | str, if_exists=False, *, engine=None):
         """
         :param engine: Used if if_exists=True but the database doesn't support it.
         """
         self.name = name
         self.schema = schema
         self.if_exists = if_exists
         self.engine = engine
@@ -256,27 +243,27 @@
 
 class DropProcedure(DDLElement):
     """
     Attention: For mssql, this statement must be prefixed with
                a 'USE <database>' statement.
     """
 
-    def __init__(self, name, schema: Schema, if_exists=False):
+    def __init__(self, name, schema: Schema | str, if_exists=False):
         self.name = name
         self.schema = schema
         self.if_exists = if_exists
 
 
 class DropFunction(DDLElement):
     """
     Attention: For mssql, this statement must be prefixed with
                a 'USE <database>' statement.
     """
 
-    def __init__(self, name, schema: Schema, if_exists=False):
+    def __init__(self, name, schema: Schema | str, if_exists=False):
         self.name = name
         self.schema = schema
         self.if_exists = if_exists
 
 
 class AddPrimaryKey(DDLElement):
     def __init__(
@@ -774,17 +761,23 @@
         "UNION",
         "EXCEPT",
         "INTERSECT",
     ]:
         regex = re.compile(r"\b" + marker + r"\b", re.IGNORECASE)
         for match in regex.finditer(select_sql):
             match_start = match.span()[0]
+            # special case handling: ignore escaped from
             prev = select_sql[0:match_start]
             # ignore marker in subqueries in select columns
-            if prev.count("(") == prev.count(")"):
+            # as well as columns called from (escaped by [] or "")
+            if (
+                prev.count("(") == prev.count(")")
+                and prev.count("[") == prev.count("]")
+                and prev.count('"') % 2 == 0
+            ):
                 into_point = match_start
                 break
         if into_point is not None:
             break
     return (
         select_sql[0:into_point] + into + " " + select_sql[into_point:]
         if into_point is not None
@@ -910,16 +903,19 @@
 
 
 @compiles(DropAlias, "ibm_db_sa")
 def visit_drop_alias_ibm_db_sa(drop: DropAlias, compiler, **kw):
     if drop.if_exists:
         from pydiverse.pipedag.backend.table.sql.reflection import PipedagDB2Reflection
 
+        schema_str = (
+            drop.schema.get() if isinstance(drop.schema, Schema) else drop.schema
+        )
         if drop.name not in PipedagDB2Reflection.get_alias_names(
-            drop.engine, schema=drop.schema.get()
+            drop.engine, schema=schema_str
         ):
             return ""
         drop = DropAlias(drop.name, drop.schema, if_exists=False)
     return _visit_drop_anything(drop, "ALIAS", compiler, **kw)
 
 
 @compiles(DropNickname, "ibm_db_sa")
@@ -941,15 +937,16 @@
     drop: DropTable | DropView | DropProcedure | DropFunction | DropAlias,
     _type,
     compiler,
     **kw,
 ):
     _ = kw
     table = compiler.preparer.quote(drop.name)
-    schema = compiler.preparer.format_schema(drop.schema.get())
+    schema_str = drop.schema.get() if isinstance(drop.schema, Schema) else drop.schema
+    schema = compiler.preparer.format_schema(schema_str)
     text = [f"DROP {_type}"]
     if drop.if_exists:
         text.append("IF EXISTS")
     text.append(f"{schema}.{table}")
     if hasattr(drop, "cascade") and drop.cascade:
         text.append("CASCADE")
     return " ".join(text)
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import warnings
 from pathlib import Path
 
 import pandas as pd
 import sqlalchemy as sa
 
 from pydiverse.pipedag import Table
-from pydiverse.pipedag.backend.table.sql.ddl import Schema
 from pydiverse.pipedag.backend.table.sql.hooks import (
     IbisTableHook,
     PandasTableHook,
     PolarsTableHook,
 )
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
 from pydiverse.pipedag.backend.table.util import DType
+from pydiverse.pipedag.materialize.container import Schema
 from pydiverse.pipedag.materialize.details import resolve_materialization_details_label
 
 try:
     import duckdb
 except ImportError as e:
     warnings.warn(str(e), ImportWarning)
     duckdb = None
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 import sqlalchemy as sa
 import sqlalchemy.exc
 
 from pydiverse.pipedag.backend.table.sql.ddl import (
     CreateTableWithSuffix,
     LockSourceTable,
     LockTable,
-    Schema,
 )
 from pydiverse.pipedag.backend.table.sql.hooks import PandasTableHook
 from pydiverse.pipedag.backend.table.sql.reflection import PipedagDB2Reflection
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
 from pydiverse.pipedag.backend.table.util import DType
 from pydiverse.pipedag.materialize import Table
+from pydiverse.pipedag.materialize.container import Schema
 from pydiverse.pipedag.materialize.details import (
     BaseMaterializationDetails,
     resolve_materialization_details_label,
 )
 
 _TABLE_SPACE_KEYWORD_MAP = {
     "table_space_data": "IN",
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 import sqlalchemy.dialects.mssql
 
 from pydiverse.pipedag.backend.table.sql.ddl import (
     AddIndex,
     AddPrimaryKey,
     ChangeColumnTypes,
     CreateAlias,
-    Schema,
     _mssql_update_definition,
 )
 from pydiverse.pipedag.backend.table.sql.hooks import IbisTableHook, PandasTableHook
 from pydiverse.pipedag.backend.table.sql.reflection import PipedagMSSqlReflection
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
 from pydiverse.pipedag.backend.table.util import DType
 from pydiverse.pipedag.materialize import Table
-from pydiverse.pipedag.materialize.container import RawSql
+from pydiverse.pipedag.materialize.container import RawSql, Schema
 
 
 class MSSqlTableStore(SQLTableStore):
     """
     SQLTableStore that supports `Microsoft SQL Server`_.
 
     In addition to the arguments of
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 
 import pandas as pd
 
 from pydiverse.pipedag.backend.table.sql.ddl import (
     ChangeTableLogged,
     LockSourceTable,
     LockTable,
-    Schema,
 )
 from pydiverse.pipedag.backend.table.sql.hooks import (
     PandasTableHook,
     SQLAlchemyTableHook,
 )
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
 from pydiverse.pipedag.backend.table.util import DType
 from pydiverse.pipedag.materialize import Table
+from pydiverse.pipedag.materialize.container import Schema
 from pydiverse.pipedag.materialize.details import (
     BaseMaterializationDetails,
     resolve_materialization_details_label,
 )
 
 
 @dataclass(frozen=True)
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/hooks.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 
 from pydiverse.pipedag import ConfigContext
 from pydiverse.pipedag._typing import T
 from pydiverse.pipedag.backend.table.base import AutoVersionSupport, TableHook
 from pydiverse.pipedag.backend.table.sql.ddl import (
     CreateTableAsSelect,
     InsertIntoSelect,
-    Schema,
 )
 from pydiverse.pipedag.backend.table.sql.sql import (
-    ExternalTableReference,
     SQLTableStore,
 )
 from pydiverse.pipedag.backend.table.util import (
     DType,
     PandasDTypeBackend,
 )
 from pydiverse.pipedag.context import TaskContext
 from pydiverse.pipedag.materialize import Table
+from pydiverse.pipedag.materialize.container import ExternalTableReference, Schema
 from pydiverse.pipedag.materialize.details import resolve_materialization_details_label
 from pydiverse.pipedag.util.computation_tracing import ComputationTracer
 
 # region SQLALCHEMY
 
 
 @SQLTableStore.register_table()
@@ -45,14 +44,18 @@
         )
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
         return type_ == sa.Table
 
     @classmethod
+    def retrieve_as_reference(cls, type_):
+        return True
+
+    @classmethod
     def materialize(
         cls,
         store: SQLTableStore,
         table: Table[sa.sql.expression.TextClause | sa.sql.expression.Selectable],
         stage_name,
     ):
         obj = table.obj
@@ -63,23 +66,27 @@
                 dict(
                     name=tbl.name,
                     schema=tbl.schema,
                     shared_lock_allowed=table.shared_lock_allowed,
                 )
             ]
         else:
+            try:
+                input_tables = TaskContext.get().input_tables
+            except LookupError:
+                input_tables = []
             source_tables = [
                 dict(
                     name=tbl.name,
                     schema=store.get_schema(tbl.stage.current_name).get()
                     if tbl.external_schema is None
                     else tbl.external_schema,
                     shared_lock_allowed=tbl.shared_lock_allowed,
                 )
-                for tbl in TaskContext.get().input_tables
+                for tbl in input_tables
             ]
 
         schema = store.get_schema(stage_name)
 
         store.check_materialization_details_supported(
             resolve_materialization_details_label(table)
         )
@@ -133,15 +140,19 @@
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
         as_type: type[sa.Table],
     ) -> sa.sql.expression.Selectable:
         table_name, schema = store.resolve_alias(table, stage_name)
-        alias_name = TaskContext.get().name_disambiguator.get_name(table_name)
+        try:
+            alias_name = TaskContext.get().name_disambiguator.get_name(table_name)
+        except LookupError:
+            # Used for imperative materialization with explicit config_context
+            alias_name = table_name
 
         tbl = store.reflect_table(table_name, schema)
         return tbl.alias(alias_name)
 
     @classmethod
     def lazy_query_str(cls, store, obj) -> str:
         if isinstance(obj, sa.sql.expression.FromClause):
@@ -359,17 +370,20 @@
         if PandasTableHook.pd_version >= Version("2.0"):
             # Once arrow is mature enough, we might want to switch to
             # arrow backed dataframes by default
             backend_str = "numpy"
         else:
             backend_str = "numpy"
 
-        if hook_args := ConfigContext.get().table_hook_args.get("pandas", None):
-            if dtype_backend := hook_args.get("dtype_backend", None):
-                backend_str = dtype_backend
+        try:
+            if hook_args := ConfigContext.get().table_hook_args.get("pandas", None):
+                if dtype_backend := hook_args.get("dtype_backend", None):
+                    backend_str = dtype_backend
+        except LookupError:
+            pass  # in case dematerialization is called without open ConfigContext
 
         if isinstance(as_type, tuple):
             backend_str = as_type[1]
         elif isinstance(as_type, dict):
             backend_str = as_type["backend"]
 
         backend = PandasDTypeBackend(backend_str)
@@ -758,14 +772,20 @@
     def can_retrieve(cls, type_) -> bool:
         from pydiverse.transform.eager import PandasTableImpl
         from pydiverse.transform.lazy import SQLTableImpl
 
         return issubclass(type_, (PandasTableImpl, SQLTableImpl))
 
     @classmethod
+    def retrieve_as_reference(cls, type_) -> bool:
+        from pydiverse.transform.lazy import SQLTableImpl
+
+        return issubclass(type_, SQLTableImpl)
+
+    @classmethod
     def materialize(cls, store, table: Table[pdt.Table], stage_name):
         from pydiverse.transform.core.verbs import collect
         from pydiverse.transform.eager import PandasTableImpl
         from pydiverse.transform.lazy import SQLTableImpl
 
         t = table.obj
         table = table.copy_without_obj()
@@ -847,14 +867,18 @@
         return issubclass(type_, ibis.api.Table)
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
         return issubclass(type_, ibis.api.Table)
 
     @classmethod
+    def retrieve_as_reference(cls, type_) -> bool:
+        return True
+
+    @classmethod
     def materialize(cls, store, table: Table[ibis.api.Table], stage_name):
         t = table.obj
         table = table.copy_without_obj()
         table.obj = sa.text(cls.lazy_query_str(store, t))
 
         sa_hook = store.get_hook_subclass(SQLAlchemyTableHook)
         return sa_hook.materialize(store, table, stage_name)
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/reflection.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/reflection.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/sql.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,25 @@
     CreateSchema,
     DropAlias,
     DropSchema,
     DropSchemaContent,
     DropTable,
     RenameSchema,
     RenameTable,
-    Schema,
     split_ddl_statement,
 )
 from pydiverse.pipedag.context import RunContext
 from pydiverse.pipedag.context.context import (
     CacheValidationMode,
     ConfigContext,
     StageCommitTechnique,
 )
 from pydiverse.pipedag.context.run_context import DeferredTableStoreOp
 from pydiverse.pipedag.errors import CacheError
-from pydiverse.pipedag.materialize.container import RawSql
+from pydiverse.pipedag.materialize.container import RawSql, Schema
 from pydiverse.pipedag.materialize.core import MaterializingTask
 from pydiverse.pipedag.materialize.metadata import (
     LazyTableMetadata,
     RawSqlMetadata,
     TaskMetadata,
 )
 from pydiverse.pipedag.util.hashing import stable_hash
@@ -100,21 +99,20 @@
 
        * - pydiverse.transform
          - ``pdt.Table``
          - | ``pdt.eager.PandasTableImpl``
            | ``pdt.lazy.SQLTableImpl``
 
        * - pydiverse.pipedag table reference
-         - | :py:class:`~.ExternalTableReference` (no materialization)
+         - :py:class:`~.ExternalTableReference` (no materialization)
          - Can be read with all dematerialization methods above
 
-
     :param url:
         The :external+sa:ref:`SQLAlchemy engine url <database_urls>`
-        use to connect to the database.
+        used to connect to the database.
 
         This URL may contain placeholders like ``{name}`` or ``{instance_id}``
         (additional ones can be defined in the ``url_attrs_file``) or
         environment variables like ``{$USER}`` which get substituted with their
         respective values.
 
     :param url_attrs_file:
@@ -1569,73 +1567,12 @@
     def get_engine_for_locking(self) -> sa.Engine:
         return self._create_engine()
 
     def get_lock_schema(self) -> Schema:
         return self.get_schema(self.LOCK_SCHEMA)
 
 
-class ExternalTableReference:
-    """Reference to a user-created table.
-
-    By returning a `ExternalTableReference` wrapped in a :py:class:`~.Table` from,
-    a task you can tell pipedag about a table, a view or DB2 nickname in an external
-    `schema`. The schema may be a multi-part identifier like "[db_name].[schema_name]"
-    if the database supports this. It is passed to SQLAlchemy as-is.
-
-    Only supported by :py:class:`~.SQLTableStore`.
-
-    Warning
-    -------
-    When using a `ExternalTableReference`, pipedag has no way of knowing the cache
-    validity of the external object. Hence, the user should provide a cache function
-    for the `Task`.
-    It is now allowed to specify a `ExternalTableReference` to a table in schema of the
-    current stage.
-
-    Example
-    -------
-    You can use a `ExternalTableReference` to tell pipedag about a table that exists
-    in an external schema::
-
-        @materialize(version="1.0")
-        def task():
-            return Table(ExternalTableReference("name_of_table", "schema"))
-
-    By using a cache function, you can establish the cache (in-)validity of the
-    external table::
-
-        from datetime import date
-
-        # The external table becomes cache invalid every day at midnight
-        def my_cache_fun():
-            return date.today().strftime("%Y/%m/%d")
-
-        @materialize(cache=my_cache_fun)
-        def task():
-            return Table(ExternalTableReference("name_of_table", "schema"))
-    """
-
-    def __init__(self, name: str, schema: str, shared_lock_allowed: bool = False):
-        """
-        :param name: The name of the table, view, or nickname/alias
-        :param schema: The external schema of the object. A multi-part schema
-            is allowed with '.' separator as also supported by SQLAlchemy Table
-            schema argument.
-        :param shared_lock_allowed: Whether to disable acquiring a shared lock
-            when using the object in a SQL query. If set to `False`, no lock is
-            used. This is useful when the user is not allowed to lock the table.
-            If pipedag does not lock source tables for this dialect, this argument
-            has no effect. The default is `False`.
-        """
-        self.name = name
-        self.schema = schema
-        self.shared_lock_allowed = shared_lock_allowed
-
-    def __repr__(self):
-        return f"<ExternalTableReference: {hex(id(self))}" f" (schema: {self.schema})>"
-
-
 # Load SQLTableStore Hooks
 import pydiverse.pipedag.backend.table.sql.hooks  # noqa
 
 # Load SQLTableStore dialect specific subclasses
 import pydiverse.pipedag.backend.table.sql.dialects  # noqa
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/util/dtype.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/util/dtype.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/context/context.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/context/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import annotations
 
 from collections.abc import Mapping
 from contextvars import ContextVar, Token
+from dataclasses import dataclass
 from enum import Enum
 from functools import cached_property
 from threading import Lock
 from typing import TYPE_CHECKING, ClassVar
 
 import structlog
 from attrs import define, evolve, field, frozen
 from box import Box
 
 from pydiverse.pipedag.util import deep_merge
 from pydiverse.pipedag.util.import_ import import_object, load_object
 from pydiverse.pipedag.util.naming import NameDisambiguator
 
 if TYPE_CHECKING:
+    from pydiverse.pipedag import Flow, GroupNode, Stage, Task, VisualizationStyle
     from pydiverse.pipedag._typing import T
     from pydiverse.pipedag.backend import BaseLockManager
     from pydiverse.pipedag.context.run_context import StageLockStateHandler
-    from pydiverse.pipedag.core import Flow, Stage, Task
     from pydiverse.pipedag.engine.base import OrchestrationEngine
     from pydiverse.pipedag.materialize import Table
 
 
 class BaseContext:
     _context_var: ClassVar[ContextVar]
     _token: Token = None
@@ -76,14 +77,15 @@
 
 @frozen
 class DAGContext(BaseAttrsContext):
     """Context during DAG definition"""
 
     flow: Flow
     stage: Stage
+    group_node: GroupNode
 
     _context_var = ContextVar("dag_context")
 
 
 @define
 class TaskContext(BaseContext):
     """Context used while executing a task
@@ -93,14 +95,15 @@
     """
 
     task: Task
     input_tables: list[Table] = None
     is_cache_valid: bool | None = None
     name_disambiguator: NameDisambiguator = field(factory=NameDisambiguator)
     override_version: str | None = None
+    imperative_materialize_callback = None
 
     _context_var = ContextVar("task_context")
 
 
 class StageCommitTechnique(Enum):
     """
     - SCHEMA_SWAP: We prepare output in a `<stage>__tmp` schema and then swap
@@ -132,14 +135,28 @@
     NORMAL = 0
     ASSERT_NO_FRESH_INPUT = 1
     IGNORE_FRESH_INPUT = 2
     FORCE_FRESH_INPUT = 3
     FORCE_CACHE_INVALID = 4
 
 
+@dataclass(frozen=True)
+class GroupNodeConfig:
+    label: str | None = None
+    tasks: list[str] | None = None
+    stages: list[str] | None = None
+    style_tag: str | None = None
+
+
+@dataclass(frozen=True)
+class VisualizationConfig:
+    styles: dict[str, VisualizationStyle] | None = None
+    group_nodes: dict[str, GroupNodeConfig] | None = None
+
+
 @frozen(slots=False)
 class ConfigContext(BaseAttrsContext):
     """Configuration context for running a particular pipedag instance.
 
     To create a `ConfigContext` instance use :py:meth:`PipedagConfig.get`.
 
     ..
@@ -184,14 +201,15 @@
 
     # per instance attributes
     fail_fast: bool
     strict_result_get_locking: bool
     instance_id: str  # may be used as database name or locking ID
     stage_commit_technique: StageCommitTechnique
     cache_validation: Box
+    visualization: dict[str, VisualizationConfig]
     network_interface: str
     disable_kroki: bool
     kroki_url: str | None
     attrs: Box
 
     table_hook_args: Box
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/context/run_context.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/context/run_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -774,15 +774,14 @@
 
 class FinalTaskState(Enum):
     UNKNOWN = 0
 
     COMPLETED = 1
     CACHE_VALID = 2
     FAILED = 10
-    SKIPPED = 20
 
     def is_successful(self) -> bool:
         return self in (FinalTaskState.COMPLETED, FinalTaskState.CACHE_VALID)
 
     def is_failure(self) -> bool:
         return self in (FinalTaskState.FAILED,)
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/config.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,19 @@
 from typing import TYPE_CHECKING, Any
 
 import sqlalchemy as sa
 import structlog
 import yaml
 from box import Box
 
-from pydiverse.pipedag.context.context import CacheValidationMode
+from pydiverse.pipedag.context.context import (
+    CacheValidationMode,
+    GroupNodeConfig,
+    VisualizationConfig,
+)
 from pydiverse.pipedag.util.deep_merge import deep_merge
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.context import ConfigContext
 
 
 # noinspection PyPep8Naming
@@ -178,14 +182,42 @@
             StageCommitTechnique, config["stage_commit_technique"]
         )
         cache_validation = copy.deepcopy(config["cache_validation"])
         cache_validation["mode"] = getattr(
             CacheValidationMode, config["cache_validation"]["mode"]
         )
 
+        # parsing visualization dictionaries into objects (this could be generalized
+        # and possible an open source solution exists)
+        from pydiverse.pipedag import VisualizationStyle
+
+        if not isinstance(config.get("visualization", {}), dict):
+            raise ValueError(
+                "Config section 'visualization' must be a dictionary, "
+                f"found {type(config['visualization'])}"
+            )
+        visualization = {}
+        for key, value in config.get("visualization", {}).items():
+            self.parse_in_object(
+                key, value, VisualizationConfig, "visualization", inout=visualization
+            )
+            for field, structure, class_type in [
+                ("styles", visualization[key].styles, VisualizationStyle),
+                ("group_nodes", visualization[key].group_nodes, GroupNodeConfig),
+            ]:
+                if structure:
+                    for key2, value2 in structure.items():
+                        self.parse_in_object(
+                            key2,
+                            value2,
+                            class_type,
+                            f"visualization.{key}.{field}",
+                            inout=structure,
+                        )
+
         if (
             cache_validation["mode"] == CacheValidationMode.NORMAL
             and cache_validation["disable_cache_function"]
         ):
             raise ValueError(
                 "cache_validation.disable_cache_function=True is not allowed in "
                 "combination with cache_validation.mode=NORMAL"
@@ -232,14 +264,15 @@
             flow_name=flow,
             instance_name=instance,
             fail_fast=config["fail_fast"],
             strict_result_get_locking=config["strict_result_get_locking"],
             instance_id=config["instance_id"],
             stage_commit_technique=stage_commit_technique,
             cache_validation=Box(cache_validation, frozen_box=True),
+            visualization=visualization,
             network_interface=config["network_interface"],
             disable_kroki=config.get("disable_kroki"),
             kroki_url=config.get("kroki_url"),
             attrs=Box(config["attrs"], frozen_box=True),
             table_hook_args=Box(
                 config["table_store"].get("hook_args", {}), frozen_box=True
             ),
@@ -261,14 +294,61 @@
                 raise RuntimeError(
                     "Error while creating backend objects from pipedag config "
                     f"(instance={instance}, flow={flow}): {self.path}"
                 ) from e
 
         return config_context
 
+    @staticmethod
+    def parse_in_object(
+        key: str,
+        value: dict[str, Any],
+        class_type: Any,
+        within: str,
+        *,
+        inout: dict[str, Any],
+    ):
+        structure = inout
+        if not isinstance(value, dict):
+            raise ValueError(
+                f"Config section '{key}' within '{within}' must be a dictionary, "
+                f"found {type(value)}"
+            )
+        members = set(class_type.__dataclass_fields__.keys())
+        if unexpected := set(value.keys()) - members:
+            raise ValueError(
+                f"Unexpected keys in section '{key}' within '{within}': "
+                f"{unexpected}; expected: '{', '.join(members)}'"
+            )
+        structure[key] = class_type(
+            **{m: copy.copy(value[m]) for m in members if m in value}
+        )
+        for m in value:
+            annotation = class_type.__annotations__[m]
+            if annotation.startswith("dict[") and not isinstance(value[m], dict):
+                raise ValueError(
+                    f"Expected dictionary for '{m}' within '{within}.{key}', "
+                    f"found {type(value[m])}"
+                )
+            if annotation.startswith("bool") and not isinstance(value[m], bool):
+                raise ValueError(
+                    f"Expected boolean for '{m}' within '{within}.{key}', "
+                    f"found {type(value[m])}"
+                )
+            if annotation.startswith("str") and not isinstance(value[m], str):
+                raise ValueError(
+                    f"Expected string for '{m}' within '{within}.{key}', "
+                    f"found {type(value[m])}"
+                )
+            if annotation.startswith("int") and not isinstance(value[m], int):
+                raise ValueError(
+                    f"Expected integer for '{m}' within '{within}.{key}', "
+                    f"found {type(value[m])}"
+                )
+
     def __get_merged_config_dict(self, instance, flow, default=None):
         search_paths = [
             ("instances", "__any__"),
             ("instances", instance),
             ("flows", "__any__"),
             ("flows", "__any__", "instances", instance),
             ("flows", flow),
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/result.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/result.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,18 @@
             successful=successful,
             config_context=ConfigContext.get(),
             task_values=task_values,
             task_states=RunContext.get().get_task_states(),
             exception=exception,
         )
 
+    def evolve(self, **changes):
+        kwargs = {**dir(self), **changes}
+        return Result(**kwargs)
+
     def get(self, task: Task | TaskGetItem, as_type: type = None) -> Any:
         """Retrieve the output produced by a task.
 
         Any tables and blobs returned by a task get loaded from their
         corresponding store.
 
         If :ref:`strict_result_get_locking` is set to True, this call, as well as
@@ -109,24 +113,24 @@
         else:
             task_output = self.task_values[task.task]
 
         with self.config_context, DematerializeRunContext(self.flow):
             store = self.config_context.store
             return dematerialize_output_from_store(store, task, task_output, as_type)
 
-    def visualize(self):
+    def visualize(self, visualization_tag: str | None = None):
         """
         Wrapper for :py:meth:`Flow.visualize()`.
         """
-        return self.subflow.visualize(result=self)
+        return self.subflow.visualize(self, visualization_tag)
 
-    def visualize_url(self) -> str:
+    def visualize_url(self, visualization_tag: str | None = None) -> str:
         """
         Wrapper for :py:meth:`Flow.visualize_url()`.
         """
-        return self.subflow.visualize_url(result=self)
+        return self.subflow.visualize_url(self, visualization_tag)
 
-    def visualize_pydot(self) -> pydot.Dot:
+    def visualize_pydot(self, visualization_tag: str | None = None) -> pydot.Dot:
         """
         Wrapper for :py:meth:`Flow.visualize_pydot()`.
         """
-        return self.subflow.visualize_pydot(result=self)
+        return self.subflow.visualize_pydot(self, visualization_tag)
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/stage.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/stage.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from pydiverse.pipedag.context import ConfigContext, DAGContext
 from pydiverse.pipedag.core.task import Task
 from pydiverse.pipedag.errors import StageError
 from pydiverse.pipedag.util import normalize_name
 
 if TYPE_CHECKING:
-    from pydiverse.pipedag.core.flow import Flow
+    from pydiverse.pipedag import Flow, GroupNode
 
 
 class Stage:
     """A stage represents a collection of related tasks.
 
     The main purpose of a Stage is to allow for a transactionality mechanism.
     Only if all tasks inside a stage finish successfully does the stage
@@ -36,26 +36,34 @@
         for each of its upstream dependencies, the associated StageCommitTask
         must be added as an upstream dependency.
         This ensures that the stage commit only happens after all tasks have
         finished writing to the transaction stage, and a task never gets executed
         before any of its upstream stage dependencies have been committed.
     """
 
-    def __init__(self, name: str, materialization_details: str | None = None):
+    def __init__(
+        self,
+        name: str,
+        materialization_details: str | None = None,
+        group_node_tag: str | None = None,
+    ):
         self._name = normalize_name(name)
         self._transaction_name = f"{self._name}__tmp"
 
         self.tasks: list[Task] = []
         self.commit_task: CommitStageTask = None  # type: ignore
+        self.barrier_tasks: list[Task] = []
         self.outer_stage: Stage | None = None
+        self.outer_group_node: GroupNode | None = None
 
         self.logger = structlog.get_logger(logger_name=type(self).__name__, stage=self)
         self.id: int = None  # type: ignore
 
         self.materialization_details = materialization_details
+        self.group_node_tag = group_node_tag
 
         self._did_enter = False
 
     @property
     def name(self) -> str:
         """The name of the stage."""
         return self._name
@@ -92,14 +100,15 @@
     def __repr__(self):
         return f"<Stage: {self.name}>"
 
     def __getstate__(self):
         state = self.__dict__.copy()
         state.pop("tasks", None)
         state.pop("commit_task", None)
+        state.pop("barrier_tasks", None)
         state.pop("logger", None)
         return state
 
     def __enter__(self):
         if self._did_enter:
             raise StageError(
                 f"Stage '{self.name}' has already been entered."
@@ -113,21 +122,25 @@
             outer_ctx = DAGContext.get()
         except LookupError as e:
             raise StageError("Stage can't be defined outside of a flow") from e
 
         outer_ctx.flow.add_stage(self)
         if outer_ctx.stage is not None:
             self.outer_stage = outer_ctx.stage
+        if outer_ctx.group_node is not None:
+            self.outer_group_node = outer_ctx.group_node
+            outer_ctx.group_node.add_stage(self)
 
         # Initialize new context (both Flow and Stage use DAGContext to transport
         # information to @materialize annotations within the flow and to support
         # nesting of stages)
         self._ctx = DAGContext(
             flow=outer_ctx.flow,
             stage=self,
+            group_node=outer_ctx.group_node,
         )
         self._ctx.__enter__()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.commit_task = CommitStageTask(self, self._ctx.flow)
         self._ctx.__exit__()
@@ -181,14 +194,15 @@
             f"Found only {len(tasks)} instances of task '{name}' in stage, "
             f"but you requested the tasks with index {index}, "
             "which is out of bounds."
         )
 
     def all_tasks(self):
         yield from self.tasks
+        yield from self.barrier_tasks
         yield self.commit_task
 
     def is_inner(self, other: Stage):
         outer = self.outer_stage
         while outer is not None:
             if outer == other:
                 return True
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/task.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,28 +30,30 @@
         for unpacking the outputs of a task.
     """
 
     def __init__(
         self,
         fn: Callable,
         *,
-        name: str = None,
-        nout: int = None,
+        name: str | None = None,
+        nout: int | None = None,
+        group_node_tag: str | None = None,
     ):
         if not callable(fn):
             raise TypeError("`fn` must be callable")
         if nout is not None and (nout <= 0 or not isinstance(nout, int)):
             raise ValueError("`nout` must be a positive integer")
 
         if name is None:
             name = getattr(fn, "__name__", type(self).__name__)
 
         self.fn = fn
         self.name = name
         self.nout = nout
+        self.group_node_tag = group_node_tag
 
         self._bound_task_type = Task
         self._signature = inspect.signature(fn)
 
     def __repr__(self):
         return f"<UnboundTask 'name' {hex(id(self))}>"
 
@@ -69,15 +71,19 @@
             return self._call_original_function(*args, **kwargs)
 
         if ctx.stage is None:
             raise StageError("Can't call pipedag task outside of a stage.")
 
         # Construct Task
         bound_args = self._signature.bind(*args, **kwargs)
-        return self._bound_task_type(self, bound_args, ctx.flow, ctx.stage)
+        task = self._bound_task_type(self, bound_args, ctx.flow, ctx.stage)
+        if ctx.group_node is not None:
+            ctx.group_node.add_task(task)
+            task.group_node = ctx.group_node
+        return task
 
     def _call_original_function(self, *args, **kwargs):
         return self.fn(*args, **kwargs)
 
 
 class Task:
     def __init__(
@@ -86,20 +92,22 @@
         bound_args: inspect.BoundArguments,
         flow: Flow,
         stage: Stage,
     ):
         self.fn = unbound_task.fn
         self.name = unbound_task.name
         self.nout = unbound_task.nout
+        self.group_node_tag = unbound_task.group_node_tag
 
         self.logger = structlog.get_logger(logger_name=f"Task '{self.name}'", task=self)
 
         self._bound_args = bound_args
         self.flow = flow
         self.stage = stage
+        self.group_node = None  # will be set by UnboundTask.__call__
         self.position_hash = self.__compute_position_hash()
 
         # The ID gets set by calling flow.add_task
         self.id: int = None  # type: ignore
 
         # Do the wiring
         self.flow.add_task(self)
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/base.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/dask.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/dask.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 run_context=run_context,
                 config_context=config_context,
             )
 
         try:
             results = dask.compute(results, **self.dask_compute_kwargs)[0]
         except Exception as e:
-            if run_kwargs.get("fail_fast", False):
+            if config_context.fail_fast:
                 raise e
             exception = e
 
         return Result.init_from(
             subflow=flow,
             underlying=results,
             successful=(exception is None),
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/prefect.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/prefect.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/errors/__init__.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/errors/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 
 class StageError(Exception):
     """
     Exception raised when something is wrong with the stage.
     """
 
 
+class GroupNodeError(Exception):
+    """
+    Exception raised when something is wrong with the stage.
+    """
+
+
 class CacheError(Exception):
     """
     Exception raised if something couldn't be retrieved from the cache.
     """
 
 
 class LockError(Exception):
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/cli.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/cli.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/commands/clear_metadata.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/commands/clear_metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/commands/delete_schemas.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/commands/delete_schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import click
 import sqlalchemy as sa
 
 from pydiverse.pipedag import PipedagConfig
 from pydiverse.pipedag.backend.table import SQLTableStore
-from pydiverse.pipedag.backend.table.sql.ddl import DropSchema, Schema
+from pydiverse.pipedag.backend.table.sql.ddl import DropSchema
 from pydiverse.pipedag.management.cli import cli
+from pydiverse.pipedag.materialize.container import Schema
 
 
 @cli.command()
 @click.option(
     "--config",
     "config_path",
     type=str,
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/core.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
 import copy
 import functools
 import inspect
 import uuid
+from collections.abc import Callable, Iterable
 from functools import partial
-from typing import TYPE_CHECKING, Any, Callable, overload
+from typing import TYPE_CHECKING, Any, overload
+
+import sqlalchemy as sa
 
 from pydiverse.pipedag._typing import CallableT
 from pydiverse.pipedag.context import ConfigContext, RunContext, TaskContext
 from pydiverse.pipedag.context.context import CacheValidationMode
 from pydiverse.pipedag.core.task import Task, TaskGetItem, UnboundTask
 from pydiverse.pipedag.errors import CacheError
 from pydiverse.pipedag.materialize.cache import TaskCacheInfo, task_cache_key
@@ -26,37 +29,38 @@
     from pydiverse.pipedag.backend.table.base import TableHook
     from pydiverse.pipedag.materialize.store import PipeDAGStore
 
 
 @overload
 def materialize(
     *,
-    name: str = None,
-    input_type: type | tuple | dict[str, Any] = None,
-    version: str = None,
-    cache: Callable = None,
+    name: str | None = None,
+    input_type: type | tuple | dict[str, Any] | None = None,
+    version: str | None = None,
+    cache: Callable[[Any], Any] | None = None,
     lazy: bool = False,
     nout: int = 1,
 ) -> Callable[[CallableT], CallableT | UnboundMaterializingTask]:
     ...
 
 
 @overload
 def materialize(fn: CallableT, /) -> CallableT | UnboundMaterializingTask:
     ...
 
 
 def materialize(
-    fn: CallableT = None,
+    fn: CallableT | None = None,
     *,
-    name: str = None,
-    input_type: type | tuple | dict[str, Any] = None,
-    version: str = None,
-    cache: Callable = None,
+    name: str | None = None,
+    input_type: type | tuple | dict[str, Any] | None = None,
+    version: str | None = None,
+    cache: Callable[[Any], Any] | None = None,
     lazy: bool = False,
+    group_node_tag: str | None = None,
     nout: int = 1,
 ):
     """Decorator to create a task whose outputs get materialized.
 
     This decorator takes a class and turns it into a :py:class:`MaterializingTask`.
     This means, that this function can only be used as part of a flow.
     Any outputs it produces get written to their appropriate storage backends
@@ -109,14 +113,16 @@
         task produces a lazy table (e.g. a SQL query), the table store checks if
         the same query has been executed before. If this is the case, then the
         query doesn't get executed, and instead, the table gets copied from the cache.
 
         This behaviour is very useful, because you don't need to manually bump
         the `version` of a lazy task. This only works because for lazy tables
         generating the query is very cheap compared to executing it.
+    :param group_node_tag:
+        Set a tag that may add this task to a configuration based group node.
     :param nout:
         The number of objects returned by the task.
         If set, this allows unpacking and iterating over the results from the task.
 
     Example
     -------
 
@@ -124,15 +130,15 @@
 
         @materialize(version="1.0", input_type=pd.DataFrame)
         def task(df: pd.DataFrame) -> pd.DataFrame:
             df = ...  # Do something with the dataframe
             return Table(df)
 
         @materialize(lazy=True, input_type=sa.Table)
-        def lazy_task(tbl: sa.Table) -> sa.Table:
+        def lazy_task(tbl: sa.Alias) -> sa.Table:
             query = sa.select(tbl).where(...)
             return Table(query)
 
     You can use the `cache` argument to specify an explicit cache function.
     In this example we define a task that reads a dataframe from a csv file.
     Without specifying a cache function, this task would only get rerun when the
     `path` argument changes. Instead, we define a function that calculates a
@@ -181,24 +187,26 @@
         return partial(
             materialize,
             name=name,
             input_type=input_type,
             version=version,
             cache=cache,
             lazy=lazy,
+            group_node_tag=group_node_tag,
             nout=nout,
         )
 
     return UnboundMaterializingTask(
         fn,
         name=name,
         input_type=input_type,
         version=version,
         cache=cache,
         lazy=lazy,
+        group_node_tag=group_node_tag,
         nout=nout,
     )
 
 
 class UnboundMaterializingTask(UnboundTask):
     """A materializing task without any bound arguments.
 
@@ -245,19 +253,20 @@
 
     """
 
     def __init__(
         self,
         fn: Callable,
         *,
-        name: str = None,
-        input_type: type = None,
-        version: str = None,
-        cache: Callable = None,
+        name: str | None = None,
+        input_type: type | None = None,
+        version: str | None = None,
+        cache: Callable[[Any], Any] | None = None,
         lazy: bool = False,
+        group_node_tag: str | None = None,
         nout: int = 1,
     ):
         super().__init__(
             MaterializationWrapper(fn),
             name=name,
             nout=nout,
         )
@@ -265,14 +274,15 @@
         self._bound_task_type = MaterializingTask
         self._original_fn = fn
 
         self.input_type = input_type
         self.version = version
         self.cache = cache
         self.lazy = lazy
+        self.group_node_tag = group_node_tag
 
         if version is AUTO_VERSION:
             if input_type is None:
                 # The input_type is used to determine which type of auto versioning
                 # to use (either not supported, lazy or tracing)
                 raise ValueError("Auto-versioning task must specify an input type")
             if lazy:
@@ -280,18 +290,35 @@
                     "Task can't be lazy and auto-versioning at the same time"
                 )
 
     def __call__(self, *args, **kwargs) -> MaterializingTask:
         return super().__call__(*args, **kwargs)  # type: ignore
 
     def _call_original_function(self, *args, **kwargs):
+        try:
+            task_context = TaskContext.get()  # this may raise Lookup Error
+            # this is a subtask call. Thus we demand identical input_types
+            sub_task: MaterializingTask = task_context.task  # type: ignore
+            if (
+                sub_task.input_type is not None
+                and self.input_type is not None
+                and sub_task.input_type != self.input_type
+            ):
+                raise RuntimeError(
+                    f"Subtask input type {self.input_type} does not match parent task "
+                    f"input type {sub_task.input_type}: "
+                    f"task={self}, sub_task={sub_task}"
+                )
+        except LookupError:
+            # this is expected when calling the task outside of flow declaration
+            pass
         result = self._original_fn(*args, **kwargs)
 
         def unwrap_mutator(x):
-            if isinstance(x, (Task, Blob)):
+            if isinstance(x, (Table, Blob)):
                 return x.obj
             if isinstance(x, RawSql):
                 return x.sql
             return x
 
         return deep_map(result, unwrap_mutator)
 
@@ -567,19 +594,29 @@
                     cached_output, cache_metadata = store.retrieve_cached_output(
                         task, input_hash, cache_fn_hash
                     )
                     store.copy_cached_output_to_transaction_stage(
                         cached_output, cache_metadata, task
                     )
                     run_context.store_task_memo(task, memo_cache_key, cached_output)
-                    task.logger.info("Found task in cache. Using cached result.")
+                    task.logger.info(
+                        "Found task in cache. Using cached result.",
+                        input_hash=input_hash,
+                        cache_fn_hash=cache_fn_hash,
+                    )
                     TaskContext.get().is_cache_valid = True
                     return cached_output
                 except CacheError as e:
-                    task.logger.info("Failed to retrieve task from cache", cause=str(e))
+                    task.logger.info(
+                        "Failed to retrieve task from cache",
+                        input_hash=input_hash,
+                        cache_fn_hash=cache_fn_hash,
+                        version=task.version,
+                        cause=str(e),
+                    )
                     TaskContext.get().is_cache_valid = False
 
             if not task.lazy:
                 if assert_no_fresh_input and task.cache is not None:
                     raise AssertionError(
                         "cache_validation.mode=ASSERT_NO_FRESH_INPUT is a "
                         "protection mechanism to prevent execution of "
@@ -604,15 +641,19 @@
                     try:
                         _, cache_metadata = store.retrieve_cached_output(
                             task, input_hash, ""
                         )
                         cache_fn_hash = cache_metadata.cache_fn_hash
                     except CacheError as e:
                         task.logger.info(
-                            "Failed to retrieve task from cache", cause=str(e)
+                            "Failed to retrieve lazy task from cache",
+                            cause=str(e),
+                            input_hash=input_hash,
+                            version=task.version,
+                            cache_fn_hash=cache_fn_hash,
                         )
 
             # Prepare TaskCacheInfo
             if not task.lazy and skip_cache_lookup:
                 # Assign random version to disable caching for this task
                 task = copy.copy(task)
                 task.version = uuid.uuid4().hex
@@ -638,28 +679,96 @@
             task_context.input_tables = input_tables
 
             # Not found in cache / lazy -> Evaluate Function
             args, kwargs = store.dematerialize_task_inputs(
                 task, bound.args, bound.kwargs
             )
 
+            def imperative_materialize(
+                table: Table,
+                config_context: ConfigContext | None,
+                return_as_type: type | None = None,
+                return_nothing: bool = False,
+            ):
+                my_store = config_context.store if config_context is not None else store
+                state = task_cache_info.imperative_materialization_state
+                if id(table) in state.table_ids:
+                    raise RuntimeError(
+                        "The table has already been imperatively materialized."
+                    )
+                table.assumed_dependencies = (
+                    list(state.assumed_dependencies)
+                    if len(state.assumed_dependencies) > 0
+                    else []
+                )
+                _ = my_store.materialize_task(
+                    task, task_cache_info, table, disable_task_finalization=True
+                )
+                if not return_nothing:
+
+                    def get_return_obj(return_as_type):
+                        if return_as_type is None:
+                            return_as_type = task.input_type
+                            if (
+                                return_as_type is None
+                                or not my_store.table_store.get_r_table_hook(
+                                    return_as_type
+                                ).retrieve_as_reference(return_as_type)
+                            ):
+                                # dematerialize as sa.Table if it would transfer all
+                                # rows to python when dematerializing with input_type
+                                return_as_type = sa.Table
+                        obj = my_store.dematerialize_item(
+                            table, return_as_type, run_context
+                        )
+                        state.add_table_lookup(obj, table)
+                        return obj
+
+                    if isinstance(return_as_type, Iterable):
+                        return tuple(get_return_obj(t) for t in return_as_type)
+                    else:
+                        return get_return_obj(return_as_type)
+
+            task_context.imperative_materialize_callback = imperative_materialize
             result = self.fn(*args, **kwargs)
+            task_context.imperative_materialize_callback = None
             if task.debug_tainted:
                 raise RuntimeError(
                     f"The task {task.name} has been tainted by interactive debugging."
                     f" Aborting."
                 )
+
+            def result_finalization_mutator(x):
+                state = task_cache_info.imperative_materialization_state
+                object_lookup = state.object_lookup
+                if id(x) in object_lookup:
+                    # substitute imperatively materialized object references with
+                    # their respective table objects
+                    x = object_lookup[id(x)]
+                if isinstance(x, (Table, RawSql)):
+                    # fill assumed_dependencies for Tables that were not yet
+                    # materialized
+                    if len(state.assumed_dependencies) > 0:
+                        if x.assumed_dependencies is None:
+                            x.assumed_dependencies = list(state.assumed_dependencies)
+                return x
+
+            result = deep_map(result, result_finalization_mutator)
             result = store.materialize_task(task, task_cache_info, result)
 
             # Delete underlying objects from result (after materializing them)
             def obj_del_mutator(x):
                 if isinstance(x, (Table, Blob)):
                     x.obj = None
                 if isinstance(x, RawSql):
                     x.loaded_tables = None
+                if isinstance(x, (Table, RawSql)):
+                    x.assumed_dependencies = deep_map(
+                        x.assumed_dependencies, obj_del_mutator
+                    )
                 return x
 
             result = deep_map(result, obj_del_mutator)
             run_context.store_task_memo(task, memo_cache_key, result)
             self.value = result
 
             return result
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/debug.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/debug.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,73 +4,108 @@
 
 import structlog
 
 from pydiverse.pipedag import ConfigContext, Table
 from pydiverse.pipedag.backend import SQLTableStore
 from pydiverse.pipedag.backend.table.sql.ddl import DropTable
 from pydiverse.pipedag.context import TaskContext
+from pydiverse.pipedag.materialize.container import Schema
 from pydiverse.pipedag.materialize.core import MaterializingTask
 from pydiverse.pipedag.materialize.store import mangle_table_name
 from pydiverse.pipedag.util.hashing import stable_hash
 
 
 def materialize_table(
     table: Table,
+    config_context: ConfigContext | None = None,
+    schema: Schema | str | None = None,
     debug_suffix: str | None = None,
     flag_task_debug_tainted: bool = True,
     keep_table_name: bool = True,
     drop_if_exists: bool = True,
 ):
     """
     This function allows the user to materialize a table ad-hoc
     whenever the TaskContext is defined.
     This can be useful during interactive debugging.
     If table.name is not given, then it is derived from the task name and a suffix.
     The suffix is either the debug_suffix (if given) or a random suffix.
     If the table name ends in %%, the %% are also replaced by a suffix.
 
     :param table: The table to be materialized.
+    :param config_context: The config context to be used for materialization.
+        If None, the current config context is used. Default: None
+    :param schema: The schema to be used for writing table. If None, the
+        schema is derived from the table's stage. Default: None
     :param debug_suffix: A suffix to be appended to the table name
         for debugging purposes. Default: None
     :param flag_task_debug_tainted: Whether to flag the task as tainted
         by this debug materialization. The flag will cause an exception if execution is
         continued. Default: True
     :param keep_table_name: if False, the table.name will be equal to the debug name
         after return. Otherwise, the original name of the table is preserved.
         Default: True
     :param drop_if_exists: If True, try to drop the table (if exists) before recreating.
         This is only supported for SQL table stores.
     """
-    config_context = ConfigContext.get()
+    if config_context is None:
+        config_context = ConfigContext.get()
     table_store = config_context.store.table_store
 
-    task_context = TaskContext.get()
-    task: MaterializingTask = task_context.task  # type: ignore
-
-    table.stage = task.stage
+    task: MaterializingTask | None = None
+    try:
+        task_context = TaskContext.get()
+        task = task_context.task  # type: ignore
+        task_name = task.name
+
+        table.stage = task.stage
+        if schema is None:
+            schema = table_store.get_schema(table.stage.transaction_name)
+    except LookupError:
+        task_name = None
+        # LookupError happens if no TaskContext is open
+        if schema is None:
+            raise ValueError(
+                "Parameter schema must be provided if task is not called by "
+                "normal pipedag orchestration."
+            ) from None
 
     suffix = (
         stable_hash(str(random.randbytes(8))) + "_0000" if debug_suffix is None else ""
     )
     old_table_name = table.name
-    table.name = mangle_table_name(table.name, task.name, suffix)
+    table.name = mangle_table_name(table.name, task_name, suffix)
     if debug_suffix is not None:
         table.name += debug_suffix
 
-    if flag_task_debug_tainted:
+    if flag_task_debug_tainted and task is not None:
         task.debug_tainted = True
 
     if drop_if_exists:
         if isinstance(table_store, SQLTableStore):
-            schema = table_store.get_schema(task.stage.transaction_name)
             table_store.execute(DropTable(table.name, schema, if_exists=True))
         else:
             logger = structlog.get_logger(logger_name="Debug materialize_table")
             logger.warning(
                 "drop_if_exists not supported for non SQLTableStore table stores."
             )
-    table_store.store_table(table, task)
+    if task is None:
+        hook = table_store.get_m_table_hook(type(table.obj))
+        schema_name = (
+            schema.name
+            if table_store.get_schema(schema.name).get() == schema.get()
+            else schema.get()
+        )
+        if table_store.get_schema(schema_name).get() != schema.get():
+            raise ValueError(
+                "Schema prefix and postfix must match prefix and postfix of provided "
+                "config_context: "
+                f"{table_store.get_schema(schema_name).get()} != {schema.get()}"
+            )
+        hook.materialize(table_store, table, schema_name)
+    else:
+        table_store.store_table(table, task)
 
     new_table_name = table.name
     if keep_table_name:
         table.name = old_table_name
     return new_table_name
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/details.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/details.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/metadata.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/store.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import itertools
 from datetime import datetime
 from typing import Any, Callable
 
 import structlog
 
 from pydiverse.pipedag import Blob, Stage, Table, backend
 from pydiverse.pipedag._typing import Materializable, T
@@ -184,14 +183,15 @@
         return d_args, d_kwargs
 
     def materialize_task(
         self,
         task: MaterializingTask,
         task_cache_info: TaskCacheInfo,
         value: Materializable,
+        disable_task_finalization=False,
     ) -> Materializable:
         """Stores the output of a task in the backend
 
         Traverses the output produced by a task, adds missing metadata,
         materializes all `Table` and `Blob` objects and returns a new
         output object with the required metadata to allow dematerialization.
 
@@ -199,14 +199,16 @@
             the correct `cache_key` attribute set.
         :param task_cache_info: Task cache information.
         :param value: The output of the task. Must be materializable; this
             means it can only contain the following object types:
             `dict`, `list`, `tuple`,
             `int`, `float`, `str`, `bool`, `None`,
             and PipeDAG's `Table` and `Blob` type.
+        :param disable_task_finalization: True for imperative materialization
+            when task is not finished, yet.
         :return: A copy of `value` with additional metadata
         """
 
         stage = task.stage
         ctx = RunContext.get()
 
         if (state := ctx.get_stage_state(stage)) != StageState.READY:
@@ -221,27 +223,28 @@
 
         def store_metadata():
             """
             Metadata must be generated after everything else has been materialized,
             because during materialization the cache_key of the different objects
             can get changed.
             """
-            output_json = self.json_encode(value)
-            metadata = TaskMetadata(
-                name=task.name,
-                stage=task.stage.name,
-                version=task.version,
-                timestamp=datetime.now(),
-                run_id=ctx.run_id,
-                position_hash=task.position_hash,
-                input_hash=task_cache_info.input_hash,
-                cache_fn_hash=task_cache_info.cache_fn_hash,
-                output_json=output_json,
-            )
-            self.table_store.store_task_metadata(metadata, stage)
+            if not disable_task_finalization:
+                output_json = self.json_encode(value)
+                metadata = TaskMetadata(
+                    name=task.name,
+                    stage=task.stage.name,
+                    version=task.version,
+                    timestamp=datetime.now(),
+                    run_id=ctx.run_id,
+                    position_hash=task.position_hash,
+                    input_hash=task_cache_info.input_hash,
+                    cache_fn_hash=task_cache_info.cache_fn_hash,
+                    output_json=output_json,
+                )
+                self.table_store.store_task_metadata(metadata, stage)
 
         def store_table(table: Table):
             if task.lazy:
                 self.table_store.store_table_lazy(table, task, task_cache_info)
             else:
                 self.table_store.store_table(table, task)
 
@@ -269,15 +272,17 @@
         value: Materializable,
     ) -> tuple[Materializable, list[Table], list[RawSql], list[Blob]]:
         tables = []
         raw_sqls = []
         blobs = []
 
         config = ConfigContext.get()
-        auto_suffix_counter = itertools.count()
+        auto_suffix_counter = (
+            task_cache_info.imperative_materialization_state.auto_suffix_counter
+        )
 
         def preparation_mutator(x):
             # Automatically convert an object to a table / blob if its
             # type is inside either `config.auto_table` or `.auto_blob`.
             if isinstance(x, config.auto_table):
                 try:
                     hook = self.table_store.get_m_table_hook(type(x))
@@ -290,27 +295,31 @@
             if isinstance(x, PipedagConfig):
                 # Config objects are not an allowed return type,
                 # because they might mess up caching.
                 raise TypeError(
                     "You can't return a PipedagConfig object from a materializing task."
                 )
 
-            # Add missing metadata
-            if isinstance(x, (Table, RawSql, Blob)):
+            # Add missing metadata (if table was not already imperatively materialized)
+            if (
+                isinstance(x, (Table, RawSql, Blob))
+                and id(x)
+                not in task_cache_info.imperative_materialization_state.table_ids
+            ):
                 if not task.lazy:
                     # task cache_key is output cache_key for eager tables
                     x.cache_key = task_cache_info.cache_key
 
                 x.stage = task.stage
 
                 # Update name:
                 # - If no name has been provided, generate on automatically
                 # - If the provided name ends with %%, perform name mangling
                 object_number = next(auto_suffix_counter)
-                auto_suffix = f"{task_cache_info.cache_key}" f"_{object_number:04d}"
+                auto_suffix = f"{task_cache_info.cache_key}_{object_number:04d}"
 
                 x.name = mangle_table_name(x.name, task.name, auto_suffix)
 
                 if isinstance(x, Table):
                     if x.obj is None:
                         raise TypeError("Underlying table object can't be None")
                     tables.append(x)
@@ -569,13 +578,15 @@
             task_output,
             lambda item: store.dematerialize_item(
                 item, as_type=as_type, ctx=run_context
             ),
         )
 
 
-def mangle_table_name(table_name: str, task_name: str, suffix: str):
+def mangle_table_name(table_name: str, task_name: str | None, suffix: str):
     if table_name is None:
+        if task_name is None:
+            return suffix
         table_name = task_name + "_" + suffix
     elif table_name.endswith("%%"):
         table_name = table_name[:-2] + suffix
     return table_name
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/computation_tracing.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/computation_tracing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/deep_map.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/deep_map.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/deep_merge.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/disposable.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/disposable.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/hashing.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/hashing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/import_.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/import_.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/ipc.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/ipc.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/json.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/json.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,32 +37,44 @@
     def __str__(self):
         return self.value
 
 
 def json_default(o):
     """Encode `Table`, `RawSql`, 'Stage', and `Blob` objects"""
     if isinstance(o, Table):
+        kwargs = {}
+        if o.assumed_dependencies is not None:
+            kwargs[
+                "assumed_dependencies"
+            ] = (
+                o.assumed_dependencies
+            )  # [json_default(t) for t in o.assumed_dependencies]
         return {
             TYPE_KEY: Type.TABLE,
             "stage": o.stage.name,
             "name": o.name,
             "primary_key": o.primary_key,
             "indexes": o.indexes,
             "cache_key": o.cache_key,
             "materialization_details": o.materialization_details,
             "external_schema": o.external_schema,
             "shared_lock_allowed": o.shared_lock_allowed,
+            **kwargs,
         }
     if isinstance(o, RawSql):
+        kwargs = {}
+        if o.assumed_dependencies is not None:
+            kwargs["assumed_dependencies"] = o.assumed_dependencies
         return {
             TYPE_KEY: Type.RAW_SQL,
             "stage": o.stage.name,
             "name": o.name,
             "cache_key": o.cache_key,
             "table_names": o.table_names,
+            **kwargs,
         }
     if isinstance(o, Blob):
         return {
             TYPE_KEY: Type.BLOB,
             "stage": o.stage.name,
             "name": o.name,
             "cache_key": o.cache_key,
@@ -114,20 +126,22 @@
             indexes=d["indexes"],
             materialization_details=d.get("materialization_details"),
         )
         tbl.stage = get_stage(d["stage"])
         tbl.cache_key = d["cache_key"]
         tbl.external_schema = d.get("external_schema")
         tbl.shared_lock_allowed = d.get("shared_lock_allowed", True)
+        tbl.assumed_dependencies = d.get("assumed_dependencies")
         return tbl
     if type_ == Type.RAW_SQL:
         raw_sql = RawSql(name=d["name"])
         raw_sql.stage = get_stage(d["stage"])
         raw_sql.cache_key = d["cache_key"]
         raw_sql.table_names = d["table_names"]
+        raw_sql.assumed_dependencies = d.get("assumed_dependencies")
         return raw_sql
     if type_ == Type.BLOB:
         blob = Blob(name=d["name"])
         blob.stage = get_stage(d["stage"])
         blob.cache_key = d["cache_key"]
         return blob
     if type_ == Type.STAGE:
```

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/naming.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/naming.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/structlog.py` & `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/structlog.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.8.0/PKG-INFO` & `pydiverse_pipedag-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiverse-pipedag
-Version: 0.8.0
+Version: 0.9.0
 Summary: A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.
 License: BSD-3-Clause
 Author: QuantCo, Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -83,30 +83,30 @@
     return sa.select(
         sa.literal(1).label("x"),
         sa.literal(2).label("y"),
     )
 
 
 @materialize(lazy=True, input_type=sa.Table)
-def lazy_task_2(input1: sa.Table, input2: sa.Table):
+def lazy_task_2(input1: sa.sql.expression.Alias, input2: sa.sql.expression.Alias):
     query = sa.select(
         (input1.c.x * 5).label("x5"),
         input2.c.a,
     ).select_from(input1.outerjoin(input2, input2.c.x == input1.c.x))
 
     return Table(query, name="task_2_out", primary_key=["a"])
 
 
 @materialize(lazy=True, input_type=sa.Table)
-def lazy_task_3(input1: sa.Table):
+def lazy_task_3(input1: sa.sql.expression.Alias):
     return sa.text(f"SELECT * FROM {input1.original.schema}.{input1.original.name}")
 
 
 @materialize(lazy=True, input_type=sa.Table)
-def lazy_task_4(input1: sa.Table):
+def lazy_task_4(input1: sa.sql.expression.Alias):
     return sa.text(f"SELECT * FROM {input1.original.schema}.{input1.original.name}")
 
 
 @materialize(nout=2, version="1.0.0")
 def eager_inputs():
     dfA = pd.DataFrame(
         {
@@ -164,14 +164,15 @@
                 assert result.get(lazy_1, as_type=pd.DataFrame)["x"][0] == 1
 
 
 if __name__ == "__main__":
     setup_logging()  # you can setup the logging and/or structlog libraries as you wish
     main()
 ```
+For SQLAlchemy >= 2.0, you can use sa.Alias instead of sa.sql.expression.Alias.
 
 The `with tempfile.TemporaryDirectory()` is only needed to have an OS independent temporary directory available.
 You can also get rid of it like this:
 
 ```python
 def main():
     cfg = create_basic_pipedag_config(
```

