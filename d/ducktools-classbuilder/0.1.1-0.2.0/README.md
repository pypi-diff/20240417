# Comparing `tmp/ducktools_classbuilder-0.1.1.tar.gz` & `tmp/ducktools_classbuilder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ducktools_classbuilder-0.1.1.tar", last modified: Mon Apr 15 13:32:09 2024, max compression
+gzip compressed data, was "ducktools_classbuilder-0.2.0.tar", last modified: Wed Apr 17 16:30:32 2024, max compression
```

## Comparing `ducktools_classbuilder-0.1.1.tar` & `ducktools_classbuilder-0.2.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.594660 ducktools_classbuilder-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-15 13:32:09.594660 ducktools_classbuilder-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.582660 ducktools_classbuilder-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/approach_vs_tool.md
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19176 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/extension_examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.582660 ducktools_classbuilder-0.1.1/docs/perf/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/perf/performance_tests.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.582660 ducktools_classbuilder-0.1.1/docs/prefab/
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/prefab/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:32:09.594660 ducktools_classbuilder-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.578660 ducktools_classbuilder-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.578660 ducktools_classbuilder-0.1.1/src/ducktools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.582660 ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/
--rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29675 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/prefab.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/prefab.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.590660 ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-15 13:32:09.000000 ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-15 13:32:09.000000 ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:32:09.000000 ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 13:32:09.000000 ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 13:32:09.000000 ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.578660 ducktools_classbuilder-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.578660 ducktools_classbuilder-0.1.1/tests/prefab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.586660 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_compare_attrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_construction.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_internals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_pre_post_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_slots_novalues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_slotted_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.586660 ducktools_classbuilder-0.1.1/tests/prefab/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.590660 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/creation_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/dunders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.590660 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/creation_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/creation_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/creation_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/creation_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/inheritance_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/inheritance_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/frozen_prefabs.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/funcs_prefabs.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/hint_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/init_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/kw_only.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/repr_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_dunders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_frozen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_hint_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_kw_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_repr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.821151 ducktools_classbuilder-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-17 16:30:32.821151 ducktools_classbuilder-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.813151 ducktools_classbuilder-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/docs/approach_vs_tool.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24506 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/docs/extension_examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.813151 ducktools_classbuilder-0.2.0/docs/perf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/docs/perf/performance_tests.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.813151 ducktools_classbuilder-0.2.0/docs/prefab/
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/docs/prefab/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:30:32.821151 ducktools_classbuilder-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.809151 ducktools_classbuilder-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.809151 ducktools_classbuilder-0.2.0/src/ducktools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.813151 ducktools_classbuilder-0.2.0/src/ducktools/classbuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)    13747 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/src/ducktools/classbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/src/ducktools/classbuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29871 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/src/ducktools/classbuilder/prefab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/src/ducktools/classbuilder/prefab.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/src/ducktools/classbuilder/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.821151 ducktools_classbuilder-0.2.0/src/ducktools_classbuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-17 16:30:32.000000 ducktools_classbuilder-0.2.0/src/ducktools_classbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-17 16:30:32.000000 ducktools_classbuilder-0.2.0/src/ducktools_classbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:30:32.000000 ducktools_classbuilder-0.2.0/src/ducktools_classbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 16:30:32.000000 ducktools_classbuilder-0.2.0/src/ducktools_classbuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 16:30:32.000000 ducktools_classbuilder-0.2.0/src/ducktools_classbuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.813151 ducktools_classbuilder-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.813151 ducktools_classbuilder-0.2.0/tests/prefab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.817151 ducktools_classbuilder-0.2.0/tests/prefab/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/dynamic/test_compare_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/dynamic/test_construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/dynamic/test_internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/dynamic/test_pre_post_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/dynamic/test_slots_novalues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/dynamic/test_slotted_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.817151 ducktools_classbuilder-0.2.0/tests/prefab/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.821151 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/creation_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/dunders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:30:32.821151 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/fails/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/fails/creation_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/fails/creation_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/fails/creation_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/fails/creation_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/fails/inheritance_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/fails/inheritance_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/frozen_prefabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/funcs_prefabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/hint_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/init_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/kw_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/repr_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/test_dunders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/test_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/test_hint_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/test_kw_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-17 16:30:28.000000 ducktools_classbuilder-0.2.0/tests/prefab/shared/test_repr.py
```

### Comparing `ducktools_classbuilder-0.1.1/LICENSE.md` & `ducktools_classbuilder-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/PKG-INFO` & `ducktools_classbuilder-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducktools-classbuilder
-Version: 0.1.1
+Version: 0.2.0
 Summary: Toolkit for creating class boilerplate generators
 Author: David C Ellis
 License: MIT License
         
         Copyright (c) 2024 David C Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ducktools_classbuilder-0.1.1/README.md` & `ducktools_classbuilder-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/docs/Makefile` & `ducktools_classbuilder-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/docs/api.md` & `ducktools_classbuilder-0.2.0/docs/api.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ```
 
 ```{eval-rst}
 .. autofunction:: ducktools.classbuilder::get_fields
 ```
 
 ```{eval-rst}
-.. autofunction:: ducktools.classbuilder::get_internals
+.. autofunction:: ducktools.classbuilder::get_flags
 ```
 
 ```{eval-rst}
 .. autoclass:: ducktools.classbuilder::MethodMaker
 ```
 
 ```{eval-rst}
```

### Comparing `ducktools_classbuilder-0.1.1/docs/approach_vs_tool.md` & `ducktools_classbuilder-0.2.0/docs/approach_vs_tool.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/docs/conf.py` & `ducktools_classbuilder-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/docs/extension_examples.md` & `ducktools_classbuilder-0.2.0/docs/extension_examples.md`

 * *Files 17% similar despite different names*

```diff
@@ -29,24 +29,39 @@
 .. autofunction:: ducktools.classbuilder::builder
   :noindex:
 ```
 
 This function is the core class generator which takes your decorated class and
 analyses and collects valid fields and then attaches the method makers.
 
-The field information is stored in the `INTERNALS_DICT` attribute and can be
-accessed using the `get_internals` function provided. This returns a dictionary
-with 2 keys: `local_fields` and `fields`. 
+The field information is stored in the `INTERNALS_DICT` attribute which should generally
+not need to be accessed directly. `get_fields` and `get_flags` functions are to be
+used to access the important keys.
 
-`"local_fields"` contains the field information obtained from **this class only**.
+`get_fields(cls)` will return the resolved information obtained from this class and subclasses.
 
-`"fields"` contains the resolved information obtained from this class and subclasses.
-This can be obtained directly using the `get_fields` function.
+`get_fields(cls, local=True)` will return the field information obtained from **this class only**.
 
-Now let's look at what the two keyword arguments need to be.
+Now let's look at what the keyword arguments to `builder` need to be.
+
+#### Flags ####
+
+Flags are information that defines how the entire class should be generated, for use by
+method generators when operating on the class.
+
+The default makers in `ducktools.classbuilder` make use of one flag - `"kw_only"` - 
+which indicates that a class `__init__` function should only take keyword arguments.
+
+Prefabs also make use of a `"slotted"` flag to indicate if the class has been generated
+with `__slots__` (checking for the existence of `__slots__` could find that a user has
+manually placed slots in the class).
+
+Flags are set using a dictionary with these keys and boolean values, for example:
+
+`cls = builder(cls, gatherer=..., methods=..., flags={"kw_only": True, "slotted": True})` 
 
 #### Gatherers ####
 
 This covers the *'gather the fields'* step of the process.
 
 A `gatherer` in this case is a function which takes in the class and returns a dict
 of `{"field_name": Field(...)}` values based on some analysis of your class.
@@ -668,66 +683,237 @@
     )
     print(ex2)
 
     print(H2G2.the_book)
     print(H2G2.the_author)
 ```
 
-#### No attributes! Only Annotations! ####
+#### What about using annotations instead of `Field(init=False, ...)` ####
 
-If you don't like your code to run quickly, but you do love type annotations.
-
-This does everything using `Annotated` and so requires Python 3.10 for both 
-this and get_annotations.
+This seems to be a feature people keep requesting for `dataclasses`.
+This is also doable.
 
 ```python
 import inspect
+from pprint import pp
 from typing import Annotated, Any, ClassVar, get_origin
 
-from ducktools.classbuilder import builder, default_methods, Field
+from ducktools.classbuilder import (
+    builder,
+    fieldclass,
+    get_fields,
+    get_flags,
+    Field,
+    MethodMaker,
+    SlotFields,
+    NOTHING,
+)
+
+
+# New equivalent to dataclasses "Field", these still need to be created
+# in order to generate the magic methods correctly.
+@fieldclass
+class AnnoField(Field):
+    __slots__ = SlotFields(
+        init=True,
+        repr=True,
+        compare=True,
+        kw_only=False,
+    )
+
+
+# Modifying objects
+class FieldModifier:
+    __slots__ = ("modifiers", )
+    modifiers: dict[str, Any]
+
+    def __init__(self, **modifiers):
+        self.modifiers = modifiers
+
+    def __repr__(self):
+        mod_args = ", ".join(f"{k}={v!r}" for k, v in self.modifiers.items())
+        return (
+            f"{type(self).__name__}({mod_args})"
+        )
+
+    def __eq__(self, other):
+        if self.__class__ == other.__class__:
+            return self.modifiers == other.modifiers
+        return NotImplemented
+
+
+KW_ONLY = FieldModifier(kw_only=True)
+NO_INIT = FieldModifier(init=False)
+NO_REPR = FieldModifier(repr=False)
+NO_COMPARE = FieldModifier(compare=False)
+IGNORE_ALL = FieldModifier(init=False, repr=False, compare=False)
 
 
 def annotated_gatherer(cls: type) -> dict[str, Any]:
+    # String annotations *MUST* be evaluated for this to work
+    # dataclasses currently does not require this
     cls_annotations = inspect.get_annotations(cls, eval_str=True)
     cls_fields = {}
 
     for key, anno in cls_annotations.items():
-        # Is there another way to do this?
+        modifiers = {}
+        typ = NOTHING
+
         if get_origin(anno) is Annotated:
             typ = anno.__args__[0]
             meta = anno.__metadata__
             for v in meta:
-                if isinstance(v, Field):
-                    fld = Field.from_field(v, type=typ)
-                    break
-            else:
-                fld = Field(type=typ)
-        elif anno is ClassVar or get_origin(anno) is ClassVar:
-            fld = None
-        else:
+                if isinstance(v, FieldModifier):
+                    modifiers.update(v.modifiers)
+
+        elif not (anno is ClassVar or get_origin(anno) is ClassVar):
             typ = anno
-            fld = Field(type=typ)
 
-        if fld:
-            cls_fields[key] = fld
+        if typ is not NOTHING:
             if key in cls.__dict__ and "__slots__" not in cls.__dict__:
-                raise AttributeError("No attributes! Only Annotations!")
+                val = cls.__dict__[key]
+                if isinstance(val, Field):
+                    fld = AnnoField.from_field(val, type=typ, **modifiers)
+                else:
+                    fld = AnnoField(default=val, type=typ, **modifiers)
+            else:
+                fld = AnnoField(type=typ, **modifiers)
+
+            cls_fields[key] = fld
 
     return cls_fields
 
 
-def annotationsclass(cls):
-    return builder(cls, gatherer=annotated_gatherer, methods=default_methods)
+def init_maker(cls):
+
+    fields = get_fields(cls)
+    flags = get_flags(cls)
+
+    arglist = []
+    kw_only_arglist = []
+
+    assignments = []
+    globs = {}
+
+    # Whole class kw_only
+    kw_only = flags.get("kw_only", False)
+
+    for k, v in fields.items():
+        if getattr(v, "init", True):
+            if v.default is not NOTHING:
+                globs[f"_{k}_default"] = v.default
+                arg = f"{k}=_{k}_default"
+                assignment = f"self.{k} = {k}"
+            elif v.default_factory is not NOTHING:
+                globs[f"_{k}_factory"] = v.default_factory
+                arg = f"{k}=None"
+                assignment = f"self.{k} = _{k}_factory() if {k} is None else {k}"
+            else:
+                arg = f"{k}"
+                assignment = f"self.{k} = {k}"
+
+            if getattr(v, "kw_only", False) or kw_only:
+                kw_only_arglist.append(arg)
+            else:
+                arglist.append(arg)
+
+            assignments.append(assignment)
+        else:
+            if v.default is not NOTHING:
+                globs[f"_{k}_default"] = v.default
+                assignment = f"self.{k} = _{k}_default"
+                assignments.append(assignment)
+            elif v.default_factory is not NOTHING:
+                globs[f"_{k}_factory"] = v.default_factory
+                assignment = f"self.{k} = _{k}_factory()"
+                assignments.append(assignment)
+
+    if kw_only_arglist:
+        arglist.append("*")
+        arglist.extend(kw_only_arglist)
+
+    args = ", ".join(arglist)
+    assigns = "\n    ".join(assignments)
+    code = f"def __init__(self, {args}):\n" f"    {assigns}\n"
+
+    return code, globs
+
+
+def repr_maker(cls):
+    fields = get_fields(cls)
+    content = ", ".join(
+        f"{name}={{self.{name}!r}}"
+        for name, fld in fields.items()
+        if getattr(fld, "repr", True)
+    )
+    code = (
+        f"def __repr__(self):\n"
+        f"    return f'{{type(self).__qualname__}}({content})'\n"
+    )
+    globs = {}
+    return code, globs
+
+
+def eq_maker(cls):
+    class_comparison = "self.__class__ is other.__class__"
+    field_names = [
+        name
+        for name, fld in get_fields(cls).items()
+        if getattr(fld, "compare", True)
+    ]
+
+    if field_names:
+        selfvals = ",".join(f"self.{name}" for name in field_names)
+        othervals = ",".join(f"other.{name}" for name in field_names)
+        instance_comparison = f"({selfvals},) == ({othervals},)"
+    else:
+        instance_comparison = "True"
+
+    code = (
+        f"def __eq__(self, other):\n"
+        f"    return {instance_comparison} if {class_comparison} else NotImplemented\n"
+    )
+    globs = {}
+
+    return code, globs
+
+
+init_method = MethodMaker("__init__", init_maker)
+repr_method = MethodMaker("__repr__", repr_maker)
+eq_method = MethodMaker("__eq__", eq_maker)
+
+methods = {init_method, repr_method, eq_method}
+
+
+def annotationsclass(cls=None, *, kw_only=False):
+    if not cls:
+        return lambda cls_: annotationsclass(cls_, kw_only=kw_only)
+
+    return builder(
+        cls,
+        gatherer=annotated_gatherer,
+        methods=methods,
+        flags={"slotted": False, "kw_only": kw_only}
+    )
 
 
 @annotationsclass
 class X:
     x: str
     y: ClassVar[str] = "This is okay"
-    a: Annotated[int, Field(default=1)]
-    b: Annotated[str, Field(default="example")]
-    c: Annotated[list[str], Field(default_factory=list)]
-
-
-print(X("Testing"))
-print(X.y)
+    a: Annotated[int, NO_INIT] = "Not In __init__ signature"
+    b: Annotated[str, NO_REPR] = "Not In Repr"
+    c: Annotated[list[str], NO_COMPARE] = AnnoField(default_factory=list)
+    d: Annotated[str, IGNORE_ALL] = "Not Anywhere"
+    e: Annotated[str, KW_ONLY, NO_COMPARE]
+
+
+ex = X("Value of x", e="Value of e")
+
+print(ex, "\n")
+
+pp(get_fields(X))
+print("\nSource:")
+print(init_maker(X)[0])
+print(eq_maker(X)[0])
+print(repr_maker(X)[0])
 ```
```

### Comparing `ducktools_classbuilder-0.1.1/docs/index.md` & `ducktools_classbuilder-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/docs/make.bat` & `ducktools_classbuilder-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/docs/perf/performance_tests.md` & `ducktools_classbuilder-0.2.0/docs/perf/performance_tests.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/docs/prefab/index.md` & `ducktools_classbuilder-0.2.0/docs/prefab/index.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/pyproject.toml` & `ducktools_classbuilder-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/__init__.py` & `ducktools_classbuilder-0.2.0/src/ducktools/classbuilder/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,48 +15,64 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-__version__ = "v0.1.1"
+__version__ = "v0.2.0"
 
 # Change this name if you make heavy modifications
 INTERNALS_DICT = "__classbuilder_internals__"
 
 
 def get_internals(cls):
     """
     Utility function to get the internals dictionary
     or return None.
 
     As generated classes will always have 'fields'
     and 'local_fields' attributes this will always
     evaluate as 'truthy' if this is a generated class.
 
+    Generally you should use the helper get_flags and
+    get_fields methods.
+
     Usage:
        if internals := get_internals(cls):
            ...
 
     :param cls: generated class
     :return: internals dictionary of the class or None
     """
     return getattr(cls, INTERNALS_DICT, None)
 
 
-def get_fields(cls):
+def get_fields(cls, *, local=False):
     """
     Utility function to gather the fields dictionary
     from the class internals.
 
     :param cls: generated class
+    :param local: get only fields that were not inherited
     :return: dictionary of keys and Field attribute info
     """
-    return getattr(cls, INTERNALS_DICT)["fields"]
+    key = "local_fields" if local else "fields"
+    return getattr(cls, INTERNALS_DICT)[key]
+
+
+def get_flags(cls):
+    """
+    Utility function to gather the flags dictionary
+    from the class internals.
+
+    :param cls: generated class
+    :return: dictionary of keys and flag values
+    """
+    return getattr(cls, INTERNALS_DICT)["flags"]
 
 
 def get_inst_fields(inst):
     return {
         k: getattr(inst, k)
         for k in get_fields(type(inst))
     }
@@ -102,22 +118,23 @@
         setattr(cls, self.funcname, method)
 
         # Use 'get' to return the generated function as a bound method
         # instead of as a regular function for first usage.
         return method.__get__(instance, cls)
 
 
-def init_maker(cls, *, null=NOTHING, kw_only=False):
+def init_maker(cls, *, null=NOTHING):
     fields = get_fields(cls)
+    flags = get_flags(cls)
 
     arglist = []
     assignments = []
     globs = {}
 
-    if kw_only:
+    if flags.get("kw_only", False):
         arglist.append("*")
 
     for k, v in fields.items():
         if v.default is not null:
             globs[f"_{k}_default"] = v.default
             arg = f"{k}=_{k}_default"
             assignment = f"self.{k} = {k}"
@@ -176,31 +193,34 @@
 # Descriptor instances for every class.
 init_desc = MethodMaker("__init__", init_maker)
 repr_desc = MethodMaker("__repr__", repr_maker)
 eq_desc = MethodMaker("__eq__", eq_maker)
 default_methods = frozenset({init_desc, repr_desc, eq_desc})
 
 
-def builder(cls=None, /, *, gatherer, methods):
+def builder(cls=None, /, *, gatherer, methods, flags=None):
     """
     The main builder for class generation
 
     :param cls: Class to be analysed and have methods generated
     :param gatherer: Function to gather field information
     :type gatherer: Callable[[type], dict[str, Field]]
     :param methods: MethodMakers to add to the class
     :type methods: set[MethodMaker]
+    :param flags: additional flags to store in the internals dictionary
+                  for use by method generators.
     :return: The modified class (the class itself is modified, but this is expected).
     """
     # Handle `None` to make wrapping with a decorator easier.
     if cls is None:
         return lambda cls_: builder(
             cls_,
             gatherer=gatherer,
             methods=methods,
+            flags=flags,
         )
 
     internals = {}
     setattr(cls, INTERNALS_DICT, internals)
 
     cls_fields = gatherer(cls)
     internals["local_fields"] = cls_fields
@@ -208,19 +228,20 @@
     mro = cls.__mro__[:-1]  # skip 'object' base class
     if mro == (cls,):  # special case of no inheritance.
         fields = cls_fields.copy()
     else:
         fields = {}
         for c in reversed(mro):
             try:
-                fields.update(get_internals(c)["local_fields"])
+                fields.update(get_fields(c, local=True))
             except AttributeError:
                 pass
 
     internals["fields"] = fields
+    internals["flags"] = flags if flags is not None else {}
 
     # Assign all of the method generators
     for method in methods:
         setattr(cls, method.funcname, method)
 
     return cls
 
@@ -292,15 +313,16 @@
     "type": Field(default=NOTHING),
     "doc": Field(default=None),
 }
 
 builder(
     Field,
     gatherer=lambda cls_: _field_internal,
-    methods=frozenset({repr_desc, eq_desc})
+    methods=frozenset({repr_desc, eq_desc}),
+    flags={"slotted": True, "kw_only": True},
 )
 
 
 # Subclass of dict to be identifiable by isinstance checks
 # For anything more complicated this could be made into a Mapping
 class SlotFields(dict):
     """
@@ -364,15 +386,15 @@
     :param syntax_check: check there are no arguments without defaults
                         after arguments with defaults.
     :return: Modified class
     """
     if not cls:
         return lambda cls_: slotclass(cls_, methods=methods, syntax_check=syntax_check)
 
-    cls = builder(cls, gatherer=slot_gatherer, methods=methods)
+    cls = builder(cls, gatherer=slot_gatherer, methods=methods, flags={"slotted": True})
 
     if syntax_check:
         fields = get_fields(cls)
         used_default = False
         for k, v in fields.items():
             if v.default is NOTHING and v.default_factory is NOTHING:
                 if used_default:
@@ -394,25 +416,26 @@
     :param cls: Field subclass
     :return: Modified subclass
     """
 
     # Fields need a way to call their validate method
     # So append it to the code from __init__.
     def field_init_func(cls_):
-        code, globs = init_maker(cls_, null=field_nothing, kw_only=True)
+        code, globs = init_maker(cls_, null=field_nothing)
         code += "    self.validate_field()\n"
         return code, globs
 
     field_nothing = _NothingType()
     field_init_desc = MethodMaker(
         "__init__",
         field_init_func,
     )
     field_methods = frozenset({field_init_desc, repr_desc, eq_desc})
 
     cls = builder(
         cls,
         gatherer=slot_gatherer,
-        methods=field_methods
+        methods=field_methods,
+        flags={"slotted": True, "kw_only": True}
     )
 
     return cls
```

### Comparing `ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/__init__.pyi` & `ducktools_classbuilder-0.2.0/src/ducktools/classbuilder/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 _py_type = type  # Alias for type where it is used as a name
 
 __version__: str
 INTERNALS_DICT: str
 
 def get_internals(cls) -> dict[str, typing.Any] | None: ...
 
-def get_fields(cls: type) -> dict[str, Field]: ...
+def get_fields(cls: type, *, local: bool = False) -> dict[str, Field]: ...
+
+def get_flags(cls:type) -> dict[str, bool]: ...
 
 def get_inst_fields(inst: typing.Any) -> dict[str, typing.Any]: ...
 
 class _NothingType:
     ...
 NOTHING: _NothingType
 
@@ -26,15 +28,14 @@
     def __repr__(self) -> str: ...
     def __get__(self, instance, cls) -> Callable: ...
 
 def init_maker(
     cls: type,
     *,
     null: _NothingType = NOTHING,
-    kw_only: bool = False
 ) -> tuple[str, dict[str, typing.Any]]: ...
 def repr_maker(cls: type) -> tuple[str, dict[str, typing.Any]]: ...
 def eq_maker(cls: type) -> tuple[str, dict[str, typing.Any]]: ...
 
 init_desc: MethodMaker
 repr_desc: MethodMaker
 eq_desc: MethodMaker
@@ -44,24 +45,26 @@
 
 @typing.overload
 def builder(
     cls: type[_T],
     /,
     *,
     gatherer: Callable[[type], dict[str, Field]],
-    methods: frozenset[MethodMaker] | set[MethodMaker]
+    methods: frozenset[MethodMaker] | set[MethodMaker],
+    flags: dict[str, bool] | None = None,
 ) -> type[_T]: ...
 
 @typing.overload
 def builder(
     cls: None = None,
     /,
     *,
     gatherer: Callable[[type], dict[str, Field]],
-    methods: frozenset[MethodMaker] | set[MethodMaker]
+    methods: frozenset[MethodMaker] | set[MethodMaker],
+    flags: dict[str, bool] | None = None,
 ) -> Callable[[type[_T]], type[_T]]: ...
 
 
 class Field:
     default: _NothingType | typing.Any
     default_factory: _NothingType | typing.Any
     type: _NothingType | _py_type
```

### Comparing `ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/prefab.py` & `ducktools_classbuilder-0.2.0/src/ducktools/classbuilder/prefab.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 """
 
 import sys
 
 from . import (
     INTERNALS_DICT, NOTHING,
     Field, MethodMaker, SlotFields,
-    builder, fieldclass, get_internals, slot_gatherer
+    builder, fieldclass, get_flags, get_fields, slot_gatherer
 )
 
 PREFAB_FIELDS = "PREFAB_FIELDS"
 PREFAB_INIT_FUNC = "__prefab_init__"
 PRE_INIT_FUNC = "__prefab_pre_init__"
 POST_INIT_FUNC = "__prefab_post_init__"
 
@@ -80,18 +80,19 @@
     return getattr(cls, INTERNALS_DICT)["fields"]
 
 
 # Method Generators
 def get_init_maker(*, init_name="__init__"):
     def __init__(cls: "type") -> "tuple[str, dict]":
         globs = {}
-        internals = get_internals(cls)
         # Get the internals dictionary and prepare attributes
-        attributes = internals["fields"]
-        kw_only = internals["kw_only"]
+        attributes = get_attributes(cls)
+        flags = get_flags(cls)
+
+        kw_only = flags.get("kw_only", False)
 
         # Handle pre/post init first - post_init can change types for __init__
         # Get pre and post init arguments
         pre_init_args = []
         post_init_args = []
         post_init_annotations = {}
 
@@ -338,22 +339,24 @@
 
     return MethodMaker("__iter__", __iter__)
 
 
 def get_frozen_setattr_maker():
     def __setattr__(cls: "type") -> "tuple[str, dict]":
         globs = {}
-        internals = get_internals(cls)
-        field_names = internals["fields"].keys()
+        attributes = get_attributes(cls)
+        flags = get_flags(cls)
 
         # Make the fields set literal
-        fields_delimited = ", ".join(f"{field!r}" for field in field_names)
+        fields_delimited = ", ".join(f"{field!r}" for field in attributes)
         field_set = f"{{ {fields_delimited} }}"
 
-        if internals["slotted"]:
+        # Better to be safe and use the method that works in both cases
+        # if somehow slotted has not been set.
+        if flags.get("slotted", True):
             globs["__prefab_setattr_func"] = object.__setattr__
             setattr_method = "__prefab_setattr_func(self, name, value)"
         else:
             setattr_method = "self.__dict__[name] = value"
 
         body = (
             f"    if hasattr(self, name) or name not in {field_set}:\n"
@@ -484,14 +487,22 @@
         in_dict=in_dict,
         exclude_field=exclude_field,
         doc=doc,
         type=type,
     )
 
 
+def slot_prefab_gatherer(cls):
+    # For prefabs it's easier if everything is an attribute
+    return {
+        name: Attribute.from_field(fld)
+        for name, fld in slot_gatherer(cls).items()
+    }
+
+
 # Gatherer for classes built on attributes or annotations
 def attribute_gatherer(cls):
     cls_annotations = cls.__dict__.get("__annotations__", {})
     cls_annotation_names = cls_annotations.keys()
 
     cls_slots = cls.__dict__.get("__slots__", {})
 
@@ -595,15 +606,15 @@
         raise PrefabError(
             f"Decorated class {cls.__name__!r} "
             f"has already been processed as a Prefab."
         )
 
     slots = cls_dict.get("__slots__")
     if isinstance(slots, SlotFields):
-        gatherer = slot_gatherer
+        gatherer = slot_prefab_gatherer
         slotted = True
     else:
         gatherer = attribute_gatherer
         slotted = False
 
     methods = set()
 
@@ -623,26 +634,28 @@
         methods.add(iter_desc)
     if frozen:
         methods.add(frozen_setattr_desc)
         methods.add(frozen_delattr_desc)
     if dict_method:
         methods.add(asdict_desc)
 
+    flags = {
+        "kw_only": kw_only,
+        "slotted": slotted,
+    }
+
     cls = builder(
         cls,
         gatherer=gatherer,
         methods=methods,
+        flags=flags,
     )
 
-    # Add fields not covered by builder
-    internals = get_internals(cls)
-    internals["slotted"] = slotted
-    internals["kw_only"] = kw_only
-    fields = internals["fields"]
-    local_fields = internals["local_fields"]
+    # Get fields now the class has been built
+    fields = get_fields(cls)
 
     # Check pre_init and post_init functions if they exist
     try:
         func = getattr(cls, PRE_INIT_FUNC)
         func_code = func.__code__
     except AttributeError:
         pass
@@ -706,16 +719,14 @@
     valid_args = []
     for name, attrib in fields.items():
         # slot_gather and parent classes may use Fields
         # prefabs require Attributes, so convert.
         if not isinstance(attrib, Attribute):
             attrib = Attribute.from_field(attrib)
             fields[name] = attrib
-            if name in local_fields:
-                local_fields[name] = attrib
 
         # Excluded fields *MUST* be forwarded to post_init
         if attrib.exclude_field:
             if name not in post_init_args:
                 raise PrefabError(
                     f"{name!r} is an excluded attribute but is not passed to post_init"
                 )
```

### Comparing `ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/prefab.pyi` & `ducktools_classbuilder-0.2.0/src/ducktools/classbuilder/prefab.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,16 @@
     compare: bool = True,
     iter: bool = True,
     kw_only: bool = False,
     in_dict: bool = True,
     exclude_field: bool = False,
 ) -> Attribute: ...
 
+def slot_prefab_gatherer(cls: type) -> dict[str, Attribute]: ...
+
 def attribute_gatherer(cls: type) -> dict[str, Attribute]: ...
 
 def _make_prefab(
     cls: type,
     *,
     init: bool = True,
     repr: bool = True,
```

### Comparing `ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/PKG-INFO` & `ducktools_classbuilder-0.2.0/src/ducktools_classbuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducktools-classbuilder
-Version: 0.1.1
+Version: 0.2.0
 Summary: Toolkit for creating class boilerplate generators
 Author: David C Ellis
 License: MIT License
         
         Copyright (c) 2024 David C Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/SOURCES.txt` & `ducktools_classbuilder-0.2.0/src/ducktools_classbuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_construction.py` & `ducktools_classbuilder-0.2.0/tests/prefab/dynamic/test_construction.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_internals.py` & `ducktools_classbuilder-0.2.0/tests/prefab/dynamic/test_internals.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_pre_post_init.py` & `ducktools_classbuilder-0.2.0/tests/prefab/dynamic/test_pre_post_init.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_slotted_class.py` & `ducktools_classbuilder-0.2.0/tests/prefab/dynamic/test_slotted_class.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/creation.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/creation.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/dunders.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/dunders.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/inheritance.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/inheritance.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/init_ex.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/init_ex.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/kw_only.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/kw_only.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/repr_func.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/examples/repr_func.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/test_creation.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/test_creation.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/test_dunders.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/test_dunders.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/test_frozen.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/test_frozen.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/test_funcs.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/test_funcs.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/test_hint_syntax.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/test_hint_syntax.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/test_inheritance.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/test_init.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/test_init.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/test_kw_only.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/test_kw_only.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.1.1/tests/prefab/shared/test_repr.py` & `ducktools_classbuilder-0.2.0/tests/prefab/shared/test_repr.py`

 * *Files identical despite different names*

