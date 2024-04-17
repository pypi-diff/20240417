# Comparing `tmp/django-history-triggers-3.4.6.tar.gz` & `tmp/django-history-triggers-3.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-history-triggers-3.4.6.tar", last modified: Fri Mar 22 15:44:37 2024, max compression
+gzip compressed data, was "django-history-triggers-3.4.7.tar", last modified: Wed Apr 17 18:14:56 2024, max compression
```

## Comparing `django-history-triggers-3.4.6.tar` & `django-history-triggers-3.4.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.395434 django-history-triggers-3.4.6/
--rw-r--r--   0 dcwatson   (501) staff       (20)     1316 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/LICENSE
--rw-r--r--   0 dcwatson   (501) staff       (20)       38 2022-03-20 13:08:52.000000 django-history-triggers-3.4.6/MANIFEST.in
--rw-r--r--   0 dcwatson   (501) staff       (20)     4844 2024-03-22 15:44:37.395382 django-history-triggers-3.4.6/PKG-INFO
--rw-r--r--   0 dcwatson   (501) staff       (20)     4196 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/README.md
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.395219 django-history-triggers-3.4.6/django_history_triggers.egg-info/
--rw-r--r--   0 dcwatson   (501) staff       (20)     4844 2024-03-22 15:44:37.000000 django-history-triggers-3.4.6/django_history_triggers.egg-info/PKG-INFO
--rw-r--r--   0 dcwatson   (501) staff       (20)     1213 2024-03-22 15:44:37.000000 django-history-triggers-3.4.6/django_history_triggers.egg-info/SOURCES.txt
--rw-r--r--   0 dcwatson   (501) staff       (20)        1 2024-03-22 15:44:37.000000 django-history-triggers-3.4.6/django_history_triggers.egg-info/dependency_links.txt
--rw-r--r--   0 dcwatson   (501) staff       (20)        8 2024-03-22 15:44:37.000000 django-history-triggers-3.4.6/django_history_triggers.egg-info/top_level.txt
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.392845 django-history-triggers-3.4.6/history/
--rw-r--r--   0 dcwatson   (501) staff       (20)     1032 2024-03-22 15:26:12.000000 django-history-triggers-3.4.6/history/__init__.py
--rw-r--r--   0 dcwatson   (501) staff       (20)     3255 2024-03-22 15:39:42.000000 django-history-triggers-3.4.6/history/admin.py
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.393233 django-history-triggers-3.4.6/history/backends/
--rw-r--r--   0 dcwatson   (501) staff       (20)      916 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/backends/__init__.py
--rw-r--r--   0 dcwatson   (501) staff       (20)     4716 2024-03-17 12:12:29.000000 django-history-triggers-3.4.6/history/backends/base.py
--rw-r--r--   0 dcwatson   (501) staff       (20)     5268 2024-03-22 15:39:29.000000 django-history-triggers-3.4.6/history/backends/postgres.py
--rw-r--r--   0 dcwatson   (501) staff       (20)     5457 2024-03-22 15:39:38.000000 django-history-triggers-3.4.6/history/backends/sqlite.py
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.393339 django-history-triggers-3.4.6/history/contrib/
--rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/contrib/__init__.py
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.393508 django-history-triggers-3.4.6/history/contrib/loaddata/
--rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/contrib/loaddata/__init__.py
--rw-r--r--   0 dcwatson   (501) staff       (20)      145 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/contrib/loaddata/apps.py
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.393610 django-history-triggers-3.4.6/history/contrib/loaddata/management/
--rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/contrib/loaddata/management/__init__.py
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.393777 django-history-triggers-3.4.6/history/contrib/loaddata/management/commands/
--rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/contrib/loaddata/management/commands/__init__.py
--rw-r--r--   0 dcwatson   (501) staff       (20)      273 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/contrib/loaddata/management/commands/loaddata.py
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.393979 django-history-triggers-3.4.6/history/contrib/migrate/
--rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/contrib/migrate/__init__.py
--rw-r--r--   0 dcwatson   (501) staff       (20)      142 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/contrib/migrate/apps.py
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.394088 django-history-triggers-3.4.6/history/contrib/migrate/management/
--rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/contrib/migrate/management/__init__.py
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.394273 django-history-triggers-3.4.6/history/contrib/migrate/management/commands/
--rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/contrib/migrate/management/commands/__init__.py
--rw-r--r--   0 dcwatson   (501) staff       (20)      270 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/contrib/migrate/management/commands/migrate.py
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.394381 django-history-triggers-3.4.6/history/management/
--rw-r--r--   0 dcwatson   (501) staff       (20)        0 2021-07-22 13:24:25.000000 django-history-triggers-3.4.6/history/management/__init__.py
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.394564 django-history-triggers-3.4.6/history/management/commands/
--rw-r--r--   0 dcwatson   (501) staff       (20)        0 2021-07-22 13:24:25.000000 django-history-triggers-3.4.6/history/management/commands/__init__.py
--rw-r--r--   0 dcwatson   (501) staff       (20)     2664 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/management/commands/triggers.py
--rw-r--r--   0 dcwatson   (501) staff       (20)      857 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/middleware.py
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.394779 django-history-triggers-3.4.6/history/migrations/
--rw-r--r--   0 dcwatson   (501) staff       (20)     2585 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/migrations/0001_initial.py
--rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/migrations/__init__.py
--rw-r--r--   0 dcwatson   (501) staff       (20)     3000 2024-03-22 15:39:13.000000 django-history-triggers-3.4.6/history/models.py
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.391389 django-history-triggers-3.4.6/history/templates/
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.394875 django-history-triggers-3.4.6/history/templates/history/
--rw-r--r--   0 dcwatson   (501) staff       (20)     2193 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/templates/history/admin_history.html
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-03-22 15:44:37.395082 django-history-triggers-3.4.6/history/templatetags/
--rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/templatetags/__init__.py
--rw-r--r--   0 dcwatson   (501) staff       (20)      826 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/templatetags/history.py
--rw-r--r--   0 dcwatson   (501) staff       (20)      543 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/history/utils.py
--rw-r--r--   0 dcwatson   (501) staff       (20)       94 2024-03-22 15:44:37.395606 django-history-triggers-3.4.6/setup.cfg
--rw-r--r--   0 dcwatson   (501) staff       (20)     1066 2024-03-07 17:46:19.000000 django-history-triggers-3.4.6/setup.py
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.313597 django-history-triggers-3.4.7/
+-rw-r--r--   0 dcwatson   (501) staff       (20)     1316 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/LICENSE
+-rw-r--r--   0 dcwatson   (501) staff       (20)       38 2022-03-20 13:08:52.000000 django-history-triggers-3.4.7/MANIFEST.in
+-rw-r--r--   0 dcwatson   (501) staff       (20)     4930 2024-04-17 18:14:56.313542 django-history-triggers-3.4.7/PKG-INFO
+-rw-r--r--   0 dcwatson   (501) staff       (20)     4282 2024-04-17 18:03:27.000000 django-history-triggers-3.4.7/README.md
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.313362 django-history-triggers-3.4.7/django_history_triggers.egg-info/
+-rw-r--r--   0 dcwatson   (501) staff       (20)     4930 2024-04-17 18:14:56.000000 django-history-triggers-3.4.7/django_history_triggers.egg-info/PKG-INFO
+-rw-r--r--   0 dcwatson   (501) staff       (20)     1213 2024-04-17 18:14:56.000000 django-history-triggers-3.4.7/django_history_triggers.egg-info/SOURCES.txt
+-rw-r--r--   0 dcwatson   (501) staff       (20)        1 2024-04-17 18:14:56.000000 django-history-triggers-3.4.7/django_history_triggers.egg-info/dependency_links.txt
+-rw-r--r--   0 dcwatson   (501) staff       (20)        8 2024-04-17 18:14:56.000000 django-history-triggers-3.4.7/django_history_triggers.egg-info/top_level.txt
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.311131 django-history-triggers-3.4.7/history/
+-rw-r--r--   0 dcwatson   (501) staff       (20)     1054 2024-04-17 18:10:17.000000 django-history-triggers-3.4.7/history/__init__.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)     3255 2024-03-22 15:39:42.000000 django-history-triggers-3.4.7/history/admin.py
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.311545 django-history-triggers-3.4.7/history/backends/
+-rw-r--r--   0 dcwatson   (501) staff       (20)      916 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/backends/__init__.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)     4782 2024-04-17 18:00:46.000000 django-history-triggers-3.4.7/history/backends/base.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)     5268 2024-03-22 15:39:29.000000 django-history-triggers-3.4.7/history/backends/postgres.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)     5457 2024-03-22 15:39:38.000000 django-history-triggers-3.4.7/history/backends/sqlite.py
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.311658 django-history-triggers-3.4.7/history/contrib/
+-rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/contrib/__init__.py
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.311811 django-history-triggers-3.4.7/history/contrib/loaddata/
+-rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/contrib/loaddata/__init__.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)      145 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/contrib/loaddata/apps.py
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.311904 django-history-triggers-3.4.7/history/contrib/loaddata/management/
+-rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/contrib/loaddata/management/__init__.py
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.312064 django-history-triggers-3.4.7/history/contrib/loaddata/management/commands/
+-rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/contrib/loaddata/management/commands/__init__.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)      273 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/contrib/loaddata/management/commands/loaddata.py
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.312244 django-history-triggers-3.4.7/history/contrib/migrate/
+-rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/contrib/migrate/__init__.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)      142 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/contrib/migrate/apps.py
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.312341 django-history-triggers-3.4.7/history/contrib/migrate/management/
+-rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/contrib/migrate/management/__init__.py
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.312517 django-history-triggers-3.4.7/history/contrib/migrate/management/commands/
+-rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/contrib/migrate/management/commands/__init__.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)      270 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/contrib/migrate/management/commands/migrate.py
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.312613 django-history-triggers-3.4.7/history/management/
+-rw-r--r--   0 dcwatson   (501) staff       (20)        0 2021-07-22 13:24:25.000000 django-history-triggers-3.4.7/history/management/__init__.py
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.312765 django-history-triggers-3.4.7/history/management/commands/
+-rw-r--r--   0 dcwatson   (501) staff       (20)        0 2021-07-22 13:24:25.000000 django-history-triggers-3.4.7/history/management/commands/__init__.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)     2664 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/management/commands/triggers.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)      857 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/middleware.py
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.312954 django-history-triggers-3.4.7/history/migrations/
+-rw-r--r--   0 dcwatson   (501) staff       (20)     2585 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/migrations/0001_initial.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/migrations/__init__.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)     3000 2024-03-22 15:39:13.000000 django-history-triggers-3.4.7/history/models.py
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.309603 django-history-triggers-3.4.7/history/templates/
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.313038 django-history-triggers-3.4.7/history/templates/history/
+-rw-r--r--   0 dcwatson   (501) staff       (20)     2193 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/templates/history/admin_history.html
+drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2024-04-17 18:14:56.313205 django-history-triggers-3.4.7/history/templatetags/
+-rw-r--r--   0 dcwatson   (501) staff       (20)        0 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/templatetags/__init__.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)      826 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/templatetags/history.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)      543 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/history/utils.py
+-rw-r--r--   0 dcwatson   (501) staff       (20)       94 2024-04-17 18:14:56.313764 django-history-triggers-3.4.7/setup.cfg
+-rw-r--r--   0 dcwatson   (501) staff       (20)     1066 2024-03-07 17:46:19.000000 django-history-triggers-3.4.7/setup.py
```

### Comparing `django-history-triggers-3.4.6/LICENSE` & `django-history-triggers-3.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-history-triggers-3.4.6/PKG-INFO` & `django-history-triggers-3.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-history-triggers
-Version: 3.4.6
+Version: 3.4.7
 Summary: Management command and middleware for Django history triggers.
 Home-page: https://github.com/imsweb/django-history-triggers
 Author: Dan Watson
 Author-email: watsond@imsweb.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -42,14 +42,15 @@
    data -- add a `--clear` option to do that.
 
 
 ## Settings
 
 * `HISTORY_MODEL` (default: `"history.ObjectHistory"`)
 * `HISTORY_IGNORE_APPS` (default: `["admin", "contenttypes", "sessions"]`)
+* `HISTORY_IGNORE_MODELS` (default `[]` - should be lowercase `app_label.model_name`)
 * `HISTORY_MIDDLEWARE_IGNORE` (default: `[]`)
 * `HISTORY_FILTER` (default: `"history.utils.default_filter"`)
 * `HISTORY_REQUEST_CONTEXT` (default: `"history.utils.get_request_context"`)
 * `HISTORY_ADMIN_ENABLED` (default: `True`)
 * `HISTORY_INCLUDE_UNMANAGED` (default: `True`)
```

### Comparing `django-history-triggers-3.4.6/README.md` & `django-history-triggers-3.4.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
    data -- add a `--clear` option to do that.
 
 
 ## Settings
 
 * `HISTORY_MODEL` (default: `"history.ObjectHistory"`)
 * `HISTORY_IGNORE_APPS` (default: `["admin", "contenttypes", "sessions"]`)
+* `HISTORY_IGNORE_MODELS` (default `[]` - should be lowercase `app_label.model_name`)
 * `HISTORY_MIDDLEWARE_IGNORE` (default: `[]`)
 * `HISTORY_FILTER` (default: `"history.utils.default_filter"`)
 * `HISTORY_REQUEST_CONTEXT` (default: `"history.utils.get_request_context"`)
 * `HISTORY_ADMIN_ENABLED` (default: `True`)
 * `HISTORY_INCLUDE_UNMANAGED` (default: `True`)
```

### Comparing `django-history-triggers-3.4.6/django_history_triggers.egg-info/PKG-INFO` & `django-history-triggers-3.4.7/django_history_triggers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-history-triggers
-Version: 3.4.6
+Version: 3.4.7
 Summary: Management command and middleware for Django history triggers.
 Home-page: https://github.com/imsweb/django-history-triggers
 Author: Dan Watson
 Author-email: watsond@imsweb.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -42,14 +42,15 @@
    data -- add a `--clear` option to do that.
 
 
 ## Settings
 
 * `HISTORY_MODEL` (default: `"history.ObjectHistory"`)
 * `HISTORY_IGNORE_APPS` (default: `["admin", "contenttypes", "sessions"]`)
+* `HISTORY_IGNORE_MODELS` (default `[]` - should be lowercase `app_label.model_name`)
 * `HISTORY_MIDDLEWARE_IGNORE` (default: `[]`)
 * `HISTORY_FILTER` (default: `"history.utils.default_filter"`)
 * `HISTORY_REQUEST_CONTEXT` (default: `"history.utils.get_request_context"`)
 * `HISTORY_ADMIN_ENABLED` (default: `True`)
 * `HISTORY_INCLUDE_UNMANAGED` (default: `True`)
```

### Comparing `django-history-triggers-3.4.6/django_history_triggers.egg-info/SOURCES.txt` & `django-history-triggers-3.4.7/django_history_triggers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-history-triggers-3.4.6/history/__init__.py` & `django-history-triggers-3.4.7/history/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 
 from django.conf import settings
 
 from .backends import get_backend, session  # noqa
 from .utils import get_history_model  # noqa
 
-__version__ = "3.4.6"
+__version__ = "3.4.7"
 __version_info__ = tuple(
     int(num) if num.isdigit() else num
     for num in re.findall(r"([a-z\d]+)", __version__, re.I)
 )
 
 
 class _Configuration:
@@ -22,14 +22,15 @@
             raise AttributeError(name)
         setting_name = "{}_{}".format(self.prefix, name).upper()
         return getattr(settings, setting_name, self.defaults[name])
 
 
 conf = _Configuration(
     IGNORE_APPS=["admin", "contenttypes", "sessions"],
+    IGNORE_MODELS=[],
     MIDDLEWARE_IGNORE=[],
     FILTER="history.utils.default_filter",
     REQUEST_CONTEXT="history.utils.get_request_context",
     ADMIN_ENABLED=True,
     SNAPSHOTS=True,
     MIGRATE_CONTEXT={},
     LOADDATA_CONTEXT={},
```

### Comparing `django-history-triggers-3.4.6/history/admin.py` & `django-history-triggers-3.4.7/history/admin.py`

 * *Files identical despite different names*

### Comparing `django-history-triggers-3.4.6/history/backends/__init__.py` & `django-history-triggers-3.4.7/history/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django-history-triggers-3.4.6/history/backends/base.py` & `django-history-triggers-3.4.7/history/backends/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 
     def get_models(self):
         return [
             model
             for model in apps.get_models(include_auto_created=True)
             if not issubclass(model, AbstractObjectHistory)
             and model._meta.app_label not in conf.IGNORE_APPS
+            and model._meta.label_lower not in conf.IGNORE_MODELS
             and (model._meta.managed or conf.INCLUDE_UNMANAGED)
         ]
 
     def session_fields(self):
         HistoryModel = get_history_model()
         auto_populated = [
             "id",
```

### Comparing `django-history-triggers-3.4.6/history/backends/postgres.py` & `django-history-triggers-3.4.7/history/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `django-history-triggers-3.4.6/history/backends/sqlite.py` & `django-history-triggers-3.4.7/history/backends/sqlite.py`

 * *Files identical despite different names*

### Comparing `django-history-triggers-3.4.6/history/management/commands/triggers.py` & `django-history-triggers-3.4.7/history/management/commands/triggers.py`

 * *Files identical despite different names*

### Comparing `django-history-triggers-3.4.6/history/middleware.py` & `django-history-triggers-3.4.7/history/middleware.py`

 * *Files identical despite different names*

### Comparing `django-history-triggers-3.4.6/history/migrations/0001_initial.py` & `django-history-triggers-3.4.7/history/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-history-triggers-3.4.6/history/models.py` & `django-history-triggers-3.4.7/history/models.py`

 * *Files identical despite different names*

### Comparing `django-history-triggers-3.4.6/history/templates/history/admin_history.html` & `django-history-triggers-3.4.7/history/templates/history/admin_history.html`

 * *Files identical despite different names*

### Comparing `django-history-triggers-3.4.6/history/templatetags/history.py` & `django-history-triggers-3.4.7/history/templatetags/history.py`

 * *Files identical despite different names*

### Comparing `django-history-triggers-3.4.6/history/utils.py` & `django-history-triggers-3.4.7/history/utils.py`

 * *Files identical despite different names*

### Comparing `django-history-triggers-3.4.6/setup.py` & `django-history-triggers-3.4.7/setup.py`

 * *Files identical despite different names*

