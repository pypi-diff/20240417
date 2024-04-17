# Comparing `tmp/function-tools-0.8.2.tar.gz` & `tmp/function-tools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function-tools-0.8.2.tar", last modified: Mon Dec 18 16:51:05 2023, max compression
+gzip compressed data, was "function-tools-0.9.0.tar", last modified: Mon Feb  5 08:31:02 2024, max compression
```

## Comparing `function-tools-0.8.2.tar` & `function-tools-0.9.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-18 16:51:05.349178 function-tools-0.8.2/
--rw-r--r--   0 toor      (1000) toor      (1000)    22094 2023-12-18 16:50:58.000000 function-tools-0.8.2/CHANGES.md
--rw-r--r--   0 toor      (1000) toor      (1000)     1069 2022-02-16 11:53:12.000000 function-tools-0.8.2/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      275 2022-07-12 08:20:24.000000 function-tools-0.8.2/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)    30635 2023-12-18 16:51:05.349178 function-tools-0.8.2/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     7804 2022-02-16 11:53:12.000000 function-tools-0.8.2/README.md
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-18 16:51:05.318178 function-tools-0.8.2/function_tools/
--rw-r--r--   0 toor      (1000) toor      (1000)       63 2022-02-16 11:53:12.000000 function-tools-0.8.2/function_tools/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      257 2023-08-04 12:26:47.000000 function-tools-0.8.2/function_tools/app_settings.py
--rw-r--r--   0 toor      (1000) toor      (1000)      863 2023-08-04 12:26:47.000000 function-tools-0.8.2/function_tools/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)    59283 2023-12-18 16:50:58.000000 function-tools-0.8.2/function_tools/caches.py
--rw-r--r--   0 toor      (1000) toor      (1000)      125 2023-08-28 09:48:57.000000 function-tools-0.8.2/function_tools/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)      458 2022-02-16 11:53:12.000000 function-tools-0.8.2/function_tools/decorators.py
--rw-r--r--   0 toor      (1000) toor      (1000)      714 2023-08-28 09:48:57.000000 function-tools-0.8.2/function_tools/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)      451 2022-02-16 11:53:12.000000 function-tools-0.8.2/function_tools/errors.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-18 16:51:05.321178 function-tools-0.8.2/function_tools/function_templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-07-05 13:57:48.000000 function-tools-0.8.2/function_tools/function_templates/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-18 16:51:05.341178 function-tools-0.8.2/function_tools/function_templates/function_sync_template/
--rw-r--r--   0 toor      (1000) toor      (1000)      271 2022-07-05 13:57:48.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/README.md
--rw-r--r--   0 toor      (1000) toor      (1000)      107 2023-11-30 11:58:19.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/__init__.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      319 2023-11-30 11:58:19.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/apps.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     1265 2023-11-30 11:58:19.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/caches.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)       66 2022-07-05 13:57:48.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/consts.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)       93 2022-07-05 13:57:48.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/enums.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      247 2023-11-30 11:58:19.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/errors.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     2752 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/functions.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     1272 2023-11-30 11:58:19.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/helpers.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     1537 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/managers.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      316 2023-11-30 11:58:19.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/presenters.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      589 2023-11-30 11:58:19.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/results.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     2743 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/runners.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      181 2022-07-05 13:57:48.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/strings.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)       59 2022-07-05 13:57:48.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/tests.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      855 2023-11-30 11:58:19.000000 function-tools-0.8.2/function_tools/function_templates/function_sync_template/validators.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)    11415 2023-08-06 20:45:45.000000 function-tools-0.8.2/function_tools/functions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5837 2023-09-01 14:45:44.000000 function-tools-0.8.2/function_tools/general.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2638 2023-08-06 20:45:45.000000 function-tools-0.8.2/function_tools/helpers.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-18 16:51:05.342178 function-tools-0.8.2/function_tools/management/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-02-16 11:53:12.000000 function-tools-0.8.2/function_tools/management/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-18 16:51:05.344178 function-tools-0.8.2/function_tools/management/commands/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-02-16 11:53:12.000000 function-tools-0.8.2/function_tools/management/commands/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7409 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/management/commands/register_entities.py
--rw-r--r--   0 toor      (1000) toor      (1000)    17354 2023-12-06 14:36:54.000000 function-tools-0.8.2/function_tools/management/commands/startfunction.py
--rw-r--r--   0 toor      (1000) toor      (1000)       52 2022-02-16 11:53:12.000000 function-tools-0.8.2/function_tools/management/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4957 2022-07-25 11:47:49.000000 function-tools-0.8.2/function_tools/managers.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-18 16:51:05.349178 function-tools-0.8.2/function_tools/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     1137 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)      533 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/migrations/0002_registeredfunction_tags.py
--rw-r--r--   0 toor      (1000) toor      (1000)      808 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/migrations/0003_implementationstrategy.py
--rw-r--r--   0 toor      (1000) toor      (1000)      490 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/migrations/0004_implementationstrategy_order_number.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2708 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/migrations/0005_auto_20220724_0050.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-07-12 12:03:22.000000 function-tools-0.8.2/function_tools/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6434 2022-07-25 11:47:49.000000 function-tools-0.8.2/function_tools/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4535 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)      685 2022-02-16 11:53:12.000000 function-tools-0.8.2/function_tools/presenters.py
--rw-r--r--   0 toor      (1000) toor      (1000)      369 2022-07-27 13:25:54.000000 function-tools-0.8.2/function_tools/receivers.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2386 2022-02-16 11:53:12.000000 function-tools-0.8.2/function_tools/results.py
--rw-r--r--   0 toor      (1000) toor      (1000)    13093 2023-08-06 20:45:45.000000 function-tools-0.8.2/function_tools/runners.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11759 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/storages.py
--rw-r--r--   0 toor      (1000) toor      (1000)    21938 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/strategies.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5198 2023-08-28 09:48:57.000000 function-tools-0.8.2/function_tools/strings.py
--rw-r--r--   0 toor      (1000) toor      (1000)      604 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/types.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5716 2023-12-03 16:53:41.000000 function-tools-0.8.2/function_tools/utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)      408 2022-02-16 11:53:12.000000 function-tools-0.8.2/function_tools/validators.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-18 16:51:05.321178 function-tools-0.8.2/function_tools.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)    30635 2023-12-18 16:51:05.000000 function-tools-0.8.2/function_tools.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     2639 2023-12-18 16:51:05.000000 function-tools-0.8.2/function_tools.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-12-18 16:51:05.000000 function-tools-0.8.2/function_tools.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       48 2023-12-18 16:51:05.000000 function-tools-0.8.2/function_tools.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       15 2023-12-18 16:51:05.000000 function-tools-0.8.2/function_tools.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       47 2023-08-19 18:05:07.000000 function-tools-0.8.2/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       79 2023-12-18 16:51:05.350178 function-tools-0.8.2/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     1707 2023-12-18 16:50:58.000000 function-tools-0.8.2/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-05 08:31:02.110930 function-tools-0.9.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)    22601 2024-02-05 06:55:41.000000 function-tools-0.9.0/CHANGES.md
+-rw-r--r--   0 toor      (1000) toor      (1000)     1069 2022-02-16 11:53:12.000000 function-tools-0.9.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      275 2022-07-12 08:20:24.000000 function-tools-0.9.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    31142 2024-02-05 08:31:02.110930 function-tools-0.9.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     7804 2022-02-16 11:53:12.000000 function-tools-0.9.0/README.md
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-05 08:31:02.079930 function-tools-0.9.0/function_tools/
+-rw-r--r--   0 toor      (1000) toor      (1000)       63 2022-02-16 11:53:12.000000 function-tools-0.9.0/function_tools/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      257 2023-08-04 12:26:47.000000 function-tools-0.9.0/function_tools/app_settings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      863 2023-08-04 12:26:47.000000 function-tools-0.9.0/function_tools/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    59283 2023-12-18 16:50:58.000000 function-tools-0.9.0/function_tools/caches.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      125 2023-08-28 09:48:57.000000 function-tools-0.9.0/function_tools/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      458 2022-02-16 11:53:12.000000 function-tools-0.9.0/function_tools/decorators.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      714 2023-08-28 09:48:57.000000 function-tools-0.9.0/function_tools/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      451 2022-02-16 11:53:12.000000 function-tools-0.9.0/function_tools/errors.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-05 08:31:02.082930 function-tools-0.9.0/function_tools/function_templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-07-05 13:57:48.000000 function-tools-0.9.0/function_tools/function_templates/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-05 08:31:02.095930 function-tools-0.9.0/function_tools/function_templates/function_sync_template/
+-rw-r--r--   0 toor      (1000) toor      (1000)      271 2022-07-05 13:57:48.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/README.md
+-rw-r--r--   0 toor      (1000) toor      (1000)      107 2023-11-30 11:58:19.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/__init__.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      319 2023-11-30 11:58:19.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/apps.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     1265 2023-11-30 11:58:19.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/caches.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)       66 2022-07-05 13:57:48.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/consts.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)       93 2022-07-05 13:57:48.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/enums.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      247 2023-11-30 11:58:19.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/errors.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     2752 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/functions.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     1272 2023-11-30 11:58:19.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/helpers.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     1537 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/managers.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      316 2023-11-30 11:58:19.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/presenters.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      589 2023-11-30 11:58:19.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/results.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     2743 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/runners.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      181 2022-07-05 13:57:48.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/strings.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)       59 2022-07-05 13:57:48.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/tests.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      855 2023-11-30 11:58:19.000000 function-tools-0.9.0/function_tools/function_templates/function_sync_template/validators.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)    11415 2023-08-06 20:45:45.000000 function-tools-0.9.0/function_tools/functions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5837 2023-09-01 14:45:44.000000 function-tools-0.9.0/function_tools/general.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2638 2023-08-06 20:45:45.000000 function-tools-0.9.0/function_tools/helpers.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-05 08:31:02.096930 function-tools-0.9.0/function_tools/management/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-02-16 11:53:12.000000 function-tools-0.9.0/function_tools/management/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-05 08:31:02.102930 function-tools-0.9.0/function_tools/management/commands/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-02-16 11:53:12.000000 function-tools-0.9.0/function_tools/management/commands/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7409 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/management/commands/register_entities.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    17354 2023-12-06 14:36:54.000000 function-tools-0.9.0/function_tools/management/commands/startfunction.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       52 2022-02-16 11:53:12.000000 function-tools-0.9.0/function_tools/management/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5295 2024-02-05 06:55:41.000000 function-tools-0.9.0/function_tools/managers.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-05 08:31:02.108930 function-tools-0.9.0/function_tools/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1137 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      533 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/migrations/0002_registeredfunction_tags.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      808 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/migrations/0003_implementationstrategy.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      490 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/migrations/0004_implementationstrategy_order_number.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2708 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/migrations/0005_auto_20220724_0050.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-07-12 12:03:22.000000 function-tools-0.9.0/function_tools/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6434 2022-07-25 11:47:49.000000 function-tools-0.9.0/function_tools/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4535 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      685 2022-02-16 11:53:12.000000 function-tools-0.9.0/function_tools/presenters.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      369 2022-07-27 13:25:54.000000 function-tools-0.9.0/function_tools/receivers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2386 2022-02-16 11:53:12.000000 function-tools-0.9.0/function_tools/results.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    15956 2024-02-05 06:55:41.000000 function-tools-0.9.0/function_tools/runners.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11759 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/storages.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    21938 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/strategies.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5198 2023-08-28 09:48:57.000000 function-tools-0.9.0/function_tools/strings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      604 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/types.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5716 2023-12-03 16:53:41.000000 function-tools-0.9.0/function_tools/utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      408 2022-02-16 11:53:12.000000 function-tools-0.9.0/function_tools/validators.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-05 08:31:02.109930 function-tools-0.9.0/function_tools.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    31142 2024-02-05 08:31:02.000000 function-tools-0.9.0/function_tools.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     2639 2024-02-05 08:31:02.000000 function-tools-0.9.0/function_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-02-05 08:31:02.000000 function-tools-0.9.0/function_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       48 2024-02-05 08:31:02.000000 function-tools-0.9.0/function_tools.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       15 2024-02-05 08:31:02.000000 function-tools-0.9.0/function_tools.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       47 2023-08-19 18:05:07.000000 function-tools-0.9.0/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       79 2024-02-05 08:31:02.111930 function-tools-0.9.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     1707 2024-02-05 08:30:54.000000 function-tools-0.9.0/setup.py
```

### Comparing `function-tools-0.8.2/CHANGES.md` & `function-tools-0.9.0/CHANGES.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,24 @@
 ### Изменено
  
 ### Исправлено
 
 ### Удалено
 
 
+## [0.9.0] - 2024-01-24
+
+Добавлен режим принудительного запуска запускаемых объектов без добавления их в очередь на исполнение.
+
+## Добавлено
+
+- [EDUSCHL-20274](https://jira.bars.group/browse/EDUSCHL-20274)
+  MINOR Добавлен режим принудительного запуска запускаемых объектов без добавления их в очередь на исполнение.
+
+
 ## [0.8.2] - 2023-12-18
  
 В класс EntityCache добавлен метод last.
 
 ### Добавлено
 
 - [EDUSCHL-19606](https://jira.bars.group/browse/EDUSCHL-19606)
```

### Comparing `function-tools-0.8.2/LICENSE` & `function-tools-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/PKG-INFO` & `function-tools-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-tools
-Version: 0.8.2
+Version: 0.9.0
 Summary: Tools for creating functions
 Home-page: https://github.com/sandanilenko/function-tools
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -128,14 +128,24 @@
 ### Изменено
  
 ### Исправлено
 
 ### Удалено
 
 
+## [0.9.0] - 2024-01-24
+
+Добавлен режим принудительного запуска запускаемых объектов без добавления их в очередь на исполнение.
+
+## Добавлено
+
+- [EDUSCHL-20274](https://jira.bars.group/browse/EDUSCHL-20274)
+  MINOR Добавлен режим принудительного запуска запускаемых объектов без добавления их в очередь на исполнение.
+
+
 ## [0.8.2] - 2023-12-18
  
 В класс EntityCache добавлен метод last.
 
 ### Добавлено
 
 - [EDUSCHL-19606](https://jira.bars.group/browse/EDUSCHL-19606)
```

### Comparing `function-tools-0.8.2/README.md` & `function-tools-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/apps.py` & `function-tools-0.9.0/function_tools/apps.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/caches.py` & `function-tools-0.9.0/function_tools/caches.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/enums.py` & `function-tools-0.9.0/function_tools/enums.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/function_templates/function_sync_template/caches.py-tpl` & `function-tools-0.9.0/function_tools/function_templates/function_sync_template/caches.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/function_templates/function_sync_template/functions.py-tpl` & `function-tools-0.9.0/function_tools/function_templates/function_sync_template/functions.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/function_templates/function_sync_template/helpers.py-tpl` & `function-tools-0.9.0/function_tools/function_templates/function_sync_template/helpers.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/function_templates/function_sync_template/managers.py-tpl` & `function-tools-0.9.0/function_tools/function_templates/function_sync_template/managers.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/function_templates/function_sync_template/results.py-tpl` & `function-tools-0.9.0/function_tools/function_templates/function_sync_template/results.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/function_templates/function_sync_template/runners.py-tpl` & `function-tools-0.9.0/function_tools/function_templates/function_sync_template/runners.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/function_templates/function_sync_template/validators.py-tpl` & `function-tools-0.9.0/function_tools/function_templates/function_sync_template/validators.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/functions.py` & `function-tools-0.9.0/function_tools/functions.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/general.py` & `function-tools-0.9.0/function_tools/general.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/helpers.py` & `function-tools-0.9.0/function_tools/helpers.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/management/commands/register_entities.py` & `function-tools-0.9.0/function_tools/management/commands/register_entities.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/management/commands/startfunction.py` & `function-tools-0.9.0/function_tools/management/commands/startfunction.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/managers.py` & `function-tools-0.9.0/function_tools/managers.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 ):
     """
     Абстрактный класс для создания менеджеров ранеров запускаемых объектов.
     Служит для добавления функций-задач, ранеров в очередь на исполнение.
     Является удобным механизмом для скрытия заполнения ранера и его запуск.
     """
 
+    # Режим принудительного запуска запускаемых объектов без постановки их в очередь на исполнение
+    # По-умолчанию не задан и определяется ранером
+    forced_run: Optional[bool] = None
+
     def __init__(
         self,
         *args,
         **kwargs,
     ):
         self._runner_class = self._prepare_runner_class()
 
@@ -104,15 +108,15 @@
     def _after_start_runner(self, *args, **kwargs):
         """
         Точка расширения поведения менеджера ранера после запуска ранера.
         """
 
     def run(self, *args, **kwargs):
         self._before_create_runner(*args, **kwargs)
-        self._create_runner(*args, **kwargs)
+        self._create_runner(*args, is_force_run=self.forced_run, **kwargs)
         self._after_create_runner(*args, **kwargs)
 
         self._before_prepare_runner(*args, **kwargs)
         self._prepare_runner(*args, **kwargs)
         self._after_prepare_runner(*args, **kwargs)
 
         self._before_start_runner(*args, **kwargs)
```

### Comparing `function-tools-0.8.2/function_tools/migrations/0001_initial.py` & `function-tools-0.9.0/function_tools/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/migrations/0002_registeredfunction_tags.py` & `function-tools-0.9.0/function_tools/migrations/0002_registeredfunction_tags.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/migrations/0003_implementationstrategy.py` & `function-tools-0.9.0/function_tools/migrations/0003_implementationstrategy.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/migrations/0005_auto_20220724_0050.py` & `function-tools-0.9.0/function_tools/migrations/0005_auto_20220724_0050.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/mixins.py` & `function-tools-0.9.0/function_tools/mixins.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/models.py` & `function-tools-0.9.0/function_tools/models.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/presenters.py` & `function-tools-0.9.0/function_tools/presenters.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/results.py` & `function-tools-0.9.0/function_tools/results.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/runners.py` & `function-tools-0.9.0/function_tools/runners.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from abc import (
     ABCMeta,
 )
 from collections import (
     deque,
 )
 from typing import (
+    TYPE_CHECKING,
     Deque,
+    Iterator,
     List,
     Optional,
     Tuple,
     Type,
     Union,
 )
 
@@ -30,54 +32,128 @@
 )
 from function_tools.mixins import (
     GlobalHelperMixin,
     HelperMixin,
 )
 
 
+if TYPE_CHECKING:
+    from function_tools.results import (
+        BaseRunnableResult,
+    )
+
+
 class BaseRunner(
     HelperMixin,
     RunnableObject,
     metaclass=ABCMeta,
 ):
     """
     Базовый класс для создания ранеров выполнения запускаемых объектов.
     """
 
-    def __init__(self, *args, **kwargs):
+    # Режим принудительного запуска запускаемых объектов без постановки их в очередь на исполнение
+    # По-умолчанию не используется
+    forced_run: Optional[bool] = None
+
+    def __init__(self, *args, is_force_run: Optional[bool] = None, **kwargs):
+        """Инициализация.
+
+        Args:
+            is_force_run: Определяет необходимость использования режима принудительного запуска запускаемых
+                объектов. Параметр игнорируется, если у класса ранера задан атрибут forced_run (не равен None).
+        """
         super().__init__(*args, **kwargs)
 
+        if self.forced_run is None and is_force_run is not None:
+            self.forced_run = is_force_run
+
         self._helper: Union[BaseHelper, BaseRunnerHelper] = self._prepare_helper(*args, **kwargs)
         self._queue: Deque[RunnableObject] = deque()
 
-        self._populate_queue_by_runnable_classes(*args, **kwargs)
+        if self.forced_run:
+            self._force_run_runnable_objects(*args, is_force_run=self.forced_run, **kwargs)
+        else:
+            self._populate_queue_by_runnable_classes(*args, **kwargs)
 
     @classmethod
     def _prepare_runnable_classes(cls) -> List[Type[RunnableObject]]:
         """
         Возвращает список классов запускаемых объектов, которые будут ставиться в очередь на исполнение.
 
         В текущий момент нужно явно указывать классы, но в будущем, появится возможность получения списка классов
         запускаемых сущностей в рамках ранера.
         """
 
-    def _populate_queue_by_runnable_classes(self, *args, **kwargs):
+    def _get_runnable_objects(self, *args, **kwargs) -> Iterator[RunnableObject]:
         """
-        Заполнение очереди запускаемыми объектами.
+        Возвращает генератор запускаемых объектов.
         """
-        runnable_classes = self._prepare_runnable_classes()
-
-        for runnable_class in runnable_classes:
+        for runnable_class in self._prepare_runnable_classes():
             runnable = runnable_class(*args, **kwargs)
+            if isinstance(runnable, tuple):
+                yield from runnable
+            else:
+                yield runnable
+
+    def _force_run_runnable_objects(self, *args, **kwargs):
+        """
+        Принудительное выполнение запускаемых объектов без добавления их в очередь.
+        """
+        self.before_validate()
+        self.validate()
+        self.after_validate()
+
+        if self.result.has_not_errors:
+            # атрибут отвечающий за передачу результата следующему в цепочке ранеру
+            prev_runnable_result = None
 
+            for runnable in self._get_runnable_objects(*args, **kwargs):
+                runnable_result = self._run_runnable(
+                    runnable,
+                    *args,
+                    prev_runnable_result=prev_runnable_result,
+                    **kwargs,
+                )
+                prev_runnable_result = runnable_result
+                self.result.append_entity(runnable_result)
+
+    @staticmethod
+    def _run_runnable(
+        runnable: RunnableObject,
+        *args,
+        prev_runnable_result: Optional[Union[BaseError, 'BaseRunnableResult']] = None,
+        **kwargs
+    ) -> Union[BaseError, 'BaseRunnableResult']:
+        """Запуск запускаемого объекта."""
+        if prev_runnable_result:
+            runnable.adopt_prev_runnable_result(prev_runnable_result=prev_runnable_result)
+
+        runnable.before_validate()
+        runnable.validate()
+        runnable.after_validate()
+
+        runnable.before_run(*args, **kwargs)
+        runnable.run(*args, **kwargs)
+        runnable.after_run(*args, **kwargs)
+
+        return runnable.result
+
+    def _populate_queue_by_runnable_classes(self, *args, **kwargs):
+        """
+        Заполнение очереди запускаемыми объектами.
+        """
+        for runnable in self._get_runnable_objects(*args, **kwargs):
             self.enqueue(runnable=runnable, *args, **kwargs)
 
     def _prepare_runnable_before_enqueue(
         self,
         runnable: RunnableObject,
+        *args,
+        **kwargs,
     ):
         """
         Подготовка запускаемого объекта к работе.
 
         В данной точке расширения можно пропатчить объект через публичные методы.
         """
         if isinstance(runnable, GlobalHelperMixin):
@@ -94,17 +170,15 @@
         """
         Добавление задачи на выполнение функции в очередь.
         """
         if not isinstance(runnable, tuple):
             runnable = (runnable, )
 
         for r in runnable:
-            self._prepare_runnable_before_enqueue(
-                runnable=r,
-            )
+            self._prepare_runnable_before_enqueue(runnable=r, *args, **kwargs)
 
             self._queue.append(r)
 
     def _update_queue(self):
         """
         Метод позволяет обновлять очередь ранеров на ходу.
         """
@@ -136,27 +210,17 @@
             self._update_queue()
 
             while self._queue:
                 runnable: RunnableObject = (
                     self._queue.popleft()
                 )
 
-                runnable.adopt_prev_runnable_result(prev_runnable_result=prev_runnable_result)
-
-                runnable.before_validate()
-                runnable.validate()
-                runnable.after_validate()
-
-                runnable.before_run(*args, **kwargs)
-                runnable.run(*args, **kwargs)
-                runnable.after_run(*args, **kwargs)
-
-                prev_runnable_result = runnable.result
-
-                self.result.append_entity(runnable.result)
+                runnable_result = self._run_runnable(runnable, *args, prev_runnable_result, **kwargs)
+                prev_runnable_result = runnable_result
+                self.result.append_entity(runnable_result)
 
 
 class LazySavingRunner(
     BaseRunner,
     LazySavingRunnableObject,
     metaclass=ABCMeta,
 ):
```

### Comparing `function-tools-0.8.2/function_tools/storages.py` & `function-tools-0.9.0/function_tools/storages.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/strategies.py` & `function-tools-0.9.0/function_tools/strategies.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/strings.py` & `function-tools-0.9.0/function_tools/strings.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/types.py` & `function-tools-0.9.0/function_tools/types.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools/utils.py` & `function-tools-0.9.0/function_tools/utils.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/function_tools.egg-info/PKG-INFO` & `function-tools-0.9.0/function_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-tools
-Version: 0.8.2
+Version: 0.9.0
 Summary: Tools for creating functions
 Home-page: https://github.com/sandanilenko/function-tools
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -128,14 +128,24 @@
 ### Изменено
  
 ### Исправлено
 
 ### Удалено
 
 
+## [0.9.0] - 2024-01-24
+
+Добавлен режим принудительного запуска запускаемых объектов без добавления их в очередь на исполнение.
+
+## Добавлено
+
+- [EDUSCHL-20274](https://jira.bars.group/browse/EDUSCHL-20274)
+  MINOR Добавлен режим принудительного запуска запускаемых объектов без добавления их в очередь на исполнение.
+
+
 ## [0.8.2] - 2023-12-18
  
 В класс EntityCache добавлен метод last.
 
 ### Добавлено
 
 - [EDUSCHL-19606](https://jira.bars.group/browse/EDUSCHL-19606)
```

### Comparing `function-tools-0.8.2/function_tools.egg-info/SOURCES.txt` & `function-tools-0.9.0/function_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `function-tools-0.8.2/setup.py` & `function-tools-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import (
     find_packages,
     setup,
 )
 
 
-__version__ = '0.8.2'
+__version__ = '0.9.0'
 
 
 here = path.abspath(path.dirname(__file__))
 
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
```

