# Comparing `tmp/dbt-snowflake-1.8.0b2.tar.gz` & `tmp/dbt_snowflake-1.8.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-snowflake-1.8.0b2.tar", last modified: Wed Apr  3 19:59:22 2024, max compression
+gzip compressed data, was "dbt_snowflake-1.8.0b3.tar", last modified: Wed Apr 17 16:37:08 2024, max compression
```

## Comparing `dbt-snowflake-1.8.0b2.tar` & `dbt_snowflake-1.8.0b3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.723668 dbt-snowflake-1.8.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-03 19:59:22.723668 dbt-snowflake-1.8.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.711668 dbt-snowflake-1.8.0b2/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.711668 dbt-snowflake-1.8.0b2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.715669 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    21917 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.715669 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/dynamic_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.711668 dbt-snowflake-1.8.0b2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.715669 dbt-snowflake-1.8.0b2/dbt/include/snowflake/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.715669 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.715669 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/clone.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/dynamic_table.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/test.sql
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/view.sql
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/metadata.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.719668 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/drop.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.719668 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/alter.sql
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/describe.sql
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/refresh.sql
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/replace.sql
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/rename.sql
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/replace.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.719668 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/table/
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/table/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/table/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/table/rename.sql
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/table/replace.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.719668 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/view/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/view/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/view/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/view/rename.sql
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/view/replace.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.723668 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.723668 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-03 19:59:22.000000 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-03 19:59:22.000000 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:59:22.000000 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:59:22.000000 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 19:59:22.000000 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 19:59:22.000000 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:59:22.723668 dbt-snowflake-1.8.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.994400 dbt_snowflake-1.8.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-17 16:37:08.994400 dbt_snowflake-1.8.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.982399 dbt_snowflake-1.8.0b3/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.978399 dbt_snowflake-1.8.0b3/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.982399 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21917 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.982399 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/dynamic_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.978399 dbt_snowflake-1.8.0b3/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.982399 dbt_snowflake-1.8.0b3/dbt/include/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.982399 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.986400 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/dynamic_table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/test.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/metadata.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.986400 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/drop.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.986400 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/alter.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/describe.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/refresh.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/replace.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.990399 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/table/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/table/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/table/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/table/replace.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.990399 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/view/
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/view/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/view/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/view/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/view/replace.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.990399 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.990399 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-17 16:37:08.000000 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-17 16:37:08.000000 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:37:08.000000 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:37:08.000000 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 16:37:08.000000 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-17 16:37:08.000000 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:37:08.994400 dbt_snowflake-1.8.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/setup.py
```

### Comparing `dbt-snowflake-1.8.0b2/LICENSE.md` & `dbt_snowflake-1.8.0b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/PKG-INFO` & `dbt_snowflake-1.8.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.8.0b2
+Version: 1.8.0b3
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.8.0b2 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.8.0b3 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `dbt-snowflake-1.8.0b2/README.md` & `dbt_snowflake-1.8.0b3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/__init__.py` & `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/column.py` & `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/column.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/connections.py` & `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/impl.py` & `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         ConstraintType.foreign_key: ConstraintSupport.NOT_ENFORCED,
     }
 
     _capabilities: CapabilityDict = CapabilityDict(
         {
             Capability.SchemaMetadataByRelations: CapabilitySupport(support=Support.Full),
             Capability.TableLastModifiedMetadata: CapabilitySupport(support=Support.Full),
+            Capability.TableLastModifiedMetadataBatch: CapabilitySupport(support=Support.Full),
         }
     )
 
     @classmethod
     def date_function(cls):
         return "CURRENT_TIMESTAMP()"
 
@@ -201,39 +202,54 @@
         schema = parsed_model["schema"]
         database = parsed_model["database"]
         identifier = parsed_model["alias"]
         python_version = parsed_model["config"].get("python_version", "3.8")
 
         packages = parsed_model["config"].get("packages", [])
         imports = parsed_model["config"].get("imports", [])
+        external_access_integrations = parsed_model["config"].get(
+            "external_access_integrations", []
+        )
+        secrets = parsed_model["config"].get("secrets", {})
         # adding default packages we need to make python model work
         default_packages = ["snowflake-snowpark-python"]
         package_names = [package.split("==")[0] for package in packages]
         for default_package in default_packages:
             if default_package not in package_names:
                 packages.append(default_package)
         packages = "', '".join(packages)
         imports = "', '".join(imports)
-        # we can't pass empty imports clause to snowflake
+        external_access_integrations = ", ".join(external_access_integrations)
+        secrets = ", ".join(f"'{key}' = {value}" for key, value in secrets.items())
+
+        # we can't pass empty imports, external_access_integrations or secrets clause to snowflake
         if imports:
             imports = f"IMPORTS = ('{imports}')"
+        if external_access_integrations:
+            # Black is trying to make this a tuple.
+            # fmt: off
+            external_access_integrations = f"EXTERNAL_ACCESS_INTEGRATIONS = ({external_access_integrations})"
+        if secrets:
+            secrets = f"SECRETS = ({secrets})"
 
         if self.config.args.SEND_ANONYMOUS_USAGE_STATS:
             snowpark_telemetry_string = "dbtLabs_dbtPython"
             snowpark_telemetry_snippet = f"""
 import sys
 sys._xoptions['snowflake_partner_attribution'].append("{snowpark_telemetry_string}")"""
         else:
             snowpark_telemetry_snippet = ""
 
         common_procedure_code = f"""
 RETURNS STRING
 LANGUAGE PYTHON
 RUNTIME_VERSION = '{python_version}'
 PACKAGES = ('{packages}')
+{external_access_integrations}
+{secrets}
 {imports}
 HANDLER = 'main'
 EXECUTE AS CALLER
 AS
 $$
 {snowpark_telemetry_snippet}
```

### Comparing `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation.py` & `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/base.py` & `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/base.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/dynamic_table.py` & `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/dynamic_table.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/policies.py` & `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/policies.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/adapters.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/catalog.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/dynamic_table.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/dynamic_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/incremental.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/merge.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/seed.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/table.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/metadata.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/alter.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/describe.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/describe.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/table/create.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/table/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/view/create.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/safe_cast.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/safe_cast.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/timestamps.sql` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt/include/snowflake/profile_template.yml` & `dbt_snowflake-1.8.0b3/dbt/include/snowflake/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/PKG-INFO` & `dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.8.0b2
+Version: 1.8.0b3
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.8.0b2 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.8.0b3 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/SOURCES.txt` & `dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b2/setup.py` & `dbt_snowflake-1.8.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         match = re.search(_version_pattern, f.read().strip())
         if match is None:
             raise ValueError(f"invalid version at {_version_path}")
         return match.groupdict()
 
 
 package_name = "dbt-snowflake"
-package_version = "1.8.0b2"
+package_version = "1.8.0b3"
 description = """The Snowflake adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
```

