# Comparing `tmp/python_dev_utils-1.2.3.tar.gz` & `tmp/python_dev_utils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dev_utils-1.2.3.tar", last modified: Tue Apr 16 07:59:14 2024, max compression
+gzip compressed data, was "python_dev_utils-1.3.0.tar", last modified: Wed Apr 17 07:02:09 2024, max compression
```

## Comparing `python_dev_utils-1.2.3.tar` & `python_dev_utils-1.3.0.tar`

### file list

```diff
@@ -1,69 +1,71 @@
--rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.2.3/LICENCE
--rw-r--r--   0        0        0     4373 2024-04-15 09:42:56.043729 python_dev_utils-1.2.3/README.md
--rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.2.3/dev_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-1.2.3/dev_utils/core/__init__.py
--rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.2.3/dev_utils/core/abstract.py
--rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.2.3/dev_utils/core/exc.py
--rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.2.3/dev_utils/core/guards.py
--rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.2.3/dev_utils/core/logging.py
--rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.2.3/dev_utils/core/results.py
--rw-r--r--   0        0        0      776 2024-04-12 09:11:29.068964 python_dev_utils-1.2.3/dev_utils/core/utils.py
--rw-r--r--   0        0        0     1618 2024-04-12 10:34:31.616028 python_dev_utils-1.2.3/dev_utils/fastapi/__init__.py
--rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.2.3/dev_utils/fastapi/middlewares/__init__.py
--rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.2.3/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
--rw-r--r--   0        0        0     1564 2024-04-12 10:31:39.700255 python_dev_utils-1.2.3/dev_utils/fastapi/verbose_http_exceptions/__init__.py
--rw-r--r--   0        0        0    12481 2024-04-12 12:10:40.465060 python_dev_utils-1.2.3/dev_utils/fastapi/verbose_http_exceptions/exc.py
--rw-r--r--   0        0        0     4341 2024-04-12 12:19:20.576031 python_dev_utils-1.2.3/dev_utils/fastapi/verbose_http_exceptions/handlers.py
--rw-r--r--   0        0        0      691 2024-04-12 09:58:17.224272 python_dev_utils-1.2.3/dev_utils/fastapi/verbose_http_exceptions/utils.py
--rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-1.2.3/dev_utils/py.typed
--rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.2.3/dev_utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.2.3/dev_utils/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    16338 2024-04-16 06:54:27.234711 python_dev_utils-1.2.3/dev_utils/sqlalchemy/filters/converters.py
--rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.2.3/dev_utils/sqlalchemy/filters/guards.py
--rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.2.3/dev_utils/sqlalchemy/filters/operators.py
--rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.2.3/dev_utils/sqlalchemy/filters/types.py
--rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.2.3/dev_utils/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     3050 2024-04-10 14:09:42.769706 python_dev_utils-1.2.3/dev_utils/sqlalchemy/mixins/audit.py
--rw-r--r--   0        0        0     1141 2024-04-10 08:55:37.140201 python_dev_utils-1.2.3/dev_utils/sqlalchemy/mixins/base.py
--rw-r--r--   0        0        0     1302 2024-04-10 10:08:21.445027 python_dev_utils-1.2.3/dev_utils/sqlalchemy/mixins/general.py
--rw-r--r--   0        0        0      888 2024-04-12 09:11:29.068964 python_dev_utils-1.2.3/dev_utils/sqlalchemy/mixins/ids.py
--rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.2.3/dev_utils/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.2.3/dev_utils/sqlalchemy/profiling/containers.py
--rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.2.3/dev_utils/sqlalchemy/profiling/profilers.py
--rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.2.3/dev_utils/sqlalchemy/profiling/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.2.3/dev_utils/sqlalchemy/types/__init__.py
--rw-r--r--   0        0        0     2244 2024-04-16 07:24:43.054226 python_dev_utils-1.2.3/dev_utils/sqlalchemy/types/datetime.py
--rw-r--r--   0        0        0     1438 2024-04-15 14:05:51.140193 python_dev_utils-1.2.3/dev_utils/sqlalchemy/types/encryption.py
--rw-r--r--   0        0        0     2058 2024-04-15 13:37:44.894136 python_dev_utils-1.2.3/dev_utils/sqlalchemy/types/pydantic.py
--rw-r--r--   0        0        0    12623 2024-04-12 09:11:29.069965 python_dev_utils-1.2.3/dev_utils/sqlalchemy/utils.py
--rw-r--r--   0        0        0     3086 2024-04-16 07:59:14.139815 python_dev_utils-1.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.2.3/tests/__init__.py
--rw-r--r--   0        0        0     9123 2024-04-12 09:01:52.921056 python_dev_utils-1.2.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.2.3/tests/core/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.2.3/tests/core/test_abstract.py
--rw-r--r--   0        0        0      508 2024-04-12 09:01:52.921056 python_dev_utils-1.2.3/tests/core/test_guards.py
--rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.2.3/tests/core/test_results.py
--rw-r--r--   0        0        0      933 2024-04-12 09:01:52.920056 python_dev_utils-1.2.3/tests/core/test_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.2.3/tests/fastapi/__init__.py
--rw-r--r--   0        0        0     1407 2024-04-12 12:14:52.442153 python_dev_utils-1.2.3/tests/fastapi/conftest.py
--rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.2.3/tests/fastapi/test_middlewares.py
--rw-r--r--   0        0        0     6068 2024-04-12 12:24:15.157626 python_dev_utils-1.2.3/tests/fastapi/test_verbose_http_exceptions.py
--rw-r--r--   0        0        0     2072 2024-04-12 12:18:33.383580 python_dev_utils-1.2.3/tests/fastapi/test_verbose_http_exceptions_handlers.py
--rw-r--r--   0        0        0      803 2024-04-12 12:23:22.923870 python_dev_utils-1.2.3/tests/fastapi/test_verbose_http_exceptions_utils.py
--rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.2.3/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.2.3/tests/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.2.3/tests/sqlalchemy/filters/test_converters.py
--rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.2.3/tests/sqlalchemy/filters/test_guards.py
--rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.2.3/tests/sqlalchemy/filters/test_operators.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.2.3/tests/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.2.3/tests/sqlalchemy/mixins/test_audit.py
--rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.2.3/tests/sqlalchemy/mixins/test_base.py
--rw-r--r--   0        0        0     1122 2024-04-12 09:01:52.921056 python_dev_utils-1.2.3/tests/sqlalchemy/mixins/test_general.py
--rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.2.3/tests/sqlalchemy/mixins/test_ids.py
--rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.2.3/tests/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.2.3/tests/sqlalchemy/profiling/test_profilers.py
--rw-r--r--   0        0        0     1423 2024-04-12 13:01:52.229885 python_dev_utils-1.2.3/tests/sqlalchemy/test_types.py
--rw-r--r--   0        0        0     7407 2024-04-12 12:47:25.071609 python_dev_utils-1.2.3/tests/sqlalchemy/test_utils.py
--rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.2.3/tests/types.py
--rw-r--r--   0        0        0     7467 2024-04-12 13:03:36.658336 python_dev_utils-1.2.3/tests/utils.py
--rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 python_dev_utils-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.3.0/LICENCE
+-rw-r--r--   0        0        0     4373 2024-04-15 09:42:56.043729 python_dev_utils-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.3.0/dev_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-1.3.0/dev_utils/core/__init__.py
+-rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/core/abstract.py
+-rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.3.0/dev_utils/core/exc.py
+-rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.3.0/dev_utils/core/guards.py
+-rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/core/logging.py
+-rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.3.0/dev_utils/core/results.py
+-rw-r--r--   0        0        0      215 2024-04-16 09:16:58.960481 python_dev_utils-1.3.0/dev_utils/core/utils/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-16 09:15:43.772084 python_dev_utils-1.3.0/dev_utils/core/utils/datetime.py
+-rw-r--r--   0        0        0      677 2024-04-16 09:16:22.025777 python_dev_utils-1.3.0/dev_utils/core/utils/inspect.py
+-rw-r--r--   0        0        0      209 2024-04-16 09:13:36.355106 python_dev_utils-1.3.0/dev_utils/core/utils/text.py
+-rw-r--r--   0        0        0     1618 2024-04-12 10:34:31.616028 python_dev_utils-1.3.0/dev_utils/fastapi/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.3.0/dev_utils/fastapi/middlewares/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
+-rw-r--r--   0        0        0     1564 2024-04-12 10:31:39.700255 python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py
+-rw-r--r--   0        0        0    12481 2024-04-12 12:10:40.465060 python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/exc.py
+-rw-r--r--   0        0        0     4341 2024-04-12 12:19:20.576031 python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py
+-rw-r--r--   0        0        0      691 2024-04-12 09:58:17.224272 python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-1.3.0/dev_utils/py.typed
+-rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.3.0/dev_utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    16338 2024-04-16 06:54:27.234711 python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/converters.py
+-rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/guards.py
+-rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/operators.py
+-rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/types.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     3050 2024-04-10 14:09:42.769706 python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/audit.py
+-rw-r--r--   0        0        0     1141 2024-04-10 08:55:37.140201 python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/base.py
+-rw-r--r--   0        0        0     1302 2024-04-10 10:08:21.445027 python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/general.py
+-rw-r--r--   0        0        0      888 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/ids.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/containers.py
+-rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/profilers.py
+-rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.3.0/dev_utils/sqlalchemy/types/__init__.py
+-rw-r--r--   0        0        0     2244 2024-04-16 07:24:43.054226 python_dev_utils-1.3.0/dev_utils/sqlalchemy/types/datetime.py
+-rw-r--r--   0        0        0     2349 2024-04-16 10:07:40.662627 python_dev_utils-1.3.0/dev_utils/sqlalchemy/types/pydantic.py
+-rw-r--r--   0        0        0    12370 2024-04-16 09:14:15.986788 python_dev_utils-1.3.0/dev_utils/sqlalchemy/utils.py
+-rw-r--r--   0        0        0     3113 2024-04-17 07:02:09.040941 python_dev_utils-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     9123 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.3.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/core/test_abstract.py
+-rw-r--r--   0        0        0      876 2024-04-16 09:26:13.267072 python_dev_utils-1.3.0/tests/core/test_guards.py
+-rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/core/test_results.py
+-rw-r--r--   0        0        0     1278 2024-04-16 09:18:12.890888 python_dev_utils-1.3.0/tests/core/test_utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.3.0/tests/fastapi/__init__.py
+-rw-r--r--   0        0        0     1407 2024-04-12 12:14:52.442153 python_dev_utils-1.3.0/tests/fastapi/conftest.py
+-rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/fastapi/test_middlewares.py
+-rw-r--r--   0        0        0     6068 2024-04-12 12:24:15.157626 python_dev_utils-1.3.0/tests/fastapi/test_verbose_http_exceptions.py
+-rw-r--r--   0        0        0     2072 2024-04-12 12:18:33.383580 python_dev_utils-1.3.0/tests/fastapi/test_verbose_http_exceptions_handlers.py
+-rw-r--r--   0        0        0      803 2024-04-12 12:23:22.923870 python_dev_utils-1.3.0/tests/fastapi/test_verbose_http_exceptions_utils.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.3.0/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.3.0/tests/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.3.0/tests/sqlalchemy/filters/test_converters.py
+-rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/sqlalchemy/filters/test_guards.py
+-rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.3.0/tests/sqlalchemy/filters/test_operators.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.3.0/tests/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_audit.py
+-rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_base.py
+-rw-r--r--   0        0        0     1122 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_general.py
+-rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_ids.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.3.0/tests/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/sqlalchemy/profiling/test_profilers.py
+-rw-r--r--   0        0        0     1423 2024-04-17 07:01:59.517966 python_dev_utils-1.3.0/tests/sqlalchemy/test_types.py
+-rw-r--r--   0        0        0     7086 2024-04-16 09:18:34.220718 python_dev_utils-1.3.0/tests/sqlalchemy/test_utils.py
+-rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.3.0/tests/types.py
+-rw-r--r--   0        0        0     7726 2024-04-16 09:37:08.400872 python_dev_utils-1.3.0/tests/utils.py
+-rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 python_dev_utils-1.3.0/PKG-INFO
```

### Comparing `python_dev_utils-1.2.3/LICENCE` & `python_dev_utils-1.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/README.md` & `python_dev_utils-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/core/abstract.py` & `python_dev_utils-1.3.0/dev_utils/core/abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/core/exc.py` & `python_dev_utils-1.3.0/dev_utils/core/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/core/guards.py` & `python_dev_utils-1.3.0/dev_utils/core/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/core/logging.py` & `python_dev_utils-1.3.0/dev_utils/core/logging.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/core/results.py` & `python_dev_utils-1.3.0/dev_utils/core/results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/fastapi/__init__.py` & `python_dev_utils-1.3.0/dev_utils/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py` & `python_dev_utils-1.3.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/fastapi/verbose_http_exceptions/__init__.py` & `python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/fastapi/verbose_http_exceptions/exc.py` & `python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/fastapi/verbose_http_exceptions/handlers.py` & `python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/fastapi/verbose_http_exceptions/utils.py` & `python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/filters/converters.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/filters/guards.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/filters/operators.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/filters/types.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/mixins/audit.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/mixins/base.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/mixins/general.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/general.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/mixins/ids.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/ids.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/profiling/containers.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/containers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/profiling/profilers.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/profiling/utils.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/types/datetime.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/types/datetime.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/types/pydantic.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/types/pydantic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 from typing import TYPE_CHECKING, Any, TypeVar
 
+from pydantic import BaseModel
 from pydantic.version import version_short
 from sqlalchemy import JSON as JSON_COLUMN
 from sqlalchemy.dialects.postgresql import JSONB
 from sqlalchemy.types import JSON as JSON_TYPE
 from sqlalchemy.types import TypeDecorator
 
 if TYPE_CHECKING:
@@ -47,14 +48,21 @@
 
     def load_dialect_impl(self, dialect: "Dialect"):  # noqa: D102, ANN201
         if dialect.name == "postgresql":
             return dialect.type_descriptor(JSONB())
         else:
             return dialect.type_descriptor(JSON_COLUMN())
 
+    def _coerce(self, value: Any):
+        if isinstance(value, str):
+            return _parse_obj_as(self.pydantic_type, _to_dict(value))
+        elif isinstance(value, dict):
+            return _parse_obj_as(self.pydantic_type, value)
+        return value
+
     def process_bind_param(  # noqa: D102
         self,
         value: "T | None",
         dialect: "Dialect",  # noqa
     ) -> "T | None":
         return _to_dict(value) if value else None
```

### Comparing `python_dev_utils-1.2.3/dev_utils/sqlalchemy/utils.py` & `python_dev_utils-1.3.0/dev_utils/sqlalchemy/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Utils module of sqlalchemy dev package.
 
 Contains functions, which inspect models, apply joins, apply options and wrap some sqlalchemy
 functionality.
 """
 
-import datetime
 import types
-import zoneinfo
 from typing import TYPE_CHECKING, Any, TypeGuard, TypeVar
 
 from sqlalchemy import Delete, Insert, Select, Table, Update, inspect
 from sqlalchemy.ext.hybrid import HybridExtensionType
 from sqlalchemy.orm import DeclarativeBase, joinedload
 
 from dev_utils.core.exc import (
@@ -34,24 +32,14 @@
     Select[tuple["DeclarativeBase"]]
     | Update["DeclarativeBase"]
     | Delete["DeclarativeBase"]
     | Insert["DeclarativeBase"]
 )
 
 
-def get_utc_now() -> datetime.datetime:
-    """Get current UTC datetime.
-
-    Returns
-    -------
-        datetime: current datetime with UTC timezone.
-    """
-    return datetime.datetime.now(zoneinfo.ZoneInfo("UTC"))
-
-
 def is_declarative(model: Any) -> TypeGuard["Mapper[Any]"]:  # noqa: ANN401
     """Get sqlalchemy field (column) or relationship object from given model.
 
     Args
     ----
     model : Any
         Any object.
```

### Comparing `python_dev_utils-1.2.3/pyproject.toml` & `python_dev_utils-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     "enum.Enum",
     "(Protocol)",
     "pragma: no cover",
+    "pragma: no coverage",
     "raise NotImplementedError",
     "if TYPE_CHECKING:",
     "if typing.TYPE_CHECKING:",
     "@overload",
 ]
 
 [tool.pytest]
@@ -168,15 +169,15 @@
     "asyncpg>=0.29.0",
     "pytest-asyncio>=0.23.6",
     "httpx>=0.27.0",
 ]
 
 [project]
 name = "python_dev_utils"
-version = "1.2.3"
+version = "1.3.0"
 description = "My project utils package, that I use in my projects."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = []
```

### Comparing `python_dev_utils-1.2.3/tests/conftest.py` & `python_dev_utils-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/core/test_abstract.py` & `python_dev_utils-1.3.0/tests/core/test_abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/core/test_results.py` & `python_dev_utils-1.3.0/tests/core/test_results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/core/test_utils.py` & `python_dev_utils-1.3.0/tests/core/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,33 @@
+import datetime
+import zoneinfo
+
 import pytest
+from freezegun import freeze_time
 
 from dev_utils.core import utils
+from tests.utils import generate_datetime_list
 
 obj = object()
 
 
 class MyObject:  # noqa: D101
     pass
 
 
 @pytest.mark.parametrize(
+    "dt",
+    generate_datetime_list(n=10, tz=zoneinfo.ZoneInfo("UTC")),
+)
+def test_get_utc_now(dt: datetime.datetime) -> None:  # noqa
+    with freeze_time(dt):
+        assert utils.get_utc_now() == dt
+
+
+@pytest.mark.parametrize(
     ("obj", "expected_result"),
     [
         (obj, "object"),
         (MyObject, "tests.core.test_utils.MyObject"),
         (MyObject(), "tests.core.test_utils.MyObject"),
     ],
 )
```

### Comparing `python_dev_utils-1.2.3/tests/fastapi/conftest.py` & `python_dev_utils-1.3.0/tests/fastapi/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/fastapi/test_verbose_http_exceptions.py` & `python_dev_utils-1.3.0/tests/fastapi/test_verbose_http_exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/fastapi/test_verbose_http_exceptions_handlers.py` & `python_dev_utils-1.3.0/tests/fastapi/test_verbose_http_exceptions_handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/fastapi/test_verbose_http_exceptions_utils.py` & `python_dev_utils-1.3.0/tests/fastapi/test_verbose_http_exceptions_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/sqlalchemy/filters/test_converters.py` & `python_dev_utils-1.3.0/tests/sqlalchemy/filters/test_converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/sqlalchemy/filters/test_guards.py` & `python_dev_utils-1.3.0/tests/sqlalchemy/filters/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/sqlalchemy/filters/test_operators.py` & `python_dev_utils-1.3.0/tests/sqlalchemy/filters/test_operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/sqlalchemy/mixins/test_audit.py` & `python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/sqlalchemy/mixins/test_base.py` & `python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/sqlalchemy/mixins/test_general.py` & `python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_general.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/sqlalchemy/profiling/test_profilers.py` & `python_dev_utils-1.3.0/tests/sqlalchemy/profiling/test_profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/sqlalchemy/test_types.py` & `python_dev_utils-1.3.0/tests/sqlalchemy/test_types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/sqlalchemy/test_utils.py` & `python_dev_utils-1.3.0/tests/sqlalchemy/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,17 @@
-import datetime
-import zoneinfo
 from collections.abc import Sequence
 from typing import Any
 
 import pytest
-from freezegun import freeze_time
 from sqlalchemy import delete, func, insert, inspect, select, update
 from sqlalchemy.orm import DeclarativeBase, joinedload, selectinload, subqueryload
 
 from dev_utils.core.exc import NoModelAttributeError, NoModelRelationshipError
 from dev_utils.sqlalchemy import utils
-from tests.utils import Base, MyModel, OtherModel, generate_datetime_list
-
-
-@pytest.mark.parametrize(
-    "dt",
-    generate_datetime_list(n=10, tz=zoneinfo.ZoneInfo("UTC")),
-)
-def test_get_utc_now(dt: datetime.datetime) -> None:  # noqa
-    with freeze_time(dt):
-        assert utils.get_utc_now() == dt
+from tests.utils import Base, MyModel, OtherModel
 
 
 @pytest.mark.parametrize(
     ("obj", "expected_result"),
     [
         (MyModel, True),
         (254, False),
```

### Comparing `python_dev_utils-1.2.3/tests/types.py` & `python_dev_utils-1.3.0/tests/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.2.3/tests/utils.py` & `python_dev_utils-1.3.0/tests/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import datetime
 import random
 from typing import TYPE_CHECKING, Any, TypeVar
 
+from pydantic import BaseModel
 from sqlalchemy import ForeignKey, inspect
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.ext.hybrid import hybrid_method, hybrid_property
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column, relationship
 from sqlalchemy_utils import create_database, database_exists, drop_database  # type: ignore
 
-from dev_utils.sqlalchemy.types.datetime import UTCDateTime  # type: ignore
+from dev_utils.sqlalchemy.types.datetime import UTCDateTime
+from dev_utils.sqlalchemy.types.pydantic import PydanticType
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import Session
 
@@ -182,14 +184,20 @@
         await session.commit() if commit else await session.flush()
     except SQLAlchemyError:
         await session.rollback()
         raise
     return item
 
 
+class PydanticTestSchema(BaseModel):  # noqa: D101
+    a: int
+    b: int
+    c: int
+
+
 class Base(DeclarativeBase):  # noqa
     pass
 
 
 class MyModel(Base):  # noqa
     __tablename__ = "my_model"
 
@@ -228,7 +236,8 @@
 
 
 class TableWithUTCDT(Base):  # noqa: D101
     __tablename__ = "table_with_UTC_dt"
 
     id: Mapped[int] = mapped_column(primary_key=True)  # noqa
     dt_field: Mapped[datetime.datetime] = mapped_column(UTCDateTime)
+    pydantic_field: Mapped[PydanticTestSchema] = mapped_column(PydanticType(PydanticTestSchema))
```

### Comparing `python_dev_utils-1.2.3/PKG-INFO` & `python_dev_utils-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_dev_utils
-Version: 1.2.3
+Version: 1.3.0
 Summary: My project utils package, that I use in my projects.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Provides-Extra: fastapi-exceptions
 Provides-Extra: profiling
 Provides-Extra: sqlalchemy-filters
```

