# Comparing `tmp/xblock-drag-and-drop-v2-4.0.0.tar.gz` & `tmp/xblock_drag_and_drop_v2-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock-drag-and-drop-v2-4.0.0.tar", last modified: Fri Mar 22 15:15:17 2024, max compression
+gzip compressed data, was "xblock_drag_and_drop_v2-4.0.1.tar", last modified: Wed Apr 17 14:22:54 2024, max compression
```

## Comparing `xblock-drag-and-drop-v2-4.0.0.tar` & `xblock_drag_and_drop_v2-4.0.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.124832 xblock-drag-and-drop-v2-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    14429 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    36361 2024-03-22 15:15:17.124832 xblock-drag-and-drop-v2-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.116832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/default_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    52941 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/drag_and_drop_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.112832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.116832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/css/
--rw-r--r--   0 runner    (1001) docker     (127)    19803 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/css/drag_and_drop.css
--rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/css/drag_and_drop_edit.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.116832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/img/
--rw-r--r--   0 runner    (1001) docker     (127)    34942 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/img/triangle.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.116832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/
--rw-r--r--   0 runner    (1001) docker     (127)    87120 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/drag_and_drop.js
--rw-r--r--   0 runner    (1001) docker     (127)    41638 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/drag_and_drop_edit.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.112832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.116832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/ar/
--rw-r--r--   0 runner    (1001) docker     (127)    39006 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/ar/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.116832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/de/
--rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/de/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.116832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/en/
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/en/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.116832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/eo/
--rw-r--r--   0 runner    (1001) docker     (127)    64209 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/eo/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.116832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/es_419/
--rw-r--r--   0 runner    (1001) docker     (127)    20270 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/es_419/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.116832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/fr/
--rw-r--r--   0 runner    (1001) docker     (127)    19590 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/fr/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.116832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/he/
--rw-r--r--   0 runner    (1001) docker     (127)    22437 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/he/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/hi/
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/hi/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/it/
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/it/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/ja/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/ja/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/ko/
--rw-r--r--   0 runner    (1001) docker     (127)    22577 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/ko/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/nl/
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/nl/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/pl/
--rw-r--r--   0 runner    (1001) docker     (127)    16851 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/pl/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/pt_BR/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/pt_PT/
--rw-r--r--   0 runner    (1001) docker     (127)    18514 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/pt_PT/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/ru/
--rw-r--r--   0 runner    (1001) docker     (127)    37990 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/ru/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/tr/
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/tr/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/zh_CN/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)    84693 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/vendor/handlebars-v1.1.2.js
--rw-r--r--   0 runner    (1001) docker     (127)    16608 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/vendor/virtual-dom-1.3.0.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/themes/
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/themes/apros.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.112832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/templates/html/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/templates/html/drag_and_drop.html
--rw-r--r--   0 runner    (1001) docker     (127)    16156 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/templates/html/drag_and_drop_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     7944 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/templates/html/js_templates.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/translations/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/translations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/translations/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/translations/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.120832 xblock-drag-and-drop-v2-4.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 15:15:17.124832 xblock-drag-and-drop-v2-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-03-22 15:15:10.000000 xblock-drag-and-drop-v2-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:17.124832 xblock-drag-and-drop-v2-4.0.0/xblock_drag_and_drop_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    36361 2024-03-22 15:15:17.000000 xblock-drag-and-drop-v2-4.0.0/xblock_drag_and_drop_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-22 15:15:17.000000 xblock-drag-and-drop-v2-4.0.0/xblock_drag_and_drop_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 15:15:17.000000 xblock-drag-and-drop-v2-4.0.0/xblock_drag_and_drop_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 15:15:17.000000 xblock-drag-and-drop-v2-4.0.0/xblock_drag_and_drop_v2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-22 15:15:17.000000 xblock-drag-and-drop-v2-4.0.0/xblock_drag_and_drop_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-22 15:15:17.000000 xblock-drag-and-drop-v2-4.0.0/xblock_drag_and_drop_v2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.383024 xblock_drag_and_drop_v2-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    36561 2024-04-17 14:22:54.383024 xblock_drag_and_drop_v2-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.375023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/default_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52941 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/drag_and_drop_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.375023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.375023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    19803 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/css/drag_and_drop.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/css/drag_and_drop_edit.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.375023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    34942 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/img/triangle.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    87120 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/drag_and_drop.js
+-rw-r--r--   0 runner    (1001) docker     (127)    41638 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/drag_and_drop_edit.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.375023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/ar/
+-rw-r--r--   0 runner    (1001) docker     (127)    39006 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/ar/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/de/
+-rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/de/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/en/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/eo/
+-rw-r--r--   0 runner    (1001) docker     (127)    64209 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/eo/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/es_419/
+-rw-r--r--   0 runner    (1001) docker     (127)    20270 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/es_419/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)    19590 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/fr/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/he/
+-rw-r--r--   0 runner    (1001) docker     (127)    22437 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/he/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/hi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/hi/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/it/
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/it/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/ja/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/ko/
+-rw-r--r--   0 runner    (1001) docker     (127)    22577 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/ko/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/nl/
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/nl/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/pl/
+-rw-r--r--   0 runner    (1001) docker     (127)    16851 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/pl/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/pt_BR/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/pt_PT/
+-rw-r--r--   0 runner    (1001) docker     (127)    18514 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/pt_PT/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)    37990 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/ru/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/tr/
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/tr/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/zh_CN/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)    84693 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/vendor/handlebars-v1.1.2.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16608 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/vendor/virtual-dom-1.3.0.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.379023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/themes/apros.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.375023 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.383024 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/templates/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/templates/html/drag_and_drop.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16156 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/templates/html/drag_and_drop_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7944 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/templates/html/js_templates.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.383024 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/translations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/translations/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/translations/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.383024 xblock_drag_and_drop_v2-4.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 14:22:54.383024 xblock_drag_and_drop_v2-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-17 14:22:40.000000 xblock_drag_and_drop_v2-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:22:54.383024 xblock_drag_and_drop_v2-4.0.1/xblock_drag_and_drop_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    36561 2024-04-17 14:22:54.000000 xblock_drag_and_drop_v2-4.0.1/xblock_drag_and_drop_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-17 14:22:54.000000 xblock_drag_and_drop_v2-4.0.1/xblock_drag_and_drop_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:22:54.000000 xblock_drag_and_drop_v2-4.0.1/xblock_drag_and_drop_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 14:22:54.000000 xblock_drag_and_drop_v2-4.0.1/xblock_drag_and_drop_v2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 14:22:54.000000 xblock_drag_and_drop_v2-4.0.1/xblock_drag_and_drop_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 14:22:54.000000 xblock_drag_and_drop_v2-4.0.1/xblock_drag_and_drop_v2.egg-info/top_level.txt
```

### Comparing `xblock-drag-and-drop-v2-4.0.0/Changelog.md` & `xblock_drag_and_drop_v2-4.0.1/Changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Drag and Drop XBlock changelog
 ==============================
 
 Unreleased
 ---------------------------
 
+Version 4.0.1 (2024-04-17)
+--------------------------
+
+* Add Python 3.11 support.
+* Add Python 3.12 support.
+* Drop Django 3.2 support.
+
 Version 4.0.0 (2024-03-12)
 --------------------------
 
 * Remove Transifex calls and bundled translation files for the OEP-58 proposal.
 
   BREAKING CHANGE: This version removes translations for Quince and earlier releases.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_pasv2l6u_/tmp46q67um4_TarContainer/0/1.md", line 385, column 0: CDATA terminal not found*

```diff
@@ -1,30 +1,31 @@
 Drag and Drop XBlock changelog ============================== Unreleased ------
---------------------- Version 4.0.0 (2024-03-12) -------------------------- *
-Remove Transifex calls and bundled translation files for the OEP-58 proposal.
-BREAKING CHANGE: This version removes translations for Quince and earlier
-releases. Version 3.4.0 (2024-01-15) --------------------------- *
-XBlockI18NService js translations support Version 3.3.0 (2023-10-24) ----------
------------------ * Removed xblock-utils package * Replace `xblockutils.*`
-imports with `xblock.utils.*`. The old imports are used as a fallback for
-compatibility with older releases. * Removed bok-choy package along with all
-integration tests. Version 3.2.2 (2023-10-19) --------------------------- * Fix
-Safari focus when there are no draggables left. Version 3.2.1 (2023-10-12) ----
------------------------ * Added support for Django 4.2 * The command `make
-extract_translations` now uses `msgcat` instead of `tail` to combine `djangojs-
-partial.po` into `django.po`. This is to avoid the possibility of having
-message compilation failure because of duplicate strings (strings shared
-between both files) Version 3.2.0 (2023-04-20) --------------------------- *
-Use the `replace_urls` service instead of a runtime property. BREAKING CHANGE:
-This version is no longer compatible with Maple. Version 3.1.3 (2023-04-15) ---
------------------------ * Prepare repository for upcoming changes related to
-[openedx-translations](https://github.com/openedx/openedx-translations). *
-`conf/locale` directory is now the source of truth for translations. *
-`translations` directory is now a symbolic link for backwards compatibility. *
-`locale` symbolic link is deleted to avoid too many symbolic links. * `en`
-translations are now extracted into `django.po` instead of `text.po`. * `en`
-`text.po` is now a symbolic link to `django.po` for backwards compatibility.
-Version 3.1.0 (2023-01-31) -------------------------- * Upgrade to be
-compatible with `bleach==6.0.0` and `bleach<6.0.0` * Make the dependency on the
-`css` extras explicit. Version 3.0.0 (2022-11-18) --------------------------- *
-Sanitize HTML tags to prevent XSS vulnerabilities. BREAKING CHANGE: Disallowed
-HTML tags (e.g. `
+--------------------- Version 4.0.1 (2024-04-17) -------------------------- *
+Add Python 3.11 support. * Add Python 3.12 support. * Drop Django 3.2 support.
+Version 4.0.0 (2024-03-12) -------------------------- * Remove Transifex calls
+and bundled translation files for the OEP-58 proposal. BREAKING CHANGE: This
+version removes translations for Quince and earlier releases. Version 3.4.0
+(2024-01-15) --------------------------- * XBlockI18NService js translations
+support Version 3.3.0 (2023-10-24) --------------------------- * Removed
+xblock-utils package * Replace `xblockutils.*` imports with `xblock.utils.*`.
+The old imports are used as a fallback for compatibility with older releases. *
+Removed bok-choy package along with all integration tests. Version 3.2.2 (2023-
+10-19) --------------------------- * Fix Safari focus when there are no
+draggables left. Version 3.2.1 (2023-10-12) --------------------------- * Added
+support for Django 4.2 * The command `make extract_translations` now uses
+`msgcat` instead of `tail` to combine `djangojs-partial.po` into `django.po`.
+This is to avoid the possibility of having message compilation failure because
+of duplicate strings (strings shared between both files) Version 3.2.0 (2023-
+04-20) --------------------------- * Use the `replace_urls` service instead of
+a runtime property. BREAKING CHANGE: This version is no longer compatible with
+Maple. Version 3.1.3 (2023-04-15) -------------------------- * Prepare
+repository for upcoming changes related to [openedx-translations](https://
+github.com/openedx/openedx-translations). * `conf/locale` directory is now the
+source of truth for translations. * `translations` directory is now a symbolic
+link for backwards compatibility. * `locale` symbolic link is deleted to avoid
+too many symbolic links. * `en` translations are now extracted into `django.po`
+instead of `text.po`. * `en` `text.po` is now a symbolic link to `django.po`
+for backwards compatibility. Version 3.1.0 (2023-01-31) -----------------------
+--- * Upgrade to be compatible with `bleach==6.0.0` and `bleach<6.0.0` * Make
+the dependency on the `css` extras explicit. Version 3.0.0 (2022-11-18) -------
+-------------------- * Sanitize HTML tags to prevent XSS vulnerabilities.
+BREAKING CHANGE: Disallowed HTML tags (e.g. `
```

### Comparing `xblock-drag-and-drop-v2-4.0.0/LICENSE` & `xblock_drag_and_drop_v2-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/PKG-INFO` & `xblock_drag_and_drop_v2-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: xblock-drag-and-drop-v2
-Version: 4.0.0
+Version: 4.0.1
 Summary: XBlock - Drag-and-Drop v2
 Home-page: https://github.com/openedx/xblock-drag-and-drop-v2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: XBlock[django]
 Requires-Dist: bleach[css]
 Requires-Dist: django-statici18n
@@ -576,14 +577,21 @@
 
 Drag and Drop XBlock changelog
 ==============================
 
 Unreleased
 ---------------------------
 
+Version 4.0.1 (2024-04-17)
+--------------------------
+
+* Add Python 3.11 support.
+* Add Python 3.12 support.
+* Drop Django 3.2 support.
+
 Version 4.0.0 (2024-03-12)
 --------------------------
 
 * Remove Transifex calls and bundled translation files for the OEP-58 proposal.
 
   BREAKING CHANGE: This version removes translations for Quince and earlier releases.
```

### Comparing `xblock-drag-and-drop-v2-4.0.0/README.md` & `xblock_drag_and_drop_v2-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/compat.py` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/compat.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/default_data.py` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/default_data.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/drag_and_drop_v2.py` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/drag_and_drop_v2.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/css/drag_and_drop.css` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/css/drag_and_drop.css`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/css/drag_and_drop_edit.css` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/css/drag_and_drop_edit.css`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/img/triangle.png` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/img/triangle.png`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/drag_and_drop.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/drag_and_drop.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/drag_and_drop_edit.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/drag_and_drop_edit.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/ar/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/ar/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/de/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/de/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/en/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/en/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/eo/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/eo/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/es_419/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/es_419/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/fr/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/fr/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/he/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/he/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/hi/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/hi/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/it/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/it/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/ja/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/ja/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/ko/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/ko/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/nl/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/nl/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/pl/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/pl/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/pt_BR/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/pt_BR/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/pt_PT/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/pt_PT/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/ru/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/ru/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/tr/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/tr/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/translations/zh_CN/text.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/translations/zh_CN/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/vendor/handlebars-v1.1.2.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/vendor/handlebars-v1.1.2.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/js/vendor/virtual-dom-1.3.0.min.js` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/js/vendor/virtual-dom-1.3.0.min.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/public/themes/apros.css` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/public/themes/apros.css`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/templates/html/drag_and_drop_edit.html` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/templates/html/drag_and_drop_edit.html`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/templates/html/js_templates.html` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/templates/html/js_templates.html`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/translations/settings.py` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/translations/settings.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/drag_and_drop_v2/utils.py` & `xblock_drag_and_drop_v2-4.0.1/drag_and_drop_v2/utils.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-4.0.0/setup.py` & `xblock_drag_and_drop_v2-4.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,16 +114,17 @@
     version=VERSION,
     description='XBlock - Drag-and-Drop v2',
     long_description=README + '\n\n' + CHANGELOG,
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.2',
     ],
     url='https://github.com/openedx/xblock-drag-and-drop-v2',
     install_requires=load_requirements('requirements/base.in'),
     entry_points={
         'xblock.v1': 'drag-and-drop-v2 = drag_and_drop_v2:DragAndDropBlock',
     },
```

### Comparing `xblock-drag-and-drop-v2-4.0.0/xblock_drag_and_drop_v2.egg-info/PKG-INFO` & `xblock_drag_and_drop_v2-4.0.1/xblock_drag_and_drop_v2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: xblock-drag-and-drop-v2
-Version: 4.0.0
+Version: 4.0.1
 Summary: XBlock - Drag-and-Drop v2
 Home-page: https://github.com/openedx/xblock-drag-and-drop-v2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: XBlock[django]
 Requires-Dist: bleach[css]
 Requires-Dist: django-statici18n
@@ -576,14 +577,21 @@
 
 Drag and Drop XBlock changelog
 ==============================
 
 Unreleased
 ---------------------------
 
+Version 4.0.1 (2024-04-17)
+--------------------------
+
+* Add Python 3.11 support.
+* Add Python 3.12 support.
+* Drop Django 3.2 support.
+
 Version 4.0.0 (2024-03-12)
 --------------------------
 
 * Remove Transifex calls and bundled translation files for the OEP-58 proposal.
 
   BREAKING CHANGE: This version removes translations for Quince and earlier releases.
```

### Comparing `xblock-drag-and-drop-v2-4.0.0/xblock_drag_and_drop_v2.egg-info/SOURCES.txt` & `xblock_drag_and_drop_v2-4.0.1/xblock_drag_and_drop_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

