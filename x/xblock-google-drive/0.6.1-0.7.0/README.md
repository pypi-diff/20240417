# Comparing `tmp/xblock-google-drive-0.6.1.tar.gz` & `tmp/xblock_google_drive-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock-google-drive-0.6.1.tar", last modified: Tue Jan 23 09:13:49 2024, max compression
+gzip compressed data, was "xblock_google_drive-0.7.0.tar", last modified: Wed Apr 17 15:29:38 2024, max compression
```

## Comparing `xblock-google-drive-0.6.1.tar` & `xblock_google_drive-0.7.0.tar`

### file list

```diff
@@ -1,82 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.114163 xblock-google-drive-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-01-23 09:13:49.114163 xblock-google-drive-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.106162 xblock-google-drive-0.6.1/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.102162 xblock-google-drive-0.6.1/google_drive/conf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.106162 xblock-google-drive-0.6.1/google_drive/conf/locale/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/conf/locale/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.102162 xblock-google-drive-0.6.1/google_drive/conf/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.106162 xblock-google-drive-0.6.1/google_drive/conf/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/conf/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/conf/locale/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.102162 xblock-google-drive-0.6.1/google_drive/conf/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.106162 xblock-google-drive-0.6.1/google_drive/conf/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/conf/locale/eo/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)     7968 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/conf/locale/eo/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.102162 xblock-google-drive-0.6.1/google_drive/conf/locale/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.106162 xblock-google-drive-0.6.1/google_drive/conf/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/conf/locale/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/conf/locale/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.102162 xblock-google-drive-0.6.1/google_drive/conf/locale/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.110162 xblock-google-drive-0.6.1/google_drive/conf/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/conf/locale/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/conf/locale/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.102162 xblock-google-drive-0.6.1/google_drive/conf/locale/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.110162 xblock-google-drive-0.6.1/google_drive/conf/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/conf/locale/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/conf/locale/ja_JP/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/google_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/google_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.106162 xblock-google-drive-0.6.1/google_drive/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.110162 xblock-google-drive-0.6.1/google_drive/public/css/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/public/css/google_calendar.css
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/public/css/google_docs.css
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/public/css/google_edit.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.110162 xblock-google-drive-0.6.1/google_drive/public/js/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/public/js/google_calendar.js
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/public/js/google_calendar_edit.js
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/public/js/google_docs.js
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/public/js/google_docs_edit.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.106162 xblock-google-drive-0.6.1/google_drive/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.110162 xblock-google-drive-0.6.1/google_drive/templates/html/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/templates/html/google_calendar.html
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/templates/html/google_calendar_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/templates/html/google_docs.html
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/templates/html/google_docs_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.110162 xblock-google-drive-0.6.1/google_drive/translations/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.106162 xblock-google-drive-0.6.1/google_drive/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.110162 xblock-google-drive-0.6.1/google_drive/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/translations/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.106162 xblock-google-drive-0.6.1/google_drive/translations/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.110162 xblock-google-drive-0.6.1/google_drive/translations/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/translations/eo/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)     7968 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/translations/eo/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.106162 xblock-google-drive-0.6.1/google_drive/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.110162 xblock-google-drive-0.6.1/google_drive/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.106162 xblock-google-drive-0.6.1/google_drive/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.110162 xblock-google-drive-0.6.1/google_drive/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.106162 xblock-google-drive-0.6.1/google_drive/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.114163 xblock-google-drive-0.6.1/google_drive/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/google_drive/translations/ja_JP/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.114163 xblock-google-drive-0.6.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-23 09:13:49.114163 xblock-google-drive-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-01-23 09:13:45.000000 xblock-google-drive-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 09:13:49.114163 xblock-google-drive-0.6.1/xblock_google_drive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-01-23 09:13:49.000000 xblock-google-drive-0.6.1/xblock_google_drive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-01-23 09:13:49.000000 xblock-google-drive-0.6.1/xblock_google_drive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 09:13:49.000000 xblock-google-drive-0.6.1/xblock_google_drive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-23 09:13:49.000000 xblock-google-drive-0.6.1/xblock_google_drive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-23 09:13:49.000000 xblock-google-drive-0.6.1/xblock_google_drive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-23 09:13:49.000000 xblock-google-drive-0.6.1/xblock_google_drive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:29:38.135052 xblock_google_drive-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-04-17 15:29:38.135052 xblock_google_drive-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:29:38.131052 xblock_google_drive-0.7.0/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:29:38.127052 xblock_google_drive-0.7.0/google_drive/conf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:29:38.131052 xblock_google_drive-0.7.0/google_drive/conf/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/conf/locale/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/google_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/google_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:29:38.127052 xblock_google_drive-0.7.0/google_drive/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:29:38.131052 xblock_google_drive-0.7.0/google_drive/public/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/public/css/google_calendar.css
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/public/css/google_docs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/public/css/google_edit.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:29:38.131052 xblock_google_drive-0.7.0/google_drive/public/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/public/js/google_calendar.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/public/js/google_calendar_edit.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/public/js/google_docs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/public/js/google_docs_edit.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:29:38.127052 xblock_google_drive-0.7.0/google_drive/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:29:38.131052 xblock_google_drive-0.7.0/google_drive/templates/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/templates/html/google_calendar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/templates/html/google_calendar_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/templates/html/google_docs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/templates/html/google_docs_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:29:38.131052 xblock_google_drive-0.7.0/google_drive/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/google_drive/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:29:38.131052 xblock_google_drive-0.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-17 15:29:38.135052 xblock_google_drive-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-17 15:29:34.000000 xblock_google_drive-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:29:38.135052 xblock_google_drive-0.7.0/xblock_google_drive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-04-17 15:29:38.000000 xblock_google_drive-0.7.0/xblock_google_drive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-17 15:29:38.000000 xblock_google_drive-0.7.0/xblock_google_drive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:29:38.000000 xblock_google_drive-0.7.0/xblock_google_drive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-17 15:29:38.000000 xblock_google_drive-0.7.0/xblock_google_drive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 15:29:38.000000 xblock_google_drive-0.7.0/xblock_google_drive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 15:29:38.000000 xblock_google_drive-0.7.0/xblock_google_drive.egg-info/top_level.txt
```

### Comparing `xblock-google-drive-0.6.1/LICENSE` & `xblock_google_drive-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.6.1/PKG-INFO` & `xblock_google_drive-0.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: xblock-google-drive
-Version: 0.6.1
+Version: 0.7.0
 Summary: An XBlock which allows embedding of Google documents and calendar within an edX course
 Home-page: https://github.com/openedx/xblock-google-drive
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Django
 Requires-Dist: XBlock[django]
 Requires-Dist: requests
@@ -90,44 +91,14 @@
     $ make coverage
 
 If you have not installed the xblock-sdk in the active virtualenv, you
 might also have to prepend ``PYTHONPATH=".:/path/to/xblock"`` to the
 command above. (``/path/to/xblock`` is the path to the xblock-sdk, where
 the workbench resides).
 
-Working with translations
--------------------------
-
-For information about working with translations, see the `Internationalization Support`_ section of
-the `Open edX XBlock Tutorial`_.
-
-Prepare your virtualenv and ensure that the `Transifex authentication file`_
-(``~/.transifexrc``) is properly set up.
-
-Push new strings to Transifex:
-
-.. code:: bash
-
-    $ make push_translations
-
-
-To get the latest translations from Transifex:
-
-.. code:: bash
-
-    $ make pull_translations
-
-
-For testing purposes it's faster to avoid Transifex and work on dummy Esperanto translations:
-
-.. code:: bash
-
-    $ make build_dummy_translations
-
-
 .. _Internationalization Support: http://edx.readthedocs.io/projects/xblock-tutorial/en/latest/edx_platform/edx_lms.html#internationalization-support
 .. _Open edX XBlock Tutorial: https://xblock-tutorial.readthedocs.io/en/latest/
 .. _Transifex authentication file: https://openedx.atlassian.net/wiki/display/OpenOPS/Running+Fullstack
 
 Changes to be documented
 ------------------------
```

### Comparing `xblock-google-drive-0.6.1/README.rst` & `xblock_google_drive-0.7.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -73,44 +73,14 @@
     $ make coverage
 
 If you have not installed the xblock-sdk in the active virtualenv, you
 might also have to prepend ``PYTHONPATH=".:/path/to/xblock"`` to the
 command above. (``/path/to/xblock`` is the path to the xblock-sdk, where
 the workbench resides).
 
-Working with translations
--------------------------
-
-For information about working with translations, see the `Internationalization Support`_ section of
-the `Open edX XBlock Tutorial`_.
-
-Prepare your virtualenv and ensure that the `Transifex authentication file`_
-(``~/.transifexrc``) is properly set up.
-
-Push new strings to Transifex:
-
-.. code:: bash
-
-    $ make push_translations
-
-
-To get the latest translations from Transifex:
-
-.. code:: bash
-
-    $ make pull_translations
-
-
-For testing purposes it's faster to avoid Transifex and work on dummy Esperanto translations:
-
-.. code:: bash
-
-    $ make build_dummy_translations
-
-
 .. _Internationalization Support: http://edx.readthedocs.io/projects/xblock-tutorial/en/latest/edx_platform/edx_lms.html#internationalization-support
 .. _Open edX XBlock Tutorial: https://xblock-tutorial.readthedocs.io/en/latest/
 .. _Transifex authentication file: https://openedx.atlassian.net/wiki/display/OpenOPS/Running+Fullstack
 
 Changes to be documented
 ------------------------
```

### Comparing `xblock-google-drive-0.6.1/google_drive/google_calendar.py` & `xblock_google_drive-0.7.0/google_drive/google_calendar.py`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.6.1/google_drive/google_docs.py` & `xblock_google_drive-0.7.0/google_drive/google_docs.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,28 +138,28 @@
 
         return {
             'result': 'success',
         }
 
     # suffix argument is specified for xblocks, but we are not using herein
     @XBlock.json_handler
-    def check_url(self, data, suffix=''):  # pylint: disable=unused-argument,no-self-use
+    def check_url(self, data, suffix=''):  # pylint: disable=unused-argument
         """
         Checks that the given document url is accessible, and therefore assumed to be valid
         """
         try:
             test_url = data['url']
         except KeyError as ex:
             LOG.debug("URL not provided - %s", six.text_type(ex))
             return {
                 'status_code': 400,
             }
 
         try:
-            url_response = requests.head(test_url)
+            url_response = requests.head(test_url)  # pylint: disable=missing-timeout
         # Catch wide range of request exceptions
         except requests.exceptions.RequestException as ex:
             LOG.debug("Unable to connect to %s - %s", test_url, six.text_type(ex))
             return {
                 'status_code': 400,
             }
```

### Comparing `xblock-google-drive-0.6.1/google_drive/public/css/google_edit.css` & `xblock_google_drive-0.7.0/google_drive/public/css/google_edit.css`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.6.1/google_drive/public/js/google_calendar.js` & `xblock_google_drive-0.7.0/google_drive/public/js/google_calendar.js`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.6.1/google_drive/public/js/google_calendar_edit.js` & `xblock_google_drive-0.7.0/google_drive/public/js/google_calendar_edit.js`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.6.1/google_drive/public/js/google_docs.js` & `xblock_google_drive-0.7.0/google_drive/public/js/google_docs.js`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.6.1/google_drive/public/js/google_docs_edit.js` & `xblock_google_drive-0.7.0/google_drive/public/js/google_docs_edit.js`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.6.1/google_drive/templates/html/google_calendar_edit.html` & `xblock_google_drive-0.7.0/google_drive/templates/html/google_calendar_edit.html`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.6.1/google_drive/templates/html/google_docs_edit.html` & `xblock_google_drive-0.7.0/google_drive/templates/html/google_docs_edit.html`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.6.1/requirements/constraints.txt` & `xblock_google_drive-0.7.0/requirements/constraints.txt`

 * *Files 17% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 # When pinning something here, please provide an explanation of why.  Ideally,
 # link to other information that will help people in the future to remove the
 # pin when possible.  Writing an issue against the offending project and
 # linking to it here is good.
 
 -c common_constraints.txt
 
-# TODO: Many pinned dependencies should be unpinned and/or moved to this constraints file.
-pylint==2.12.2
+# Temporary to Support the python 3.11 Upgrade
+backports.zoneinfo;python_version<"3.9"  # Newer versions have zoneinfo available in the standard library
```

### Comparing `xblock-google-drive-0.6.1/setup.py` & `xblock_google_drive-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,16 +111,17 @@
     version=VERSION,
     description='An XBlock which allows embedding of Google documents and calendar within an edX course',
     long_description=README,
     long_description_content_type='text/x-rst',
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.2',
     ],
     url='https://github.com/openedx/xblock-google-drive',
     install_requires=load_requirements('requirements/base.in'),
     entry_points={
         'xblock.v1': [
             'google-document = google_drive:GoogleDocumentBlock',
```

### Comparing `xblock-google-drive-0.6.1/xblock_google_drive.egg-info/PKG-INFO` & `xblock_google_drive-0.7.0/xblock_google_drive.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: xblock-google-drive
-Version: 0.6.1
+Version: 0.7.0
 Summary: An XBlock which allows embedding of Google documents and calendar within an edX course
 Home-page: https://github.com/openedx/xblock-google-drive
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Django
 Requires-Dist: XBlock[django]
 Requires-Dist: requests
@@ -90,44 +91,14 @@
     $ make coverage
 
 If you have not installed the xblock-sdk in the active virtualenv, you
 might also have to prepend ``PYTHONPATH=".:/path/to/xblock"`` to the
 command above. (``/path/to/xblock`` is the path to the xblock-sdk, where
 the workbench resides).
 
-Working with translations
--------------------------
-
-For information about working with translations, see the `Internationalization Support`_ section of
-the `Open edX XBlock Tutorial`_.
-
-Prepare your virtualenv and ensure that the `Transifex authentication file`_
-(``~/.transifexrc``) is properly set up.
-
-Push new strings to Transifex:
-
-.. code:: bash
-
-    $ make push_translations
-
-
-To get the latest translations from Transifex:
-
-.. code:: bash
-
-    $ make pull_translations
-
-
-For testing purposes it's faster to avoid Transifex and work on dummy Esperanto translations:
-
-.. code:: bash
-
-    $ make build_dummy_translations
-
-
 .. _Internationalization Support: http://edx.readthedocs.io/projects/xblock-tutorial/en/latest/edx_platform/edx_lms.html#internationalization-support
 .. _Open edX XBlock Tutorial: https://xblock-tutorial.readthedocs.io/en/latest/
 .. _Transifex authentication file: https://openedx.atlassian.net/wiki/display/OpenOPS/Running+Fullstack
 
 Changes to be documented
 ------------------------
```

