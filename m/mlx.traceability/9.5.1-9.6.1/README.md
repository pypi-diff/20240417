# Comparing `tmp/mlx.traceability-9.5.1.tar.gz` & `tmp/mlx.traceability-9.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mlx.traceability-9.5.1.tar", last modified: Tue Nov 29 22:13:22 2022, max compression
+gzip compressed data, was "dist/mlx.traceability-9.6.1.tar", last modified: Wed Feb 22 13:24:14 2023, max compression
```

## Comparing `mlx.traceability-9.5.1.tar` & `mlx.traceability-9.6.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (122)       62 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      179 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2338 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (122)      357 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     2415 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    35141 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      652 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      196 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)     3608 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2193 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      929 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/doc/
--rw-r--r--   0 runner    (1001) docker     (122)      392 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/.env.example
--rw-r--r--   0 runner    (1001) docker     (122)     5744 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/doc/_static/css/
--rw-r--r--   0 runner    (1001) docker     (122)      299 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/_static/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (122)     1917 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/checklist.rst
--rw-r--r--   0 runner    (1001) docker     (122)    15807 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)    17154 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2416 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/contributing.rst
--rwxr-xr-x   0 runner    (1001) docker     (122)    14309 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/design.rst
--rw-r--r--   0 runner    (1001) docker     (122)      195 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/example_usage.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1091 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/goal.rst
--rwxr-xr-x   0 runner    (1001) docker     (122)      962 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/implementation.rst
--rwxr-xr-x   0 runner    (1001) docker     (122)      207 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      128 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (122)    19260 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/integration_test_report.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6984 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)      654 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/meeting_notes.rst
--rw-r--r--   0 runner    (1001) docker     (122)      635 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (122)     7502 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/requirements.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/doc/rqts/
--rwxr-xr-x   0 runner    (1001) docker     (122)      447 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/rqts/SRS.rst
--rwxr-xr-x   0 runner    (1001) docker     (122)      461 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/rqts/SSS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2736 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/unit_test.rst
--rw-r--r--   0 runner    (1001) docker     (122)    39018 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/doc/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/mlx/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/mlx/assets/
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/assets/traceability.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/mlx/directives/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2313 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/attribute_link_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     2124 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/attribute_sort_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/checkbox_result_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/checklist_item_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     5229 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/item_2d_matrix_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     2790 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/item_attribute_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     5976 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/item_attributes_matrix_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     9041 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/item_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     3928 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/item_link_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     2576 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/item_list_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)    34473 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/item_matrix_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)    23295 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/item_pie_chart_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     4490 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/item_relink_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     7092 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/directives/item_tree_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)    27590 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/traceability.py
--rw-r--r--   0 runner    (1001) docker     (122)     2110 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/traceability_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/traceable_attribute.py
--rw-r--r--   0 runner    (1001) docker     (122)     8563 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/traceable_base_class.py
--rw-r--r--   0 runner    (1001) docker     (122)    10214 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/traceable_base_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)    10067 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/traceable_base_node.py
--rw-r--r--   0 runner    (1001) docker     (122)    14508 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/traceable_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)    19321 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/mlx/traceable_item.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/mlx.traceability.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3608 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/mlx.traceability.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/mlx.traceability.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/mlx.traceability.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/mlx.traceability.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/mlx.traceability.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       74 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/mlx.traceability.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/mlx.traceability.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      118 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      271 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1963 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/tests/directives/
--rw-r--r--   0 runner    (1001) docker     (122)     2484 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/tests/directives/test_item_2d_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)     7270 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/tests/directives/test_item_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     1319 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/tests/directives/test_item_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)      763 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/tests/directives/test_item_pie_chart.py
--rw-r--r--   0 runner    (1001) docker     (122)     5348 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/tests/test_process_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     2595 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/tests/test_traceable_base_class.py
--rw-r--r--   0 runner    (1001) docker     (122)    21706 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/tests/test_traceable_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)    20225 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/tests/test_traceable_item.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 22:13:22.000000 mlx.traceability-9.5.1/tools/
--rw-r--r--   0 runner    (1001) docker     (122)      493 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/tools/doc-warnings.json
--rw-r--r--   0 runner    (1001) docker     (122)     2367 2022-11-29 22:13:00.000000 mlx.traceability-9.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/.env.example
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/doc/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/_static/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/checklist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14309 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/design.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/example_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/goal.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/implementation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19357 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/integration_test_report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/meeting_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7502 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/requirements.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/doc/rqts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/rqts/SRS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/rqts/SSS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/unit_test.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    39018 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/doc/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/mlx/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/mlx/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/assets/traceability.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/mlx/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/attribute_link_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/attribute_sort_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/checkbox_result_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/checklist_item_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/item_2d_matrix_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/item_attribute_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/item_attributes_matrix_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/item_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/item_link_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/item_list_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34473 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/item_matrix_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23295 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/item_pie_chart_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/item_relink_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/directives/item_tree_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28145 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/traceability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/traceability_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/traceable_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/traceable_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/traceable_base_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/traceable_base_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/traceable_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19321 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/mlx/traceable_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/mlx.traceability.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/mlx.traceability.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/mlx.traceability.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/mlx.traceability.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/mlx.traceability.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/mlx.traceability.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/mlx.traceability.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/mlx.traceability.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/tests/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/tests/directives/test_item_2d_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/tests/directives/test_item_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/tests/directives/test_item_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/tests/directives/test_item_pie_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/tests/test_process_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/tests/test_traceable_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21445 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/tests/test_traceable_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20225 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/tests/test_traceable_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:24:14.000000 mlx.traceability-9.6.1/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/tools/doc-warnings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-02-22 13:23:52.000000 mlx.traceability-9.6.1/tox.ini
```

### Comparing `mlx.traceability-9.5.1/.codeclimate.yml` & `mlx.traceability-9.6.1/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/.github/workflows/codeql-analysis.yml` & `mlx.traceability-9.6.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/.github/workflows/python-package.yml` & `mlx.traceability-9.6.1/.github/workflows/python-package.yml`

 * *Files 9% similar despite different names*

```diff
@@ -12,67 +12,67 @@
 jobs:
   test:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox tox-gh-actions
         sudo apt-get update -y
         sudo apt-get install -y latexmk texlive-latex-extra
         sudo apt-get install -y graphviz
         sudo apt-get install -y plantuml
     - name: Run test
       run: tox -e py
     - name: Build documentation with different Sphinx versions
-      run: tox -e sphinx2.1,sphinx-latest
+      run: tox -e sphinx2.4.5,sphinx-latest
     - name: Codecov
       if: matrix.python-version == 3.9
       run: tox -e codecov
     - name: Static checks
       if: matrix.python-version == 3.9
       run: tox -e check
     - name: Upload HTML documentation
       if: matrix.python-version == 3.9
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: html-doc
         path: doc/_build/html
 
   deploy:
 
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     needs: test
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Download HTML documentation from job 'test'
-      uses: actions/download-artifact@v2
+      uses: actions/download-artifact@v3
       with:
         name: html-doc
         path: doc/_build/html
     - name: Disable jekyll
       run: touch doc/_build/html/.nojekyll
     - name: Deploy documentation
-      uses: JamesIves/github-pages-deploy-action@4.1.3
+      uses: JamesIves/github-pages-deploy-action@v4
       with:
         branch: gh-pages
         folder: doc/_build/html
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.7'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
     - name: Build and publish
```

### Comparing `mlx.traceability-9.5.1/CONTRIBUTING.md` & `mlx.traceability-9.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/LICENSE.txt` & `mlx.traceability-9.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/MANIFEST.in` & `mlx.traceability-9.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/PKG-INFO` & `mlx.traceability-9.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: mlx.traceability
-Version: 9.5.1
+Version: 9.6.1
 Summary: Sphinx traceability extension (Melexis fork)
 Home-page: https://github.com/melexis/sphinx-traceability-extension
 Author: Melexis
 Author-email: jce@melexis.com
 License: GNU General Public License v3 (GPLv3)
+Project-URL: Documentation, https://melexis.github.io/sphinx-traceability-extension
+Project-URL: Source, https://github.com/melexis/sphinx-traceability-extension
+Project-URL: Tracker, https://github.com/melexis/sphinx-traceability-extension/issues
 Description: [![GPL3 License](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
         [![PyPI packaged release](https://badge.fury.io/py/mlx.traceability.svg)](https://badge.fury.io/py/mlx.traceability)
         [![Build status](https://github.com/melexis/sphinx-traceability-extension/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/melexis/sphinx-traceability-extension/actions/workflows/python-package.yml)
         [![Documentation](https://img.shields.io/badge/Documentation-published-brightgreen.svg)](https://melexis.github.io/sphinx-traceability-extension/)
         [![Code Coverage](https://codecov.io/gh/melexis/sphinx-traceability-extension/coverage.svg)](https://codecov.io/gh/melexis/sphinx-traceability-extension)
         [![Code Climate Status](https://codeclimate.com/github/melexis/sphinx-traceability-extension/badges/gpa.svg)](https://codeclimate.com/github/melexis/sphinx-traceability-extension)
         [![Requirements Status](https://requires.io/github/melexis/sphinx-traceability-extension/requirements.svg?branch=master)](https://requires.io/github/melexis/sphinx-traceability-extension/requirements/?branch=master)
```

### Comparing `mlx.traceability-9.5.1/README.md` & `mlx.traceability-9.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/SECURITY.md` & `mlx.traceability-9.6.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/doc/Makefile` & `mlx.traceability-9.6.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/doc/checklist.rst` & `mlx.traceability-9.6.1/doc/checklist.rst`

 * *Files 5% similar despite different names*

```diff
@@ -49,18 +49,14 @@
     Checklist items inherit from regular items.
 
 .. item:: CL-UNDEFINED_CL_ITEM Item that should be a checklist-item
 
     The item ID is present in the queried PR description, but won't get the configured checklist-attribute added since
     it's defined with the regular *item* directive.
 
-.. attribute-link::
-    :filter: CL-
-    :asil: A
-
 ---------------------------
 Matrices of checklist items
 ---------------------------
 
 .. item-attributes-matrix:: Questions and answers
     :filter: QUE-
     :attributes: checked
```

### Comparing `mlx.traceability-9.5.1/doc/conf.py` & `mlx.traceability-9.6.1/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath('../mlx'))
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-needs_sphinx = '1.8'
+needs_sphinx = '2.4.5'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.doctest',
     'sphinx.ext.coverage',
```

### Comparing `mlx.traceability-9.5.1/doc/configuration.rst` & `mlx.traceability-9.6.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/doc/contributing.rst` & `mlx.traceability-9.6.1/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/doc/design.rst` & `mlx.traceability-9.6.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/doc/goal.rst` & `mlx.traceability-9.6.1/doc/goal.rst`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/doc/implementation.rst` & `mlx.traceability-9.6.1/doc/implementation.rst`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/doc/integration_test_report.rst` & `mlx.traceability-9.6.1/doc/integration_test_report.rst`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 .. attribute-sort::
     :filter: r003
     :sort: status
 
 .. attribute-sort::
     :sort: aspice nonexistent
 
+.. process attribute-link before rendering matrices
+.. attribute-link::
+    :filter: CL-
+    :asil: A
+
 .. triggers a warning about r003 already having a configuration for attribute-sort
 
 .. item:: r001 First requirement
     :class: functional requirement
     :status: Draft
     :asil: C
     :aspice: 1
@@ -673,16 +678,16 @@
 
 Empty tree
 ----------
 
 .. item-tree:: Empty
     :top: this_regex_doesnt_match_anything
 
-Succesfull SYS tree
--------------------
+Successful trees
+----------------
 
 .. item-tree:: SYS
     :top: SYS
     :top_relation_filter: depends_on
     :type: fulfilled_by
 
 .. item-tree:: SYS (no captions)
```

### Comparing `mlx.traceability-9.5.1/doc/make.bat` & `mlx.traceability-9.6.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/doc/meeting_notes.rst` & `mlx.traceability-9.6.1/doc/meeting_notes.rst`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/doc/readme.rst` & `mlx.traceability-9.6.1/doc/readme.rst`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/doc/requirements.rst` & `mlx.traceability-9.6.1/doc/requirements.rst`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/doc/unit_test.rst` & `mlx.traceability-9.6.1/doc/unit_test.rst`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/doc/usage.rst` & `mlx.traceability-9.6.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/assets/traceability.js` & `mlx.traceability-9.6.1/mlx/assets/traceability.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,7 +1,8 @@
+// jQuery is included via the sphinxcontrib-jquery extension that we depend on
 // item-tree
 jQuery(function() {
     $('ul.bonsai').bonsai();
 });
 
 $(document).ready(function() {
     $('div.collapsible_links div.admonition.item').each(function(i) {
```

### Comparing `mlx.traceability-9.5.1/mlx/directives/attribute_link_directive.py` & `mlx.traceability-9.6.1/mlx/directives/attribute_sort_directive.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,62 @@
 from docutils.parsers.rst import directives
 
-from mlx.traceability_exception import TraceabilityException, report_warning
+from mlx.traceability import report_warning
 from mlx.traceable_base_directive import TraceableBaseDirective
 from mlx.traceable_base_node import TraceableBaseNode
 
 
-class AttributeLink(TraceableBaseNode):
-    """Node that adds one or more attributes to one or more items."""
+class AttributeSort(TraceableBaseNode):
+    """Node that configures the order of filtered items' attributes in the generated output."""
 
     def perform_replacement(self, app, collection):
-        """ Processes the attribute-link items.
+        """ Processes the attribute-sort items.
 
-        The AttributeLink node has no final representation, so it is removed from the tree.
+        The AttributeSort node has no final representation, so it is removed from the tree.
 
         Args:
             app: Sphinx application object to use.
             collection (TraceableCollection): Collection for which to generate the nodes.
         """
-        filtered_items = collection.get_item_objects(self['filter'])
-        for attribute, value in self['filter-attributes'].items():
-            for item in filtered_items:
-                if not self['nooverwrite'] or not item.get_attribute(attribute):
-                    try:
-                        item.add_attribute(attribute, value)
-                    except TraceabilityException as err:
-                        report_warning(err, self['document'], self['line'])
+        ignored_items = collection.add_attribute_sorting_rule(self['filter'], self['sort'])
+        for item in ignored_items:
+            report_warning("The sorting of the attributes of item {} has already been configured by {}; ignoring {}"
+                           .format(item.identifier, item.attribute_order, self['sort']), self['document'], self['line'])
         self.replace_self([])
 
 
-class AttributeLinkDirective(TraceableBaseDirective):
-    """ Directive to add attributes to items outside of the items' definition.
+class AttributeSortDirective(TraceableBaseDirective):
+    """
+    Directive to store the configuration of the order of filtered items' attributes.
 
     The node will be responsible for applying the configuration to the Item. First, all directives must be parsed.
 
     Syntax::
 
-      .. attribute-link::
+      .. attribute-sort::
          :filter: regex
-         :<<attribute>>: attribute_value
-         :nooverwrite:
+         :sort: list_of_attributes
     """
     # Options
     option_spec = {
         'filter': directives.unchanged,
-        'nooverwrite': directives.flag,
+        'sort': directives.unchanged,
     }
     # Content disallowed
     has_content = False
 
     def run(self):
         """ Processes the contents of the directive. Just store the configuration. """
         env = self.state.document.settings.env
 
-        node = AttributeLink('')
+        node = AttributeSort('')
         node['document'] = env.docname
         node['line'] = self.lineno
 
         self.process_options(
             node,
             {
+                'sort':   {'default': []},
                 'filter': {'default': r"\S+", 'is_pattern': True},
             },
         )
-        self.add_found_attributes(node)
-        self.check_option_presence(node, 'nooverwrite')
-
         return [node]
```

### Comparing `mlx.traceability-9.5.1/mlx/directives/attribute_sort_directive.py` & `mlx.traceability-9.6.1/mlx/directives/attribute_link_directive.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,75 @@
 from docutils.parsers.rst import directives
 
-from mlx.traceability import report_warning
+from mlx.traceability_exception import TraceabilityException, report_warning
 from mlx.traceable_base_directive import TraceableBaseDirective
 from mlx.traceable_base_node import TraceableBaseNode
 
 
-class AttributeSort(TraceableBaseNode):
-    """Node that configures the order of filtered items' attributes in the generated output."""
+class AttributeLink(TraceableBaseNode):
+    """Node that adds one or more attributes to one or more items."""
+    order = 3
 
     def perform_replacement(self, app, collection):
-        """ Processes the attribute-sort items.
-
-        The AttributeSort node has no final representation, so it is removed from the tree.
+        """ The AttributeLink node has no final representation, so it is removed from the tree.
 
         Args:
             app: Sphinx application object to use.
             collection (TraceableCollection): Collection for which to generate the nodes.
         """
-        ignored_items = collection.add_attribute_sorting_rule(self['filter'], self['sort'])
-        for item in ignored_items:
-            report_warning("The sorting of the attributes of item {} has already been configured by {}; ignoring {}"
-                           .format(item.identifier, item.attribute_order, self['sort']), self['document'], self['line'])
         self.replace_self([])
 
+    def apply_effect(self, collection):
+        """ Processes the attribute-link items, which shall be done before converting anything to docutils.
+
+        Args:
+            collection (TraceableCollection): Collection for which to generate the nodes.
+        """
+        filtered_items = collection.get_item_objects(self['filter'])
+        for attribute, value in self['filter-attributes'].items():
+            for item in filtered_items:
+                if not self['nooverwrite'] or not item.get_attribute(attribute):
+                    try:
+                        item.add_attribute(attribute, value)
+                    except TraceabilityException as err:
+                        report_warning(err, self['document'], self['line'])
 
-class AttributeSortDirective(TraceableBaseDirective):
-    """
-    Directive to store the configuration of the order of filtered items' attributes.
+
+class AttributeLinkDirective(TraceableBaseDirective):
+    """ Directive to add attributes to items outside of the items' definition.
 
     The node will be responsible for applying the configuration to the Item. First, all directives must be parsed.
 
     Syntax::
 
-      .. attribute-sort::
+      .. attribute-link::
          :filter: regex
-         :sort: list_of_attributes
+         :<<attribute>>: attribute_value
+         :nooverwrite:
     """
     # Options
     option_spec = {
         'filter': directives.unchanged,
-        'sort': directives.unchanged,
+        'nooverwrite': directives.flag,
     }
     # Content disallowed
     has_content = False
 
     def run(self):
         """ Processes the contents of the directive. Just store the configuration. """
         env = self.state.document.settings.env
 
-        node = AttributeSort('')
+        node = AttributeLink('')
         node['document'] = env.docname
         node['line'] = self.lineno
 
         self.process_options(
             node,
             {
-                'sort':   {'default': []},
                 'filter': {'default': r"\S+", 'is_pattern': True},
             },
         )
+        self.add_found_attributes(node)
+        self.check_option_presence(node, 'nooverwrite')
+
+        env.traceability_collection.add_intermediate_node(node)
         return [node]
```

### Comparing `mlx.traceability-9.5.1/mlx/directives/checkbox_result_directive.py` & `mlx.traceability-9.6.1/mlx/directives/checkbox_result_directive.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/directives/checklist_item_directive.py` & `mlx.traceability-9.6.1/mlx/directives/checklist_item_directive.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/directives/item_2d_matrix_directive.py` & `mlx.traceability-9.6.1/mlx/directives/item_2d_matrix_directive.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/directives/item_attribute_directive.py` & `mlx.traceability-9.6.1/mlx/directives/item_attribute_directive.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/directives/item_attributes_matrix_directive.py` & `mlx.traceability-9.6.1/mlx/directives/item_attributes_matrix_directive.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,24 +20,21 @@
                                         attributes=self['filter-attributes'],
                                         sortattributes=self['sort'],
                                         reverse=self['reverse'])
         top_node = self.create_top_node(self['title'])
         table = nodes.table()
         if self.get('classes'):
             table.get('classes').extend(self.get('classes'))
-        tgroup = nodes.tgroup()
         tbody = nodes.tbody()
-        colspecs = [nodes.colspec(colwidth=5)]
-        hrow = nodes.row('', nodes.entry('', nodes.paragraph('', '')))
+        titles = [nodes.paragraph('', '')]
 
         for item_id in item_ids:
             p_node = self.make_internal_item_ref(app, item_id)  # 1st col
             if self['transpose']:
-                colspecs.append(nodes.colspec(colwidth=5))
-                hrow.append(nodes.entry('', p_node))
+                titles.append(p_node)
             else:
                 row = nodes.row()
                 row.append(nodes.entry('', p_node))
                 item = collection.get_item(item_id)
                 self.fill_item_row(row, item)
                 tbody += row
 
@@ -45,19 +42,21 @@
             p_node = self.make_attribute_ref(app, attr)
             if self['transpose']:
                 row = nodes.row()
                 row.append(nodes.entry('', p_node))
                 self.fill_attribute_row(row, attr, item_ids, collection)
                 tbody += row
             else:
-                colspecs.append(nodes.colspec(colwidth=5))
-                hrow.append(nodes.entry('', p_node))
+                titles.append(p_node)
 
-        tgroup += colspecs
-        tgroup += nodes.thead('', hrow)
+        headings = [nodes.entry('', title) for title in titles]
+        number_of_columns = len(titles)
+        tgroup = nodes.tgroup()
+        tgroup += [nodes.colspec(colwidth=5) for _ in range(number_of_columns)]
+        tgroup += nodes.thead('', nodes.row('', *headings))
         tgroup += tbody
         table += tgroup
         top_node += table
         self.replace_self(top_node)
 
     def fill_item_row(self, row, item):
         """ Fills the row for one item with the specified attributes.
```

### Comparing `mlx.traceability-9.5.1/mlx/directives/item_directive.py` & `mlx.traceability-9.6.1/mlx/directives/item_directive.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/directives/item_link_directive.py` & `mlx.traceability-9.6.1/mlx/directives/item_link_directive.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/directives/item_list_directive.py` & `mlx.traceability-9.6.1/mlx/directives/item_list_directive.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/directives/item_matrix_directive.py` & `mlx.traceability-9.6.1/mlx/directives/item_matrix_directive.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/directives/item_pie_chart_directive.py` & `mlx.traceability-9.6.1/mlx/directives/item_pie_chart_directive.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/directives/item_relink_directive.py` & `mlx.traceability-9.6.1/mlx/directives/item_relink_directive.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/directives/item_tree_directive.py` & `mlx.traceability-9.6.1/mlx/directives/item_tree_directive.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/traceability.py` & `mlx.traceability-9.6.1/mlx/traceability.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 See readme for more details.
 """
 from collections import namedtuple
 from re import fullmatch, match
 from os import path
 
 from requests import Session
+from sphinx import version_info as sphinx_version
 from sphinx.roles import XRefRole
 from sphinx.util.nodes import make_refnode
 from sphinx.errors import NoUri
 from docutils import nodes
 from docutils.parsers.rst import directives
 
 from mlx.__traceability_version__ import version
@@ -468,14 +469,22 @@
 def setup(app):
     """Extension setup"""
     # Javascript and stylesheet for the tree-view
     app.add_js_file('https://cdn.rawgit.com/aexmachina/jquery-bonsai/master/jquery.bonsai.js')
     app.add_css_file('https://cdn.rawgit.com/aexmachina/jquery-bonsai/master/jquery.bonsai.css')
     app.add_js_file('traceability.js')
 
+    # Since Sphinx 6, jquery isn't bundled anymore and we need to ensure that
+    # the sphinxcontrib-jquery extension is enabled.
+    # See: https://dev.readthedocs.io/en/latest/design/sphinx-jquery.html
+    if sphinx_version >= (6, 0, 0):
+        # Documentation of Sphinx guarantees that an extension is added and enabled at most once.
+        # See: https://www.sphinx-doc.org/en/master/extdev/appapi.html#sphinx.application.Sphinx.setup_extension
+        app.setup_extension("sphinxcontrib.jquery")
+
     # Configuration for exporting collection to json
     app.add_config_value('traceability_json_export_path', None, 'env')
 
     # Configuration for adapting items through a callback while processing the ``item`` directives
     app.add_config_value('traceability_callback_per_item', None, 'env')
 
     # Configuration for inspecting items through a callback after all directives have been processed
```

### Comparing `mlx.traceability-9.5.1/mlx/traceability_exception.py` & `mlx.traceability-9.6.1/mlx/traceability_exception.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/traceable_attribute.py` & `mlx.traceability-9.6.1/mlx/traceable_attribute.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/traceable_base_class.py` & `mlx.traceability-9.6.1/mlx/traceable_base_class.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/traceable_base_directive.py` & `mlx.traceability-9.6.1/mlx/traceable_base_directive.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/traceable_base_node.py` & `mlx.traceability-9.6.1/mlx/traceable_base_node.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/traceable_collection.py` & `mlx.traceability-9.6.1/mlx/traceable_collection.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx/traceable_item.py` & `mlx.traceability-9.6.1/mlx/traceable_item.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/mlx.traceability.egg-info/PKG-INFO` & `mlx.traceability-9.6.1/mlx.traceability.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: mlx.traceability
-Version: 9.5.1
+Version: 9.6.1
 Summary: Sphinx traceability extension (Melexis fork)
 Home-page: https://github.com/melexis/sphinx-traceability-extension
 Author: Melexis
 Author-email: jce@melexis.com
 License: GNU General Public License v3 (GPLv3)
+Project-URL: Documentation, https://melexis.github.io/sphinx-traceability-extension
+Project-URL: Source, https://github.com/melexis/sphinx-traceability-extension
+Project-URL: Tracker, https://github.com/melexis/sphinx-traceability-extension/issues
 Description: [![GPL3 License](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
         [![PyPI packaged release](https://badge.fury.io/py/mlx.traceability.svg)](https://badge.fury.io/py/mlx.traceability)
         [![Build status](https://github.com/melexis/sphinx-traceability-extension/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/melexis/sphinx-traceability-extension/actions/workflows/python-package.yml)
         [![Documentation](https://img.shields.io/badge/Documentation-published-brightgreen.svg)](https://melexis.github.io/sphinx-traceability-extension/)
         [![Code Coverage](https://codecov.io/gh/melexis/sphinx-traceability-extension/coverage.svg)](https://codecov.io/gh/melexis/sphinx-traceability-extension)
         [![Code Climate Status](https://codeclimate.com/github/melexis/sphinx-traceability-extension/badges/gpa.svg)](https://codeclimate.com/github/melexis/sphinx-traceability-extension)
         [![Requirements Status](https://requires.io/github/melexis/sphinx-traceability-extension/requirements.svg?branch=master)](https://requires.io/github/melexis/sphinx-traceability-extension/requirements/?branch=master)
```

### Comparing `mlx.traceability-9.5.1/mlx.traceability.egg-info/SOURCES.txt` & `mlx.traceability-9.6.1/mlx.traceability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/setup.py` & `mlx.traceability-9.6.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 project_url = 'https://github.com/melexis/sphinx-traceability-extension'
 
 requires = [
-    'Sphinx>=2.1,<6.*',
+    'Sphinx>=2.4.5,<7.0',
+    'sphinxcontrib-jquery>=2.0.0,!=3.0.0',
     'docutils',
-    'matplotlib<4.*',
+    'matplotlib<4.0',
     'natsort',
     'python-decouple',
     'requests',
 ]
 
 setup(
     name='mlx.traceability',
@@ -22,14 +23,19 @@
     url=project_url,
     license='GNU General Public License v3 (GPLv3)',
     author='Melexis',
     author_email='jce@melexis.com',
     description='Sphinx traceability extension (Melexis fork)',
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
+    project_urls={
+        'Documentation': 'https://melexis.github.io/sphinx-traceability-extension',
+        'Source': 'https://github.com/melexis/sphinx-traceability-extension',
+        'Tracker': 'https://github.com/melexis/sphinx-traceability-extension/issues',
+    },
     zip_safe=False,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Environment :: Web Environment',
         'Framework :: Sphinx :: Extension',
         'Intended Audience :: Developers',
```

### Comparing `mlx.traceability-9.5.1/tests/directives/test_item_2d_matrix.py` & `mlx.traceability-9.6.1/tests/directives/test_item_2d_matrix.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/tests/directives/test_item_directive.py` & `mlx.traceability-9.6.1/tests/directives/test_item_directive.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 def raise_no_uri(*args, **kwargs):
     raise NoUri
 
 
 class TestItemDirective(TestCase):
 
     def setUp(self):
-        self.app = Mock(spec=Sphinx)
+        self.app = MagicMock(autospec=Sphinx)
         self.node = dut('')
         self.node['document'] = 'some_doc'
         self.node['id'] = 'some_id'
         self.node['line'] = 1
         self.item = TraceableItem(self.node['id'])
         self.item.set_location(self.node['document'], self.node['line'])
         self.item.node = self.node
         self.app.config = Mock()
         self.app.config.traceability_hyperlink_colors = {}
 
     def test_make_internal_item_ref_no_caption(self):
         mock_builder = MagicMock(spec=StandaloneHTMLBuilder)
         mock_builder.link_suffix = '.html'
-        mock_builder.env = BuildEnvironment()
+        mock_builder.env = BuildEnvironment(self.app)
         self.app.builder = mock_builder
         self.app.builder.env.traceability_collection = TraceableCollection()
         self.app.builder.env.traceability_ref_nodes = {}
         self.app.builder.env.traceability_collection.add_item(self.item)
         p_node = self.node.make_internal_item_ref(self.app, self.node['id'])
         ref_node = p_node.children[0]
         em_node = ref_node.children[0]
@@ -52,15 +52,15 @@
         self.assertEqual(p_node, cache['default'][f'{self.node["document"]}.html'])
         self.assertNotIn('nocaptions', cache)
         self.assertNotIn('onlycaptions', cache)
 
     def test_make_internal_item_ref_show_caption(self):
         mock_builder = MagicMock(spec=StandaloneHTMLBuilder)
         mock_builder.link_suffix = '.html'
-        mock_builder.env = BuildEnvironment()
+        mock_builder.env = BuildEnvironment(self.app)
         self.app.builder = mock_builder
         self.app.builder.env.traceability_collection = TraceableCollection()
         self.app.builder.env.traceability_ref_nodes = {}
         self.app.builder.env.traceability_collection.add_item(self.item)
         self.item.caption = 'caption text'
         p_node = self.node.make_internal_item_ref(self.app, self.node['id'])
         ref_node = p_node.children[0]
@@ -73,15 +73,15 @@
         self.assertEqual(em_node.rawsource, 'some_id : caption text')
         cache = self.app.builder.env.traceability_ref_nodes[self.node['id']]
         self.assertEqual(p_node, cache['default'][f'{self.node["document"]}.html'])
 
     def test_make_internal_item_ref_only_caption(self):
         mock_builder = MagicMock(spec=StandaloneHTMLBuilder)
         mock_builder.link_suffix = '.html'
-        mock_builder.env = BuildEnvironment()
+        mock_builder.env = BuildEnvironment(self.app)
         self.app.builder = mock_builder
         self.app.builder.env.traceability_collection = TraceableCollection()
         self.app.builder.env.traceability_ref_nodes = {}
         self.app.builder.env.traceability_collection.add_item(self.item)
         self.item.caption = 'caption text'
         self.node['nocaptions'] = True
         self.node['onlycaptions'] = True
@@ -98,15 +98,15 @@
         self.assertEqual(em_node.rawsource, 'caption text')
         cache = self.app.builder.env.traceability_ref_nodes[self.node['id']]
         self.assertEqual(p_node, cache['onlycaptions'][f'{self.node["document"]}.html'])
 
     def test_make_internal_item_ref_hide_caption_html(self):
         mock_builder = MagicMock(spec=StandaloneHTMLBuilder)
         mock_builder.link_suffix = '.html'
-        mock_builder.env = BuildEnvironment()
+        mock_builder.env = BuildEnvironment(self.app)
         self.app.builder = mock_builder
         self.app.builder.env.traceability_collection = TraceableCollection()
         self.app.builder.env.traceability_ref_nodes = {}
         self.app.builder.env.traceability_collection.add_item(self.item)
         self.item.caption = 'caption text'
         self.node['nocaptions'] = True
         p_node = self.node.make_internal_item_ref(self.app, self.node['id'])
@@ -122,15 +122,15 @@
         self.assertEqual(em_node.rawsource, 'some_id')
         cache = self.app.builder.env.traceability_ref_nodes[self.node['id']]
         self.assertEqual(p_node, cache['nocaptions'][f'{self.node["document"]}.html'])
 
     def test_make_internal_item_ref_hide_caption_latex(self):
         mock_builder = MagicMock(spec=LaTeXBuilder)
         mock_builder.get_relative_uri = Mock(side_effect=raise_no_uri)
-        mock_builder.env = BuildEnvironment()
+        mock_builder.env = BuildEnvironment(self.app)
         self.app.builder = mock_builder
         self.app.builder.env.traceability_collection = TraceableCollection()
         self.app.builder.env.traceability_ref_nodes = {}
         self.app.builder.env.traceability_collection.add_item(self.item)
         self.item.caption = 'caption text'
         self.node['nocaptions'] = True
         p_node = self.node.make_internal_item_ref(self.app, self.node['id'])
```

### Comparing `mlx.traceability-9.5.1/tests/directives/test_item_matrix.py` & `mlx.traceability-9.6.1/tests/directives/test_item_matrix.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/tests/directives/test_item_pie_chart.py` & `mlx.traceability-9.6.1/tests/directives/test_item_pie_chart.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/tests/test_process_options.py` & `mlx.traceability-9.6.1/tests/test_process_options.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/tests/test_traceable_base_class.py` & `mlx.traceability-9.6.1/tests/test_traceable_base_class.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/tests/test_traceable_collection.py` & `mlx.traceability-9.6.1/tests/test_traceable_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from unittest import TestCase
-try:
-    from unittest.mock import MagicMock, patch, mock_open
-except ImportError:
-    from mock import MagicMock, patch, mock_open
+from unittest.mock import patch, mock_open
 
 import mlx.traceable_item as item
 import mlx.traceable_attribute as attribute
 import mlx.traceability_exception as exception
 import mlx.traceable_collection as dut
 
 
@@ -385,18 +382,15 @@
     def test_export_no_items(self):
         open_mock = mock_open()
         coll = dut.TraceableCollection()
         with patch('mlx.traceable_collection.open', open_mock, create=True):
             coll.export(self.mock_export_file)
         open_mock.assert_called_once_with(self.mock_export_file, 'w')
 
-    @patch('mlx.traceable_collection.json', autospec=True)
-    def test_export_single_item(self, json_mock):
-        json_mock_object = MagicMock(spec=dut.json)
-        json_mock.return_value = json_mock_object
+    def test_export_single_item(self):
         open_mock = mock_open()
         coll = dut.TraceableCollection()
         item1 = item.TraceableItem(self.identification_src)
         coll.add_item(item1)
         with patch('mlx.traceable_collection.open', open_mock, create=True):
             coll.export(self.mock_export_file)
         open_mock.assert_called_once_with(self.mock_export_file, 'w')
```

### Comparing `mlx.traceability-9.5.1/tests/test_traceable_item.py` & `mlx.traceability-9.6.1/tests/test_traceable_item.py`

 * *Files identical despite different names*

### Comparing `mlx.traceability-9.5.1/tox.ini` & `mlx.traceability-9.6.1/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tox]
 envlist =
     py37, py38, py39, py10
     clean,
     check,
-    {sphinx2.1,sphinx-latest},
+    {sphinx2.4.5,sphinx-latest},
 
 [gh-actions]
 python =
     3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310
@@ -17,15 +17,15 @@
     py: python3
     pypy: {env:TOXPYTHON:pypy}
     py37: {env:TOXPYTHON:python3.7}
     py38: {env:TOXPYTHON:python3.8}
     py39: {env:TOXPYTHON:python3.9}
     py310: {env:TOXPYTHON:python3.10}
     {clean,check,report,coveralls,codecov}: python3
-    {sphinx2.1,sphinx-latest}: python3
+    {sphinx2.4.5,sphinx-latest}: python3
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
 passenv =
     *
 usedevelop = true
 deps=
@@ -34,15 +34,15 @@
     pytest-cov
     coverage
     reportlab
     natsort
     matplotlib
     sphinx-testing >= 0.5.2
     sphinx_selective_exclude>=1.0.3
-    sphinx_rtd_theme==0.5.2
+    sphinx_rtd_theme<2.0.0
     parameterized
 commands=
     {posargs:py.test --cov=mlx --cov-report=term-missing -vv tests/}
 
 [testenv:check]
 deps =
     docutils
@@ -54,34 +54,34 @@
 skip_install = true
 commands =
     python setup.py sdist
     twine check dist/*
     check-manifest {toxinidir} -u
     flake8 mlx tests setup.py --per-file-ignores mlx/directives/item_pie_chart_directive.py:E402
 
-[testenv:sphinx2.1]
+[testenv:sphinx2.4.5]
 deps=
     {[testenv]deps}
     jinja2 == 2.11.3
     markupsafe == 1.1.0
-    sphinx <= 2.1.9999  # rq.filter: <=2.1.9999
+    sphinx == 2.4.5  # rq.filter: ==2.4.5
     sphinxcontrib-plantuml
     mlx.warnings >= 1.3.0
 whitelist_externals =
     make
     tee
     mlx-warnings
 commands=
     mlx-warnings --config tools/doc-warnings.json --command make -C doc html
     mlx-warnings --config tools/doc-warnings.json --command make -C doc latexpdf
 
 [testenv:sphinx-latest]
 deps=
     {[testenv]deps}
-    sphinx<6.*
+    sphinx<7.0
     sphinxcontrib-plantuml
     mlx.warnings >= 1.3.0
 whitelist_externals =
     make
     tee
     mlx-warnings
 commands=
```

