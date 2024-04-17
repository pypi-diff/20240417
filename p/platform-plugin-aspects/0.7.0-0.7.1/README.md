# Comparing `tmp/platform_plugin_aspects-0.7.0.tar.gz` & `tmp/platform_plugin_aspects-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform_plugin_aspects-0.7.0.tar", last modified: Tue Apr 16 16:07:41 2024, max compression
+gzip compressed data, was "platform_plugin_aspects-0.7.1.tar", last modified: Wed Apr 17 16:59:35 2024, max compression
```

## Comparing `platform_plugin_aspects-0.7.0.tar` & `platform_plugin_aspects-0.7.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.239516 platform_plugin_aspects-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-16 16:07:41.239516 platform_plugin_aspects-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.231516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/extensions/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/base_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/course_overview_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/external_id_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/user_profile_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/user_retire_sink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.231516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/css/superset.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/html/superset.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/html/superset_student.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/js/embed_dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/js/install_required.js
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/js/superset.js
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.231516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/templates/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/waffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.239516 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.239516 platform_plugin_aspects-0.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 16:07:41.239516 platform_plugin_aspects-0.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6977 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.953396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.953396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/extensions/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.953396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.953396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/load_test_tracking_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/base_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/course_overview_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/external_id_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/user_profile_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/user_retire_sink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.949396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/css/superset.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/html/superset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/html/superset_student.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/js/embed_dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/js/install_required.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/js/superset.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.949396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/templates/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6977 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/setup.py
```

### Comparing `platform_plugin_aspects-0.7.0/CHANGELOG.rst` & `platform_plugin_aspects-0.7.1/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,23 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.7.1 - 2024-04-17
+******************
+
+Fixed
+=====
+
+* Fixed issue with embedded dashboards throwing javascript errors
+* Fixed issues with translated embedded dashboards erroring in Superset
+
 0.7.0 - 2024-04-12
 ******************
 
 Added
 =====
 
 * Add endpoint for fetchGuestToken
```

### Comparing `platform_plugin_aspects-0.7.0/LICENSE` & `platform_plugin_aspects-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/PKG-INFO` & `platform_plugin_aspects-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.7.0
+Version: 0.7.1
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -276,14 +276,23 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.7.1 - 2024-04-17
+******************
+
+Fixed
+=====
+
+* Fixed issue with embedded dashboards throwing javascript errors
+* Fixed issues with translated embedded dashboards erroring in Superset
+
 0.7.0 - 2024-04-12
 ******************
 
 Added
 =====
 
 * Add endpoint for fetchGuestToken
```

### Comparing `platform_plugin_aspects-0.7.0/README.rst` & `platform_plugin_aspects-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/apps.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/apps.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/extensions/filters.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/extensions/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         html = template.render(Context(context))
         frag = Fragment(html)
         frag.add_css(self.resource_string("static/css/superset.css"))
         frag.add_javascript(self.resource_string("static/js/embed_dashboard.js"))
         section_data = {
             "fragment": frag,
             "section_key": BLOCK_CATEGORY,
-            "section_display_name": _("Analytics"),
+            "section_display_name": _("Reports"),
             "course_id": str(context.get("course_id")),
             "superset_guest_token_url": str(context.get("superset_guest_token_url")),
             "superset_url": str(context.get("superset_url")),
             "template_path_prefix": TEMPLATE_ABSOLUTE_PATH,
         }
         context["sections"].append(section_data)
         return {
```

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/load_test_tracking_events.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/settings/common.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/settings/common.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/settings/production.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/settings/production.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/signals.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/signals.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/base_sink.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/base_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/course_overview_sink.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/course_overview_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/external_id_sink.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/external_id_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/serializers.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/serializers.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/user_profile_sink.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/user_profile_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/user_retire_sink.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/user_retire_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/css/superset.css` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/css/superset.css`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/html/superset.html` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/html/superset.html`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
             <label for="tab-{{forloop.counter}}">{{dashboard.name}}</label>
             <div class="aspects-content superset-embedded-container" id="superset-embedded-container-{{dashboard.uuid}}"></div>
         </div>
         {% endfor %}
     </div>
     {% endif %}
 
+    {{superset_dashboards|json_script:"superset_dashboards"}}
+
     <script type="text/javascript">
-        window.superset_dashboards = {{superset_dashboards | safe }};
+        window.superset_dashboards = JSON.parse(document.getElementById('superset_dashboards').textContent);
         window.superset_url = "{{superset_url}}";
         window.superset_guest_token_url = "{{superset_guest_token_url}}";
     </script>
     {% endif %}
 </div>
```

#### html2text {}

```diff
@@ -7,9 +7,9 @@
 {% elif not superset_dashboards %}
 Dashboard UUID is not set. Please set the dashboard UUID in the Studio.
 {% elif superset_url and superset_guest_token_url %} {% if xblock_id %}
 {% else %}
 {% for dashboard in superset_dashboards %}
 {% if forloop.counter == 1 %} #{% else %} o{% endif %} {{dashboard.name}}
 {% endfor %}
-{% endif %}
+{% endif %} {{superset_dashboards|json_script:"superset_dashboards"}}
 {% endif %}
```

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/js/embed_dashboard.js` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/js/embed_dashboard.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/js/superset.js` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/js/superset.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/tasks.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/tasks.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/templates/instructor_dashboard/aspects.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/urls.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/urls.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/utils.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Utilities for the Aspects app.
 """
 
 from __future__ import annotations
 
+import copy
 import logging
 import os
 import uuid
 from importlib import import_module
 from urllib.parse import urljoin
 
 from django.conf import settings
@@ -45,35 +46,38 @@
         dashboards (list): list of superset dashboard uuid.
         filters (list): list of filters to apply to the dashboard.
         language (str): the language code of the end user.
     """
     course_id = context["course_id"]
     superset_config = settings.SUPERSET_CONFIG
 
+    # We're modifying this, keep a local copy
+    rtn_dashboards = copy.deepcopy(dashboards)
+
     if language:
-        for dashboard in dashboards:
+        for dashboard in rtn_dashboards:
             if not dashboard.get("allow_translations"):
                 continue
             dashboard["slug"] = f"{dashboard['slug']}-{language}"
-            dashboard["uuid"] = str(get_uuid5(dashboard["uuid"], language))
+            dashboard["uuid"] = get_localized_uuid(dashboard["uuid"], language)
 
     superset_url = _fix_service_url(superset_config.get("service_url"))
 
     # Use an absolute LMS URL here, just in case we're being rendered in an MFE.
     guest_token_url = urljoin(
         settings.LMS_ROOT_URL,
         reverse(
             "platform_plugin_aspects:superset_guest_token",
             kwargs={"course_id": course_id},
         ),
     )
 
     context.update(
         {
-            "superset_dashboards": dashboards,
+            "superset_dashboards": rtn_dashboards,
             "superset_url": superset_url,
             "superset_guest_token_url": guest_token_url,
         }
     )
 
     return context
 
@@ -100,19 +104,32 @@
         or superset_config.get("service_url")
     )
     superset_username = superset_config.get("username")
     superset_password = superset_config.get("password")
 
     formatted_filters = [filter.format(course=course, user=user) for filter in filters]
 
+    resources = []
+
+    # Get permissions for all localized versions of the dashboards
+    for dashboard in dashboards:
+        resources.append({"type": "dashboard", "id": dashboard["uuid"]})
+
+        if dashboard.get("allow_translations"):
+            for locale in settings.SUPERSET_DASHBOARD_LOCALES:
+                resources.append(
+                    {
+                        "type": "dashboard",
+                        "id": get_localized_uuid(dashboard["uuid"], locale),
+                    }
+                )
+
     data = {
         "user": _superset_user_data(user),
-        "resources": [
-            {"type": "dashboard", "id": dashboard["uuid"]} for dashboard in dashboards
-        ],
+        "resources": resources,
         "rls": [{"clause": filter} for filter in formatted_filters],
     }
 
     try:
         client = SupersetClient(
             host=superset_internal_host,
             username=superset_username,
@@ -241,14 +258,14 @@
     Get the CCX courses for a given course.
     """
     if settings.FEATURES.get("CUSTOM_COURSES_EDX"):
         return get_model("custom_course_edx").objects.filter(course_id=course_id)
     return []
 
 
-def get_uuid5(base_uuid, language):
+def get_localized_uuid(base_uuid, language):
     """
     Generate an idempotent uuid.
     """
     base_uuid = uuid.UUID(base_uuid)
     base_namespace = uuid.uuid5(base_uuid, "superset")
-    return uuid.uuid5(base_namespace, language)
+    return str(uuid.uuid5(base_namespace, language))
```

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/views.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/views.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects/xblock.py` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects/xblock.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/PKG-INFO` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.7.0
+Version: 0.7.1
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -276,14 +276,23 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.7.1 - 2024-04-17
+******************
+
+Fixed
+=====
+
+* Fixed issue with embedded dashboards throwing javascript errors
+* Fixed issues with translated embedded dashboards erroring in Superset
+
 0.7.0 - 2024-04-12
 ******************
 
 Added
 =====
 
 * Add endpoint for fetchGuestToken
```

### Comparing `platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/SOURCES.txt` & `platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/requirements/constraints.txt` & `platform_plugin_aspects-0.7.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.0/setup.py` & `platform_plugin_aspects-0.7.1/setup.py`

 * *Files identical despite different names*

