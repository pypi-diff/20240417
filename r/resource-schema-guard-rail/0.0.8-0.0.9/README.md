# Comparing `tmp/resource-schema-guard-rail-0.0.8.tar.gz` & `tmp/resource-schema-guard-rail-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resource-schema-guard-rail-0.0.8.tar", last modified: Tue Sep 12 20:46:15 2023, max compression
+gzip compressed data, was "resource-schema-guard-rail-0.0.9.tar", last modified: Tue Jan 23 22:02:20 2024, max compression
```

## Comparing `resource-schema-guard-rail-0.0.8.tar` & `resource-schema-guard-rail-0.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.417015 resource-schema-guard-rail-0.0.8/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)    10142 2022-09-16 09:27:12.000000 resource-schema-guard-rail-0.0.8/LICENSE
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)       63 2023-06-07 17:01:38.000000 resource-schema-guard-rail-0.0.8/MANIFEST.in
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     4383 2023-09-12 20:46:15.417255 resource-schema-guard-rail-0.0.8/PKG-INFO
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     3748 2023-06-07 17:01:38.000000 resource-schema-guard-rail-0.0.8/README.md
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)      593 2023-09-12 20:46:15.418514 resource-schema-guard-rail-0.0.8/setup.cfg
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     2010 2023-09-12 20:45:01.000000 resource-schema-guard-rail-0.0.8/setup.py
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.356936 resource-schema-guard-rail-0.0.8/src/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     2538 2023-09-12 01:19:18.000000 resource-schema-guard-rail-0.0.8/src/cli.py
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.359237 resource-schema-guard-rail-0.0.8/src/resource_schema_guard_rail.egg-info/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     4383 2023-09-12 20:46:15.000000 resource-schema-guard-rail-0.0.8/src/resource_schema_guard_rail.egg-info/PKG-INFO
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     1661 2023-09-12 20:46:15.000000 resource-schema-guard-rail-0.0.8/src/resource_schema_guard_rail.egg-info/SOURCES.txt
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)        1 2023-09-12 20:46:15.000000 resource-schema-guard-rail-0.0.8/src/resource_schema_guard_rail.egg-info/dependency_links.txt
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)       66 2023-09-12 20:46:15.000000 resource-schema-guard-rail-0.0.8/src/resource_schema_guard_rail.egg-info/entry_points.txt
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)      258 2023-09-12 20:46:15.000000 resource-schema-guard-rail-0.0.8/src/resource_schema_guard_rail.egg-info/requires.txt
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)        9 2023-09-12 20:46:15.000000 resource-schema-guard-rail-0.0.8/src/resource_schema_guard_rail.egg-info/top_level.txt
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.359548 resource-schema-guard-rail-0.0.8/src/rpdk/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2022-09-16 10:31:53.000000 resource-schema-guard-rail-0.0.8/src/rpdk/__init__.py
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.359804 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2022-09-16 10:01:38.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/__init__.py
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.361606 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/core/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2022-09-16 10:02:13.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/core/__init__.py
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     4237 2023-09-12 01:19:18.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/core/data_types.py
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     6338 2023-09-12 01:19:21.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/core/runner.py
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)    11111 2023-09-11 16:37:49.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/core/stateful.py
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.362223 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/core/templates/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)      765 2023-09-12 17:46:10.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/core/templates/guard-result-pojo.output
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.363095 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2022-09-16 10:02:03.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/__init__.py
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.364083 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/combiners/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2022-09-16 09:54:19.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/combiners/__init__.py
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     1608 2023-09-12 00:16:58.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/combiners/schema-linter-combiner-rules.guard
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.366377 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/core/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2022-09-16 09:54:30.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/core/__init__.py
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)      555 2023-06-07 17:01:38.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/core/schema-linter-core-arn-rules.guard
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     4050 2023-09-12 20:27:36.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/core/schema-linter-core-rules.guard
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.367591 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/permissions/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2022-09-21 06:00:22.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/permissions/__init__.py
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     2699 2023-06-07 17:01:38.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/permissions/schema-linter-core-permission-rules.guard
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.368768 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/stateful/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-06-07 17:01:38.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/stateful/__init__.py
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)    12380 2023-06-07 17:01:38.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/stateful/schema-stateful-cfn-enforced-checks.guard
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.409567 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/tags/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2022-09-21 06:43:21.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/tags/__init__.py
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     2711 2023-06-07 17:01:38.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/tags/schema-linter-core-tagging-rules.guard
-drwxr-xr-x   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2023-09-12 20:46:15.415922 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/utils/
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)        0 2022-09-16 10:01:53.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/utils/__init__.py
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     4384 2023-09-12 03:54:02.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/utils/arg_handler.py
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     1121 2023-09-12 03:53:19.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/utils/common.py
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)      928 2023-06-07 17:01:38.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/utils/logger.py
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)      893 2023-04-06 03:57:42.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/utils/miscellaneous.py
--rw-r--r--   0 ammokhov (153045500) ANT\Domain Users (1896053708)     2510 2023-06-07 17:01:38.000000 resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/utils/schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.021379 resource-schema-guard-rail-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-01-23 22:02:20.021379 resource-schema-guard-rail-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-23 22:02:20.021379 resource-schema-guard-rail-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.017379 resource-schema-guard-rail-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.017379 resource-schema-guard-rail-0.0.9/src/resource_schema_guard_rail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-01-23 22:02:19.000000 resource-schema-guard-rail-0.0.9/src/resource_schema_guard_rail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-01-23 22:02:19.000000 resource-schema-guard-rail-0.0.9/src/resource_schema_guard_rail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 22:02:19.000000 resource-schema-guard-rail-0.0.9/src/resource_schema_guard_rail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-23 22:02:19.000000 resource-schema-guard-rail-0.0.9/src/resource_schema_guard_rail.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-23 22:02:19.000000 resource-schema-guard-rail-0.0.9/src/resource_schema_guard_rail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-23 22:02:19.000000 resource-schema-guard-rail-0.0.9/src/resource_schema_guard_rail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.017379 resource-schema-guard-rail-0.0.9/src/rpdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.017379 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.017379 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/core/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/core/stateful.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.017379 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/core/templates/guard-result-pojo.output
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.017379 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.017379 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/combiners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/combiners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/combiners/schema-linter-combiner-rules.guard
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.017379 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/core/schema-linter-core-arn-rules.guard
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/core/schema-linter-core-rules.guard
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.021379 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/permissions/schema-linter-core-permission-rules.guard
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.021379 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/stateful/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/stateful/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/stateful/schema-stateful-cfn-enforced-checks.guard
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.021379 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/tags/schema-linter-core-tagging-rules.guard
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:20.021379 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/utils/arg_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/utils/miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-01-23 22:02:13.000000 resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/utils/schema_utils.py
```

### Comparing `resource-schema-guard-rail-0.0.8/LICENSE` & `resource-schema-guard-rail-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/PKG-INFO` & `resource-schema-guard-rail-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,100 +1,101 @@
 Metadata-Version: 2.1
 Name: resource-schema-guard-rail
-Version: 0.0.8
+Version: 0.0.9
 Summary: Schema Guard Rail
+Home-page: UNKNOWN
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
+Description: # CloudFormation - Resource Schema Guard Rail
+        ![Apache 2.0 License](https://img.shields.io/github/license/aws-cloudformation/resource-schema-guard-rail)
+        [![Pull Request CI](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml/badge.svg?branch=main)](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml)
+        [![PyPI](https://img.shields.io/pypi/v/resource-schema-guard-rail?label=pypi)](https://badge.fury.io/py/resource-schema-guard-rail)
+        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resource-schema-guard-rail?label=python)](https://pypi.org/project/resource-schema-guard-rail/)
+        
+        ### Notes
+        This is not a stable version (Beta), it's still under development
+        
+        ## Overview
+        AWS CloudFormation Resource Schema Guard Rail is an open-source tool, which uses [CloudFormation Guard](https://github.com/aws-cloudformation/cloudformation-guard/) policy-as-code evaluation engine to assess resource schema compliance. It validates json resource schemas against the AWS CloudFormation modeling best practices.
+        
+        ### Contribute
+        See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
+        #### Rule Development
+        Read [Guard Rail: Rule Development](docs/RULE_DEVELOPMENT.md) for more information on how to write resource schema rules.
+        
+        ### How to use it?
+        Schema guard rail package has a built-in library of rules, that CloudFormation believe are the best practices that resource modelers should follow. It supports two types of evaluation - Basic Linting & Breaking Change;
+        
+        #### Basic Linter (Stateless)
+        Linter works only with current version of resource schema and runs CloudFormation authored rules, which will highlight problematic schema constructs. A provider developers can run multiple independent schemas at once as well as attach custom rules.
+        
+        In order to start using Basic Linting you need to run following command:
+        ```bash
+        $ guard-rail --schema file://path-to-schema-1 --schema file://path-to-schema-2 --rule file://path-to-custom-ruleset1 --rule file://path-to-custom-ruleset2
+        ```
+        
+        **[List of Linting Rules](docs/BASIC_LINTING.md)**
+        
+        #### Breaking Change (Stateful)
+        Along with basic linting, guard rail supports capability of breaking change evaluation. Provider developer must provider two json objects - previous & current versions of the same resource schema. CloudFormation authored rules will be run and evaluation current version of the schema whether it is compliant or not.
+        
+        In order to start using Basic Linting you need to run following command:
+        ```bash
+        $ guard-rail --schema file://path-to-schema-1 --schema file://path-to-schema-2 --rule ... --stateful
+        ```
+        
+        **[List of Breaking Change Rules](docs/BREAKING_CHANGE.md)**
+        
+        
+        *Additionally, you can specify `format` argument, which will produce a nicely formatted output.
+        
+        ### How to install it locally?
+        
+        Use following commands
+        
+        #### Clone github repo
+        ```bash
+        $ git clone git@github.com:aws-cloudformation/resource-schema-guard-rail.git
+        ```
+        #### Create Virtual Environment & Activate
+        ```
+        python3 -m venv env
+        source env/bin/activate
+        ```
+        
+        #### Install Package Locally from the root
+        
+        ```
+        pip install -e . -r requirements.txt
+        pre-commit install
+        ```
+        
+        #### Run CI Locally
+        
+        ```
+        # run all hooks on all files, mirrors what the CI runs
+        pre-commit run --all-files
+        ```
+        
+        ## License
+        
+        This project is licensed under the Apache-2.0 License.
+        
+        ## Community
+        
+        Join us on Discord! Connect & interact with CloudFormation developers &
+        experts, find channels to discuss and get help for our CLI, cfn-lint, CloudFormation registry, StackSets,
+        Guard and more:
+        
+        [![Join our Discord](https://discordapp.com/api/guilds/981586120448020580/widget.png?style=banner3)](https://discord.gg/9zpd7TTRwq)
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# CloudFormation - Resource Schema Guard Rail
-![Apache 2.0 License](https://img.shields.io/github/license/aws-cloudformation/resource-schema-guard-rail)
-[![Pull Request CI](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml/badge.svg?branch=main)](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml)
-[![PyPI](https://img.shields.io/pypi/v/resource-schema-guard-rail?label=pypi)](https://badge.fury.io/py/resource-schema-guard-rail)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resource-schema-guard-rail?label=python)](https://pypi.org/project/resource-schema-guard-rail/)
-
-### Notes
-This is not a stable version (Beta), it's still under development
-
-## Overview
-AWS CloudFormation Resource Schema Guard Rail is an open-source tool, which uses [CloudFormation Guard](https://github.com/aws-cloudformation/cloudformation-guard/) policy-as-code evaluation engine to assess resource schema compliance. It validates json resource schemas against the AWS CloudFormation modeling best practices.
-
-### Contribute
-See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
-#### Rule Development
-Read [Guard Rail: Rule Development](docs/RULE_DEVELOPMENT.md) for more information on how to write resource schema rules.
-
-### How to use it?
-Schema guard rail package has a built-in library of rules, that CloudFormation believe are the best practices that resource modelers should follow. It supports two types of evaluation - Basic Linting & Breaking Change;
-
-#### Basic Linter (Stateless)
-Linter works only with current version of resource schema and runs CloudFormation authored rules, which will highlight problematic schema constructs. A provider developers can run multiple independent schemas at once as well as attach custom rules.
-
-In order to start using Basic Linting you need to run following command:
-```bash
-$ guard-rail --schema file://path-to-schema-1 --schema file://path-to-schema-2 --rule file://path-to-custom-ruleset1 --rule file://path-to-custom-ruleset2
-```
-
-**[List of Linting Rules](docs/BASIC_LINTING.md)**
-
-#### Breaking Change (Stateful)
-Along with basic linting, guard rail supports capability of breaking change evaluation. Provider developer must provider two json objects - previous & current versions of the same resource schema. CloudFormation authored rules will be run and evaluation current version of the schema whether it is compliant or not.
-
-In order to start using Basic Linting you need to run following command:
-```bash
-$ guard-rail --schema file://path-to-schema-1 --schema file://path-to-schema-2 --rule ... --stateful
-```
-
-**[List of Breaking Change Rules](docs/BREAKING_CHANGE.md)**
-
-
-*Additionally, you can specify `format` argument, which will produce a nicely formatted output.
-
-### How to install it locally?
-
-Use following commands
-
-#### Clone github repo
-```bash
-$ git clone git@github.com:aws-cloudformation/resource-schema-guard-rail.git
-```
-#### Create Virtual Environment & Activate
-```
-python3 -m venv env
-source env/bin/activate
-```
-
-#### Install Package Locally from the root
-
-```
-pip install -e . -r requirements_dev.txt
-pre-commit install
-```
-
-#### Run CI Locally
-
-```
-# run all hooks on all files, mirrors what the CI runs
-pre-commit run --all-files
-```
-
-## License
-
-This project is licensed under the Apache-2.0 License.
-
-## Community
-
-Join us on Discord! Connect & interact with CloudFormation developers &
-experts, find channels to discuss and get help for our CLI, cfn-lint, CloudFormation registry, StackSets,
-Guard and more:
-
-[![Join our Discord](https://discordapp.com/api/guilds/981586120448020580/widget.png?style=banner3)](https://discord.gg/9zpd7TTRwq)
```

### Comparing `resource-schema-guard-rail-0.0.8/README.md` & `resource-schema-guard-rail-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 python3 -m venv env
 source env/bin/activate
 ```
 
 #### Install Package Locally from the root
 
 ```
-pip install -e . -r requirements_dev.txt
+pip install -e . -r requirements.txt
 pre-commit install
 ```
 
 #### Run CI Locally
 
 ```
 # run all hooks on all files, mirrors what the CI runs
```

### Comparing `resource-schema-guard-rail-0.0.8/setup.cfg` & `resource-schema-guard-rail-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/setup.py` & `resource-schema-guard-rail-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,24 +32,24 @@
         else:
             requirements.append(line)
     return requirements
 
 
 setuptools.setup(
     name="resource-schema-guard-rail",
-    version="0.0.8",
+    version="0.0.9",
     description="Schema Guard Rail",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Amazon Web Services",
     author_email="aws-cloudformation-developers@amazon.com",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
     py_modules=["cli"],
-    install_requires=read_requirements("requirements_dev.txt"),
+    install_requires=read_requirements("requirements.txt"),
     include_package_data=True,
     python_requires=">=3.7",
     entry_points={
         "console_scripts": [
             "guard-rail-cli = cli:main",
             "guard-rail = cli:main",
         ]
```

### Comparing `resource-schema-guard-rail-0.0.8/src/cli.py` & `resource-schema-guard-rail-0.0.9/src/cli.py`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/src/resource_schema_guard_rail.egg-info/PKG-INFO` & `resource-schema-guard-rail-0.0.9/src/resource_schema_guard_rail.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,100 +1,101 @@
 Metadata-Version: 2.1
 Name: resource-schema-guard-rail
-Version: 0.0.8
+Version: 0.0.9
 Summary: Schema Guard Rail
+Home-page: UNKNOWN
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
+Description: # CloudFormation - Resource Schema Guard Rail
+        ![Apache 2.0 License](https://img.shields.io/github/license/aws-cloudformation/resource-schema-guard-rail)
+        [![Pull Request CI](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml/badge.svg?branch=main)](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml)
+        [![PyPI](https://img.shields.io/pypi/v/resource-schema-guard-rail?label=pypi)](https://badge.fury.io/py/resource-schema-guard-rail)
+        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resource-schema-guard-rail?label=python)](https://pypi.org/project/resource-schema-guard-rail/)
+        
+        ### Notes
+        This is not a stable version (Beta), it's still under development
+        
+        ## Overview
+        AWS CloudFormation Resource Schema Guard Rail is an open-source tool, which uses [CloudFormation Guard](https://github.com/aws-cloudformation/cloudformation-guard/) policy-as-code evaluation engine to assess resource schema compliance. It validates json resource schemas against the AWS CloudFormation modeling best practices.
+        
+        ### Contribute
+        See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
+        #### Rule Development
+        Read [Guard Rail: Rule Development](docs/RULE_DEVELOPMENT.md) for more information on how to write resource schema rules.
+        
+        ### How to use it?
+        Schema guard rail package has a built-in library of rules, that CloudFormation believe are the best practices that resource modelers should follow. It supports two types of evaluation - Basic Linting & Breaking Change;
+        
+        #### Basic Linter (Stateless)
+        Linter works only with current version of resource schema and runs CloudFormation authored rules, which will highlight problematic schema constructs. A provider developers can run multiple independent schemas at once as well as attach custom rules.
+        
+        In order to start using Basic Linting you need to run following command:
+        ```bash
+        $ guard-rail --schema file://path-to-schema-1 --schema file://path-to-schema-2 --rule file://path-to-custom-ruleset1 --rule file://path-to-custom-ruleset2
+        ```
+        
+        **[List of Linting Rules](docs/BASIC_LINTING.md)**
+        
+        #### Breaking Change (Stateful)
+        Along with basic linting, guard rail supports capability of breaking change evaluation. Provider developer must provider two json objects - previous & current versions of the same resource schema. CloudFormation authored rules will be run and evaluation current version of the schema whether it is compliant or not.
+        
+        In order to start using Basic Linting you need to run following command:
+        ```bash
+        $ guard-rail --schema file://path-to-schema-1 --schema file://path-to-schema-2 --rule ... --stateful
+        ```
+        
+        **[List of Breaking Change Rules](docs/BREAKING_CHANGE.md)**
+        
+        
+        *Additionally, you can specify `format` argument, which will produce a nicely formatted output.
+        
+        ### How to install it locally?
+        
+        Use following commands
+        
+        #### Clone github repo
+        ```bash
+        $ git clone git@github.com:aws-cloudformation/resource-schema-guard-rail.git
+        ```
+        #### Create Virtual Environment & Activate
+        ```
+        python3 -m venv env
+        source env/bin/activate
+        ```
+        
+        #### Install Package Locally from the root
+        
+        ```
+        pip install -e . -r requirements.txt
+        pre-commit install
+        ```
+        
+        #### Run CI Locally
+        
+        ```
+        # run all hooks on all files, mirrors what the CI runs
+        pre-commit run --all-files
+        ```
+        
+        ## License
+        
+        This project is licensed under the Apache-2.0 License.
+        
+        ## Community
+        
+        Join us on Discord! Connect & interact with CloudFormation developers &
+        experts, find channels to discuss and get help for our CLI, cfn-lint, CloudFormation registry, StackSets,
+        Guard and more:
+        
+        [![Join our Discord](https://discordapp.com/api/guilds/981586120448020580/widget.png?style=banner3)](https://discord.gg/9zpd7TTRwq)
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# CloudFormation - Resource Schema Guard Rail
-![Apache 2.0 License](https://img.shields.io/github/license/aws-cloudformation/resource-schema-guard-rail)
-[![Pull Request CI](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml/badge.svg?branch=main)](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml)
-[![PyPI](https://img.shields.io/pypi/v/resource-schema-guard-rail?label=pypi)](https://badge.fury.io/py/resource-schema-guard-rail)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resource-schema-guard-rail?label=python)](https://pypi.org/project/resource-schema-guard-rail/)
-
-### Notes
-This is not a stable version (Beta), it's still under development
-
-## Overview
-AWS CloudFormation Resource Schema Guard Rail is an open-source tool, which uses [CloudFormation Guard](https://github.com/aws-cloudformation/cloudformation-guard/) policy-as-code evaluation engine to assess resource schema compliance. It validates json resource schemas against the AWS CloudFormation modeling best practices.
-
-### Contribute
-See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
-#### Rule Development
-Read [Guard Rail: Rule Development](docs/RULE_DEVELOPMENT.md) for more information on how to write resource schema rules.
-
-### How to use it?
-Schema guard rail package has a built-in library of rules, that CloudFormation believe are the best practices that resource modelers should follow. It supports two types of evaluation - Basic Linting & Breaking Change;
-
-#### Basic Linter (Stateless)
-Linter works only with current version of resource schema and runs CloudFormation authored rules, which will highlight problematic schema constructs. A provider developers can run multiple independent schemas at once as well as attach custom rules.
-
-In order to start using Basic Linting you need to run following command:
-```bash
-$ guard-rail --schema file://path-to-schema-1 --schema file://path-to-schema-2 --rule file://path-to-custom-ruleset1 --rule file://path-to-custom-ruleset2
-```
-
-**[List of Linting Rules](docs/BASIC_LINTING.md)**
-
-#### Breaking Change (Stateful)
-Along with basic linting, guard rail supports capability of breaking change evaluation. Provider developer must provider two json objects - previous & current versions of the same resource schema. CloudFormation authored rules will be run and evaluation current version of the schema whether it is compliant or not.
-
-In order to start using Basic Linting you need to run following command:
-```bash
-$ guard-rail --schema file://path-to-schema-1 --schema file://path-to-schema-2 --rule ... --stateful
-```
-
-**[List of Breaking Change Rules](docs/BREAKING_CHANGE.md)**
-
-
-*Additionally, you can specify `format` argument, which will produce a nicely formatted output.
-
-### How to install it locally?
-
-Use following commands
-
-#### Clone github repo
-```bash
-$ git clone git@github.com:aws-cloudformation/resource-schema-guard-rail.git
-```
-#### Create Virtual Environment & Activate
-```
-python3 -m venv env
-source env/bin/activate
-```
-
-#### Install Package Locally from the root
-
-```
-pip install -e . -r requirements_dev.txt
-pre-commit install
-```
-
-#### Run CI Locally
-
-```
-# run all hooks on all files, mirrors what the CI runs
-pre-commit run --all-files
-```
-
-## License
-
-This project is licensed under the Apache-2.0 License.
-
-## Community
-
-Join us on Discord! Connect & interact with CloudFormation developers &
-experts, find channels to discuss and get help for our CLI, cfn-lint, CloudFormation registry, StackSets,
-Guard and more:
-
-[![Join our Discord](https://discordapp.com/api/guilds/981586120448020580/widget.png?style=banner3)](https://discord.gg/9zpd7TTRwq)
```

### Comparing `resource-schema-guard-rail-0.0.8/src/resource_schema_guard_rail.egg-info/SOURCES.txt` & `resource-schema-guard-rail-0.0.9/src/resource_schema_guard_rail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/core/data_types.py` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/core/data_types.py`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/core/runner.py` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/core/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     Stateful,
     Stateless,
 )
 from rpdk.guard_rail.core.stateful import schema_diff
 from rpdk.guard_rail.rule_library import combiners, core, permissions, stateful, tags
 from rpdk.guard_rail.utils.common import is_guard_rule
 from rpdk.guard_rail.utils.logger import LOG, logdebug
+from rpdk.guard_rail.utils.schema_utils import add_paths_to_schema
 
 NON_COMPLIANT = "NON_COMPLIANT"
 WARNING = "WARNING"
 
 
 @logdebug
 def prepare_ruleset(mode: str = "stateless"):
@@ -146,15 +147,16 @@
     def __execute_rules__(schema_exec, ruleset):
         output = None
         for rules in ruleset:
             output = schema_exec(rules)
         return output
 
     for schema in payload.schemas:
-        schema_to_execute = __exec_rules__(schema=schema)
+        schema_with_paths = add_paths_to_schema(schema=schema)
+        schema_to_execute = __exec_rules__(schema=schema_with_paths)
         output = __execute_rules__(schema_exec=schema_to_execute, ruleset=ruleset)
         compliance_output.append(output)
     return compliance_output
 
 
 @exec_compliance.register(Stateful)
 def _(payload):
```

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/core/stateful.py` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/core/stateful.py`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/core/templates/guard-result-pojo.output` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/core/templates/guard-result-pojo.output`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/combiners/schema-linter-combiner-rules.guard` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/combiners/schema-linter-combiner-rules.guard`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/core/schema-linter-core-arn-rules.guard` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/core/schema-linter-core-arn-rules.guard`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/core/schema-linter-core-rules.guard` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/core/schema-linter-core-rules.guard`

 * *Files 14% similar despite different names*

```diff
@@ -113,14 +113,70 @@
                 }
                 >>
             }
         }
     }
 }
 
+rule verify_property_notation
+{
+    let paths = paths
+    when primaryIdentifier exists {
+        primaryIdentifier[*] {
+            this IN %paths
+            <<
+            {
+                "result": "NON_COMPLIANT",
+                "check_id": "PR005",
+                "message": "primaryIdentifier MUST have properties defined in the schema"
+            }
+            >>
+        }
+    }
+
+    when createOnlyProperties exists {
+        createOnlyProperties[*] {
+            this IN %paths
+            <<
+            {
+                "result": "NON_COMPLIANT",
+                "check_id": "PR006",
+                "message": "createOnlyProperties MUST have properties defined in the schema"
+            }
+            >>
+        }
+    }
+
+    when readOnlyProperties exists {
+        readOnlyProperties[*] {
+            this IN %paths
+            <<
+            {
+                "result": "NON_COMPLIANT",
+                "check_id": "PR007",
+                "message": "readOnlyProperties MUST have properties defined in the schema"
+            }
+            >>
+        }
+    }
+
+    when writeOnlyProperties exists {
+        writeOnlyProperties[*] {
+            this IN %paths
+            <<
+            {
+                "result": "NON_COMPLIANT",
+                "check_id": "PR008",
+                "message": "writeOnlyProperties MUST have properties defined in the schema"
+            }
+            >>
+        }
+    }
+}
+
 
 
 rule ensure_description_is_descriptive {
     description != /^Resource Type definition for/
     <<
     {
         "result": "WARNING",
```

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/permissions/schema-linter-core-permission-rules.guard` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/permissions/schema-linter-core-permission-rules.guard`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/stateful/schema-stateful-cfn-enforced-checks.guard` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/stateful/schema-stateful-cfn-enforced-checks.guard`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/rule_library/tags/schema-linter-core-tagging-rules.guard` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/rule_library/tags/schema-linter-core-tagging-rules.guard`

 * *Files 2% similar despite different names*

```diff
@@ -63,42 +63,42 @@
         "check_id": "TAG006",
         "message": "`taggable` MUST BE specified when `tagging` is provided"
     }
     >>
 
     when tagging.taggable == true {
 
-        tagOnCreate exists
+        tagging.tagOnCreate exists
         <<
         {
             "result": "NON_COMPLIANT",
             "check_id": "TAG007",
             "message": "Resource MUST provide `tagOnCreate` {true|false} if `tagging.taggable` is true"
         }
         >>
 
-        tagUpdatable exists
+        tagging.tagUpdatable exists
         <<
         {
             "result": "NON_COMPLIANT",
             "check_id": "TAG008",
             "message": "Resource MUST provide `tagUpdatable` {true|false} if `tagging.taggable` is true"
         }
         >>
 
-        cloudFormationSystemTags exists
+        tagging.cloudFormationSystemTags exists
         <<
         {
             "result": "NON_COMPLIANT",
             "check_id": "TAG009",
             "message": "Resource MUST provide `cloudFormationSystemTags` {true|false} if `tagging.taggable` is true"
         }
         >>
 
-        tagProperty exists
+        tagging.tagProperty exists
         <<
         {
             "result": "NON_COMPLIANT",
             "check_id": "TAG010",
             "message": "Resource MUST provide `tagProperty` {/properties/Tags} if `tagging.taggable` is true"
         }
         >>
```

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/utils/arg_handler.py` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/utils/arg_handler.py`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/utils/common.py` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/utils/common.py`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/utils/logger.py` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/utils/logger.py`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.8/src/rpdk/guard_rail/utils/miscellaneous.py` & `resource-schema-guard-rail-0.0.9/src/rpdk/guard_rail/utils/miscellaneous.py`

 * *Files identical despite different names*

