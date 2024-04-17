# Comparing `tmp/firebolt_sdk-1.4.0.tar.gz` & `tmp/firebolt_sdk-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/firebolt-python-sdk/firebolt-python-sdk/dist/.tmp-17rkunnd/firebolt_sdk-1.4.0.tar", last modified: Thu Mar 21 09:32:06 2024, max compression
+gzip compressed data, was "/home/runner/work/firebolt-python-sdk/firebolt-python-sdk/dist/.tmp-lg12hel_/firebolt_sdk-1.4.1.tar", last modified: Wed Apr 17 09:22:21 2024, max compression
```

## Comparing `firebolt_sdk-1.4.0.tar` & `firebolt_sdk-1.4.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:06.000000 firebolt_sdk-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-03-21 09:32:06.000000 firebolt_sdk-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2221 2024-03-21 09:32:06.000000 firebolt_sdk-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-21 09:32:01.000000 firebolt_sdk-1.4.0/src/firebolt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt/async_db/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/async_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11821 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/async_db/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    23574 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/async_db/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/async_db/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt/client/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt/client/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/client/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/client/auth/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/client/auth/client_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/client/auth/request_auth_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/client/auth/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/client/auth/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/client/auth/username_password.py
--rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/client/http_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/client/resource_manager_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt/common/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/common/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/common/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15793 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/common/base_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/common/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/common/token_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/common/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/common/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt/db/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21770 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/db/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/db/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt/model/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt/model/V1/
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/model/V1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/model/V1/binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/model/V1/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/model/V1/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/model/V1/engine_revision.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/model/V1/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/model/V1/region.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt/model/V2/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/model/V2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/model/V2/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8728 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/model/V2/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/model/V2/instance_type.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/model/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt/service/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt/service/V1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V1/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V1/binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V1/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V1/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V1/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V1/region.py
--rw-r--r--   0 runner    (1001) docker     (127)    10219 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V1/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt/service/V2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V2/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V2/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V2/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V2/instance_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/V2/types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/service/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:06.000000 firebolt_sdk-1.4.0/src/firebolt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/utils/token_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/utils/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/utils/usage_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-03-21 09:31:52.000000 firebolt_sdk-1.4.0/src/firebolt/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:32:06.000000 firebolt_sdk-1.4.0/src/firebolt_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-21 09:32:05.000000 firebolt_sdk-1.4.0/src/firebolt_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2221 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 09:22:15.000000 firebolt_sdk-1.4.1/src/firebolt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/async_db/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/async_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/async_db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19455 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/async_db/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/async_db/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/client_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/request_auth_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/username_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/http_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/resource_manager_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/base_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/token_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11435 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17855 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/db/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/db/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/model/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/engine_revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/region.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/model/V2/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V2/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V2/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V2/instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/service/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10219 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/utils/token_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/utils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/utils/usage_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/top_level.txt
```

### Comparing `firebolt_sdk-1.4.0/LICENSE` & `firebolt_sdk-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/PKG-INFO` & `firebolt_sdk-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebolt_sdk
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python SDK for Firebolt
 Home-page: https://github.com/firebolt-db/firebolt-sdk
 Author: Firebolt
 Author-email: support@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/firebolt-sdk/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `firebolt_sdk-1.4.0/README.md` & `firebolt_sdk-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/setup.cfg` & `firebolt_sdk-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/async_db/__init__.py` & `firebolt_sdk-1.4.1/src/firebolt/async_db/__init__.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/async_db/connection.py` & `firebolt_sdk-1.4.1/src/firebolt/async_db/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from types import TracebackType
 from typing import Any, Dict, List, Optional, Type
 
 from httpx import Timeout
 
 from firebolt.async_db.cursor import Cursor, CursorV1, CursorV2
-from firebolt.async_db.util import _get_system_engine_url
+from firebolt.async_db.util import _get_system_engine_url_and_params
 from firebolt.client import DEFAULT_API_URL
 from firebolt.client.auth import Auth
 from firebolt.client.client import AsyncClient, AsyncClientV1, AsyncClientV2
 from firebolt.common.base_connection import BaseConnection
 from firebolt.common.constants import (
     DEFAULT_TIMEOUT_SECONDS,
     ENGINE_STATUS_RUNNING_LIST,
@@ -202,16 +202,16 @@
 
     # Type checks
     assert auth is not None
     assert account_name is not None
 
     api_endpoint = fix_url_schema(api_endpoint)
 
-    system_engine_url = fix_url_schema(
-        await _get_system_engine_url(auth, account_name, api_endpoint)
+    system_engine_url, system_engine_params = await _get_system_engine_url_and_params(
+        auth, account_name, api_endpoint
     )
 
     client = AsyncClientV2(
         auth=auth,
         account_name=account_name,
         base_url=system_engine_url,
         api_endpoint=api_endpoint,
@@ -223,14 +223,15 @@
     system_engine_connection = Connection(
         system_engine_url,
         database,
         client,
         CursorV2,
         None,
         api_endpoint,
+        system_engine_params,
     )
 
     account_version = await system_engine_connection._client._account_version
     if account_version == 2:
         cursor = system_engine_connection.cursor()
         if database:
             await cursor.execute(f"USE DATABASE {database}")
```

### Comparing `firebolt_sdk-1.4.0/src/firebolt/async_db/cursor.py` & `firebolt_sdk-1.4.1/src/firebolt/async_db/cursor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import logging
-import re
 import time
 from abc import ABCMeta, abstractmethod
 from functools import wraps
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
@@ -31,37 +30,35 @@
 from firebolt.common.base_cursor import (
     JSON_OUTPUT_FORMAT,
     RESET_SESSION_HEADER,
     UPDATE_ENDPOINT_HEADER,
     UPDATE_PARAMETERS_HEADER,
     BaseCursor,
     CursorState,
-    QueryStatus,
     Statistics,
     _parse_update_endpoint,
     _parse_update_parameters,
     _raise_if_internal_set_parameter,
     check_not_closed,
     check_query_executed,
 )
 from firebolt.common.constants import ENGINE_STATUS_RUNNING_LIST
 from firebolt.utils.exception import (
-    AsyncExecutionUnavailableError,
     EngineNotRunningError,
     FireboltDatabaseError,
     FireboltEngineError,
     OperationalError,
     ProgrammingError,
 )
 from firebolt.utils.urls import DATABASES_URL, ENGINES_URL
 
 if TYPE_CHECKING:
     from firebolt.async_db.connection import Connection
 
-from firebolt.utils.util import Timer, _print_error_body
+from firebolt.utils.util import _print_error_body
 
 logger = logging.getLogger(__name__)
 
 
 class Cursor(BaseCursor, metaclass=ABCMeta):
     """
     Class, responsible for executing queries to Firebolt Database.
@@ -122,20 +119,14 @@
             )
         _print_error_body(resp)
         resp.raise_for_status()
 
     async def _validate_set_parameter(self, parameter: SetParameter) -> None:
         """Validate parameter by executing simple query with it."""
         _raise_if_internal_set_parameter(parameter)
-        if parameter.name == "async_execution":
-            raise AsyncExecutionUnavailableError(
-                "It is not possible to set async_execution using a SET command. "
-                "Instead, pass it as an argument to the execute() or "
-                "executemany() function."
-            )
         resp = await self._api_request("select 1", {parameter.name: parameter.value})
         # Handle invalid set parameter
         if resp.status_code == codes.BAD_REQUEST:
             raise OperationalError(resp.text)
         await self._raise_if_error(resp)
 
         # set parameter passed validation
@@ -166,70 +157,34 @@
             self._update_set_parameters(param_dict)
 
     async def _do_execute(
         self,
         raw_query: str,
         parameters: Sequence[Sequence[ParameterType]],
         skip_parsing: bool = False,
-        async_execution: Optional[bool] = False,
     ) -> None:
         self._reset()
         # Allow users to manually skip parsing for performance improvement.
         queries: List[Union[SetParameter, str]] = (
             [raw_query] if skip_parsing else split_format_sql(raw_query, parameters)
         )
         try:
             for query in queries:
                 start_time = time.time()
-                # Our CREATE EXTERNAL TABLE queries currently require credentials,
-                # so we will skip logging those queries.
-                # https://docs.firebolt.io/sql-reference/commands/create-external-table.html
-                if isinstance(query, SetParameter) or not re.search(
-                    "aws_key_id|credentials", query, flags=re.IGNORECASE
-                ):
-                    logger.debug(f"Running query: {query}")
+                Cursor._log_query(query)
 
                 # Define type for mypy
                 row_set: Tuple[
                     int,
                     Optional[List[Column]],
                     Optional[Statistics],
                     Optional[List[List[RawColType]]],
                 ] = (-1, None, None, None)
                 if isinstance(query, SetParameter):
                     await self._validate_set_parameter(query)
-                elif async_execution:
-                    self._validate_server_side_async_settings(
-                        parameters,
-                        queries,
-                        skip_parsing,
-                        async_execution,
-                    )
-
-                    with Timer(
-                        f"[PERFORMANCE] Running query {query[:50]} "
-                        f"{'... ' if len(query) > 50 else ''}"
-                    ):
-                        response = await self._api_request(
-                            query,
-                            {
-                                "async_execution": 1,
-                                "output_format": JSON_OUTPUT_FORMAT,
-                            },
-                        )
-
-                    await self._raise_if_error(response)
-                    if response.headers.get("content-length", "") == "0":
-                        raise OperationalError("No response to asynchronous query.")
-                    resp = response.json()
-                    if "query_id" not in resp or resp["query_id"] == "":
-                        raise OperationalError(
-                            "Invalid response to asynchronous query: missing query_id."
-                        )
-                    self._query_id = resp["query_id"]
                 else:
                     resp = await self._api_request(
                         query, {"output_format": JSON_OUTPUT_FORMAT}
                     )
                     await self._raise_if_error(resp)
                     await self._parse_response_headers(resp.headers)
                     row_set = self._row_set_from_response(resp)
@@ -249,15 +204,14 @@
 
     @check_not_closed
     async def execute(
         self,
         query: str,
         parameters: Optional[Sequence[ParameterType]] = None,
         skip_parsing: bool = False,
-        async_execution: Optional[bool] = False,
     ) -> Union[int, str]:
         """Prepare and execute a database query.
 
         Supported features:
             Parameterized queries: placeholder characters ('?') are substituted
                 with values provided in `parameters`. Values are formatted to
                 be properly recognized by database and to exclude SQL injection.
@@ -273,29 +227,27 @@
             query (str): SQL query to execute
             parameters (Optional[Sequence[ParameterType]]): A sequence of substitution
                 parameters. Used to replace '?' placeholders inside a query with
                 actual values
             skip_parsing (bool): Flag to disable query parsing. This will
                 disable parameterized, multi-statement and SET queries,
                 while improving performance
-            async_execution (bool): flag to determine if query should be asynchronous
 
         Returns:
             int: Query row count.
         """
         params_list = [parameters] if parameters else []
-        await self._do_execute(query, params_list, skip_parsing, async_execution)
-        return self.query_id if async_execution else self.rowcount
+        await self._do_execute(query, params_list, skip_parsing)
+        return self.rowcount
 
     @check_not_closed
     async def executemany(
         self,
         query: str,
         parameters_seq: Sequence[Sequence[ParameterType]],
-        async_execution: Optional[bool] = False,
     ) -> Union[int, str]:
         """Prepare and execute a database query.
 
         Supports providing multiple substitution parameter sets, executing them
         as multiple statements sequentially.
 
         Supported features:
@@ -312,54 +264,20 @@
 
         Args:
             query (str): SQL query to execute.
             parameters_seq (Sequence[Sequence[ParameterType]]): A sequence of
                substitution parameter sets. Used to replace '?' placeholders inside a
                query with actual values from each set in a sequence. Resulting queries
                for each subset are executed sequentially.
-            async_execution (bool): flag to determine if query should be asynchronous
 
         Returns:
-            int|str: Query row count for synchronous execution of queries,
-            query ID string for asynchronous execution.
+            int: Query row count.
         """
-        await self._do_execute(query, parameters_seq, async_execution=async_execution)
-        if async_execution:
-            return self.query_id
-        else:
-            return self.rowcount
-
-    @check_not_closed
-    async def get_status(self, query_id: str) -> QueryStatus:
-        """Get status of a server-side async query. Return the state of the query."""
-        try:
-            resp = await self._api_request(
-                # output_format must be empty for status to work correctly.
-                # And set parameters will cause 400 errors.
-                parameters={"query_id": query_id},
-                path="status",
-                use_set_parameters=False,
-            )
-            if resp.status_code == codes.BAD_REQUEST:
-                raise OperationalError(
-                    f"Asynchronous query {query_id} status check failed: "
-                    f"{resp.status_code}."
-                )
-            resp_json = resp.json()
-            if "status" not in resp_json:
-                raise OperationalError(
-                    "Invalid response to asynchronous query: missing status."
-                )
-        except Exception:
-            self._state = CursorState.ERROR
-            raise
-        # Remember that query_id might be empty.
-        if resp_json["status"] == "":
-            return QueryStatus.NOT_READY
-        return QueryStatus[resp_json["status"]]
+        await self._do_execute(query, parameters_seq)
+        return self.rowcount
 
     @abstractmethod
     async def is_db_available(self, database: str) -> bool:
         """Verify that the database exists."""
         ...
 
     @abstractmethod
@@ -385,23 +303,14 @@
         """Fetch all remaining rows of a query result."""
         return super().fetchall()
 
     @wraps(BaseCursor.nextset)
     async def nextset(self) -> None:
         return super().nextset()
 
-    @check_not_closed
-    async def cancel(self, query_id: str) -> None:
-        """Cancel a server-side async query."""
-        await self._api_request(
-            parameters={"query_id": query_id},
-            path="cancel",
-            use_set_parameters=False,
-        )
-
     # Iteration support
     @check_not_closed
     @check_query_executed
     def __aiter__(self) -> Cursor:
         return self
 
     # TODO: figure out how to implement __aenter__ and __await__
@@ -465,20 +374,21 @@
                     JSON_OUTPUT_FORMAT will be used.
             path (str): endpoint suffix, for example "cancel" or "status"
             use_set_parameters: Optional[bool]: Some queries will fail if additional
                 set parameters are sent. Setting this to False will allow
                 self._set_parameters to be ignored.
         """
         parameters = parameters or {}
+        account_version = await self._client._account_version
         if use_set_parameters:
             parameters = {**(self._set_parameters or {}), **parameters}
         if self.parameters:
             parameters = {**self.parameters, **parameters}
-        # Engines v2 always require account_id
-        if self.connection._is_system or (await self._client._account_version) == 2:
+        # Engines v2 will have account context in the URL
+        if self.connection._is_system and account_version == 1:
             assert isinstance(self._client, AsyncClientV2)
             parameters["account_id"] = await self._client.account_id
         return await self._client.request(
             url=f"/{path}" if path else "",
             method="POST",
             params=parameters,
             content=query,
@@ -552,15 +462,15 @@
     ) -> None:
         assert isinstance(client, AsyncClientV1)
         super().__init__(*args, client=client, connection=connection, **kwargs)
 
     async def _api_request(
         self,
         query: Optional[str] = "",
-        parameters: Optional[dict[str, Any]] = {},
+        parameters: Optional[dict[str, Any]] = None,
         path: Optional[str] = "",
         use_set_parameters: Optional[bool] = True,
     ) -> Response:
         """
         Query API, return Response object.
 
         Args:
```

### Comparing `firebolt_sdk-1.4.0/src/firebolt/async_db/util.py` & `firebolt_sdk-1.4.1/src/firebolt/db/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from __future__ import annotations
 
+from typing import Dict, Tuple
+
 from httpx import Timeout, codes
 
+from firebolt.client import ClientV2
 from firebolt.client.auth import Auth
-from firebolt.client.client import AsyncClientV2
 from firebolt.common.constants import DEFAULT_TIMEOUT_SECONDS
 from firebolt.utils.exception import (
     AccountNotFoundOrNoAccessError,
     InterfaceError,
 )
 from firebolt.utils.urls import GATEWAY_HOST_BY_ACCOUNT_NAME
+from firebolt.utils.util import parse_url_and_params
 
 
-async def _get_system_engine_url(
+def _get_system_engine_url_and_params(
     auth: Auth,
     account_name: str,
     api_endpoint: str,
-) -> str:
-    async with AsyncClientV2(
+) -> Tuple[str, Dict[str, str]]:
+    with ClientV2(
         auth=auth,
         base_url=api_endpoint,
         account_name=account_name,
         api_endpoint=api_endpoint,
         timeout=Timeout(DEFAULT_TIMEOUT_SECONDS),
     ) as client:
         url = GATEWAY_HOST_BY_ACCOUNT_NAME.format(account_name=account_name)
-        response = await client.get(url=url)
+        response = client.get(url=url)
         if response.status_code == codes.NOT_FOUND:
             raise AccountNotFoundOrNoAccessError(account_name)
         if response.status_code != codes.OK:
             raise InterfaceError(
                 f"Unable to retrieve system engine endpoint {url}: "
                 f"{response.status_code} {response.content.decode()}"
             )
-        return response.json()["engineUrl"]
+        return parse_url_and_params(response.json()["engineUrl"])
```

### Comparing `firebolt_sdk-1.4.0/src/firebolt/client/auth/base.py` & `firebolt_sdk-1.4.1/src/firebolt/client/auth/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod
 from time import time
 from typing import AsyncGenerator, Generator, Optional
 
-from anyio import Lock
+from anyio import Lock, get_current_task
 from httpx import Auth as HttpxAuth
 from httpx import Request, Response, codes
 
 from firebolt.utils.token_storage import TokenSecureStorage
 from firebolt.utils.util import Timer, cached_property, get_internal_error_code
 
 
@@ -145,20 +145,31 @@
         Overridden in order to lock and ensure no more than
         one authentication request is sent at a time. This
         avoids excessive load on the auth server.
         """
         if self.requires_request_body:
             await request.aread()
 
-        async with self._lock:
-            flow = self.auth_flow(request)
-            request = next(flow)
-
-            while True:
-                response = yield request
-                if self.requires_response_body:
-                    await response.aread()
-
-                try:
-                    request = flow.send(response)
-                except StopIteration:
-                    break
+        if not self.token or self.expired:
+            await self._lock.acquire()
+            # If another task has already updated the token,
+            # we don't need to hold the lock
+            if self.token and not self.expired:
+                self._lock.release()
+
+        flow = self.auth_flow(request)
+        request = next(flow)
+
+        while True:
+            response = yield request
+            if self.requires_response_body:
+                await response.aread()
+
+            try:
+                request = flow.send(response)
+            except StopIteration:
+                break
+            finally:
+                # token gets updated only after flow.send is called
+                # so unlock only after that
+                if self._lock.locked() and self._lock._owner_task == get_current_task():
+                    self._lock.release()
```

### Comparing `firebolt_sdk-1.4.0/src/firebolt/client/auth/client_credentials.py` & `firebolt_sdk-1.4.1/src/firebolt/client/auth/client_credentials.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/client/auth/request_auth_base.py` & `firebolt_sdk-1.4.1/src/firebolt/client/auth/request_auth_base.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/client/auth/service_account.py` & `firebolt_sdk-1.4.1/src/firebolt/client/auth/service_account.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/client/auth/token.py` & `firebolt_sdk-1.4.1/src/firebolt/client/auth/token.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/client/auth/username_password.py` & `firebolt_sdk-1.4.1/src/firebolt/client/auth/username_password.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/client/client.py` & `firebolt_sdk-1.4.1/src/firebolt/client/client.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/client/http_backend.py` & `firebolt_sdk-1.4.1/src/firebolt/client/http_backend.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/client/resource_manager_hooks.py` & `firebolt_sdk-1.4.1/src/firebolt/client/resource_manager_hooks.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/common/_types.py` & `firebolt_sdk-1.4.1/src/firebolt/common/_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         if value.tzinfo is not None:
             value = value.astimezone(timezone.utc)
         return f"'{value.strftime('%Y-%m-%d %H:%M:%S')}'"
     elif isinstance(value, date):
         return f"'{value.isoformat()}'"
     elif isinstance(value, bytes):
         # Encode each byte into hex
-        return "'" + "".join(f"\\x{b:02x}" for b in value) + "'"
+        return "E'" + "".join(f"\\x{b:02x}" for b in value) + "'"
     if value is None:
         return "NULL"
     elif isinstance(value, Sequence):
         return f"[{', '.join(format_value(it) for it in value)}]"
 
     raise DataError(f"unsupported parameter type {type(value)}")
```

### Comparing `firebolt_sdk-1.4.0/src/firebolt/common/base_connection.py` & `firebolt_sdk-1.4.1/src/firebolt/common/base_connection.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/common/base_cursor.py` & `firebolt_sdk-1.4.1/src/firebolt/common/base_cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from __future__ import annotations
 
 import logging
+import re
 from dataclasses import dataclass, fields
 from enum import Enum
 from functools import wraps
 from types import TracebackType
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from httpx import URL, Response
 
 from firebolt.common._types import (
     ColType,
     Column,
-    ParameterType,
     RawColType,
     SetParameter,
     parse_type,
     parse_value,
 )
 from firebolt.utils.exception import (
-    AsyncExecutionUnavailableError,
     ConfigurationError,
     CursorClosedError,
     DataError,
     QueryNotRunError,
 )
 from firebolt.utils.util import Timer, fix_url_schema
 
@@ -36,31 +35,18 @@
 class CursorState(Enum):
     NONE = 1
     ERROR = 2
     DONE = 3
     CLOSED = 4
 
 
-class QueryStatus(Enum):
-    """Enumeration of query responses on server-side async queries."""
-
-    RUNNING = 1
-    ENDED_SUCCESSFULLY = 2
-    ENDED_UNSUCCESSFULLY = 3
-    NOT_READY = 4
-    STARTED_EXECUTION = 5
-    PARSE_ERROR = 6
-    CANCELED_EXECUTION = 7
-    EXECUTION_ERROR = 8
-
-
 # Parameters that should be set using USE instead of SET
 USE_PARAMETER_LIST = ["database", "engine"]
 # parameters that can only be set by the backend
-DISALLOWED_PARAMETER_LIST = ["account_id", "output_format"]
+DISALLOWED_PARAMETER_LIST = ["output_format"]
 # parameters that are set by the backend and should not be set by the user
 IMMUTABLE_PARAMETER_LIST = USE_PARAMETER_LIST + DISALLOWED_PARAMETER_LIST
 
 UPDATE_ENDPOINT_HEADER = "Firebolt-Update-Endpoint"
 UPDATE_PARAMETERS_HEADER = "Firebolt-Update-Parameters"
 RESET_SESSION_HEADER = "Firebolt-Reset-Session"
 
@@ -321,14 +307,24 @@
 
         self._set_parameters.update(user_parameters)
 
     def _update_server_parameters(self, parameters: Dict[str, Any]) -> None:
         for key, value in parameters.items():
             self.parameters[key] = value
 
+    @staticmethod
+    def _log_query(query: Union[str, SetParameter]) -> None:
+        # Our CREATE EXTERNAL TABLE queries currently require credentials,
+        # so we will skip logging those queries.
+        # https://docs.firebolt.io/sql-reference/commands/create-external-table.html
+        if isinstance(query, SetParameter) or not re.search(
+            "aws_key_id|credentials", query, flags=re.IGNORECASE
+        ):
+            logger.debug(f"Running query: {query}")
+
     @property
     def engine_name(self) -> str:
         """
         Get the name of the engine that we're using.
 
         Args:
             engine_url (str): URL of the engine
@@ -378,41 +374,14 @@
     ) -> None:
         """Store information about executed query."""
         self._row_sets.append(row_set)
         if self._next_set_idx == 0:
             # Populate values for first set
             self._pop_next_set()
 
-    def _validate_server_side_async_settings(
-        self,
-        parameters: Sequence[Sequence[ParameterType]],
-        queries: List[Union[SetParameter, str]],
-        skip_parsing: bool = False,
-        async_execution: Optional[bool] = False,
-    ) -> None:
-        if async_execution and self._set_parameters.get("use_standard_sql", "1") == "0":
-            raise AsyncExecutionUnavailableError(
-                "It is not possible to execute queries asynchronously if "
-                "use_standard_sql=0."
-            )
-        if parameters and skip_parsing:
-            logger.warning(
-                "Query formatting parameters are provided but skip_parsing "
-                "is specified. They will be ignored."
-            )
-        non_set_queries = 0
-        for query in queries:
-            if type(query) is not SetParameter:
-                non_set_queries += 1
-        if non_set_queries > 1 and async_execution:
-            raise AsyncExecutionUnavailableError(
-                "It is not possible to execute multi-statement "
-                "queries asynchronously."
-            )
-
     def _parse_row(self, row: List[RawColType]) -> List[ColType]:
         """Parse a single data row based on query column types."""
         assert len(row) == len(self.description)
         return [
             parse_value(col, self.description[i].type_code) for i, col in enumerate(row)
         ]
```

### Comparing `firebolt_sdk-1.4.0/src/firebolt/common/settings.py` & `firebolt_sdk-1.4.1/src/firebolt/common/settings.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/db/__init__.py` & `firebolt_sdk-1.4.1/src/firebolt/db/__init__.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/db/connection.py` & `firebolt_sdk-1.4.1/src/firebolt/db/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from firebolt.client.auth import Auth
 from firebolt.common.base_connection import BaseConnection
 from firebolt.common.constants import (
     DEFAULT_TIMEOUT_SECONDS,
     ENGINE_STATUS_RUNNING_LIST,
 )
 from firebolt.db.cursor import Cursor, CursorV1, CursorV2
-from firebolt.db.util import _get_system_engine_url
+from firebolt.db.util import _get_system_engine_url_and_params
 from firebolt.utils.exception import (
     ConfigurationError,
     ConnectionClosedError,
     EngineNotRunningError,
     InterfaceError,
 )
 from firebolt.utils.usage_tracker import get_user_agent_header
@@ -105,16 +105,16 @@
 
     # Type checks
     assert auth is not None
     assert account_name is not None
 
     api_endpoint = fix_url_schema(api_endpoint)
 
-    system_engine_url = fix_url_schema(
-        _get_system_engine_url(auth, account_name, api_endpoint)
+    system_engine_url, system_engine_params = _get_system_engine_url_and_params(
+        auth, account_name, api_endpoint
     )
 
     client = ClientV2(
         auth=auth,
         account_name=account_name,
         base_url=system_engine_url,
         api_endpoint=api_endpoint,
@@ -126,14 +126,15 @@
     system_engine_connection = Connection(
         system_engine_url,
         database,
         client,
         CursorV2,
         None,
         api_endpoint,
+        system_engine_params,
     )
 
     if system_engine_connection._client._account_version == 2:
         cursor = system_engine_connection.cursor()
         if database:
             cursor.execute(f"USE DATABASE {database}")
         if engine_name:
```

### Comparing `firebolt_sdk-1.4.0/src/firebolt/db/cursor.py` & `firebolt_sdk-1.4.1/src/firebolt/db/cursor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import logging
-import re
 import time
 from abc import ABCMeta, abstractmethod
 from typing import (
     TYPE_CHECKING,
     Any,
     Generator,
     List,
@@ -29,25 +28,23 @@
 from firebolt.common.base_cursor import (
     JSON_OUTPUT_FORMAT,
     RESET_SESSION_HEADER,
     UPDATE_ENDPOINT_HEADER,
     UPDATE_PARAMETERS_HEADER,
     BaseCursor,
     CursorState,
-    QueryStatus,
     Statistics,
     _parse_update_endpoint,
     _parse_update_parameters,
     _raise_if_internal_set_parameter,
     check_not_closed,
     check_query_executed,
 )
 from firebolt.common.constants import ENGINE_STATUS_RUNNING_LIST
 from firebolt.utils.exception import (
-    AsyncExecutionUnavailableError,
     EngineNotRunningError,
     FireboltDatabaseError,
     FireboltEngineError,
     OperationalError,
     ProgrammingError,
 )
 from firebolt.utils.urls import DATABASES_URL, ENGINES_URL
@@ -121,20 +118,14 @@
         use_set_parameters: bool = True,
     ) -> Response:
         ...
 
     def _validate_set_parameter(self, parameter: SetParameter) -> None:
         """Validate parameter by executing simple query with it."""
         _raise_if_internal_set_parameter(parameter)
-        if parameter.name == "async_execution":
-            raise AsyncExecutionUnavailableError(
-                "It is not possible to set async_execution using a SET command. "
-                "Instead, pass it as an argument to the execute() or "
-                "executemany() function."
-            )
         resp = self._api_request("select 1", {parameter.name: parameter.value})
         # Handle invalid set parameter
         if resp.status_code == codes.BAD_REQUEST:
             raise OperationalError(resp.text)
         self._raise_if_error(resp)
 
         # set parameter passed validation
@@ -165,64 +156,35 @@
             self._update_set_parameters(param_dict)
 
     def _do_execute(
         self,
         raw_query: str,
         parameters: Sequence[Sequence[ParameterType]],
         skip_parsing: bool = False,
-        async_execution: Optional[bool] = False,
     ) -> None:
         self._reset()
         # Allow users to manually skip parsing for performance improvement.
         queries: List[Union[SetParameter, str]] = (
             [raw_query] if skip_parsing else split_format_sql(raw_query, parameters)
         )
         try:
             for query in queries:
                 start_time = time.time()
-                # Our CREATE EXTERNAL TABLE queries currently require credentials,
-                # so we will skip logging those queries.
-                # https://docs.firebolt.io/sql-reference/commands/create-external-table.html
-                if isinstance(query, SetParameter) or not re.search(
-                    "aws_key_id|credentials", query, flags=re.IGNORECASE
-                ):
-                    logger.debug(f"Running query: {query}")
+
+                Cursor._log_query(query)
 
                 # Define type for mypy
                 row_set: Tuple[
                     int,
                     Optional[List[Column]],
                     Optional[Statistics],
                     Optional[List[List[RawColType]]],
                 ] = (-1, None, None, None)
                 if isinstance(query, SetParameter):
                     self._validate_set_parameter(query)
-                elif async_execution:
-                    self._validate_server_side_async_settings(
-                        parameters,
-                        queries,
-                        skip_parsing,
-                        async_execution,
-                    )
-                    response = self._api_request(
-                        query,
-                        {
-                            "async_execution": 1,
-                            "output_format": JSON_OUTPUT_FORMAT,
-                        },
-                    )
-                    self._raise_if_error(response)
-                    if response.headers.get("content-length", "") == "0":
-                        raise OperationalError("No response to asynchronous query.")
-                    resp = response.json()
-                    if "query_id" not in resp or resp["query_id"] == "":
-                        raise OperationalError(
-                            "Invalid response to asynchronous query: missing query_id."
-                        )
-                    self._query_id = resp["query_id"]
                 else:
                     resp = self._api_request(
                         query, {"output_format": JSON_OUTPUT_FORMAT}
                     )
                     self._raise_if_error(resp)
                     self._parse_response_headers(resp.headers)
                     row_set = self._row_set_from_response(resp)
@@ -242,15 +204,14 @@
 
     @check_not_closed
     def execute(
         self,
         query: str,
         parameters: Optional[Sequence[ParameterType]] = None,
         skip_parsing: bool = False,
-        async_execution: Optional[bool] = False,
     ) -> Union[int, str]:
         """Prepare and execute a database query.
 
         Supported features:
             Parameterized queries: placeholder characters ('?') are substituted
                 with values provided in `parameters`. Values are formatted to
                 be properly recognized by database and to exclude SQL injection.
@@ -266,29 +227,25 @@
             query (str): SQL query to execute
             parameters (Optional[Sequence[ParameterType]]): A sequence of substitution
                 parameters. Used to replace '?' placeholders inside a query with
                 actual values
             skip_parsing (bool): Flag to disable query parsing. This will
                 disable parameterized, multi-statement and SET queries,
                 while improving performance
-            async_execution (bool): flag to determine if query should be asynchronous
 
         Returns:
             int: Query row count.
         """
         params_list = [parameters] if parameters else []
-        self._do_execute(query, params_list, skip_parsing, async_execution)
-        return self.query_id if async_execution else self.rowcount
+        self._do_execute(query, params_list, skip_parsing)
+        return self.rowcount
 
     @check_not_closed
     def executemany(
-        self,
-        query: str,
-        parameters_seq: Sequence[Sequence[ParameterType]],
-        async_execution: Optional[bool] = False,
+        self, query: str, parameters_seq: Sequence[Sequence[ParameterType]]
     ) -> Union[int, str]:
         """Prepare and execute a database query.
 
         Supports providing multiple substitution parameter sets, executing them
         as multiple statements sequentially.
 
         Supported features:
@@ -305,74 +262,31 @@
 
         Args:
             query (str): SQL query to execute.
             parameters_seq (Sequence[Sequence[ParameterType]]): A sequence of
                substitution parameter sets. Used to replace '?' placeholders inside a
                query with actual values from each set in a sequence. Resulting queries
                for each subset are executed sequentially.
-            async_execution (bool): flag to determine if query should be asynchronous
 
         Returns:
-            int|str: Query row count for synchronous execution of queries,
-            query ID string for asynchronous execution.
+            int: Query row count.
         """
-        self._do_execute(query, parameters_seq, async_execution=async_execution)
-        if async_execution:
-            return self.query_id
-        else:
-            return self.rowcount
-
-    @check_not_closed
-    def get_status(self, query_id: str) -> QueryStatus:
-        """Get status of a server-side async query. Return the state of the query."""
-        try:
-            resp = self._api_request(
-                # output_format must be empty for status to work correctly.
-                # And set parameters will cause 400 errors.
-                parameters={"query_id": query_id},
-                path="status",
-                use_set_parameters=False,
-            )
-            if resp.status_code == codes.BAD_REQUEST:
-                raise OperationalError(
-                    f"Asynchronous query {query_id} status check failed: "
-                    f"{resp.status_code}."
-                )
-            resp_json = resp.json()
-            if "status" not in resp_json:
-                raise OperationalError(
-                    "Invalid response to asynchronous query: missing status."
-                )
-        except Exception:
-            self._state = CursorState.ERROR
-            raise
-        # Remember that query_id might be empty.
-        if resp_json["status"] == "":
-            return QueryStatus.NOT_READY
-        return QueryStatus[resp_json["status"]]
+        self._do_execute(query, parameters_seq)
+        return self.rowcount
 
     @abstractmethod
     def is_db_available(self, database: str) -> bool:
         """Verify that the database exists."""
         ...
 
     @abstractmethod
     def is_engine_running(self, engine_url: str) -> bool:
         """Verify that the engine is running."""
         ...
 
-    @check_not_closed
-    def cancel(self, query_id: str) -> None:
-        """Cancel a server-side async query."""
-        self._api_request(
-            parameters={"query_id": query_id},
-            path="cancel",
-            use_set_parameters=False,
-        )
-
     # Iteration support
     @check_not_closed
     @check_query_executed
     def __iter__(self) -> Generator[List[ColType], None, None]:
         while True:
             row = self.fetchone()
             if row is None:
@@ -414,16 +328,16 @@
                 self._set_parameters to be ignored.
         """
         parameters = parameters or {}
         if use_set_parameters:
             parameters = {**(self._set_parameters or {}), **parameters}
         if self.parameters:
             parameters = {**self.parameters, **parameters}
-        # Engines v2 always require account_id
-        if self.connection._is_system or self._client._account_version == 2:
+        # Engines v2 will have account context in the URL
+        if self.connection._is_system and self._client._account_version == 1:
             assert isinstance(self._client, ClientV2)  # Type check
             parameters["account_id"] = self._client.account_id
         return self._client.request(
             url=f"/{path}" if path else "",
             method="POST",
             params=parameters,
             content=query,
@@ -494,15 +408,15 @@
     ) -> None:
         assert isinstance(client, ClientV1)  # Type check
         super().__init__(*args, client=client, connection=connection, **kwargs)
 
     def _api_request(
         self,
         query: Optional[str] = "",
-        parameters: Optional[dict[str, Any]] = {},
+        parameters: Optional[dict[str, Any]] = None,
         path: Optional[str] = "",
         use_set_parameters: Optional[bool] = True,
     ) -> Response:
         """
         Query API, return Response object.
 
         Args:
```

### Comparing `firebolt_sdk-1.4.0/src/firebolt/model/V1/__init__.py` & `firebolt_sdk-1.4.1/src/firebolt/model/V1/__init__.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/model/V1/binding.py` & `firebolt_sdk-1.4.1/src/firebolt/model/V1/binding.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/model/V1/database.py` & `firebolt_sdk-1.4.1/src/firebolt/model/V1/database.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/model/V1/engine.py` & `firebolt_sdk-1.4.1/src/firebolt/model/V1/engine.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/model/V2/__init__.py` & `firebolt_sdk-1.4.1/src/firebolt/model/V2/__init__.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/model/V2/database.py` & `firebolt_sdk-1.4.1/src/firebolt/model/V2/database.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/model/V2/engine.py` & `firebolt_sdk-1.4.1/src/firebolt/model/V2/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,17 @@
         parameters = []
         for param, value in zip(
             self.ALTER_PARAMETER_NAMES,
             (scale, spec, auto_stop, name, warmup, engine_type),
         ):
             if value is not None:
                 sql += f"{param} = ? "
-                parameters.append(str(value))
+                if isinstance(value, (EngineType, InstanceType, WarmupMethod)):
+                    value = str(value)
+                parameters.append(value)
 
         with self._service._connection.cursor() as c:
             c.execute(sql, parameters)
         self.refresh()
         return self
 
     def delete(self) -> None:
```

### Comparing `firebolt_sdk-1.4.0/src/firebolt/model/V2/instance_type.py` & `firebolt_sdk-1.4.1/src/firebolt/model/V2/instance_type.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/service/V1/base.py` & `firebolt_sdk-1.4.1/src/firebolt/service/V1/base.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/service/V1/binding.py` & `firebolt_sdk-1.4.1/src/firebolt/service/V1/binding.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/service/V1/database.py` & `firebolt_sdk-1.4.1/src/firebolt/service/V1/database.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/service/V1/engine.py` & `firebolt_sdk-1.4.1/src/firebolt/service/V1/engine.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/service/V1/region.py` & `firebolt_sdk-1.4.1/src/firebolt/service/V1/region.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/service/V1/types.py` & `firebolt_sdk-1.4.1/src/firebolt/service/V1/types.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/service/V2/base.py` & `firebolt_sdk-1.4.1/src/firebolt/service/V2/base.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/service/V2/database.py` & `firebolt_sdk-1.4.1/src/firebolt/service/V2/database.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/service/V2/engine.py` & `firebolt_sdk-1.4.1/src/firebolt/service/V2/engine.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/service/V2/instance_type.py` & `firebolt_sdk-1.4.1/src/firebolt/service/V2/instance_type.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/service/V2/types.py` & `firebolt_sdk-1.4.1/src/firebolt/service/V2/types.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/service/manager.py` & `firebolt_sdk-1.4.1/src/firebolt/service/manager.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/utils/exception.py` & `firebolt_sdk-1.4.1/src/firebolt/utils/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,18 +263,7 @@
     by the database, e.g., requesting a .rollback() on a connection that
     does not support transaction or has transactions turned off.
     """
 
 
 class ConfigurationError(InterfaceError):
     """Invalid configuration error."""
-
-
-class AsyncExecutionUnavailableError(ProgrammingError):
-    """
-    If `use_standard_sql` is specified the query status endpoint returns a JSON
-    object with empty values instead of a proper status object. In that case,
-    it is not possible to retrieve the results of an asynchronous query.
-    """
-
-    def __init__(self, error_message):  # type: ignore
-        super().__init__(error_message)
```

### Comparing `firebolt_sdk-1.4.0/src/firebolt/utils/token_storage.py` & `firebolt_sdk-1.4.1/src/firebolt/utils/token_storage.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/utils/urls.py` & `firebolt_sdk-1.4.1/src/firebolt/utils/urls.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/utils/usage_tracker.py` & `firebolt_sdk-1.4.1/src/firebolt/utils/usage_tracker.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt/utils/util.py` & `firebolt_sdk-1.4.1/src/firebolt/utils/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 import logging
 from functools import lru_cache
 from os import environ
 from time import time
 from types import TracebackType
-from typing import TYPE_CHECKING, Callable, Optional, Type, TypeVar
+from typing import (
+    TYPE_CHECKING,
+    Callable,
+    Dict,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+)
+from urllib.parse import parse_qs, urljoin, urlparse
 
 from httpx import URL, Response, codes
 
 from firebolt.utils.exception import ConfigurationError
 
 T = TypeVar("T")
 logger = logging.getLogger(__name__)
@@ -177,7 +186,26 @@
         self.elapsed_time: str = "{:.2f}".format(round((time() - self._start_time), 2))
         if (
             environ.get("FIREBOLT_SDK_PERFORMANCE_DEBUG", "0") == "1"
             and self._message != ""
         ):
             log_message = self._message + self.elapsed_time + "s"
             logger.debug(log_message)
+
+
+def parse_url_and_params(url: str) -> Tuple[str, Dict[str, str]]:
+    """Extract URL and query parameters separately from a URL."""
+    url = fix_url_schema(url)
+    parsed_url = urlparse(url)
+    query_params = parse_qs(parsed_url.query)
+    # This strips query parameters from the URL by joining base URL and path
+    # skipping the query parameters.
+    result_url = urljoin(url, parsed_url.path)
+    # parse_qs returns a dictionary with values as lists.
+    # We want the last value in the list.
+    query_params_dict = {}
+    for key, values in query_params.items():
+        # Multiple values for the same key are not expected
+        if len(values) > 1:
+            raise ValueError(f"Multiple values found for key '{key}'")
+        query_params_dict[key] = values[0]
+    return result_url, query_params_dict
```

### Comparing `firebolt_sdk-1.4.0/src/firebolt_sdk.egg-info/PKG-INFO` & `firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebolt-sdk
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python SDK for Firebolt
 Home-page: https://github.com/firebolt-db/firebolt-sdk
 Author: Firebolt
 Author-email: support@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/firebolt-sdk/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `firebolt_sdk-1.4.0/src/firebolt_sdk.egg-info/SOURCES.txt` & `firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.0/src/firebolt_sdk.egg-info/requires.txt` & `firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

