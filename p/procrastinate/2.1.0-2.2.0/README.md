# Comparing `tmp/procrastinate-2.1.0.tar.gz` & `tmp/procrastinate-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procrastinate-2.1.0.tar", max compression
+gzip compressed data, was "procrastinate-2.2.0.tar", max compression
```

## Comparing `procrastinate-2.1.0.tar` & `procrastinate-2.2.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1122 2024-03-25 18:47:34.236663 procrastinate-2.1.0/LICENSE.md
--rw-r--r--   0        0        0     5140 2024-03-25 18:47:34.236663 procrastinate-2.1.0/README.md
--rw-r--r--   0        0        0     1196 2024-03-25 18:47:34.236663 procrastinate-2.1.0/procrastinate/__init__.py
--rw-r--r--   0        0        0      180 2024-03-25 18:47:34.236663 procrastinate-2.1.0/procrastinate/__main__.py
--rw-r--r--   0        0        0    11994 2024-03-25 18:47:34.236663 procrastinate-2.1.0/procrastinate/app.py
--rw-r--r--   0        0        0    10104 2024-03-25 18:47:34.236663 procrastinate-2.1.0/procrastinate/blueprints.py
--rw-r--r--   0        0        0     1090 2024-03-25 18:47:34.236663 procrastinate-2.1.0/procrastinate/builtin_tasks.py
--rw-r--r--   0        0        0    19205 2024-03-25 18:47:34.236663 procrastinate-2.1.0/procrastinate/cli.py
--rw-r--r--   0        0        0     3197 2024-03-25 18:47:34.236663 procrastinate-2.1.0/procrastinate/connector.py
--rw-r--r--   0        0        0      181 2024-03-25 18:47:34.236663 procrastinate-2.1.0/procrastinate/contrib/README.md
--rw-r--r--   0        0        0        0 2024-03-25 18:47:34.236663 procrastinate-2.1.0/procrastinate/contrib/__init__.py
--rw-r--r--   0        0        0      110 2024-03-25 18:47:34.236663 procrastinate-2.1.0/procrastinate/contrib/aiopg/__init__.py
--rw-r--r--   0        0        0    12731 2024-03-25 18:47:34.236663 procrastinate-2.1.0/procrastinate/contrib/aiopg/aiopg_connector.py
--rw-r--r--   0        0        0     6148 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/README.md
--rw-r--r--   0        0        0      234 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/__init__.py
--rw-r--r--   0        0        0      733 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/admin.py
--rw-r--r--   0        0        0     1649 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/apps.py
--rw-r--r--   0        0        0     5662 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/django_connector.py
--rw-r--r--   0        0        0      208 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/exceptions.py
--rw-r--r--   0        0        0     1558 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/healthchecks.py
--rw-r--r--   0        0        0        0 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/management/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/management/commands/__init__.py
--rw-r--r--   0        0        0      899 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/management/commands/procrastinate.py
--rw-r--r--   0        0        0     4788 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/migrations_magic.py
--rw-r--r--   0        0        0     3450 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/models.py
--rw-r--r--   0        0        0     2424 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/procrastinate_app.py
--rw-r--r--   0        0        0      736 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/settings.py
--rw-r--r--   0        0        0     3450 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/static_migrations.py
--rw-r--r--   0        0        0     1139 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/django/utils.py
--rw-r--r--   0        0        0      119 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/psycopg2/__init__.py
--rw-r--r--   0        0        0     7864 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/psycopg2/psycopg2_connector.py
--rw-r--r--   0        0        0      428 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/sqlalchemy/README.md
--rw-r--r--   0        0        0      187 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     6050 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/contrib/sqlalchemy/psycopg2_connector.py
--rw-r--r--   0        0        0     3406 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/exceptions.py
--rw-r--r--   0        0        0     3172 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/job_context.py
--rw-r--r--   0        0        0     4948 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/jobs.py
--rw-r--r--   0        0        0    20361 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/manager.py
--rw-r--r--   0        0        0      477 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/metadata.py
--rw-r--r--   0        0        0     8874 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/periodic.py
--rw-r--r--   0        0        0     9703 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/psycopg_connector.py
--rw-r--r--   0        0        0        0 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/py.typed
--rw-r--r--   0        0        0     3762 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/retry.py
--rw-r--r--   0        0        0     1555 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/schema.py
--rw-r--r--   0        0        0     5662 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/shell.py
--rw-r--r--   0        0        0     2947 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/signals.py
--rw-r--r--   0        0        0     1325 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/__init__.py
--rw-r--r--   0        0        0      120 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/future_migrations/02.00.00_01_drop_old_procrastinate_finish_job.sql
--rw-r--r--   0        0        0     6554 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.00.00_01_initial.sql
--rw-r--r--   0        0        0     1212 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.05.00_01_drop_started_at_column.sql
--rw-r--r--   0        0        0      121 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.05.00_02_drop_started_at_column.sql
--rw-r--r--   0        0        0       84 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.05.00_03_drop_procrastinate_version_table.sql
--rw-r--r--   0        0        0     1188 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.06.00_01_fix_procrastinate_fetch_job.sql
--rw-r--r--   0        0        0      394 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.07.01_01_fix_trigger_status_events_insert.sql
--rw-r--r--   0        0        0      242 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.08.01_01_add_queueing_lock_column.sql
--rw-r--r--   0        0        0     1742 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.10.00_01_close_fetch_job_race_condition.sql
--rw-r--r--   0        0        0      502 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.10.00_02_add_defer_job_function.sql
--rw-r--r--   0        0        0     2081 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.11.00_03_add_procrastinate_periodic_defers.sql
--rw-r--r--   0        0        0       97 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.12.00_01_add_foreign_key_index.sql
--rw-r--r--   0        0        0     1791 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.14.00_01_add_locks_to_periodic_defer.sql
--rw-r--r--   0        0        0     1553 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.15.02_01_fix_procrastinate_defer_periodic_job.sql
--rw-r--r--   0        0        0      561 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.16.00_01_add_finish_job_and_retry_job_functions.sql
--rw-r--r--   0        0        0      384 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.17.00_01_add_trigger_on_job_deletion.sql
--rw-r--r--   0        0        0      401 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.17.00_02_delete_finished_jobs.sql
--rw-r--r--   0        0        0      987 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.17.00_03_add_checks_to_finish_job.sql
--rw-r--r--   0        0        0      499 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.17.00_04_add_checks_to_retry_job.sql
--rw-r--r--   0        0        0     1115 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.18.01_01_fix_finish_job_compat_issue.sql
--rw-r--r--   0        0        0      188 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.19.00_01_add_index_on_procrastinate_jobs.sql
--rw-r--r--   0        0        0     2068 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.22.00_01_add_kwargs_to_defer_periodic_job.sql
--rw-r--r--   0        0        0     1361 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/00.23.00_01_null_locks_excluded.sql
--rw-r--r--   0        0        0     1699 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/01.00.00_01_remove_old_finish_job_function.sql
--rw-r--r--   0        0        0     1736 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/01.01.01_01_job_id_bigint.sql
--rw-r--r--   0        0        0        0 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/migrations/__init__.py
--rw-r--r--   0        0        0     5802 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/queries.sql
--rw-r--r--   0        0        0    12318 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sql/schema.sql
--rw-r--r--   0        0        0     5996 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/sync_psycopg_connector.py
--rw-r--r--   0        0        0     7235 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/tasks.py
--rw-r--r--   0        0        0    10224 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/testing.py
--rw-r--r--   0        0        0      174 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/types.py
--rw-r--r--   0        0        0    13732 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/utils.py
--rw-r--r--   0        0        0    11926 2024-03-25 18:47:34.240663 procrastinate-2.1.0/procrastinate/worker.py
--rw-r--r--   0        0        0     4104 2024-03-25 18:47:35.092671 procrastinate-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     6752 1970-01-01 00:00:00.000000 procrastinate-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1122 2024-04-17 21:42:41.056214 procrastinate-2.2.0/LICENSE.md
+-rw-r--r--   0        0        0     5140 2024-04-17 21:42:41.056214 procrastinate-2.2.0/README.md
+-rw-r--r--   0        0        0     1196 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/__main__.py
+-rw-r--r--   0        0        0    11994 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/app.py
+-rw-r--r--   0        0        0    10104 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/blueprints.py
+-rw-r--r--   0        0        0     1090 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/builtin_tasks.py
+-rw-r--r--   0        0        0    19466 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/cli.py
+-rw-r--r--   0        0        0     3197 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/connector.py
+-rw-r--r--   0        0        0      181 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/__init__.py
+-rw-r--r--   0        0        0      110 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/aiopg/__init__.py
+-rw-r--r--   0        0        0    12731 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/aiopg/aiopg_connector.py
+-rw-r--r--   0        0        0     6148 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/README.md
+-rw-r--r--   0        0        0      234 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/admin.py
+-rw-r--r--   0        0        0     1649 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/apps.py
+-rw-r--r--   0        0        0     5662 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/django_connector.py
+-rw-r--r--   0        0        0      208 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/exceptions.py
+-rw-r--r--   0        0        0     1558 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/healthchecks.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/management/commands/__init__.py
+-rw-r--r--   0        0        0      899 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/management/commands/procrastinate.py
+-rw-r--r--   0        0        0     4788 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/migrations_magic.py
+-rw-r--r--   0        0        0     3450 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/models.py
+-rw-r--r--   0        0        0     2424 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/procrastinate_app.py
+-rw-r--r--   0        0        0      736 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/settings.py
+-rw-r--r--   0        0        0     3450 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/static_migrations.py
+-rw-r--r--   0        0        0     1139 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/utils.py
+-rw-r--r--   0        0        0      119 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/psycopg2/__init__.py
+-rw-r--r--   0        0        0     7864 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/contrib/psycopg2/psycopg2_connector.py
+-rw-r--r--   0        0        0      428 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/contrib/sqlalchemy/README.md
+-rw-r--r--   0        0        0      187 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     6050 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/contrib/sqlalchemy/psycopg2_connector.py
+-rw-r--r--   0        0        0     3406 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/exceptions.py
+-rw-r--r--   0        0        0     3172 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/job_context.py
+-rw-r--r--   0        0        0     4948 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/jobs.py
+-rw-r--r--   0        0        0    20361 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/manager.py
+-rw-r--r--   0        0        0      477 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/metadata.py
+-rw-r--r--   0        0        0     8874 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/periodic.py
+-rw-r--r--   0        0        0     9703 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/psycopg_connector.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/py.typed
+-rw-r--r--   0        0        0     3762 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/retry.py
+-rw-r--r--   0        0        0     1555 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/schema.py
+-rw-r--r--   0        0        0     5662 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/shell.py
+-rw-r--r--   0        0        0     2947 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/signals.py
+-rw-r--r--   0        0        0     1325 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/__init__.py
+-rw-r--r--   0        0        0      120 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/future_migrations/02.00.00_01_drop_old_procrastinate_finish_job.sql
+-rw-r--r--   0        0        0     6554 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.00.00_01_initial.sql
+-rw-r--r--   0        0        0     1212 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.05.00_01_drop_started_at_column.sql
+-rw-r--r--   0        0        0      121 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.05.00_02_drop_started_at_column.sql
+-rw-r--r--   0        0        0       84 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.05.00_03_drop_procrastinate_version_table.sql
+-rw-r--r--   0        0        0     1188 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.06.00_01_fix_procrastinate_fetch_job.sql
+-rw-r--r--   0        0        0      394 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.07.01_01_fix_trigger_status_events_insert.sql
+-rw-r--r--   0        0        0      242 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.08.01_01_add_queueing_lock_column.sql
+-rw-r--r--   0        0        0     1742 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.10.00_01_close_fetch_job_race_condition.sql
+-rw-r--r--   0        0        0      502 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.10.00_02_add_defer_job_function.sql
+-rw-r--r--   0        0        0     2081 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.11.00_03_add_procrastinate_periodic_defers.sql
+-rw-r--r--   0        0        0       97 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.12.00_01_add_foreign_key_index.sql
+-rw-r--r--   0        0        0     1791 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.14.00_01_add_locks_to_periodic_defer.sql
+-rw-r--r--   0        0        0     1553 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.15.02_01_fix_procrastinate_defer_periodic_job.sql
+-rw-r--r--   0        0        0      561 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.16.00_01_add_finish_job_and_retry_job_functions.sql
+-rw-r--r--   0        0        0      384 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.17.00_01_add_trigger_on_job_deletion.sql
+-rw-r--r--   0        0        0      401 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.17.00_02_delete_finished_jobs.sql
+-rw-r--r--   0        0        0      987 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.17.00_03_add_checks_to_finish_job.sql
+-rw-r--r--   0        0        0      499 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.17.00_04_add_checks_to_retry_job.sql
+-rw-r--r--   0        0        0     1115 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.18.01_01_fix_finish_job_compat_issue.sql
+-rw-r--r--   0        0        0      188 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.19.00_01_add_index_on_procrastinate_jobs.sql
+-rw-r--r--   0        0        0     2068 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.22.00_01_add_kwargs_to_defer_periodic_job.sql
+-rw-r--r--   0        0        0     1361 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.23.00_01_null_locks_excluded.sql
+-rw-r--r--   0        0        0     1699 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/01.00.00_01_remove_old_finish_job_function.sql
+-rw-r--r--   0        0        0     1736 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/01.01.01_01_job_id_bigint.sql
+-rw-r--r--   0        0        0        0 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/__init__.py
+-rw-r--r--   0        0        0     5802 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/queries.sql
+-rw-r--r--   0        0        0    12318 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/schema.sql
+-rw-r--r--   0        0        0     5996 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sync_psycopg_connector.py
+-rw-r--r--   0        0        0     7235 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/tasks.py
+-rw-r--r--   0        0        0    10224 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/testing.py
+-rw-r--r--   0        0        0      174 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/types.py
+-rw-r--r--   0        0        0    13732 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/utils.py
+-rw-r--r--   0        0        0    11926 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/worker.py
+-rw-r--r--   0        0        0     4104 2024-04-17 21:42:41.920210 procrastinate-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6752 1970-01-01 00:00:00.000000 procrastinate-2.2.0/PKG-INFO
```

### Comparing `procrastinate-2.1.0/LICENSE.md` & `procrastinate-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/README.md` & `procrastinate-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/__init__.py` & `procrastinate-2.2.0/procrastinate/__init__.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/app.py` & `procrastinate-2.2.0/procrastinate/app.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/blueprints.py` & `procrastinate-2.2.0/procrastinate/blueprints.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/builtin_tasks.py` & `procrastinate-2.2.0/procrastinate/builtin_tasks.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/cli.py` & `procrastinate-2.2.0/procrastinate/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import argparse
 import asyncio
 import functools
 import json
 import logging
 import os
+import shlex
 import sys
 from typing import Any, Awaitable, Callable, Literal, Union
 
 import procrastinate
 from procrastinate import connector, exceptions, jobs, shell, types, utils, worker
 
 logger = logging.getLogger(__name__)
@@ -471,14 +472,20 @@
 def configure_shell_parser(subparsers: argparse._SubParsersAction):
     # --- Shell ---
     shell_parser = subparsers.add_parser(
         "shell",
         help="Administration shell for procrastinate",
         **parser_options,
     )
+    add_argument(
+        shell_parser,
+        "args",
+        nargs="*",
+        help="Invoke a shell command and exit",
+    )
     shell_parser.set_defaults(func=shell_)
 
 
 async def cli(args):
     parser = create_parser()
     add_arguments(parser)
     add_cli_features(parser)
@@ -623,20 +630,23 @@
             "found. Have you applied database migrations (see "
             "`procrastinate schema -h`)?"
         )
 
     print("Found procrastinate_jobs table: OK")
 
 
-async def shell_(app: procrastinate.App):
+async def shell_(app: procrastinate.App, args: list[str]):
     """
     Administration shell for procrastinate.
     """
     shell_obj = shell.ProcrastinateShell(
         job_manager=app.job_manager,
     )
 
-    await utils.sync_to_async(shell_obj.cmdloop)
+    if args:
+        await utils.sync_to_async(shell_obj.onecmd, line=shlex.join(args))
+    else:
+        await utils.sync_to_async(shell_obj.cmdloop)
 
 
 def main():
     asyncio.run(cli(sys.argv[1:]))
```

### Comparing `procrastinate-2.1.0/procrastinate/connector.py` & `procrastinate-2.2.0/procrastinate/connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/aiopg/aiopg_connector.py` & `procrastinate-2.2.0/procrastinate/contrib/aiopg/aiopg_connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/django/README.md` & `procrastinate-2.2.0/procrastinate/contrib/django/README.md`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/django/admin.py` & `procrastinate-2.2.0/procrastinate/contrib/django/admin.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/django/apps.py` & `procrastinate-2.2.0/procrastinate/contrib/django/apps.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/django/django_connector.py` & `procrastinate-2.2.0/procrastinate/contrib/django/django_connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/django/healthchecks.py` & `procrastinate-2.2.0/procrastinate/contrib/django/healthchecks.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/django/management/commands/procrastinate.py` & `procrastinate-2.2.0/procrastinate/contrib/django/management/commands/procrastinate.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/django/migrations_magic.py` & `procrastinate-2.2.0/procrastinate/contrib/django/migrations_magic.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/django/models.py` & `procrastinate-2.2.0/procrastinate/contrib/django/models.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/django/procrastinate_app.py` & `procrastinate-2.2.0/procrastinate/contrib/django/procrastinate_app.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/django/settings.py` & `procrastinate-2.2.0/procrastinate/contrib/django/settings.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/django/static_migrations.py` & `procrastinate-2.2.0/procrastinate/contrib/django/static_migrations.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/django/utils.py` & `procrastinate-2.2.0/procrastinate/contrib/django/utils.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/psycopg2/psycopg2_connector.py` & `procrastinate-2.2.0/procrastinate/contrib/psycopg2/psycopg2_connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/contrib/sqlalchemy/psycopg2_connector.py` & `procrastinate-2.2.0/procrastinate/contrib/sqlalchemy/psycopg2_connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/exceptions.py` & `procrastinate-2.2.0/procrastinate/exceptions.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/job_context.py` & `procrastinate-2.2.0/procrastinate/job_context.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/jobs.py` & `procrastinate-2.2.0/procrastinate/jobs.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/manager.py` & `procrastinate-2.2.0/procrastinate/manager.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/periodic.py` & `procrastinate-2.2.0/procrastinate/periodic.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/psycopg_connector.py` & `procrastinate-2.2.0/procrastinate/psycopg_connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/retry.py` & `procrastinate-2.2.0/procrastinate/retry.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/schema.py` & `procrastinate-2.2.0/procrastinate/schema.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/shell.py` & `procrastinate-2.2.0/procrastinate/shell.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/signals.py` & `procrastinate-2.2.0/procrastinate/signals.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/__init__.py` & `procrastinate-2.2.0/procrastinate/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/00.00.00_01_initial.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/00.00.00_01_initial.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/00.05.00_01_drop_started_at_column.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/00.05.00_01_drop_started_at_column.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/00.06.00_01_fix_procrastinate_fetch_job.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/00.06.00_01_fix_procrastinate_fetch_job.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/00.10.00_01_close_fetch_job_race_condition.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/00.10.00_01_close_fetch_job_race_condition.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/00.11.00_03_add_procrastinate_periodic_defers.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/00.11.00_03_add_procrastinate_periodic_defers.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/00.14.00_01_add_locks_to_periodic_defer.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/00.14.00_01_add_locks_to_periodic_defer.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/00.15.02_01_fix_procrastinate_defer_periodic_job.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/00.15.02_01_fix_procrastinate_defer_periodic_job.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/00.16.00_01_add_finish_job_and_retry_job_functions.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/00.16.00_01_add_finish_job_and_retry_job_functions.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/00.17.00_03_add_checks_to_finish_job.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/00.17.00_03_add_checks_to_finish_job.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/00.18.01_01_fix_finish_job_compat_issue.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/00.18.01_01_fix_finish_job_compat_issue.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/00.22.00_01_add_kwargs_to_defer_periodic_job.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/00.22.00_01_add_kwargs_to_defer_periodic_job.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/00.23.00_01_null_locks_excluded.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/00.23.00_01_null_locks_excluded.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/01.00.00_01_remove_old_finish_job_function.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/01.00.00_01_remove_old_finish_job_function.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/migrations/01.01.01_01_job_id_bigint.sql` & `procrastinate-2.2.0/procrastinate/sql/migrations/01.01.01_01_job_id_bigint.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/queries.sql` & `procrastinate-2.2.0/procrastinate/sql/queries.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sql/schema.sql` & `procrastinate-2.2.0/procrastinate/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/sync_psycopg_connector.py` & `procrastinate-2.2.0/procrastinate/sync_psycopg_connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/tasks.py` & `procrastinate-2.2.0/procrastinate/tasks.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/testing.py` & `procrastinate-2.2.0/procrastinate/testing.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/utils.py` & `procrastinate-2.2.0/procrastinate/utils.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/procrastinate/worker.py` & `procrastinate-2.2.0/procrastinate/worker.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.1.0/pyproject.toml` & `procrastinate-2.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "procrastinate"
-version = "2.1.0"
+version = "2.2.0"
 description = "Postgres-based distributed task processing library"
 authors = ["Joachim Jablon", "Eric Lemoine"]
 license = "MIT License"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `procrastinate-2.1.0/PKG-INFO` & `procrastinate-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procrastinate
-Version: 2.1.0
+Version: 2.2.0
 Summary: Postgres-based distributed task processing library
 Home-page: https://procrastinate.readthedocs.io/
 License: MIT
 Keywords: postgres,task-queue
 Author: Joachim Jablon
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

