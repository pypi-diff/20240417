# Comparing `tmp/gloe-0.5.5.tar.gz` & `tmp/gloe-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gloe-0.5.5.tar", last modified: Mon Apr 15 20:24:08 2024, max compression
+gzip compressed data, was "gloe-0.5.6.tar", last modified: Tue Apr 16 22:39:19 2024, max compression
```

## Comparing `gloe-0.5.5.tar` & `gloe-0.5.6.tar`

### file list

```diff
@@ -1,89 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.482239 gloe-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-15 20:23:57.000000 gloe-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-15 20:23:57.000000 gloe-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-15 20:24:08.482239 gloe-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-15 20:23:57.000000 gloe-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.466239 gloe-0.5.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.470239 gloe-0.5.5/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.470239 gloe-0.5.5/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.470239 gloe-0.5.5/docs/source/_static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_static/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_static/assets/gloe-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_static/assets/gloe-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_static/assets/graph_example.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_static/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_static/theme_customs.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.470239 gloe-0.5.5/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.474238 gloe-0.5.5/docs/source/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/api-reference/gloe.collection.md
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/api-reference/gloe.experimental.md
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/api-reference/gloe.utils.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/docutils.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.474238 gloe-0.5.5/docs/source/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/async-transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/conditional-flows.md
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/ensurers.md
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/partial-transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/plotting.md
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/utilities.md
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/limitations.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.474238 gloe-0.5.5/docs/source/pygments/
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/pygments/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/theory.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.474238 gloe-0.5.5/gloe/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/_composition_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/_transformer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/_typing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/async_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13736 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/base_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.478238 gloe-0.5.5/gloe/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/collection/_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/collection/_mapover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.478238 gloe-0.5.5/gloe/conditional/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/conditional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/conditional/_conditioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.478238 gloe-0.5.5/gloe/ensurer/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/ensurer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/ensurer/_transformer_ensurer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.478238 gloe-0.5.5/gloe/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.478238 gloe-0.5.5/gloe/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/experimental/_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.482239 gloe-0.5.5/gloe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-15 20:24:08.000000 gloe-0.5.5/gloe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-15 20:24:08.000000 gloe-0.5.5/gloe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:24:08.000000 gloe-0.5.5/gloe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 20:24:08.000000 gloe-0.5.5/gloe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 20:24:08.000000 gloe-0.5.5/gloe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-15 20:23:57.000000 gloe-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:24:08.482239 gloe-0.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.482239 gloe-0.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.482239 gloe-0.5.5/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/lib/conditioners.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/lib/ensurers.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/lib/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_async_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_conditioner_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_transformer_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_transformer_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_transformer_ensurer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_transformer_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_transformer_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_transformer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.054177 gloe-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-16 22:39:12.000000 gloe-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 22:39:12.000000 gloe-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-16 22:39:19.054177 gloe-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-16 22:39:12.000000 gloe-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.038177 gloe-0.5.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.042177 gloe-0.5.6/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.042177 gloe-0.5.6/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.042177 gloe-0.5.6/docs/source/_static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/_static/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/_static/assets/gloe-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/_static/assets/gloe-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/_static/assets/graph_example.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/_static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/_static/theme_customs.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.042177 gloe-0.5.6/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.042177 gloe-0.5.6/docs/source/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/api-reference/gloe.collection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/api-reference/gloe.experimental.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/api-reference/gloe.utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/docutils.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.046177 gloe-0.5.6/docs/source/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/getting-started/async-transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/getting-started/conditional-flows.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/getting-started/ensurers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/getting-started/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/getting-started/partial-transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/getting-started/plotting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/getting-started/transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/getting-started/utilities.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/limitations.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.046177 gloe-0.5.6/docs/source/pygments/
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/pygments/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-16 22:39:12.000000 gloe-0.5.6/docs/source/theory.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.046177 gloe-0.5.6/gloe/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/_composition_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/_generic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/_plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/_supports_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/_transformer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/_typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/async_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15038 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/base_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.050177 gloe-0.5.6/gloe/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/collection/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/collection/_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/collection/_mapover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.050177 gloe-0.5.6/gloe/conditional/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/conditional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/conditional/_conditioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.050177 gloe-0.5.6/gloe/ensurer/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/ensurer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/ensurer/_transformer_ensurer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.050177 gloe-0.5.6/gloe/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.050177 gloe-0.5.6/gloe/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/experimental/_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 22:39:12.000000 gloe-0.5.6/gloe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.054177 gloe-0.5.6/gloe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-16 22:39:19.000000 gloe-0.5.6/gloe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-16 22:39:19.000000 gloe-0.5.6/gloe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:39:19.000000 gloe-0.5.6/gloe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 22:39:19.000000 gloe-0.5.6/gloe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 22:39:19.000000 gloe-0.5.6/gloe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-16 22:39:12.000000 gloe-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:39:19.054177 gloe-0.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.054177 gloe-0.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:39:19.054177 gloe-0.5.6/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/lib/conditioners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/lib/ensurers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/lib/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/test_async_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/test_conditioner_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/test_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/test_transformer_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/test_transformer_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/test_transformer_ensurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/test_transformer_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/test_transformer_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-16 22:39:12.000000 gloe-0.5.6/tests/test_transformer_utils.py
```

### Comparing `gloe-0.5.5/LICENSE` & `gloe-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/PKG-INFO` & `gloe-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gloe
-Version: 0.5.5
+Version: 0.5.6
 Summary: Gloe (pronounced /ɡloʊ/, like "glow") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code.
 Author-email: Samir Braga <samirchavess@gmail.com>
 Project-URL: Homepage, https://gloe.ideos.com.br
 Project-URL: Documentation, https://gloe.ideos.com.br
 Project-URL: Issues, https://github.com/ideos/gloe/issues
 Project-URL: Repository, https://github.com/ideos/gloe
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -44,15 +44,15 @@
 ## Motivation
 
 Software development has lots of patterns and good practices related to the code itself, like how to document, test, structure and what programming paradigm to use. However, beyond all that, we believe that the key point of a successful software project is a good communication between everyone involved in the development. Of course, this communication is not necessarily restricted to meetings or text messages, it is present also in documentation artifacts and in a well-written code.
 
 When developers write a code, they are telling a story to the next person who will read or/and refactor it. Depending on the code's quality, this story could be quite confusing, with no clear roles of the characters and a messy plot (sometimes with an undesired twist). The next person to maintain the software may take a long time to clearly understand the narrative and make it clear, or they will simply give up, leaving it as is.
 
 
-### How Gloe Can Help Me?
+### How Can Gloe Help Me?
 
 Gloe comes to turn this story coherent, logically organized and easy to follow. This is achieved by dividing the code into [concise steps](https://gloe.ideos.com.br/theory.html) with an unambiguous responsibility and explicit interface. Then, Gloe allows you to connect these steps, clarifying their collaboration and identifying necessary changes during refactoring. Thus, you can quickly understand the entire story being told and enhance it. Inspired by things like [natural transformation](https://ncatlab.org/nlab/show/natural+transformation) and Free Monad (present in [Scala](https://typelevel.org/cats/datatypes/freemonad.html) and [Haskell](https://serokell.io/blog/introduction-to-free-monads)), Gloe implemented this approach using functional programming and strong typing concepts.
 
 ### Gloe is not a workflow orchestrator
 
 Currently, unlike platforms like [Air Flow](https://airflow.apache.org/) that include scheduler backends for task orchestration, Gloe's primary purpose is to aid in development. The graph structure, which will be discussed in subsequent sections, aims to make the code [more flat and hence readable](https://en.wikibooks.org/wiki/Computer_Programming/Coding_Style/Minimize_nesting). However, it is important to note that Gloe does not offer functionalities for executing tasks in a dedicated environment, nor does it directly contribute to execution speed or scalability improvements.
```

### Comparing `gloe-0.5.5/README.md` & `gloe-0.5.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ## Motivation
 
 Software development has lots of patterns and good practices related to the code itself, like how to document, test, structure and what programming paradigm to use. However, beyond all that, we believe that the key point of a successful software project is a good communication between everyone involved in the development. Of course, this communication is not necessarily restricted to meetings or text messages, it is present also in documentation artifacts and in a well-written code.
 
 When developers write a code, they are telling a story to the next person who will read or/and refactor it. Depending on the code's quality, this story could be quite confusing, with no clear roles of the characters and a messy plot (sometimes with an undesired twist). The next person to maintain the software may take a long time to clearly understand the narrative and make it clear, or they will simply give up, leaving it as is.
 
 
-### How Gloe Can Help Me?
+### How Can Gloe Help Me?
 
 Gloe comes to turn this story coherent, logically organized and easy to follow. This is achieved by dividing the code into [concise steps](https://gloe.ideos.com.br/theory.html) with an unambiguous responsibility and explicit interface. Then, Gloe allows you to connect these steps, clarifying their collaboration and identifying necessary changes during refactoring. Thus, you can quickly understand the entire story being told and enhance it. Inspired by things like [natural transformation](https://ncatlab.org/nlab/show/natural+transformation) and Free Monad (present in [Scala](https://typelevel.org/cats/datatypes/freemonad.html) and [Haskell](https://serokell.io/blog/introduction-to-free-monads)), Gloe implemented this approach using functional programming and strong typing concepts.
 
 ### Gloe is not a workflow orchestrator
 
 Currently, unlike platforms like [Air Flow](https://airflow.apache.org/) that include scheduler backends for task orchestration, Gloe's primary purpose is to aid in development. The graph structure, which will be discussed in subsequent sections, aims to make the code [more flat and hence readable](https://en.wikibooks.org/wiki/Computer_Programming/Coding_Style/Minimize_nesting). However, it is important to note that Gloe does not offer functionalities for executing tasks in a dedicated environment, nor does it directly contribute to execution speed or scalability improvements.
```

### Comparing `gloe-0.5.5/docs/source/_static/assets/favicon.ico` & `gloe-0.5.6/docs/source/_static/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/_static/assets/gloe-logo-small.png` & `gloe-0.5.6/docs/source/_static/assets/gloe-logo-small.png`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/_static/assets/gloe-logo.png` & `gloe-0.5.6/docs/source/_static/assets/gloe-logo.png`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/_static/assets/graph_example.jpeg` & `gloe-0.5.6/docs/source/_static/assets/graph_example.jpeg`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/_templates/page.html` & `gloe-0.5.6/docs/source/_templates/page.html`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/api-reference/index.md` & `gloe-0.5.6/docs/source/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/conf.py` & `gloe-0.5.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/getting-started/async-transformers.md` & `gloe-0.5.6/docs/source/getting-started/async-transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/getting-started/conditional-flows.md` & `gloe-0.5.6/docs/source/getting-started/conditional-flows.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/getting-started/ensurers.md` & `gloe-0.5.6/docs/source/getting-started/ensurers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/getting-started/partial-transformers.md` & `gloe-0.5.6/docs/source/getting-started/partial-transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/getting-started/plotting.md` & `gloe-0.5.6/docs/source/getting-started/plotting.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/getting-started/transformers.md` & `gloe-0.5.6/docs/source/getting-started/transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/getting-started/utilities.md` & `gloe-0.5.6/docs/source/getting-started/utilities.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/index.md` & `gloe-0.5.6/docs/source/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ## Motivation
 
 Software development has lots of patterns and good practices related to the code itself, like how to document, test, structure and what programming paradigm to use. However, beyond all that, we believe that the key point of a successful software project is a good communication between everyone involved in the development. Of course, this communication is not necessarily restricted to meetings or text messages, it is present also in documentation artifacts and in a well-written code.
 
 When developers write a code, they are telling a story to the next person who will read or/and refactor it. Depending on the code's quality, this story could be quite confusing, with no clear roles of the characters and a messy plot (sometimes with an undesired twist). The next person to maintain the software may take a long time to clearly understand the narrative and make it clear, or they will simply give up, leaving it as is.
 
 
-### How Gloe Can Help Me?
+### How Can Gloe Help Me?
 
 Gloe comes to turn this story coherent, logically organized and easy to follow. This is achieved by dividing the code into [concise steps](https://gloe.ideos.com.br/theory.html) with an unambiguous responsibility and explicit interface. Then, Gloe allows you to connect these steps, clarifying their collaboration and identifying necessary changes during refactoring. Thus, you can quickly understand the entire story being told and enhance it. Inspired by things like [natural transformation](https://ncatlab.org/nlab/show/natural+transformation) and Free Monad (present in [Scala](https://typelevel.org/cats/datatypes/freemonad.html) and [Haskell](https://serokell.io/blog/introduction-to-free-monads)), Gloe implemented this approach using functional programming and strong typing concepts.
 
 ### Gloe is not a workflow orchestrator
 
 Currently, unlike platforms like [Air Flow](https://airflow.apache.org/) that include scheduler backends for task orchestration, Gloe's primary purpose is to aid in development. The graph structure, which will be discussed in subsequent sections, aims to make the code [more flat and hence readable](https://en.wikibooks.org/wiki/Computer_Programming/Coding_Style/Minimize_nesting). However, it is important to note that Gloe does not offer functionalities for executing tasks in a dedicated environment, nor does it directly contribute to execution speed or scalability improvements.
```

### Comparing `gloe-0.5.5/docs/source/limitations.md` & `gloe-0.5.6/docs/source/limitations.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/pygments/styles.py` & `gloe-0.5.6/docs/source/pygments/styles.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/docs/source/theory.md` & `gloe-0.5.6/docs/source/theory.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/gloe/__init__.py` & `gloe-0.5.6/gloe/__init__.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/gloe/_composition_utils.py` & `gloe-0.5.6/gloe/_composition_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import types
 from inspect import Signature
 from types import GenericAlias
 from typing import TypeVar, Any, cast
 
+from gloe._plotting_utils import PlottingSettings, NodeType
 from gloe.async_transformer import AsyncTransformer
 from gloe.base_transformer import BaseTransformer
 from gloe.transformers import Transformer
 from gloe._typing_utils import _match_types, _specify_types
 from gloe.exceptions import UnsupportedTransformerArgException
 
 _In = TypeVar("_In")
@@ -21,26 +22,14 @@
     return isinstance(node, Transformer)
 
 
 def is_async_transformer(node):
     return isinstance(node, AsyncTransformer)
 
 
-def _resolve_new_merge_transformers(
-    new_transformer: BaseTransformer, transformer2: BaseTransformer
-):
-    new_transformer.__class__.__name__ = transformer2.__class__.__name__
-    new_transformer._label = transformer2.label
-    new_transformer._children = transformer2.children
-    new_transformer._invisible = transformer2.invisible
-    new_transformer._graph_node_props = transformer2.graph_node_props
-    new_transformer._set_previous(transformer2.previous)
-    return new_transformer
-
-
 def _resolve_serial_connection_signatures(
     transformer2: BaseTransformer, generic_vars: dict, signature2: Signature
 ) -> Signature:
     first_param = list(signature2.parameters.values())[0]
     new_parameter = first_param.replace(
         annotation=_specify_types(transformer2.input_type, generic_vars)
     )
@@ -130,15 +119,20 @@
                 return transformed
 
         new_transformer = NewTransformer4()
 
     else:
         raise UnsupportedTransformerArgException(transformer2)  # pragma: no cover
 
-    return _resolve_new_merge_transformers(new_transformer, transformer2)
+    new_transformer.__class__.__name__ = transformer2.__class__.__name__
+    new_transformer._label = transformer2.label
+    new_transformer._children = transformer2.children
+    new_transformer._plotting_settings = transformer2._plotting_settings
+    new_transformer._set_previous(transformer2.previous)
+    return new_transformer
 
 
 def _merge_diverging(
     incident_transformer,
     *receiving_transformers,
 ):
     if incident_transformer.previous is None:
@@ -238,19 +232,15 @@
                 return await split_result_async(data)
 
         new_transformer = NewTransformer2()
 
     new_transformer._previous = cast(Transformer, receiving_transformers)
     new_transformer.__class__.__name__ = "Converge"
     new_transformer._label = ""
-    new_transformer._graph_node_props = {
-        "shape": "diamond",
-        "width": 0.5,
-        "height": 0.5,
-    }
+    new_transformer._plotting_settings = PlottingSettings(node_type=NodeType.Convergent)
 
     return new_transformer
 
 
 def _compose_nodes(
     current: BaseTransformer,
     next_node: tuple | BaseTransformer,
```

### Comparing `gloe-0.5.5/gloe/_transformer_utils.py` & `gloe-0.5.6/gloe/_transformer_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import traceback
+from typing import Any
 
+from gloe._plotting_utils import NodeType
 from gloe.base_transformer import BaseTransformer, TransformerException
 
 
 def catch_transformer_exception(
     exception: Exception, raiser_transformer: BaseTransformer
 ) -> TransformerException:
     transformer_name = raiser_transformer.__class__.__name__
```

### Comparing `gloe-0.5.5/gloe/_typing_utils.py` & `gloe-0.5.6/gloe/_typing_utils.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/gloe/async_transformer.py` & `gloe-0.5.6/gloe/async_transformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 import copy
-import traceback
 import types
 import uuid
 from abc import abstractmethod, ABC
 from inspect import Signature
-from typing import TypeVar, overload, cast, Any, Callable, Awaitable
+from typing import TypeVar, overload, cast, Callable, Awaitable
 
+from gloe._plotting_utils import PlottingSettings, NodeType
 from gloe._transformer_utils import catch_transformer_exception
 from gloe.base_transformer import (
-    TransformerException,
     BaseTransformer,
     PreviousTransformer,
 )
 
 __all__ = ["AsyncTransformer"]
 
-_In = TypeVar("_In")
-_Out = TypeVar("_Out")
+_In = TypeVar("_In", contravariant=True)
+_Out = TypeVar("_Out", covariant=True)
 _NextOut = TypeVar("_NextOut")
 
 _Out2 = TypeVar("_Out2")
 _Out3 = TypeVar("_Out3")
 _Out4 = TypeVar("_Out4")
 _Out5 = TypeVar("_Out5")
 _Out6 = TypeVar("_Out6")
 _Out7 = TypeVar("_Out7")
 
 
-class AsyncTransformer(BaseTransformer[_In, _Out, "AsyncTransformer"], ABC):
+class AsyncTransformer(BaseTransformer[_In, _Out], ABC):
     def __init__(self):
         super().__init__()
 
-        self._graph_node_props: dict[str, Any] = {
-            **self._graph_node_props,
-            "isAsync": True,
-        }
+        self._plotting_settings = PlottingSettings(
+            node_type=NodeType.Transformer, is_async=True
+        )
         self.__class__.__annotations__ = self.transform_async.__annotations__
 
     @abstractmethod
     async def transform_async(self, data: _In) -> _Out:
         """
         Method to perform the transformation asynchronously.
 
@@ -100,88 +98,86 @@
             child.copy(regenerate_instance_id=True) for child in self.children
         ]
 
         return copied
 
     @overload
     def __rshift__(
-        self, next_node: BaseTransformer[_Out, _NextOut, Any]
+        self, next_node: BaseTransformer[_Out, _NextOut]
     ) -> "AsyncTransformer[_In, _NextOut]":
         pass
 
     @overload
     def __rshift__(
         self,
-        next_node: tuple[
-            BaseTransformer[_Out, _NextOut, Any], BaseTransformer[_Out, _Out2, Any]
-        ],
+        next_node: tuple[BaseTransformer[_Out, _NextOut], BaseTransformer[_Out, _Out2]],
     ) -> "AsyncTransformer[_In, tuple[_NextOut, _Out2]]":
         pass
 
     @overload
     def __rshift__(
         self,
         next_node: tuple[
-            BaseTransformer[_Out, _NextOut, Any],
-            BaseTransformer[_Out, _Out2, Any],
-            BaseTransformer[_Out, _Out3, Any],
+            BaseTransformer[_Out, _NextOut],
+            BaseTransformer[_Out, _Out2],
+            BaseTransformer[_Out, _Out3],
         ],
     ) -> "AsyncTransformer[_In, tuple[_NextOut, _Out2, _Out3]]":
         pass
 
     @overload
     def __rshift__(
         self,
         next_node: tuple[
-            BaseTransformer[_Out, _NextOut, Any],
-            BaseTransformer[_Out, _Out2, Any],
-            BaseTransformer[_Out, _Out3, Any],
-            BaseTransformer[_Out, _Out4, Any],
+            BaseTransformer[_Out, _NextOut],
+            BaseTransformer[_Out, _Out2],
+            BaseTransformer[_Out, _Out3],
+            BaseTransformer[_Out, _Out4],
         ],
     ) -> "AsyncTransformer[_In, tuple[_NextOut, _Out2, _Out3, _Out4]]":
         pass
 
     @overload
     def __rshift__(
         self,
         next_node: tuple[
-            BaseTransformer[_Out, _NextOut, Any],
-            BaseTransformer[_Out, _Out2, Any],
-            BaseTransformer[_Out, _Out3, Any],
-            BaseTransformer[_Out, _Out4, Any],
-            BaseTransformer[_Out, _Out5, Any],
+            BaseTransformer[_Out, _NextOut],
+            BaseTransformer[_Out, _Out2],
+            BaseTransformer[_Out, _Out3],
+            BaseTransformer[_Out, _Out4],
+            BaseTransformer[_Out, _Out5],
         ],
     ) -> "AsyncTransformer[_In, tuple[_NextOut, _Out2, _Out3, _Out4, _Out5]]":
         pass
 
     @overload
     def __rshift__(
         self,
         next_node: tuple[
-            BaseTransformer[_Out, _NextOut, Any],
-            BaseTransformer[_Out, _Out2, Any],
-            BaseTransformer[_Out, _Out3, Any],
-            BaseTransformer[_Out, _Out4, Any],
-            BaseTransformer[_Out, _Out5, Any],
-            BaseTransformer[_Out, _Out6, Any],
+            BaseTransformer[_Out, _NextOut],
+            BaseTransformer[_Out, _Out2],
+            BaseTransformer[_Out, _Out3],
+            BaseTransformer[_Out, _Out4],
+            BaseTransformer[_Out, _Out5],
+            BaseTransformer[_Out, _Out6],
         ],
     ) -> "AsyncTransformer[_In, tuple[_NextOut, _Out2, _Out3, _Out4, _Out5, _Out6]]":
         pass
 
     @overload
     def __rshift__(
         self,
         next_node: tuple[
-            BaseTransformer[_Out, _NextOut, Any],
-            BaseTransformer[_Out, _Out2, Any],
-            BaseTransformer[_Out, _Out3, Any],
-            BaseTransformer[_Out, _Out4, Any],
-            BaseTransformer[_Out, _Out5, Any],
-            BaseTransformer[_Out, _Out6, Any],
-            BaseTransformer[_Out, _Out7, Any],
+            BaseTransformer[_Out, _NextOut],
+            BaseTransformer[_Out, _Out2],
+            BaseTransformer[_Out, _Out3],
+            BaseTransformer[_Out, _Out4],
+            BaseTransformer[_Out, _Out5],
+            BaseTransformer[_Out, _Out6],
+            BaseTransformer[_Out, _Out7],
         ],
     ) -> (
         "AsyncTransformer[_In, tuple[_NextOut, _Out2, _Out3, _Out4, _Out5, _Out6, _Out7]]"
     ):
         pass
 
     def __rshift__(self, next_node):  # pragma: no cover
```

### Comparing `gloe-0.5.5/gloe/base_transformer.py` & `gloe-0.5.6/gloe/base_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,20 +19,19 @@
     get_origin,
     TypeAlias,
     Type,
 )
 from uuid import UUID
 from itertools import groupby
 
+from gloe._plotting_utils import PlottingSettings, NodeType
 from gloe._typing_utils import _format_return_annotation
 
 __all__ = ["BaseTransformer", "TransformerException", "PreviousTransformer"]
 
-_In = TypeVar("_In")
-_Out = TypeVar("_Out")
 _NextOut = TypeVar("_NextOut")
 _Self = TypeVar("_Self", bound="BaseTransformer")
 
 _Out2 = TypeVar("_Out2")
 _Out3 = TypeVar("_Out3")
 _Out4 = TypeVar("_Out4")
 _Out5 = TypeVar("_Out5")
@@ -47,14 +46,16 @@
     tuple[_Self, _Self, _Self],
     tuple[_Self, _Self, _Self, _Self],
     tuple[_Self, _Self, _Self, _Self, _Self],
     tuple[_Self, _Self, _Self, _Self, _Self, _Self],
     tuple[_Self, _Self, _Self, _Self, _Self, _Self, _Self],
 ]
 
+TransformerChildren: TypeAlias = list["BaseTransformer"]
+
 
 class TransformerException(Exception):
     def __init__(
         self,
         internal_exception: Union["TransformerException", Exception],
         raiser_transformer: "BaseTransformer",
         message: str | None = None,
@@ -66,23 +67,29 @@
         super().__init__(message)
 
     @property
     def internal_exception(self):
         return self._internal_exception.with_traceback(self._traceback)
 
 
-class BaseTransformer(Generic[_In, _Out, _Self]):
+_In = TypeVar("_In", contravariant=True)
+_Out = TypeVar("_Out", covariant=True)
+
+
+class BaseTransformer(Generic[_In, _Out]):
     def __init__(self):
         self._previous: PreviousTransformer["BaseTransformer"] = None
-        self._children: list["BaseTransformer"] = []
-        self._invisible = False
+        self._children: TransformerChildren = []
         self.id = uuid.uuid4()
         self.instance_id = uuid.uuid4()
         self._label = self.__class__.__name__
-        self._graph_node_props: dict[str, Any] = {"shape": "box"}
+        self._plotting_settings: PlottingSettings = PlottingSettings(
+            invisible=False,
+            node_type=NodeType.Transformer,
+        )
         self.events = []
 
     @property
     def label(self) -> str:
         """
         Label used in visualization.
 
@@ -91,32 +98,35 @@
 
         When creating a transformer by extending the `Transformer` class, it is the name of
         the class.
         """
         return self._label
 
     @property
-    def graph_node_props(self) -> dict[str, Any]:
-        return self._graph_node_props
-
-    @property
-    def children(self) -> list["BaseTransformer"]:
+    def children(self) -> TransformerChildren:
+        """
+        Used when a transformer encapsulates other transformer. The encapsulated
+        transformers are called children transformers.
+        """
         return self._children
 
     @property
     def previous(self) -> PreviousTransformer["BaseTransformer"]:
         """
-        Previous transformers. It can be None, a single transformer, or a tuple of many
-        transformers.
+        Previous transformers. It can be None (when the transformer is the first of its
+        pipeline), a single transformer, or a tuple of many transformers.
         """
         return self._previous
 
     @property
-    def invisible(self) -> bool:
-        return self._invisible
+    def plotting_settings(self) -> PlottingSettings:
+        """
+        Defines how the transformer will be plotted.
+        """
+        return self._plotting_settings
 
     def __hash__(self) -> int:
         return hash(self.id)
 
     def __eq__(self, other):
         if isinstance(other, BaseTransformer):
             return self.id == other.id
@@ -241,17 +251,41 @@
             parameter_type = parameters[0][1].annotation
             return parameter_type
 
     @property
     def input_annotation(self) -> str:
         return self.input_type.__name__
 
+    def export_dot_props(self) -> dict[str, Any]:
+        settings = self.plotting_settings
+        node_props: dict[str, Any] = {"shape": "box"}
+
+        match settings.node_type:
+            case NodeType.Condition:
+                node_props = {"shape": "diamond", "style": "filled", "port": "n"}
+            case NodeType.Convergent:
+                node_props = {
+                    "shape": "diamond",
+                    "width": 0.5,
+                    "height": 0.5,
+                }
+
+        if settings.has_children:
+            node_props = node_props | {
+                "parent_id": self.instance_id,
+                "bounding_box": True,
+                "box_label": "mapping",
+            }
+
+        return node_props
+
     def _add_net_node(self, net: Graph, custom_data: dict[str, Any] = {}):
         node_id = self.node_id
-        props = {**self.graph_node_props, **custom_data, "label": self.label}
+        graph_node_props = self.export_dot_props()
+        props = {**graph_node_props, **custom_data, "label": self.label}
         if node_id not in net.nodes:
             net.add_node(node_id, **props)
         else:
             nx.set_node_attributes(net, {node_id: props})
         return node_id
 
     def _add_child_node(
@@ -268,15 +302,15 @@
         return str(self.instance_id)
 
     @cached_property
     def visible_previous(self) -> PreviousTransformer["BaseTransformer"]:
         previous = self.previous
 
         if isinstance(previous, BaseTransformer):
-            if previous.invisible:
+            if previous.plotting_settings.invisible:
                 if previous.previous is None:
                     return previous
 
                 if type(previous.previous) == tuple:
                     return previous.previous
 
                 return previous.visible_previous
@@ -298,15 +332,15 @@
             child_root_node = [n for n in child_net.nodes if child_net.in_degree(n) == 0][
                 0
             ]
             child_final_node = [
                 n for n in child_net.nodes if child_net.out_degree(n) == 0
             ][0]
 
-            if self.invisible:
+            if self.plotting_settings.invisible:
                 if type(visible_previous) == tuple:
                     for prev in visible_previous:
                         net.add_edge(
                             prev.node_id, child_root_node, label=prev.output_annotation
                         )
                 elif isinstance(visible_previous, BaseTransformer):
                     net.add_edge(
@@ -330,44 +364,44 @@
         custom_data: dict[str, Any] = {},
     ):
         in_nodes = [edge[1] for edge in net.in_edges()]
 
         previous = self.previous
         if previous is not None:
             if type(previous) == tuple:
-                if self.invisible and next_node is not None:
+                if self.plotting_settings.invisible and next_node is not None:
                     next_node_id = next_node._add_net_node(net)
                     _next_node = next_node
                 else:
                     next_node_id = self._add_net_node(net, custom_data)
                     _next_node = self
 
                 for prev in previous:
                     previous_node_id = prev.node_id
 
                     # TODO: check the impact of the below line to the Mapper transformer
-                    if not prev.invisible and len(prev.children) == 0:
+                    if not prev.plotting_settings.invisible and len(prev.children) == 0:
                         net.add_edge(
                             previous_node_id, next_node_id, label=prev.output_annotation
                         )
 
                     if previous_node_id not in in_nodes:
                         prev._dag(net, _next_node, custom_data)
             elif isinstance(previous, BaseTransformer):
-                if self.invisible and next_node is not None:
+                if self.plotting_settings.invisible and next_node is not None:
                     next_node_id = next_node._add_net_node(net)
                     _next_node = next_node
                 else:
                     next_node_id = self._add_net_node(net, custom_data)
                     _next_node = self
 
                 previous_node_id = previous.node_id
 
                 if len(previous.children) == 0 and (
-                    not previous.invisible or previous.previous is None
+                    not previous.plotting_settings.invisible or previous.previous is None
                 ):
                     previous_node_id = previous._add_net_node(net)
                     net.add_edge(
                         previous_node_id, next_node_id, label=previous.output_annotation
                     )
 
                 if previous_node_id not in in_nodes:
```

### Comparing `gloe-0.5.5/gloe/collection/_mapover.py` & `gloe-0.5.6/gloe/collection/_mapover.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self,
         iterable: list[_S],
         mapping_transformer: Transformer[tuple[_T, _S], _U],
     ):
         super().__init__()
         self.iterable = iterable
         self.mapping_transformer = mapping_transformer
-        self._invisible = True
+        self.plotting_settings.invisible = True
         self._children = [mapping_transformer]
 
     def transform(self, data: _T) -> list[_U]:
         lopping_result = []
         for item in self.iterable:
             lopping_result.append(self.mapping_transformer((data, item)))
         return lopping_result
```

### Comparing `gloe-0.5.5/gloe/conditional/_conditioner.py` & `gloe-0.5.6/gloe/conditional/_conditioner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 from inspect import Signature
 from types import GenericAlias, UnionType
 from typing import Callable, Generic, Optional, TypeVar, Union
 
+from gloe._plotting_utils import PlottingSettings, NodeType
 from gloe.transformers import Transformer
 from gloe.utils import forget
 
 
 In = TypeVar("In")
 ThenOut = TypeVar("ThenOut")
 ElseOut = TypeVar("ElseOut")
@@ -27,15 +28,15 @@
         self,
         implications: list[_Implication[In, ThenOut]],
         else_transformer: Transformer[In, ElseOut],
     ):
         super().__init__()
         self.implications = implications
         self.else_transformer = else_transformer
-        self._graph_node_props = {"shape": "diamond", "style": "filled", "port": "n"}
+        self._plotting_settings = PlottingSettings(node_type=NodeType.Condition)
         self._children = [
             *[impl.then_transformer for impl in implications],
             else_transformer,
         ]
 
     def transform(self, data: In) -> Union[ThenOut, ElseOut]:
         for implication in self.implications:
```

### Comparing `gloe-0.5.5/gloe/ensurer/_transformer_ensurer.py` & `gloe-0.5.6/gloe/ensurer/_transformer_ensurer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/gloe/experimental/_bridge.py` & `gloe-0.5.6/gloe/experimental/_bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
             f"The bridge {bridge_name} has tried to be dropped but its value was not initialized"
         )
 
 
 class _pick(Generic[T], Transformer[T, T]):
     def __init__(self, variable: ContextVar[T]):
         super().__init__()
-        self._invisible = True
+        self.plotting_settings.invisible = True
         self.variable = variable
 
     def transform(self, data: T) -> T:
         self.variable.set(data)
         return data
 
 
 class _drop(Generic[B, T], Transformer[B, tuple[B, T]]):
     def __init__(self, variable: ContextVar[T]):
         super().__init__()
-        self._invisible = True
+        self.plotting_settings.invisible = True
         self._variable = variable
 
     def transform(self, data: B) -> tuple[B, T]:
         current_value: T
         try:
             current_value = self._variable.get()
         except LookupError:
```

### Comparing `gloe-0.5.5/gloe/functional.py` & `gloe-0.5.6/gloe/functional.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/gloe/utils.py` & `gloe-0.5.6/gloe/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,20 +14,17 @@
 @transformer
 def forget(data: Any) -> None:
     """Transform any input data to `None`"""
     return None
 
 
 class debug(Generic[_In], Transformer[_In, _In]):
-    def __init__(self, custom_debugger: str | None = None):
+    def __init__(self):
         super().__init__()
-        self._invisible = True
-        self._possible_debuggers = ["pdb", "pydevd", "pydevd_runpy"]
-        if custom_debugger is not None:
-            self._possible_debuggers.append(custom_debugger)
+        self.plotting_settings.invisible = True
 
     def _is_under_debug(self):
         if hasattr(sys, "gettrace") and sys.gettrace() is not None:
             trace = sys.gettrace()
             if hasattr(trace, "_args"):
                 return True
         return False
@@ -46,15 +43,15 @@
     def _debugging(self, current_data: _In):
         breakpoint()
 
 
 class forward(Generic[_In], Transformer[_In, _In]):
     def __init__(self):
         super().__init__()
-        self._invisible = True
+        self.plotting_settings.invisible = True
 
     def transform(self, data: _In) -> _In:
         return data
 
 
 def forward_incoming(
     inner_transformer: Transformer[_In, _Out]
```

### Comparing `gloe-0.5.5/gloe.egg-info/PKG-INFO` & `gloe-0.5.6/gloe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gloe
-Version: 0.5.5
+Version: 0.5.6
 Summary: Gloe (pronounced /ɡloʊ/, like "glow") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code.
 Author-email: Samir Braga <samirchavess@gmail.com>
 Project-URL: Homepage, https://gloe.ideos.com.br
 Project-URL: Documentation, https://gloe.ideos.com.br
 Project-URL: Issues, https://github.com/ideos/gloe/issues
 Project-URL: Repository, https://github.com/ideos/gloe
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -44,15 +44,15 @@
 ## Motivation
 
 Software development has lots of patterns and good practices related to the code itself, like how to document, test, structure and what programming paradigm to use. However, beyond all that, we believe that the key point of a successful software project is a good communication between everyone involved in the development. Of course, this communication is not necessarily restricted to meetings or text messages, it is present also in documentation artifacts and in a well-written code.
 
 When developers write a code, they are telling a story to the next person who will read or/and refactor it. Depending on the code's quality, this story could be quite confusing, with no clear roles of the characters and a messy plot (sometimes with an undesired twist). The next person to maintain the software may take a long time to clearly understand the narrative and make it clear, or they will simply give up, leaving it as is.
 
 
-### How Gloe Can Help Me?
+### How Can Gloe Help Me?
 
 Gloe comes to turn this story coherent, logically organized and easy to follow. This is achieved by dividing the code into [concise steps](https://gloe.ideos.com.br/theory.html) with an unambiguous responsibility and explicit interface. Then, Gloe allows you to connect these steps, clarifying their collaboration and identifying necessary changes during refactoring. Thus, you can quickly understand the entire story being told and enhance it. Inspired by things like [natural transformation](https://ncatlab.org/nlab/show/natural+transformation) and Free Monad (present in [Scala](https://typelevel.org/cats/datatypes/freemonad.html) and [Haskell](https://serokell.io/blog/introduction-to-free-monads)), Gloe implemented this approach using functional programming and strong typing concepts.
 
 ### Gloe is not a workflow orchestrator
 
 Currently, unlike platforms like [Air Flow](https://airflow.apache.org/) that include scheduler backends for task orchestration, Gloe's primary purpose is to aid in development. The graph structure, which will be discussed in subsequent sections, aims to make the code [more flat and hence readable](https://en.wikibooks.org/wiki/Computer_Programming/Coding_Style/Minimize_nesting). However, it is important to note that Gloe does not offer functionalities for executing tasks in a dedicated environment, nor does it directly contribute to execution speed or scalability improvements.
```

### Comparing `gloe-0.5.5/gloe.egg-info/SOURCES.txt` & `gloe-0.5.6/gloe.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -25,28 +25,32 @@
 docs/source/getting-started/partial-transformers.md
 docs/source/getting-started/plotting.md
 docs/source/getting-started/transformers.md
 docs/source/getting-started/utilities.md
 docs/source/pygments/styles.py
 gloe/__init__.py
 gloe/_composition_utils.py
+gloe/_generic_types.py
+gloe/_plotting_utils.py
+gloe/_supports_composition.py
 gloe/_transformer_utils.py
 gloe/_typing_utils.py
 gloe/async_transformer.py
 gloe/base_transformer.py
 gloe/functional.py
 gloe/py.typed
 gloe/transformers.py
 gloe/utils.py
 gloe.egg-info/PKG-INFO
 gloe.egg-info/SOURCES.txt
 gloe.egg-info/dependency_links.txt
 gloe.egg-info/requires.txt
 gloe.egg-info/top_level.txt
 gloe/collection/__init__.py
+gloe/collection/_filter.py
 gloe/collection/_map.py
 gloe/collection/_mapover.py
 gloe/conditional/__init__.py
 gloe/conditional/_conditioner.py
 gloe/ensurer/__init__.py
 gloe/ensurer/_transformer_ensurer.py
 gloe/exceptions/__init__.py
```

### Comparing `gloe-0.5.5/pyproject.toml` & `gloe-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gloe"
-version = "0.5.5"
+version = "0.5.6"
 authors = [
   { name="Samir Braga", email="samirchavess@gmail.com" },
 ]
 description = "Gloe (pronounced /ɡloʊ/, like \"glow\") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gloe-0.5.5/tests/lib/ensurers.py` & `gloe-0.5.6/tests/lib/ensurers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/tests/lib/transformers.py` & `gloe-0.5.6/tests/lib/transformers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/tests/test_async_transformer.py` & `gloe-0.5.6/tests/test_async_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/tests/test_conditioner_transformer.py` & `gloe-0.5.6/tests/test_conditioner_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/tests/test_function_transformer.py` & `gloe-0.5.6/tests/test_function_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/tests/test_transformer_bridge.py` & `gloe-0.5.6/tests/test_transformer_bridge.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/tests/test_transformer_collections.py` & `gloe-0.5.6/tests/test_transformer_collections.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 
-from gloe.collection import Map, MapOver
+from gloe.functional import transformer
+from gloe.collection import Map, MapOver, Filter
 from tests.lib.transformers import square, plus1, sum_tuple2
 
 
 class TestTransformerCollections(unittest.TestCase):
     def test_transformer_map(self):
         """
         Test the mapping transformer
@@ -17,14 +18,31 @@
         result1 = list(mapping1(seq))
         result2 = list(mapping2(seq))
 
         expected = [101.0, 82.0, 10.0, 5.0, 2.0]
         self.assertListEqual(expected, result1)
         self.assertListEqual(expected, result2)
 
+    def test_transformer_filter(self):
+        """
+        Test the filter transformer
+        """
+
+        @transformer
+        def is_even(num: int) -> bool:
+            return num % 2 == 0
+
+        _filter = Filter(is_even)
+
+        seq = [10, 9, 3, 2, 1]
+        result = _filter(seq)
+
+        expected = [10, 2]
+        self.assertListEqual(expected, list(result))
+
     def test_transformer_map_over(self):
         """
         Test the mapping transformer
         """
 
         data = [10.0, 9.0, 3.0, 2.0, -1.0]
         mapping = MapOver(data, sum_tuple2) >> Map(plus1)
```

### Comparing `gloe-0.5.5/tests/test_transformer_ensurer.py` & `gloe-0.5.6/tests/test_transformer_ensurer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.5/tests/test_transformer_graph.py` & `gloe-0.5.6/tests/test_transformer_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         begin3 = begin1 >> begin2
 
         graph: DiGraph = begin3.graph()
 
         self._assert_nodes_count(9, graph)
         self._assert_edges_count(10, graph)
 
-    def test_transformer_init_case(self):
+    def test_partial_transformer_case(self):
         init_graph = logarithm(2) >> square
 
         graph: DiGraph = init_graph.graph()
 
         self._assert_nodes_count(2, graph)
         self._assert_edges_count(1, graph)
```

### Comparing `gloe-0.5.5/tests/test_transformer_types.py` & `gloe-0.5.6/tests/test_transformer_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import os
 import unittest
 from pathlib import Path
-from typing import TypeVar
+from typing import TypeVar, Iterable
 from typing_extensions import assert_type
 
 from tests.lib.conditioners import if_not_zero, if_is_even
 from tests.lib.ensurers import is_even, same_value, same_value_int, is_greater_than_10
 from tests.lib.transformers import (
     square,
     square_root,
@@ -150,15 +150,15 @@
         Test the transformer map collection operation
         """
 
         mapped_logarithm = forward[list[float]]() >> Map(
             format_currency(thousands_separator=",")
         )
 
-        assert_type(mapped_logarithm, Transformer[list[float], list[str]])
+        assert_type(mapped_logarithm, Transformer[list[float], Iterable[str]])
 
     def _test_transformer_ensurer(self):
         @ensure(incoming=[is_even])
         @transformer
         def t1(n1: int) -> int:
             return n1 * n1
```

### Comparing `gloe-0.5.5/tests/test_transformer_utils.py` & `gloe-0.5.6/tests/test_transformer_utils.py`

 * *Files identical despite different names*

