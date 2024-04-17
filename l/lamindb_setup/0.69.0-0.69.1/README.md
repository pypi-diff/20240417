# Comparing `tmp/lamindb_setup-0.69.0.tar.gz` & `tmp/lamindb_setup-0.69.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.69.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.69.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.69.0.tar` & `lamindb_setup-0.69.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     8290 2024-03-29 13:22:22.689587 lamindb_setup-0.69.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.69.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.69.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1219 2024-02-29 20:00:56.143781 lamindb_setup-0.69.0/.gitignore
--rw-r--r--   0        0        0     1931 2024-02-29 20:00:56.143838 lamindb_setup-0.69.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.69.0/LICENSE
--rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.69.0/README.md
--rw-r--r--   0        0        0    95916 2024-04-08 10:45:38.348479 lamindb_setup-0.69.0/docs/changelog.md
--rw-r--r--   0        0        0     7378 2024-03-07 18:05:18.839544 lamindb_setup-0.69.0/docs/hub-cloud/01-init-on-prem-instance.ipynb
--rw-r--r--   0        0        0     4054 2024-03-07 18:05:18.839906 lamindb_setup-0.69.0/docs/hub-cloud/02-connect-on-prem-instance.ipynb
--rw-r--r--   0        0        0     5812 2024-03-07 18:05:18.840396 lamindb_setup-0.69.0/docs/hub-cloud/03-set-storage.ipynb
--rw-r--r--   0        0        0     3339 2024-03-07 00:06:34.620916 lamindb_setup-0.69.0/docs/hub-cloud/04-test-bionty.ipynb
--rw-r--r--   0        0        0     3106 2024-04-08 06:13:37.564530 lamindb_setup-0.69.0/docs/hub-cloud/05-init-hosted-instance.ipynb
--rw-r--r--   0        0        0     3383 2024-04-08 09:34:48.611032 lamindb_setup-0.69.0/docs/hub-cloud/06-connect-hosted-instance.ipynb
--rw-r--r--   0        0        0     3160 2024-03-07 16:07:21.923709 lamindb_setup-0.69.0/docs/hub-cloud/test-multi-session.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 00:06:34.621529 lamindb_setup-0.69.0/docs/hub-cloud/test_notebooks.py
--rw-r--r--   0        0        0     6105 2024-03-07 18:05:18.841099 lamindb_setup-0.69.0/docs/hub-prod/test-cache-management.ipynb
--rw-r--r--   0        0        0    11402 2024-03-26 10:01:31.777978 lamindb_setup-0.69.0/docs/hub-prod/test-cloud-sync.ipynb
--rw-r--r--   0        0        0     1595 2024-03-18 14:07:20.594957 lamindb_setup-0.69.0/docs/hub-prod/test-connect-anonymously.ipynb
--rw-r--r--   0        0        0     2706 2024-03-07 00:06:34.621901 lamindb_setup-0.69.0/docs/hub-prod/test-empty-init.ipynb
--rw-r--r--   0        0        0     2681 2024-03-09 06:05:04.471802 lamindb_setup-0.69.0/docs/hub-prod/test-import-schema.ipynb
--rw-r--r--   0        0        0     4394 2024-03-07 00:06:34.622152 lamindb_setup-0.69.0/docs/hub-prod/test-insufficient-user-info.ipynb
--rw-r--r--   0        0        0      994 2024-03-07 00:06:34.622232 lamindb_setup-0.69.0/docs/hub-prod/test-invalid-schema.ipynb
--rw-r--r--   0        0        0     6181 2024-03-22 15:00:34.131177 lamindb_setup-0.69.0/docs/hub-prod/test-sqlite-lock.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 00:06:34.622645 lamindb_setup-0.69.0/docs/hub-prod/test_notebooks2.py
--rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.69.0/docs/index.md
--rw-r--r--   0        0        0      486 2024-03-26 10:01:31.778544 lamindb_setup-0.69.0/docs/notebooks.md
--rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.69.0/docs/reference.md
--rw-r--r--   0        0        0     1558 2024-04-08 10:45:26.010300 lamindb_setup-0.69.0/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     1802 2024-03-29 23:29:05.334743 lamindb_setup-0.69.0/lamindb_setup/_add_remote_storage.py
--rw-r--r--   0        0        0      809 2024-02-29 20:00:56.145929 lamindb_setup-0.69.0/lamindb_setup/_cache.py
--rw-r--r--   0        0        0       92 2024-02-29 20:00:56.145990 lamindb_setup-0.69.0/lamindb_setup/_check.py
--rw-r--r--   0        0        0     2543 2024-03-08 11:38:29.530179 lamindb_setup-0.69.0/lamindb_setup/_check_setup.py
--rw-r--r--   0        0        0     1150 2024-03-06 12:44:01.598158 lamindb_setup-0.69.0/lamindb_setup/_close.py
--rw-r--r--   0        0        0    11848 2024-04-08 10:44:47.691260 lamindb_setup-0.69.0/lamindb_setup/_connect_instance.py
--rw-r--r--   0        0        0     3111 2024-03-22 15:00:34.131907 lamindb_setup-0.69.0/lamindb_setup/_delete.py
--rw-r--r--   0        0        0     1500 2024-03-06 12:44:01.598969 lamindb_setup-0.69.0/lamindb_setup/_django.py
--rw-r--r--   0        0        0     2052 2024-03-09 06:05:04.472107 lamindb_setup-0.69.0/lamindb_setup/_exportdb.py
--rw-r--r--   0        0        0     1788 2024-02-29 20:00:56.146417 lamindb_setup-0.69.0/lamindb_setup/_importdb.py
--rw-r--r--   0        0        0    11479 2024-04-08 10:33:42.801066 lamindb_setup-0.69.0/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     7356 2024-03-08 11:38:29.531124 lamindb_setup-0.69.0/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0      795 2024-03-08 11:38:29.531409 lamindb_setup-0.69.0/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0      642 2024-03-08 11:38:29.531579 lamindb_setup-0.69.0/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     3657 2024-03-29 23:29:05.335131 lamindb_setup-0.69.0/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0     1548 2024-02-29 20:00:56.147217 lamindb_setup-0.69.0/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      416 2024-04-05 12:59:33.027651 lamindb_setup-0.69.0/lamindb_setup/core/__init__.py
--rw-r--r--   0        0        0     1762 2024-04-08 09:34:48.611370 lamindb_setup-0.69.0/lamindb_setup/core/_aws_storage.py
--rw-r--r--   0        0        0     2491 2024-03-05 09:37:50.121160 lamindb_setup-0.69.0/lamindb_setup/core/_deprecated.py
--rw-r--r--   0        0        0      240 2024-03-05 09:37:50.121230 lamindb_setup-0.69.0/lamindb_setup/core/_docs.py
--rw-r--r--   0        0        0     5215 2024-03-17 22:17:13.346585 lamindb_setup-0.69.0/lamindb_setup/core/_hub_client.py
--rw-r--r--   0        0        0    11522 2024-04-08 09:34:48.611681 lamindb_setup-0.69.0/lamindb_setup/core/_hub_core.py
--rw-r--r--   0        0        0     4505 2024-03-29 23:01:12.640293 lamindb_setup-0.69.0/lamindb_setup/core/_hub_crud.py
--rw-r--r--   0        0        0     1862 2024-03-05 09:37:50.121645 lamindb_setup-0.69.0/lamindb_setup/core/_hub_utils.py
--rw-r--r--   0        0        0     3241 2024-03-14 13:29:19.826564 lamindb_setup-0.69.0/lamindb_setup/core/_settings.py
--rw-r--r--   0        0        0    11565 2024-03-14 17:58:31.758814 lamindb_setup-0.69.0/lamindb_setup/core/_settings_instance.py
--rw-r--r--   0        0        0     3744 2024-03-14 17:58:31.759147 lamindb_setup-0.69.0/lamindb_setup/core/_settings_load.py
--rw-r--r--   0        0        0     2563 2024-03-18 14:07:20.595611 lamindb_setup-0.69.0/lamindb_setup/core/_settings_save.py
--rw-r--r--   0        0        0    11515 2024-04-08 09:34:48.612020 lamindb_setup-0.69.0/lamindb_setup/core/_settings_storage.py
--rw-r--r--   0        0        0     1929 2024-03-14 17:58:31.759632 lamindb_setup-0.69.0/lamindb_setup/core/_settings_store.py
--rw-r--r--   0        0        0     1281 2024-03-07 18:05:18.845546 lamindb_setup-0.69.0/lamindb_setup/core/_settings_user.py
--rw-r--r--   0        0        0     2908 2024-03-05 09:37:50.122398 lamindb_setup-0.69.0/lamindb_setup/core/_setup_bionty_sources.py
--rw-r--r--   0        0        0     6835 2024-03-26 10:01:31.779365 lamindb_setup-0.69.0/lamindb_setup/core/cloud_sqlite_locker.py
--rw-r--r--   0        0        0     5924 2024-04-08 10:33:42.801416 lamindb_setup-0.69.0/lamindb_setup/core/django.py
--rw-r--r--   0        0        0      275 2024-03-08 11:38:29.532093 lamindb_setup-0.69.0/lamindb_setup/core/exceptions.py
--rw-r--r--   0        0        0     2011 2024-03-12 21:48:08.236470 lamindb_setup-0.69.0/lamindb_setup/core/hashing.py
--rw-r--r--   0        0        0      497 2024-04-05 12:59:33.028024 lamindb_setup-0.69.0/lamindb_setup/core/types.py
--rw-r--r--   0        0        0    23860 2024-04-08 06:08:13.400154 lamindb_setup-0.69.0/lamindb_setup/core/upath.py
--rw-r--r--   0        0        0     4265 2024-04-08 09:34:48.612298 lamindb_setup-0.69.0/noxfile.py
--rw-r--r--   0        0        0      992 2024-03-26 10:01:31.780237 lamindb_setup-0.69.0/pyproject.toml
--rw-r--r--   0        0        0     5492 2024-03-29 23:10:03.082274 lamindb_setup-0.69.0/tests/hub-cloud/test_connect_instance.py
--rw-r--r--   0        0        0      285 2024-03-07 00:06:34.623314 lamindb_setup-0.69.0/tests/hub-cloud/test_delete_instance.py
--rw-r--r--   0        0        0     7021 2024-03-07 01:53:25.975859 lamindb_setup-0.69.0/tests/hub-cloud/test_init_instance.py
--rw-r--r--   0        0        0      502 2024-03-07 00:06:34.623653 lamindb_setup-0.69.0/tests/hub-cloud/test_login.py
--rw-r--r--   0        0        0      469 2024-03-07 00:06:34.623714 lamindb_setup-0.69.0/tests/hub-cloud/test_migrate.py
--rw-r--r--   0        0        0      338 2024-03-07 18:05:18.846365 lamindb_setup-0.69.0/tests/hub-cloud/test_set_storage.py
--rw-r--r--   0        0        0      548 2024-04-08 09:34:48.612599 lamindb_setup-0.69.0/tests/hub-local/conftest.py
--rw-r--r--   0        0        0    11280 2024-03-29 23:01:12.640680 lamindb_setup-0.69.0/tests/hub-local/test_all.py
--rw-r--r--   0        0        0      452 2024-03-07 00:06:34.623879 lamindb_setup-0.69.0/tests/hub-prod/conftest.py
--rw-r--r--   0        0        0      365 2024-03-07 18:05:18.846587 lamindb_setup-0.69.0/tests/hub-prod/test_auto_connect.py
--rw-r--r--   0        0        0      285 2024-03-07 00:06:34.624007 lamindb_setup-0.69.0/tests/hub-prod/test_django.py
--rw-r--r--   0        0        0     1438 2024-03-07 01:53:25.976258 lamindb_setup-0.69.0/tests/hub-prod/test_switch_and_fallback_env.py
--rw-r--r--   0        0        0      595 2024-03-07 00:06:34.624340 lamindb_setup-0.69.0/tests/hub-prod/test_upath.py
--rw-r--r--   0        0        0     1411 2024-03-12 21:17:07.347266 lamindb_setup-0.69.0/tests/storage/test_hashing.py
--rw-r--r--   0        0        0     1985 2024-03-07 18:05:18.846898 lamindb_setup-0.69.0/tests/storage/test_storage_access.py
--rw-r--r--   0        0        0      787 2024-03-28 20:35:14.618464 lamindb_setup-0.69.0/tests/storage/test_storage_basis.py
--rw-r--r--   0        0        0      842 2024-03-26 15:38:38.001397 lamindb_setup-0.69.0/tests/storage/test_storage_stats.py
--rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 lamindb_setup-0.69.0/PKG-INFO
+-rw-r--r--   0        0        0     8290 2024-04-16 19:27:14.643060 lamindb_setup-0.69.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.69.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.69.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1219 2024-04-16 19:27:14.643308 lamindb_setup-0.69.1/.gitignore
+-rw-r--r--   0        0        0     1931 2024-02-29 20:00:56.143838 lamindb_setup-0.69.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.69.1/LICENSE
+-rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.69.1/README.md
+-rw-r--r--   0        0        0    96385 2024-04-17 07:50:06.359489 lamindb_setup-0.69.1/docs/changelog.md
+-rw-r--r--   0        0        0     7378 2024-03-07 18:05:18.839544 lamindb_setup-0.69.1/docs/hub-cloud/01-init-on-prem-instance.ipynb
+-rw-r--r--   0        0        0     4054 2024-03-07 18:05:18.839906 lamindb_setup-0.69.1/docs/hub-cloud/02-connect-on-prem-instance.ipynb
+-rw-r--r--   0        0        0     5812 2024-03-07 18:05:18.840396 lamindb_setup-0.69.1/docs/hub-cloud/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3339 2024-03-07 00:06:34.620916 lamindb_setup-0.69.1/docs/hub-cloud/04-test-bionty.ipynb
+-rw-r--r--   0        0        0     3106 2024-04-08 06:13:37.564530 lamindb_setup-0.69.1/docs/hub-cloud/05-init-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3383 2024-04-08 09:34:48.611032 lamindb_setup-0.69.1/docs/hub-cloud/06-connect-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3160 2024-03-07 16:07:21.923709 lamindb_setup-0.69.1/docs/hub-cloud/test-multi-session.ipynb
+-rw-r--r--   0        0        0      142 2024-03-07 00:06:34.621529 lamindb_setup-0.69.1/docs/hub-cloud/test_notebooks.py
+-rw-r--r--   0        0        0     6105 2024-03-07 18:05:18.841099 lamindb_setup-0.69.1/docs/hub-prod/test-cache-management.ipynb
+-rw-r--r--   0        0        0    11402 2024-03-26 10:01:31.777978 lamindb_setup-0.69.1/docs/hub-prod/test-cloud-sync.ipynb
+-rw-r--r--   0        0        0     1595 2024-03-18 14:07:20.594957 lamindb_setup-0.69.1/docs/hub-prod/test-connect-anonymously.ipynb
+-rw-r--r--   0        0        0     2706 2024-03-07 00:06:34.621901 lamindb_setup-0.69.1/docs/hub-prod/test-empty-init.ipynb
+-rw-r--r--   0        0        0     2681 2024-03-09 06:05:04.471802 lamindb_setup-0.69.1/docs/hub-prod/test-import-schema.ipynb
+-rw-r--r--   0        0        0     4394 2024-03-07 00:06:34.622152 lamindb_setup-0.69.1/docs/hub-prod/test-insufficient-user-info.ipynb
+-rw-r--r--   0        0        0      994 2024-03-07 00:06:34.622232 lamindb_setup-0.69.1/docs/hub-prod/test-invalid-schema.ipynb
+-rw-r--r--   0        0        0     6181 2024-03-22 15:00:34.131177 lamindb_setup-0.69.1/docs/hub-prod/test-sqlite-lock.ipynb
+-rw-r--r--   0        0        0      142 2024-03-07 00:06:34.622645 lamindb_setup-0.69.1/docs/hub-prod/test_notebooks2.py
+-rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.69.1/docs/index.md
+-rw-r--r--   0        0        0      486 2024-03-26 10:01:31.778544 lamindb_setup-0.69.1/docs/notebooks.md
+-rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.69.1/docs/reference.md
+-rw-r--r--   0        0        0     1558 2024-04-17 07:49:48.062086 lamindb_setup-0.69.1/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     1802 2024-03-29 23:29:05.334743 lamindb_setup-0.69.1/lamindb_setup/_add_remote_storage.py
+-rw-r--r--   0        0        0      809 2024-02-29 20:00:56.145929 lamindb_setup-0.69.1/lamindb_setup/_cache.py
+-rw-r--r--   0        0        0       92 2024-02-29 20:00:56.145990 lamindb_setup-0.69.1/lamindb_setup/_check.py
+-rw-r--r--   0        0        0     2543 2024-03-08 11:38:29.530179 lamindb_setup-0.69.1/lamindb_setup/_check_setup.py
+-rw-r--r--   0        0        0     1150 2024-03-06 12:44:01.598158 lamindb_setup-0.69.1/lamindb_setup/_close.py
+-rw-r--r--   0        0        0    11624 2024-04-16 19:47:35.808485 lamindb_setup-0.69.1/lamindb_setup/_connect_instance.py
+-rw-r--r--   0        0        0     3111 2024-03-22 15:00:34.131907 lamindb_setup-0.69.1/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0     1500 2024-03-06 12:44:01.598969 lamindb_setup-0.69.1/lamindb_setup/_django.py
+-rw-r--r--   0        0        0     2084 2024-04-15 04:44:50.596309 lamindb_setup-0.69.1/lamindb_setup/_exportdb.py
+-rw-r--r--   0        0        0     1836 2024-04-15 06:35:29.022278 lamindb_setup-0.69.1/lamindb_setup/_importdb.py
+-rw-r--r--   0        0        0    11479 2024-04-08 10:33:42.801066 lamindb_setup-0.69.1/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     8529 2024-04-16 15:26:03.848281 lamindb_setup-0.69.1/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0      795 2024-03-08 11:38:29.531409 lamindb_setup-0.69.1/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0      642 2024-03-08 11:38:29.531579 lamindb_setup-0.69.1/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     3657 2024-03-29 23:29:05.335131 lamindb_setup-0.69.1/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0     1548 2024-02-29 20:00:56.147217 lamindb_setup-0.69.1/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      369 2024-04-16 15:26:03.848647 lamindb_setup-0.69.1/lamindb_setup/core/__init__.py
+-rw-r--r--   0        0        0     1762 2024-04-08 09:34:48.611370 lamindb_setup-0.69.1/lamindb_setup/core/_aws_storage.py
+-rw-r--r--   0        0        0     2491 2024-03-05 09:37:50.121160 lamindb_setup-0.69.1/lamindb_setup/core/_deprecated.py
+-rw-r--r--   0        0        0      240 2024-03-05 09:37:50.121230 lamindb_setup-0.69.1/lamindb_setup/core/_docs.py
+-rw-r--r--   0        0        0     5520 2024-04-15 15:03:26.266397 lamindb_setup-0.69.1/lamindb_setup/core/_hub_client.py
+-rw-r--r--   0        0        0    10990 2024-04-15 15:03:26.266901 lamindb_setup-0.69.1/lamindb_setup/core/_hub_core.py
+-rw-r--r--   0        0        0     4505 2024-03-29 23:01:12.640293 lamindb_setup-0.69.1/lamindb_setup/core/_hub_crud.py
+-rw-r--r--   0        0        0     1862 2024-03-05 09:37:50.121645 lamindb_setup-0.69.1/lamindb_setup/core/_hub_utils.py
+-rw-r--r--   0        0        0     3241 2024-03-14 13:29:19.826564 lamindb_setup-0.69.1/lamindb_setup/core/_settings.py
+-rw-r--r--   0        0        0    11556 2024-04-16 19:47:35.808698 lamindb_setup-0.69.1/lamindb_setup/core/_settings_instance.py
+-rw-r--r--   0        0        0     3744 2024-03-14 17:58:31.759147 lamindb_setup-0.69.1/lamindb_setup/core/_settings_load.py
+-rw-r--r--   0        0        0     2563 2024-03-18 14:07:20.595611 lamindb_setup-0.69.1/lamindb_setup/core/_settings_save.py
+-rw-r--r--   0        0        0    13044 2024-04-16 19:47:35.808927 lamindb_setup-0.69.1/lamindb_setup/core/_settings_storage.py
+-rw-r--r--   0        0        0     1929 2024-03-14 17:58:31.759632 lamindb_setup-0.69.1/lamindb_setup/core/_settings_store.py
+-rw-r--r--   0        0        0     1281 2024-03-07 18:05:18.845546 lamindb_setup-0.69.1/lamindb_setup/core/_settings_user.py
+-rw-r--r--   0        0        0     2908 2024-03-05 09:37:50.122398 lamindb_setup-0.69.1/lamindb_setup/core/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     6835 2024-03-26 10:01:31.779365 lamindb_setup-0.69.1/lamindb_setup/core/cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     3335 2024-04-16 15:26:03.848992 lamindb_setup-0.69.1/lamindb_setup/core/django.py
+-rw-r--r--   0        0        0      275 2024-03-08 11:38:29.532093 lamindb_setup-0.69.1/lamindb_setup/core/exceptions.py
+-rw-r--r--   0        0        0     2011 2024-03-12 21:48:08.236470 lamindb_setup-0.69.1/lamindb_setup/core/hashing.py
+-rw-r--r--   0        0        0      497 2024-04-05 12:59:33.028024 lamindb_setup-0.69.1/lamindb_setup/core/types.py
+-rw-r--r--   0        0        0    23860 2024-04-16 19:27:14.644297 lamindb_setup-0.69.1/lamindb_setup/core/upath.py
+-rw-r--r--   0        0        0     4265 2024-04-08 09:34:48.612298 lamindb_setup-0.69.1/noxfile.py
+-rw-r--r--   0        0        0      992 2024-03-26 10:01:31.780237 lamindb_setup-0.69.1/pyproject.toml
+-rw-r--r--   0        0        0     5492 2024-03-29 23:10:03.082274 lamindb_setup-0.69.1/tests/hub-cloud/test_connect_instance.py
+-rw-r--r--   0        0        0      285 2024-03-07 00:06:34.623314 lamindb_setup-0.69.1/tests/hub-cloud/test_delete_instance.py
+-rw-r--r--   0        0        0     7021 2024-03-07 01:53:25.975859 lamindb_setup-0.69.1/tests/hub-cloud/test_init_instance.py
+-rw-r--r--   0        0        0      502 2024-03-07 00:06:34.623653 lamindb_setup-0.69.1/tests/hub-cloud/test_login.py
+-rw-r--r--   0        0        0      469 2024-03-07 00:06:34.623714 lamindb_setup-0.69.1/tests/hub-cloud/test_migrate.py
+-rw-r--r--   0        0        0      338 2024-03-07 18:05:18.846365 lamindb_setup-0.69.1/tests/hub-cloud/test_set_storage.py
+-rw-r--r--   0        0        0      548 2024-04-08 09:34:48.612599 lamindb_setup-0.69.1/tests/hub-local/conftest.py
+-rw-r--r--   0        0        0    11318 2024-04-15 15:03:26.267377 lamindb_setup-0.69.1/tests/hub-local/test_all.py
+-rw-r--r--   0        0        0      452 2024-03-07 00:06:34.623879 lamindb_setup-0.69.1/tests/hub-prod/conftest.py
+-rw-r--r--   0        0        0      365 2024-03-07 18:05:18.846587 lamindb_setup-0.69.1/tests/hub-prod/test_auto_connect.py
+-rw-r--r--   0        0        0      158 2024-04-16 15:26:03.849537 lamindb_setup-0.69.1/tests/hub-prod/test_django.py
+-rw-r--r--   0        0        0     1432 2024-04-15 15:03:26.267758 lamindb_setup-0.69.1/tests/hub-prod/test_switch_and_fallback_env.py
+-rw-r--r--   0        0        0      595 2024-03-07 00:06:34.624340 lamindb_setup-0.69.1/tests/hub-prod/test_upath.py
+-rw-r--r--   0        0        0     1411 2024-03-12 21:17:07.347266 lamindb_setup-0.69.1/tests/storage/test_hashing.py
+-rw-r--r--   0        0        0     1985 2024-03-07 18:05:18.846898 lamindb_setup-0.69.1/tests/storage/test_storage_access.py
+-rw-r--r--   0        0        0      787 2024-03-28 20:35:14.618464 lamindb_setup-0.69.1/tests/storage/test_storage_basis.py
+-rw-r--r--   0        0        0      842 2024-03-26 15:38:38.001397 lamindb_setup-0.69.1/tests/storage/test_storage_stats.py
+-rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 lamindb_setup-0.69.1/PKG-INFO
```

### Comparing `lamindb_setup-0.69.0/.github/workflows/build.yml` & `lamindb_setup-0.69.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/.github/workflows/latest-changes.yml` & `lamindb_setup-0.69.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/.gitignore` & `lamindb_setup-0.69.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/.pre-commit-config.yaml` & `lamindb_setup-0.69.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/LICENSE` & `lamindb_setup-0.69.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/changelog.md` & `lamindb_setup-0.69.1/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✨ Enable hybrid storage mode | [717](https://github.com/laminlabs/lamindb-setup/pull/717) | [falexwolf](https://github.com/falexwolf) | 2024-04-16 | 0.69.1
+🚸 Better migrations warning | [716](https://github.com/laminlabs/lamindb-setup/pull/716) | [falexwolf](https://github.com/falexwolf) | 2024-04-16 |
+🚸 Refresh token also upon access-aws | [715](https://github.com/laminlabs/lamindb-setup/pull/715) | [falexwolf](https://github.com/falexwolf) | 2024-04-15 |
 🚸 Skip hub request for a purely local instance | [713](https://github.com/laminlabs/lamindb-setup/pull/713) | [falexwolf](https://github.com/falexwolf) | 2024-04-08 | 0.69.0
 🐛 Fix clashes for multi process | [712](https://github.com/laminlabs/lamindb-setup/pull/712) | [falexwolf](https://github.com/falexwolf) | 2024-04-08 |
 ♻️ No longer need AWS account | [711](https://github.com/laminlabs/lamindb-setup/pull/711) | [falexwolf](https://github.com/falexwolf) | 2024-04-08 |
 📝 Fix docs | [709](https://github.com/laminlabs/lamindb-setup/pull/709) | [falexwolf](https://github.com/falexwolf) | 2024-04-05 |
 ♻️ Replace TypeVar with TypeAlias | [707](https://github.com/laminlabs/lamindb-setup/pull/707) | [falexwolf](https://github.com/falexwolf) | 2024-04-04 |
 ♻️ Refactor clean up | [706](https://github.com/laminlabs/lamindb-setup/pull/706) | [falexwolf](https://github.com/falexwolf) | 2024-04-04 |
 🩹 Do bucket injection trick only for s3 | [705](https://github.com/laminlabs/lamindb-setup/pull/705) | [Koncopd](https://github.com/Koncopd) | 2024-04-04 |
```

### Comparing `lamindb_setup-0.69.0/docs/hub-cloud/01-init-on-prem-instance.ipynb` & `lamindb_setup-0.69.1/docs/hub-cloud/01-init-on-prem-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-cloud/02-connect-on-prem-instance.ipynb` & `lamindb_setup-0.69.1/docs/hub-cloud/02-connect-on-prem-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-cloud/03-set-storage.ipynb` & `lamindb_setup-0.69.1/docs/hub-cloud/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-cloud/04-test-bionty.ipynb` & `lamindb_setup-0.69.1/docs/hub-cloud/04-test-bionty.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-cloud/05-init-hosted-instance.ipynb` & `lamindb_setup-0.69.1/docs/hub-cloud/05-init-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-cloud/06-connect-hosted-instance.ipynb` & `lamindb_setup-0.69.1/docs/hub-cloud/06-connect-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-cloud/test-multi-session.ipynb` & `lamindb_setup-0.69.1/docs/hub-cloud/test-multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-prod/test-cache-management.ipynb` & `lamindb_setup-0.69.1/docs/hub-prod/test-cache-management.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-prod/test-cloud-sync.ipynb` & `lamindb_setup-0.69.1/docs/hub-prod/test-cloud-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-prod/test-connect-anonymously.ipynb` & `lamindb_setup-0.69.1/docs/hub-prod/test-connect-anonymously.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-prod/test-empty-init.ipynb` & `lamindb_setup-0.69.1/docs/hub-prod/test-empty-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-prod/test-import-schema.ipynb` & `lamindb_setup-0.69.1/docs/hub-prod/test-import-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-prod/test-insufficient-user-info.ipynb` & `lamindb_setup-0.69.1/docs/hub-prod/test-insufficient-user-info.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-prod/test-invalid-schema.ipynb` & `lamindb_setup-0.69.1/docs/hub-prod/test-invalid-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/docs/hub-prod/test-sqlite-lock.ipynb` & `lamindb_setup-0.69.1/docs/hub-prod/test-sqlite-lock.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/__init__.py` & `lamindb_setup-0.69.1/lamindb_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
    settings
    core
    django
 
 """
 
-__version__ = "0.69.0"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.69.1"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import core
 from ._close import close  # noqa
 from ._delete import delete  # noqa
```

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_add_remote_storage.py` & `lamindb_setup-0.69.1/lamindb_setup/_add_remote_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_cache.py` & `lamindb_setup-0.69.1/lamindb_setup/_cache.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_check_setup.py` & `lamindb_setup-0.69.1/lamindb_setup/_check_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_close.py` & `lamindb_setup-0.69.1/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_connect_instance.py` & `lamindb_setup-0.69.1/lamindb_setup/_connect_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 from ._silence_loggers import silence_loggers
 from .core._settings_load import load_instance_settings
 from .core._settings_storage import StorageSettings
 from .core._settings_store import instance_settings_file
 from .core.cloud_sqlite_locker import unlock_cloud_sqlite_upon_exception
 from ._init_instance import MESSAGE_NO_MULTIPLE_INSTANCE
 from ._check_setup import _check_instance_setup
-from .core._hub_core import connect_instance as connect_instance_from_hub
+from .core._hub_core import connect_instance as load_instance_from_hub
+from ._migrate import check_whether_migrations_in_sync
 
 
 # this is for testing purposes only
 # set to True only to test failed load
 _TEST_FAILED_LOAD = False
 
 
@@ -119,46 +120,38 @@
             isettings = load_instance_settings(settings_file)
             # skip hub request for a purely local instance
             make_hub_request = isettings.is_remote
 
         if make_hub_request:
             # the following will return a string if the instance does not exist
             # on the hub
-            hub_result = connect_instance_from_hub(owner=owner, name=name)
+            hub_result = load_instance_from_hub(owner=owner, name=name)
             # if hub_result is not a string, it means it made a request
             # that successfully returned metadata
             if not isinstance(hub_result, str):
                 instance_result, storage_result = hub_result
                 db_updated = update_db_using_local(
                     instance_result, settings_file, db=db
                 )
                 ssettings = StorageSettings(
                     root=storage_result["root"],
                     region=storage_result["region"],
                     uid=storage_result["lnid"],
+                    is_hybrid=instance_result["storage_mode"] == "hybrid",
                 )
                 isettings = InstanceSettings(
                     id=UUID(instance_result["id"]),
                     owner=owner,
                     name=name,
                     storage=ssettings,
                     db=db_updated,
                     schema=instance_result["schema_str"],
                     git_repo=instance_result["git_repo"],
                 )
-                from importlib import metadata
-
-                try:
-                    lamindb_version = metadata.version("lamindb")
-                except metadata.PackageNotFoundError:
-                    lamindb_version = None
-                logger.important(
-                    f"last migration: lamindb=={instance_result['lamindb_version']} <>"
-                    f" your env: lamindb=={lamindb_version}"
-                )
+                check_whether_migrations_in_sync(instance_result["lamindb_version"])
             else:
                 error_message = (
                     f"'{owner}/{name}' not loadable:"
                     f" '{hub_result}'\nCheck your permissions:"
                     f" https://lamin.ai/{owner}/{name}?tab=collaborators"
                 )
                 if settings_file.exists():
```

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_delete.py` & `lamindb_setup-0.69.1/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_django.py` & `lamindb_setup-0.69.1/lamindb_setup/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_exportdb.py` & `lamindb_setup-0.69.1/lamindb_setup/_exportdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,30 +10,30 @@
         "Run": True,
         "User": False,
         "Storage": False,
         "Feature": False,
         "FeatureSet": False,
         "ULabel": False,
     },
-    "bionty": {
-        "Organism": False,
-        "Gene": False,
-        "Protein": False,
-        "CellMarker": False,
-        "Tissue": False,
-        "CellType": False,
-        "Disease": False,
-        "CellLine": False,
-        "Phenotype": False,
-        "Pathway": False,
-        "ExperimentalFactor": False,
-        "DevelopmentalStage": False,
-        "Ethnicity": False,
-        "PublicSource": False,
-    },
+    # "bionty": {
+    #     "Organism": False,
+    #     "Gene": False,
+    #     "Protein": False,
+    #     "CellMarker": False,
+    #     "Tissue": False,
+    #     "CellType": False,
+    #     "Disease": False,
+    #     "CellLine": False,
+    #     "Phenotype": False,
+    #     "Pathway": False,
+    #     "ExperimentalFactor": False,
+    #     "DevelopmentalStage": False,
+    #     "Ethnicity": False,
+    #     "PublicSource": False,
+    # },
     # "wetlab": {
     #     "ExperimentType": False,
     #     "Experiment": False,
     #     "Well": False,
     #     "TreatmentTarget": False,
     #     "Treatment": False,
     #     "Biosample": False,
```

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_importdb.py` & `lamindb_setup-0.69.1/lamindb_setup/_importdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from ._export import MODELS
+from ._exportdb import MODELS
 from importlib import import_module
 
 
 def import_registry(registry, directory, connection):
     import pandas as pd
 
     table_name = registry._meta.db_table
@@ -21,23 +21,24 @@
     directory = Path("./lamindb_export/")
     if directory.exists():
         response = input(
             f"\n\nDo you want to import registries from here: {directory}? (y/n)\n"
         )
         if response != "y":
             return None
-    from sqlalchemy import create_engine
+    from sqlalchemy import create_engine, text
     import lamindb_setup as ln_setup
 
     engine = create_engine(ln_setup.settings.instance.db, echo=False)
     with engine.begin() as connection:
         if ln_setup.settings.instance.dialect == "postgresql":
-            connection.execute("SET CONSTRAINTS ALL DEFERRED;")
+            connection.execute(text("SET CONSTRAINTS ALL DEFERRED;"))
         for schema_name, models in MODELS.items():
             for model_name in models.keys():
+                print(model_name)
                 schema_module = import_module(f"lnschema_{schema_name}")
                 registry = getattr(schema_module, model_name)
                 import_registry(registry, directory, connection)
                 many_to_many_names = [
                     field.name for field in registry._meta.many_to_many
                 ]
                 for many_to_many_name in many_to_many_names:
```

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_init_instance.py` & `lamindb_setup-0.69.1/lamindb_setup/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_migrate.py` & `lamindb_setup-0.69.1/lamindb_setup/_migrate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,47 @@
 from typing import Optional, Dict
 from lamin_utils import logger
-
+from packaging import version
 from ._check_setup import _check_instance_setup
 from .core._settings import settings
 from .core.django import setup_django
 from django.db import connection
 from django.db.migrations.loader import MigrationLoader
 
 
+# for the django-based synching code, see laminhub_rest
+def check_whether_migrations_in_sync(db_version_str: str):
+    from importlib import metadata
+
+    try:
+        installed_version_str = metadata.version("lamindb")
+    except metadata.PackageNotFoundError:
+        return None
+    installed_version = version.parse(installed_version_str)
+    db_version = version.parse(db_version_str)
+    if (
+        installed_version.major < db_version.major
+        or installed_version.minor < db_version.minor
+    ):
+        logger.warning(
+            f"Your database ({db_version_str}) is ahead of your lamindb installation"
+            f" ({installed_version_str}). \nPlease update your Python library to match"
+            f" the database: pip install -U lamindb=={db_version_str}"
+        )
+    elif (
+        installed_version.major > db_version.major
+        or installed_version.minor > db_version.minor
+    ):
+        logger.warning(
+            f"Your database ({db_version_str}) is behind your lamindb installation"
+            f" ({installed_version_str}). \nPlease migrate your database: lamin migrate"
+            " deploy"
+        )
+
+
 # for tests, see lamin-cli
 class migrate:
     """Manage migrations.
 
     Examples:
 
     >>> import lamindb as ln
```

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_register_instance.py` & `lamindb_setup-0.69.1/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_schema.py` & `lamindb_setup-0.69.1/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_setup_user.py` & `lamindb_setup-0.69.1/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.69.1/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_aws_storage.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_aws_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_deprecated.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_hub_client.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_hub_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from typing import Optional
 from supabase.lib.client_options import ClientOptions
 from urllib.request import urlretrieve
 from supabase import create_client, Client
 from pydantic import BaseSettings
-from postgrest import APIError as PostgrestAPIError
 from gotrue.errors import AuthUnknownError
+from lamin_utils import logger
 
 
 class Connector(BaseSettings):
     url: str
     key: str
 
 
@@ -112,20 +112,27 @@
                 client.auth.sign_out()
             except NameError:
                 pass
         return result
 
     for renew_token, fallback_env in [(False, False), (True, False), (False, True)]:
         try:
+            if renew_token:
+                logger.important(
+                    "Renewing expired lamin token: call lamin login to avoid this"
+                )
             client = connect_hub_with_auth(
                 renew_token=renew_token, fallback_env=fallback_env
             )
             result = callable(**kwargs, client=client)
             break
-        except (PostgrestAPIError, AuthUnknownError) as e:
+        # we use Exception here as the ways in which the client fails upon 401
+        # are not consistent and keep changing
+        # because we ultimately raise the error, it's OK I'd say
+        except Exception as e:
             if fallback_env:
                 raise e
         finally:
             try:
                 client.auth.sign_out()
             except NameError:
                 pass
```

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_hub_core.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_hub_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from typing import Optional, Tuple, Union, Dict
 import uuid
 from postgrest.exceptions import APIError
 from uuid import UUID
 from lamin_utils import logger
 from supabase import Client
-from supafunc.errors import FunctionsRelayError, FunctionsHttpError
 import lamindb_setup
 import json
 from importlib import metadata
 from ._settings_instance import InstanceSettings
 from ._settings_storage import StorageSettings, base62
 
 
@@ -237,40 +236,27 @@
         )
         return credentials
     else:
         raise RuntimeError("Can only get access to AWS if authenticated.")
 
 
 def _access_aws(*, storage_root: str, client: Client) -> Dict[str, str]:
-    from time import sleep
-
-    response = None
-    max_retries = 5
-    for retry in range(max_retries):
-        try:
-            response = client.functions.invoke(
-                "access-aws",
-                invoke_options={"body": {"storage_root": storage_root}},
-            )
-        except (FunctionsRelayError, FunctionsHttpError, json.JSONDecodeError) as error:
-            print("no valid response, retry", response)
-            sleep(1)
-            if retry == max_retries - 1:
-                raise error
-            else:
-                continue
-        if response is not None and response != b"{}":
-            loaded_credentials = json.loads(response)["Credentials"]
-            credentials = {}
-            credentials["key"] = loaded_credentials["AccessKeyId"]
-            credentials["secret"] = loaded_credentials["SecretAccessKey"]
-            credentials["token"] = loaded_credentials["SessionToken"]
-            return credentials
-        elif lamindb_setup._TESTING:
-            raise RuntimeError(f"access-aws errored: {response}")
+    response = client.functions.invoke(
+        "access-aws",
+        invoke_options={"body": {"storage_root": storage_root}},
+    )
+    if response is not None and response != b"{}":
+        loaded_credentials = json.loads(response)["Credentials"]
+        credentials = {}
+        credentials["key"] = loaded_credentials["AccessKeyId"]
+        credentials["secret"] = loaded_credentials["SecretAccessKey"]
+        credentials["token"] = loaded_credentials["SessionToken"]
+        return credentials
+    elif lamindb_setup._TESTING:
+        raise RuntimeError(f"access-aws errored: {response}")
     return {}
 
 
 def get_lamin_site_base_url():
     if "LAMIN_ENV" in os.environ:
         if os.environ["LAMIN_ENV"] == "local":
             return "http://localhost:3000"
```

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_hub_crud.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_hub_utils.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_settings.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_settings_instance.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_settings_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     """Instance settings."""
 
     def __init__(
         self,
         id: UUID,  # instance id/uuid
         owner: str,  # owner handle
         name: str,  # instance name
-        storage: StorageSettings,  # storage location on cloud
+        storage: StorageSettings,  # storage location
         uid: Optional[str] = None,  # instance uid/lnid
         db: Optional[str] = None,  # DB URI
         schema: Optional[str] = None,  # comma-separated string of schema names
         git_repo: Optional[str] = None,  # a git repo URL
     ):
         from ._hub_utils import validate_db_arg
 
         self._id: UUID = id
         self._owner: str = owner
         self._name: str = name
-        self._storage: StorageSettings = storage
         self._uid: Optional[str] = uid
+        self._storage: StorageSettings = storage
         validate_db_arg(db)
         self._db: Optional[str] = db
         self._schema_str: Optional[str] = schema
         self._git_repo = None if git_repo is None else sanitize_git_repo_url(git_repo)
 
     def __repr__(self):
         """Rich string representation."""
```

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_settings_load.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_settings_save.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_settings_storage.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_settings_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import shutil
 from lamin_utils import logger
 from pathlib import Path
-from typing import Any, Optional, Union
+from typing import Any, Optional, Union, Literal
 from ._aws_storage import find_closest_aws_region
 from appdirs import AppDirs
 from ._settings_save import save_system_storage_settings
 from ._settings_store import system_storage_settings_file
 from .upath import LocalPathClasses, UPath, create_path, convert_pathlike
 from uuid import UUID
 import string
@@ -117,25 +117,28 @@
 class StorageSettings:
     """Manage cloud or local storage settings."""
 
     def __init__(
         self,
         root: UPathStr,
         region: Optional[str] = None,
+        is_hybrid: bool = False,  # refers to storage mode
         uid: Optional[str] = None,
         uuid: Optional[UUID] = None,
         access_token: Optional[str] = None,
     ):
         self._uid = uid
         self._uuid = uuid
+        self._is_hybrid = is_hybrid
         self._root_init = convert_pathlike(root)
         if isinstance(self._root_init, LocalPathClasses):  # local paths
             self._root_init.mkdir(parents=True, exist_ok=True)
             self._root_init = self._root_init.resolve()
         self._root = None
+        self._remote_root = None
         self._aws_account_id: Optional[int] = None
         self._description: Optional[str] = None
         # we don't yet infer region here to make init fast
         self._region = region
         # would prefer to type below as Registry, but need to think through import order
         self._record: Optional[Any] = None
         # cache settings
@@ -173,36 +176,71 @@
     def record(self) -> Any:
         """Storage record."""
         if self._record is None:
             # dynamic import because of import order
             from lnschema_core.models import Storage
             from ._settings import settings
 
-            self._record = Storage.objects.using(settings._using_key).get(
-                root=self.root_as_str
-            )
+            if not self.is_hybrid:
+                self._record = Storage.objects.using(settings._using_key).get(
+                    root=self.root_as_str
+                )
+            else:
+                # this has to be redone
+                records = Storage.objects.filter(type="local").all()
+                for record in records:
+                    if Path(record.root).exists():
+                        self._record = record
+                        logger.warning("found local storage location")
+                        break
         return self._record
 
     def __repr__(self):
         """String rep."""
         s = f"root='{self.root_as_str}', uid='{self.uid}'"
         if self.uuid is not None:
             s += f", uuid='{self.uuid.hex}'"
         return f"StorageSettings({s})"
 
     @property
+    def is_hybrid(self) -> bool:
+        """Qualifies storage mode.
+
+        A storage location can be local, in the cloud, or hybrid. See
+        :attr:`~lamindb.setup.core.StorageSettings.type`.
+
+        Hybrid means that a default local storage location is backed by an
+        optional cloud storage location.
+        """
+        return self._is_hybrid
+
+    @property
     def root(self) -> UPath:
         """Root storage location."""
         if self._root is None:
-            # below also makes network requests to get credentials
-            # right
-            root_path = create_path(self._root_init, access_token=self.access_token)
+            if not self.is_hybrid:
+                # below makes network requests to get credentials
+                root_path = create_path(self._root_init, access_token=self.access_token)
+            else:
+                # this is a local path
+                root_path = create_path(self.record.root)
             self._root = root_path
         return self._root
 
+    @property
+    def remote_root(self) -> UPath:
+        """Remote storage location. Only needed for hybrid storage."""
+        if not self.is_hybrid:
+            raise ValueError("remote_root is only defined for hybrid storage")
+        if self._remote_root is None:
+            self._remote_root = create_path(
+                self._root_init, access_token=self.access_token
+            )
+        return self._remote_root
+
     def _set_fs_kwargs(self, **kwargs):
         """Set additional fsspec arguments for cloud root.
 
         Example:
 
         >>> ln.setup.settings.storage._set_fs_kwargs(  # any fsspec args
         >>>    profile="some_profile", cache_regions=True
@@ -269,24 +307,24 @@
     def region(self) -> Optional[str]:
         """Storage region."""
         if self._region is None:
             self._region = get_storage_region(self.root_as_str)
         return self._region
 
     @property
-    def type(self) -> str:
-        """AWS S3 vs. Google Cloud vs. local vs. the other protocols.
+    def type(self) -> Literal["local", "s3", "gs"]:
+        """AWS S3 vs. Google Cloud vs. local.
 
-        Returns the protocol.
+        Returns the protocol as a string: "local", "s3", "gs".
         """
         import fsspec
 
         convert = {"file": "local"}
         protocol = fsspec.utils.get_protocol(self.root_as_str)
-        return convert.get(protocol, protocol)
+        return convert.get(protocol, protocol)  # type: ignore
 
     def key_to_filepath(self, filekey: Union[Path, UPath, str]) -> UPath:
         """Cloud or local filepath from filekey."""
         return self.root / filekey
 
     def cloud_to_local(self, filepath: Union[Path, UPath], **kwargs) -> UPath:
         """Local (cache) filepath from filepath."""
```

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_settings_store.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_settings_user.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/_setup_bionty_sources.py` & `lamindb_setup-0.69.1/lamindb_setup/core/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/cloud_sqlite_locker.py` & `lamindb_setup-0.69.1/lamindb_setup/core/cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/hashing.py` & `lamindb_setup-0.69.1/lamindb_setup/core/hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/lamindb_setup/core/upath.py` & `lamindb_setup-0.69.1/lamindb_setup/core/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/noxfile.py` & `lamindb_setup-0.69.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/pyproject.toml` & `lamindb_setup-0.69.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/tests/hub-cloud/test_connect_instance.py` & `lamindb_setup-0.69.1/tests/hub-cloud/test_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/tests/hub-cloud/test_init_instance.py` & `lamindb_setup-0.69.1/tests/hub-cloud/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/tests/hub-local/conftest.py` & `lamindb_setup-0.69.1/tests/hub-local/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/tests/hub-local/test_all.py` & `lamindb_setup-0.69.1/tests/hub-local/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from uuid import UUID, uuid4
 import pytest
 from lamindb_setup.core._hub_utils import LaminDsnModel
 from gotrue.errors import AuthApiError
+from postgrest.exceptions import APIError
 import lamindb_setup as ln_setup
 from lamindb_setup.core._settings_instance import InstanceSettings
 from lamindb_setup.core._hub_client import (
     Environment,
     connect_hub_with_auth,
 )
 from lamindb_setup.core._hub_core import (
@@ -296,15 +297,15 @@
 def test_connect_instance_corrupted_or_expired_credentials(
     create_myinstance, create_testadmin1_session
 ):
     # assume token & password are corrupted or expired
     ln_setup.settings.user.access_token = "corrupted_or_expired_token"
     correct_password = ln_setup.settings.user.password
     ln_setup.settings.user.password = "corrupted_password"
-    with pytest.raises(AuthApiError):
+    with pytest.raises(APIError):
         connect_instance(
             owner="testadmin1",
             name=create_myinstance["name"],
         )
     # now, let's assume only the token is expired or corrupted
     # re-creating the auth client triggers a re-generated token because it
     # excepts the error assuming the token is expired
```

### Comparing `lamindb_setup-0.69.0/tests/hub-prod/test_switch_and_fallback_env.py` & `lamindb_setup-0.69.1/tests/hub-prod/test_switch_and_fallback_env.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import os
 import pytest
 import lamindb_setup as ln_setup
-from gotrue.errors import AuthUnknownError
+from gotrue.errors import AuthRetryableError
 from lamindb_setup import login, settings
 from lamindb_setup.core._hub_core import (
     connect_instance,
     sign_in_hub,
 )
 
 
 def test_switch_env():
     # testuser1 is defined in prod & staging with the same password
     assert os.getenv("LAMIN_ENV") == "prod"
 
     # check whether we can log in
-    login("static-testuser1@lamin.ai", password="static-testuser1-password")
+    login("static-testuser1@lamin.ai", key="static-testuser1-password")
     assert settings.user.email == "static-testuser1@lamin.ai"
 
     # testuser1.staging is defined only in staging
     os.environ["LAMIN_ENV"] = "staging"
 
-    login("testuser1.staging@lamin.ai", password="password")
+    login("testuser1.staging@lamin.ai", key="password")
     assert settings.user.email == "testuser1.staging@lamin.ai"
 
     # back to prod
     os.environ["LAMIN_ENV"] = "prod"
 
 
 def test_connect_instance_fallbacks():
     prod_url = ln_setup.core._hub_client.PROD_URL
     ln_setup.core._hub_client.PROD_URL = (  # deactivated prod url
         "https://inactive.lamin.ai"
     )
-    with pytest.raises(AuthUnknownError):
+    with pytest.raises(AuthRetryableError):
         ln_setup.core._hub_client.connect_hub_with_auth(renew_token=True)
     assert not isinstance(
         sign_in_hub(
             email="static-testuser1@lamin.ai", password="static-testuser1-password"
         ),
         str,
     )
```

### Comparing `lamindb_setup-0.69.0/tests/hub-prod/test_upath.py` & `lamindb_setup-0.69.1/tests/hub-prod/test_upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/tests/storage/test_hashing.py` & `lamindb_setup-0.69.1/tests/storage/test_hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/tests/storage/test_storage_access.py` & `lamindb_setup-0.69.1/tests/storage/test_storage_access.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/tests/storage/test_storage_basis.py` & `lamindb_setup-0.69.1/tests/storage/test_storage_basis.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/tests/storage/test_storage_stats.py` & `lamindb_setup-0.69.1/tests/storage/test_storage_stats.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.0/PKG-INFO` & `lamindb_setup-0.69.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.69.0
+Version: 0.69.1
 Summary: Setup & configure LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.51.0
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django>4.2,<5.2.0
 Requires-Dist: dj_database_url>=1.3.0,<3.0.0
```

