# Comparing `tmp/hcs-core-0.1.225.tar.gz` & `tmp/hcs_core-0.1.226.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-core-0.1.225.tar", last modified: Tue Apr  9 22:15:22 2024, max compression
+gzip compressed data, was "hcs_core-0.1.226.tar", last modified: Wed Apr 17 16:56:49 2024, max compression
```

## Comparing `hcs-core-0.1.225.tar` & `hcs_core-0.1.226.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-09 22:15:22.613326 hcs-core-0.1.225/
--rw-r--r--   0 nanw       (501) staff       (20)     1371 2024-04-09 22:15:22.612477 hcs-core-0.1.225/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)       25 2024-04-09 21:58:38.000000 hcs-core-0.1.225/README.md
--rw-r--r--   0 nanw       (501) staff       (20)        7 2024-04-09 22:15:18.000000 hcs-core-0.1.225/VERSION
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-09 22:15:22.553187 hcs-core-0.1.225/hcs_core/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-09 22:15:22.576485 hcs-core-0.1.225/hcs_core/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)      790 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-09 22:15:22.579564 hcs-core-0.1.225/hcs_core/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3086 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/built_in_cmds/_ut.py
--rw-r--r--   0 nanw       (501) staff       (20)     2387 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     4034 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     2274 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/cli_options.py
--rw-r--r--   0 nanw       (501) staff       (20)     5791 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      936 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1160 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)    14088 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/data_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2856 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     1623 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/extension.py
--rw-r--r--   0 nanw       (501) staff       (20)     6432 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     3792 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     6346 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/logger.py
--rw-r--r--   0 nanw       (501) staff       (20)     6518 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1565 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/profile_store.py
--rw-r--r--   0 nanw       (501) staff       (20)     1767 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/recent.py
--rw-r--r--   0 nanw       (501) staff       (20)     1597 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     7933 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3245 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/ctxp/var_template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-09 22:15:22.585488 hcs-core-0.1.225/hcs_core/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      203 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      125 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/plan/actions.py
--rw-r--r--   0 nanw       (501) staff       (20)     1298 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/plan/base_provider.py
--rw-r--r--   0 nanw       (501) staff       (20)      116 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/plan/context.py
--rw-r--r--   0 nanw       (501) staff       (20)    20914 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/plan/core.py
--rw-r--r--   0 nanw       (501) staff       (20)    12918 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/plan/dag.py
--rw-r--r--   0 nanw       (501) staff       (20)     7784 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/plan/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     5363 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/plan/kop.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-09 22:15:22.586807 hcs-core-0.1.225/hcs_core/plan/provider/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-09 22:15:22.589729 hcs-core-0.1.225/hcs_core/plan/provider/dev/
--rw-r--r--   0 nanw       (501) staff       (20)       30 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       34 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1994 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/plan/provider/dev/dummy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1104 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/plan/provider/dev/fibonacci.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-09 22:15:22.596484 hcs-core-0.1.225/hcs_core/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     5194 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1790 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/sglib/cli_options.py
--rw-r--r--   0 nanw       (501) staff       (20)     8357 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/sglib/client_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     8043 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     5167 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      901 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)    10056 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/sglib/login_support.py
--rw-r--r--   0 nanw       (501) staff       (20)      684 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/sglib/payload_util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-09 22:15:22.609935 hcs-core-0.1.225/hcs_core/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     3482 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)      838 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/util/exit.py
--rw-r--r--   0 nanw       (501) staff       (20)     1755 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/util/hcs_constants.py
--rw-r--r--   0 nanw       (501) staff       (20)     8438 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/util/job_view.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1946 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2958 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/util/scheduler.py
--rw-r--r--   0 nanw       (501) staff       (20)     1239 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/util/ssl_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1727 2024-04-09 21:58:38.000000 hcs-core-0.1.225/hcs_core/util/versions.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-09 22:15:22.611335 hcs-core-0.1.225/hcs_core.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     1371 2024-04-09 22:15:22.000000 hcs-core-0.1.225/hcs_core.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1810 2024-04-09 22:15:22.000000 hcs-core-0.1.225/hcs_core.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2024-04-09 22:15:22.000000 hcs-core-0.1.225/hcs_core.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)      265 2024-04-09 22:15:22.000000 hcs-core-0.1.225/hcs_core.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)        9 2024-04-09 22:15:22.000000 hcs-core-0.1.225/hcs_core.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)     1250 2024-04-09 21:58:38.000000 hcs-core-0.1.225/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      265 2024-04-09 21:58:38.000000 hcs-core-0.1.225/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2024-04-09 22:15:22.613467 hcs-core-0.1.225/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)      808 2024-04-09 21:58:38.000000 hcs-core-0.1.225/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.954002 hcs_core-0.1.226/
+-rw-r--r--   0 nanw       (501) staff       (20)     1371 2024-04-17 16:56:49.952642 hcs_core-0.1.226/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)       25 2024-04-09 21:58:38.000000 hcs_core-0.1.226/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)        7 2024-04-17 16:56:42.000000 hcs_core-0.1.226/VERSION
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.410520 hcs_core-0.1.226/hcs_core/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.597107 hcs_core-0.1.226/hcs_core/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.609506 hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3086 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/_ut.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2387 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4034 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2274 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/cli_options.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5791 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      936 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1160 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    14088 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/data_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2856 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1623 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/extension.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6432 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3792 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6346 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/logger.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6518 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1767 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/recent.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1597 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7933 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3245 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/ctxp/var_template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.660148 hcs_core-0.1.226/hcs_core/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      203 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      125 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/actions.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1298 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/base_provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)      116 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    20914 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)    12918 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7784 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5363 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/kop.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.661334 hcs_core-0.1.226/hcs_core/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.698263 hcs_core-0.1.226/hcs_core/plan/provider/dev/
+-rw-r--r--   0 nanw       (501) staff       (20)       30 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       34 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1994 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/provider/dev/dummy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1104 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/plan/provider/dev/fibonacci.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.756372 hcs_core-0.1.226/hcs_core/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5194 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1790 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/cli_options.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8378 2024-04-11 21:31:53.000000 hcs_core-0.1.226/hcs_core/sglib/client_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8043 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5167 2024-04-16 17:06:43.000000 hcs_core-0.1.226/hcs_core/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      901 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)    10056 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/login_support.py
+-rw-r--r--   0 nanw       (501) staff       (20)      684 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/sglib/payload_util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.949971 hcs_core-0.1.226/hcs_core/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3482 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)      838 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/exit.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1755 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/hcs_constants.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8438 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/job_view.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1946 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2958 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/scheduler.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1239 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/ssl_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1727 2024-04-09 21:58:38.000000 hcs_core-0.1.226/hcs_core/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-17 16:56:49.951318 hcs_core-0.1.226/hcs_core.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     1371 2024-04-17 16:56:49.000000 hcs_core-0.1.226/hcs_core.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1810 2024-04-17 16:56:49.000000 hcs_core-0.1.226/hcs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2024-04-17 16:56:49.000000 hcs_core-0.1.226/hcs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      265 2024-04-17 16:56:49.000000 hcs_core-0.1.226/hcs_core.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        9 2024-04-17 16:56:49.000000 hcs_core-0.1.226/hcs_core.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)     1250 2024-04-09 21:58:38.000000 hcs_core-0.1.226/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      265 2024-04-09 21:58:38.000000 hcs_core-0.1.226/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2024-04-17 16:56:49.954342 hcs_core-0.1.226/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)      808 2024-04-09 21:58:38.000000 hcs_core-0.1.226/setup.py
```

### Comparing `hcs-core-0.1.225/PKG-INFO` & `hcs_core-0.1.226/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.225
+Version: 0.1.226
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/__init__.py` & `hcs_core-0.1.226/hcs_core/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/_init.py` & `hcs_core-0.1.226/hcs_core/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/built_in_cmds/_ut.py` & `hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/_ut.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/built_in_cmds/context.py` & `hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/built_in_cmds/profile.py` & `hcs_core-0.1.226/hcs_core/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/cli_options.py` & `hcs_core-0.1.226/hcs_core/ctxp/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/cli_processor.py` & `hcs_core-0.1.226/hcs_core/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/config.py` & `hcs_core-0.1.226/hcs_core/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/context.py` & `hcs_core-0.1.226/hcs_core/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/data_util.py` & `hcs_core-0.1.226/hcs_core/ctxp/data_util.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/duration.py` & `hcs_core-0.1.226/hcs_core/ctxp/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/extension.py` & `hcs_core-0.1.226/hcs_core/ctxp/extension.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/fstore.py` & `hcs_core-0.1.226/hcs_core/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/init.py` & `hcs_core-0.1.226/hcs_core/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/jsondot.py` & `hcs_core-0.1.226/hcs_core/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/logger.py` & `hcs_core-0.1.226/hcs_core/ctxp/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/profile.py` & `hcs_core-0.1.226/hcs_core/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/profile_store.py` & `hcs_core-0.1.226/hcs_core/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/recent.py` & `hcs_core-0.1.226/hcs_core/ctxp/recent.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/state.py` & `hcs_core-0.1.226/hcs_core/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/util.py` & `hcs_core-0.1.226/hcs_core/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/ctxp/var_template.py` & `hcs_core-0.1.226/hcs_core/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/plan/base_provider.py` & `hcs_core-0.1.226/hcs_core/plan/base_provider.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/plan/core.py` & `hcs_core-0.1.226/hcs_core/plan/core.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/plan/dag.py` & `hcs_core-0.1.226/hcs_core/plan/dag.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/plan/helper.py` & `hcs_core-0.1.226/hcs_core/plan/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/plan/kop.py` & `hcs_core-0.1.226/hcs_core/plan/kop.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/plan/provider/dev/dummy.py` & `hcs_core-0.1.226/hcs_core/plan/provider/dev/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/plan/provider/dev/fibonacci.py` & `hcs_core-0.1.226/hcs_core/plan/provider/dev/fibonacci.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/sglib/__init__.py` & `hcs_core-0.1.226/hcs_core/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/sglib/auth.py` & `hcs_core-0.1.226/hcs_core/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/sglib/cli_options.py` & `hcs_core-0.1.226/hcs_core/sglib/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/sglib/client_util.py` & `hcs_core-0.1.226/hcs_core/sglib/client_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         self._base_context = base_context
         self._resource_type_name = resource_type_name
 
     def get(self, id: str, org_id: str, **kwargs):
         if org_id:
             kwargs["org_id"] = org_id
         url = with_query(f"{self._base_context}/{id}", **kwargs)
+        # print(url)
         return self._client.get(url)
 
     def list(self, org_id: str, **kwargs):
         if org_id:
             kwargs["org_id"] = org_id
 
         def _get_page(query_string):
```

### Comparing `hcs-core-0.1.225/hcs_core/sglib/csp.py` & `hcs_core-0.1.226/hcs_core/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/sglib/ez_client.py` & `hcs_core-0.1.226/hcs_core/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/sglib/hcs_client.py` & `hcs_core-0.1.226/hcs_core/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/sglib/login_support.py` & `hcs_core-0.1.226/hcs_core/sglib/login_support.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/sglib/payload_util.py` & `hcs_core-0.1.226/hcs_core/sglib/payload_util.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/util/check_license.py` & `hcs_core-0.1.226/hcs_core/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/util/duration.py` & `hcs_core-0.1.226/hcs_core/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/util/exit.py` & `hcs_core-0.1.226/hcs_core/util/exit.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/util/hcs_constants.py` & `hcs_core-0.1.226/hcs_core/util/hcs_constants.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/util/job_view.py` & `hcs_core-0.1.226/hcs_core/util/job_view.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/util/pki_util.py` & `hcs_core-0.1.226/hcs_core/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/util/query_util.py` & `hcs_core-0.1.226/hcs_core/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/util/scheduler.py` & `hcs_core-0.1.226/hcs_core/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/util/ssl_util.py` & `hcs_core-0.1.226/hcs_core/util/ssl_util.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core/util/versions.py` & `hcs_core-0.1.226/hcs_core/util/versions.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/hcs_core.egg-info/PKG-INFO` & `hcs_core-0.1.226/hcs_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.225
+Version: 0.1.226
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-core-0.1.225/hcs_core.egg-info/SOURCES.txt` & `hcs_core-0.1.226/hcs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/pyproject.toml` & `hcs_core-0.1.226/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.225/setup.py` & `hcs_core-0.1.226/setup.py`

 * *Files identical despite different names*

