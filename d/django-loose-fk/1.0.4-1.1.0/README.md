# Comparing `tmp/django-loose-fk-1.0.4.tar.gz` & `tmp/django_loose_fk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-loose-fk-1.0.4.tar", last modified: Fri Apr  5 10:34:58 2024, max compression
+gzip compressed data, was "django_loose_fk-1.1.0.tar", last modified: Wed Apr 17 09:57:20 2024, max compression
```

## Comparing `django-loose-fk-1.0.4.tar` & `django_loose_fk-1.1.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.120771 django-loose-fk-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-05 10:34:58.120771 django-loose-fk-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.112771 django-loose-fk-1.0.4/django_loose_fk/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/drf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.116771 django-loose-fk-1.0.4/django_loose_fk/inspectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/inspectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/inspectors/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/inspectors/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/lookups.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/query_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/virtual_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.120771 django-loose-fk-1.0.4/django_loose_fk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-05 10:34:58.000000 django-loose-fk-1.0.4/django_loose_fk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-05 10:34:58.000000 django-loose-fk-1.0.4/django_loose_fk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:34:58.000000 django-loose-fk-1.0.4/django_loose_fk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:34:58.000000 django-loose-fk-1.0.4/django_loose_fk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-05 10:34:58.000000 django-loose-fk-1.0.4/django_loose_fk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 10:34:58.000000 django-loose-fk-1.0.4/django_loose_fk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-05 10:34:58.120771 django-loose-fk-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.116771 django-loose-fk-1.0.4/testapp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.116771 django-loose-fk-1.0.4/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/migrations/0002_auto_20220310_1612.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/migrations/0003_auto_20230705_0917.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.120771 django-loose-fk-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_api_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_chain_loose_fk.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_integrity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_is_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_model_field_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_model_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_querying.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_querylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_serializer_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_system_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.549281 django_loose_fk-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-17 09:57:20.549281 django_loose_fk-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.541281 django_loose_fk-1.1.0/django_loose_fk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/drf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.545281 django_loose_fk-1.1.0/django_loose_fk/inspectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/inspectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/inspectors/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/inspectors/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/lookups.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/query_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/virtual_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.549281 django_loose_fk-1.1.0/django_loose_fk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-17 09:57:20.000000 django_loose_fk-1.1.0/django_loose_fk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-17 09:57:20.000000 django_loose_fk-1.1.0/django_loose_fk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:57:20.000000 django_loose_fk-1.1.0/django_loose_fk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:57:20.000000 django_loose_fk-1.1.0/django_loose_fk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 09:57:20.000000 django_loose_fk-1.1.0/django_loose_fk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 09:57:20.000000 django_loose_fk-1.1.0/django_loose_fk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-17 09:57:20.549281 django_loose_fk-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.545281 django_loose_fk-1.1.0/testapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.545281 django_loose_fk-1.1.0/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/migrations/0002_auto_20220310_1612.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/migrations/0003_auto_20230705_0917.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.549281 django_loose_fk-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_api_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_chain_loose_fk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_is_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_model_field_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_model_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_querying.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_querylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_serializer_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_system_checks.py
```

### Comparing `django-loose-fk-1.0.4/CHANGELOG.rst` & `django_loose_fk-1.1.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+1.1.0 (2024-04-15)
+==================
+
+* Supported Django 4.2
+* Supported python 3.11
+* Dropped support of python 3.7, python 3.8, python 3.9
+
 1.0.4 (2024-04-05)
 ==================
 
 * Added setting ``LOOSE_FK_LOCAL_BASE_URLS``, which explicitly list allowed prefixes for
 local urls to fine-tune resolving local and remote urls, now they can be hosted within
 the same domain (#28).
```

### Comparing `django-loose-fk-1.0.4/LICENSE` & `django_loose_fk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/PKG-INFO` & `django_loose_fk-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: django-loose-fk
-Version: 1.0.4
+Version: 1.1.0
 Summary: Django Loose FK handles local or remote "ForeignKey" references.
 Home-page: https://github.com/maykinmedia/django-loose-fk
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Keywords: ForeignKey,URL reference,decentralization,integrity
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 Requires-Dist: django>=3.2
 Requires-Dist: djangorestframework>=3.11.0
 Requires-Dist: django-filter
 Requires-Dist: coreapi
 Provides-Extra: openapi
@@ -45,15 +44,15 @@
 Provides-Extra: release
 Requires-Dist: bump2version; extra == "release"
 
 ===============
 Django Loose FK
 ===============
 
-:Version: 1.0.4
+:Version: 1.1.0
 :Source: https://github.com/maykinmedia/django-loose-fk
 :Keywords: ``ForeignKey``, ``URL reference``, ``decentralization``, ``integrity``
 
 |build-status| |code-quality| |black| |coverage|
 
 |python-versions| |django-versions| |pypi-version|
 
@@ -77,15 +76,15 @@
 
 Installation
 ============
 
 Requirements
 ------------
 
-* Python 3.7 or above
+* Python 3.10 or above
 * setuptools 30.3.0 or above
 * Django 3.2 or newer
 
 
 Install
 -------
```

### Comparing `django-loose-fk-1.0.4/README.rst` & `django_loose_fk-1.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===============
 Django Loose FK
 ===============
 
-:Version: 1.0.4
+:Version: 1.1.0
 :Source: https://github.com/maykinmedia/django-loose-fk
 :Keywords: ``ForeignKey``, ``URL reference``, ``decentralization``, ``integrity``
 
 |build-status| |code-quality| |black| |coverage|
 
 |python-versions| |django-versions| |pypi-version|
 
@@ -30,15 +30,15 @@
 
 Installation
 ============
 
 Requirements
 ------------
 
-* Python 3.7 or above
+* Python 3.10 or above
 * setuptools 30.3.0 or above
 * Django 3.2 or newer
 
 
 Install
 -------
```

### Comparing `django-loose-fk-1.0.4/django_loose_fk/apps.py` & `django_loose_fk-1.1.0/django_loose_fk/apps.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/django_loose_fk/checks.py` & `django_loose_fk-1.1.0/django_loose_fk/checks.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/django_loose_fk/constraints.py` & `django_loose_fk-1.1.0/django_loose_fk/constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,13 +68,13 @@
         return check_constraint.remove_sql(model, schema_editor)
 
     def validate(self, model, instance, exclude=None, using=DEFAULT_DB_ALIAS):
         check_constraint = self._get_check_constraint(model)
         return check_constraint.validate(model, instance, exclude, using)
 
     def __repr__(self):
-        return "<%s: field=%r>" % (self.__class__.__name__, self.name)
+        return "<{}: field={!r}>".format(self.__class__.__name__, self.name)
 
     def __eq__(self, other):
         if isinstance(other, FkOrURLFieldConstraint):
             return self.name == other.name
         return super().__eq__(other)
```

### Comparing `django-loose-fk-1.0.4/django_loose_fk/drf.py` & `django_loose_fk-1.1.0/django_loose_fk/drf.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/django_loose_fk/fields.py` & `django_loose_fk-1.1.0/django_loose_fk/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         Uses deconstruct() to clone a new copy of this Field.
         Will not preserve any class attachments/attribute names.
         """
         name, path, args, kwargs = self.deconstruct()
         return self.__class__(*args, **kwargs)
 
     def deconstruct(self):
-        path = "%s.%s" % (self.__class__.__module__, self.__class__.__qualname__)
+        path = "{}.{}".format(self.__class__.__module__, self.__class__.__qualname__)
         keywords = {
             "fk_field": self.fk_field,
             "url_field": self.url_field,
             "blank": self.blank,
             "null": self.null,
         }
         return (self.name, path, [], keywords)
```

### Comparing `django-loose-fk-1.0.4/django_loose_fk/filters.py` & `django_loose_fk-1.1.0/django_loose_fk/filters.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/django_loose_fk/inspectors/fields.py` & `django_loose_fk-1.1.0/django_loose_fk/inspectors/fields.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/django_loose_fk/inspectors/query.py` & `django_loose_fk-1.1.0/django_loose_fk/inspectors/query.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/django_loose_fk/loaders.py` & `django_loose_fk-1.1.0/django_loose_fk/loaders.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/django_loose_fk/lookups.py` & `django_loose_fk-1.1.0/django_loose_fk/lookups.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,28 +137,28 @@
 
         if not fk_rhs_sql and not url_rhs_sql:
             raise EmptyResultSet()
 
         if fk_rhs_sql:
             fk_rhs_sql = self.get_rhs_op(connection, fk_rhs_sql)
             fk_sql = (
-                "%s %s" % (fk_lhs_sql, fk_rhs_sql),
+                "{} {}".format(fk_lhs_sql, fk_rhs_sql),
                 tuple(fk_params) + fk_rhs_params,
             )
 
         if url_rhs_sql:
             url_rhs_sql = self.get_rhs_op(connection, url_rhs_sql)
             url_sql = (
-                "%s %s" % (url_lhs_sql, url_rhs_sql),
+                "{} {}".format(url_lhs_sql, url_rhs_sql),
                 tuple(url_params) + url_rhs_params,
             )
 
         if not fk_rhs_sql:
             return url_sql
 
         if not url_rhs_sql:
             return fk_sql
 
         params = url_sql[1] + fk_sql[1]
-        sql = "(%s OR %s)" % (url_sql[0], fk_sql[0])
+        sql = "({} OR {})".format(url_sql[0], fk_sql[0])
 
         return sql, params
```

### Comparing `django-loose-fk-1.0.4/django_loose_fk/query_list.py` & `django_loose_fk-1.1.0/django_loose_fk/query_list.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/django_loose_fk/utils.py` & `django_loose_fk-1.1.0/django_loose_fk/utils.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/django_loose_fk/virtual_models.py` & `django_loose_fk-1.1.0/django_loose_fk/virtual_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     def __set__(self, instance: models.Model, value: List[DictOrUrl]):
         instance._loose_fk_data[self.field_name] = value
 
 
 class M2MHandler(BaseHandler):
     def __get__(self, instance, cls=None) -> QueryList:
         raw_data = instance._loose_fk_data.get(self.field_name, [])
-        assert all((isinstance(url, str) for url in raw_data))
+        assert all(isinstance(url, str) for url in raw_data)
 
         loaded_data = [
             self.loader.load(url=url, model=self.remote_model) for url in raw_data
         ]
 
         return QueryList(loaded_data)
```

### Comparing `django-loose-fk-1.0.4/django_loose_fk.egg-info/PKG-INFO` & `django_loose_fk-1.1.0/django_loose_fk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: django-loose-fk
-Version: 1.0.4
+Version: 1.1.0
 Summary: Django Loose FK handles local or remote "ForeignKey" references.
 Home-page: https://github.com/maykinmedia/django-loose-fk
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Keywords: ForeignKey,URL reference,decentralization,integrity
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 Requires-Dist: django>=3.2
 Requires-Dist: djangorestframework>=3.11.0
 Requires-Dist: django-filter
 Requires-Dist: coreapi
 Provides-Extra: openapi
@@ -45,15 +44,15 @@
 Provides-Extra: release
 Requires-Dist: bump2version; extra == "release"
 
 ===============
 Django Loose FK
 ===============
 
-:Version: 1.0.4
+:Version: 1.1.0
 :Source: https://github.com/maykinmedia/django-loose-fk
 :Keywords: ``ForeignKey``, ``URL reference``, ``decentralization``, ``integrity``
 
 |build-status| |code-quality| |black| |coverage|
 
 |python-versions| |django-versions| |pypi-version|
 
@@ -77,15 +76,15 @@
 
 Installation
 ============
 
 Requirements
 ------------
 
-* Python 3.7 or above
+* Python 3.10 or above
 * setuptools 30.3.0 or above
 * Django 3.2 or newer
 
 
 Install
 -------
```

### Comparing `django-loose-fk-1.0.4/django_loose_fk.egg-info/SOURCES.txt` & `django_loose_fk-1.1.0/django_loose_fk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/setup.cfg` & `django_loose_fk-1.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [metadata]
 name = django-loose-fk
-version = 1.0.4
+version = 1.1.0
 description = Django Loose FK handles local or remote "ForeignKey" references.
 long_description = file: README.rst
 url = https://github.com/maykinmedia/django-loose-fk
 license = MIT
 author = Maykin Media
 author_email = support@maykinmedia.nl
 keywords = ForeignKey, URL reference, decentralization, integrity
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 3.2
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	Operating System :: Unix
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires =
```

### Comparing `django-loose-fk-1.0.4/testapp/api.py` & `django_loose_fk-1.1.0/testapp/api.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/testapp/migrations/0001_initial.py` & `django_loose_fk-1.1.0/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/testapp/migrations/0002_auto_20220310_1612.py` & `django_loose_fk-1.1.0/testapp/migrations/0002_auto_20220310_1612.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/testapp/migrations/0003_auto_20230705_0917.py` & `django_loose_fk-1.1.0/testapp/migrations/0003_auto_20230705_0917.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/testapp/models.py` & `django_loose_fk-1.1.0/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/testapp/settings.py` & `django_loose_fk-1.1.0/testapp/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,7 +49,9 @@
         },
     }
 ]
 
 ROOT_URLCONF = "testapp.urls"
 
 ALLOWED_HOSTS = ["testserver.com"]
+
+USE_TZ = False
```

### Comparing `django-loose-fk-1.0.4/tests/test_api.py` & `django_loose_fk-1.1.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/tests/test_api_docs.py` & `django_loose_fk-1.1.0/tests/test_api_docs.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/tests/test_chain_loose_fk.py` & `django_loose_fk-1.1.0/tests/test_chain_loose_fk.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/tests/test_compare.py` & `django_loose_fk-1.1.0/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/tests/test_filter.py` & `django_loose_fk-1.1.0/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/tests/test_integrity.py` & `django_loose_fk-1.1.0/tests/test_integrity.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/tests/test_is_local.py` & `django_loose_fk-1.1.0/tests/test_is_local.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/tests/test_loaders.py` & `django_loose_fk-1.1.0/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/tests/test_model_field_interface.py` & `django_loose_fk-1.1.0/tests/test_model_field_interface.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/tests/test_querying.py` & `django_loose_fk-1.1.0/tests/test_querying.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/tests/test_querylist.py` & `django_loose_fk-1.1.0/tests/test_querylist.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/tests/test_serializer_field.py` & `django_loose_fk-1.1.0/tests/test_serializer_field.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.4/tests/test_system_checks.py` & `django_loose_fk-1.1.0/tests/test_system_checks.py`

 * *Files identical despite different names*

