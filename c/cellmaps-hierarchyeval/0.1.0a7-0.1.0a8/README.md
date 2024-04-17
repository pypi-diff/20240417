# Comparing `tmp/cellmaps_hierarchyeval-0.1.0a7.tar.gz` & `tmp/cellmaps_hierarchyeval-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmaps_hierarchyeval-0.1.0a7.tar", last modified: Tue Mar 12 21:17:47 2024, max compression
+gzip compressed data, was "dist/cellmaps_hierarchyeval-0.1.0a8.tar", last modified: Wed Apr 17 01:00:56 2024, max compression
```

## Comparing `cellmaps_hierarchyeval-0.1.0a7.tar` & `cellmaps_hierarchyeval-0.1.0a8.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-03-12 21:17:47.803656 cellmaps_hierarchyeval-0.1.0a7/
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      265 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/AUTHORS.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     3707 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/CONTRIBUTING.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)       89 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/HISTORY.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1102 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/LICENSE
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      262 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/MANIFEST.in
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     4761 2024-03-12 21:17:47.803598 cellmaps_hierarchyeval-0.1.0a7/PKG-INFO
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     3735 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/README.rst
-drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-03-12 21:17:47.795790 cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval/
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      314 2024-03-12 21:14:25.000000 cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval/__init__.py
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     6132 2024-03-12 21:05:29.000000 cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval/cellmaps_hierarchyevalcmd.py
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      142 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval/exceptions.py
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)    46934 2024-02-14 20:44:11.000000 cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval/runner.py
-drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-03-12 21:17:47.797024 cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval.egg-info/
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     4761 2024-03-12 21:17:47.000000 cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval.egg-info/PKG-INFO
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1359 2024-03-12 21:17:47.000000 cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval.egg-info/SOURCES.txt
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)        1 2024-03-12 21:17:47.000000 cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval.egg-info/dependency_links.txt
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)        1 2024-03-12 21:17:47.000000 cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval.egg-info/not-zip-safe
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)       64 2024-03-12 21:17:47.000000 cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval.egg-info/requires.txt
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)       23 2024-03-12 21:17:47.000000 cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval.egg-info/top_level.txt
-drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-03-12 21:17:47.800470 cellmaps_hierarchyeval-0.1.0a7/docs/
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      623 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/docs/Makefile
-drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-03-12 21:17:47.793578 cellmaps_hierarchyeval-0.1.0a7/docs/_build/
-drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-03-12 21:17:47.793647 cellmaps_hierarchyeval-0.1.0a7/docs/_build/html/
-drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-03-12 21:17:47.801025 cellmaps_hierarchyeval-0.1.0a7/docs/_build/html/_static/
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      286 2024-01-30 22:17:04.000000 cellmaps_hierarchyeval-0.1.0a7/docs/_build/html/_static/file.png
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)       90 2024-01-30 22:17:04.000000 cellmaps_hierarchyeval-0.1.0a7/docs/_build/html/_static/minus.png
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)       90 2024-01-30 22:17:04.000000 cellmaps_hierarchyeval-0.1.0a7/docs/_build/html/_static/plus.png
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)       28 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/docs/authors.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      819 2023-10-30 17:09:13.000000 cellmaps_hierarchyeval-0.1.0a7/docs/cellmaps_hierarchyeval.rst
--rwxr-xr-x   0 jlenkiewicz   (503) staff       (20)     6122 2024-03-07 21:48:15.000000 cellmaps_hierarchyeval-0.1.0a7/docs/conf.py
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)       33 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/docs/contributing.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      275 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/docs/developer.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)       28 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/docs/history.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1296 2024-03-12 16:14:20.000000 cellmaps_hierarchyeval-0.1.0a7/docs/index.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     6256 2024-02-29 23:50:19.000000 cellmaps_hierarchyeval-0.1.0a7/docs/inputs.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1238 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/docs/installation.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      466 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/docs/integrationtesting.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      820 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/docs/make.bat
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)       81 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/docs/modules.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     4400 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/docs/newrelease.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     7153 2024-02-13 23:21:23.000000 cellmaps_hierarchyeval-0.1.0a7/docs/outputs.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      792 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/docs/pypircfile.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1733 2024-02-13 23:21:23.000000 cellmaps_hierarchyeval-0.1.0a7/docs/usage.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      817 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/docs/versioningscheme.rst
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      405 2024-03-12 21:17:47.803914 cellmaps_hierarchyeval-0.1.0a7/setup.cfg
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     2278 2024-01-31 22:23:25.000000 cellmaps_hierarchyeval-0.1.0a7/setup.py
-drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-03-12 21:17:47.802768 cellmaps_hierarchyeval-0.1.0a7/tests/
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     8196 2024-02-02 01:25:05.000000 cellmaps_hierarchyeval-0.1.0a7/tests/.DS_Store
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)       77 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/tests/__init__.py
-drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-03-12 21:17:47.803239 cellmaps_hierarchyeval-0.1.0a7/tests/data/
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)    10536 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/tests/data/4nodehierarchy.cx
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)    17601 2024-01-10 16:59:23.000000 cellmaps_hierarchyeval-0.1.0a7/tests/data/hierarchy.cx
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)    19898 2024-01-10 16:59:23.000000 cellmaps_hierarchyeval-0.1.0a7/tests/data/hierarchy.cx2
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1944 2024-01-10 16:59:23.000000 cellmaps_hierarchyeval-0.1.0a7/tests/test_cellmaps_hierarchyevalcmd.py
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     2313 2024-01-10 16:59:23.000000 cellmaps_hierarchyeval-0.1.0a7/tests/test_cellmapshierarchyeval_enrichmentresult.py
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     3513 2024-02-14 20:44:11.000000 cellmaps_hierarchyeval-0.1.0a7/tests/test_cellmapshierarchyeval_enrichmentterms.py
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     7188 2024-01-10 16:59:23.000000 cellmaps_hierarchyeval-0.1.0a7/tests/test_cellmapshierarchyevalhelpers.py
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)     5661 2024-02-14 20:44:11.000000 cellmaps_hierarchyeval-0.1.0a7/tests/test_cellmapshierarchyevalrunner.py
--rw-r--r--   0 jlenkiewicz   (503) staff       (20)      807 2023-10-30 16:57:38.000000 cellmaps_hierarchyeval-0.1.0a7/tests/test_integration_cellmaps_hierarchyeval.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-17 01:00:56.073627 cellmaps_hierarchyeval-0.1.0a8/
+-rw-r--r--   0 churas     (504) staff       (20)      265 2023-08-07 23:13:47.000000 cellmaps_hierarchyeval-0.1.0a8/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3707 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-08-07 23:13:47.000000 cellmaps_hierarchyeval-0.1.0a8/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     5787 2024-04-17 01:00:56.074847 cellmaps_hierarchyeval-0.1.0a8/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     3735 2023-10-24 21:35:16.000000 cellmaps_hierarchyeval-0.1.0a8/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-17 01:00:56.031230 cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval/
+-rw-r--r--   0 churas     (504) staff       (20)      303 2024-04-17 00:59:28.000000 cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    16243 2024-04-17 00:59:28.000000 cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval/analysis.py
+-rw-r--r--   0 churas     (504) staff       (20)    11727 2024-04-17 00:59:28.000000 cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval/cellmaps_hierarchyevalcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      142 2023-08-04 18:11:01.000000 cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    51127 2024-04-17 00:59:28.000000 cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-17 01:00:56.033663 cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     5787 2024-04-17 01:00:55.000000 cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1422 2024-04-17 01:00:55.000000 cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2024-04-17 01:00:55.000000 cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2024-04-17 01:00:55.000000 cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       73 2024-04-17 01:00:55.000000 cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       23 2024-04-17 01:00:55.000000 cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-17 01:00:56.051234 cellmaps_hierarchyeval-0.1.0a8/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      623 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-17 01:00:56.022489 cellmaps_hierarchyeval-0.1.0a8/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-17 01:00:56.022584 cellmaps_hierarchyeval-0.1.0a8/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-17 01:00:56.054954 cellmaps_hierarchyeval-0.1.0a8/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_hierarchyeval-0.1.0a8/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_hierarchyeval-0.1.0a8/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_hierarchyeval-0.1.0a8/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1003 2024-03-28 22:57:07.000000 cellmaps_hierarchyeval-0.1.0a8/docs/cellmaps_hierarchyeval.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6122 2024-04-17 00:59:20.000000 cellmaps_hierarchyeval-0.1.0a8/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      275 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1296 2024-04-17 00:59:20.000000 cellmaps_hierarchyeval-0.1.0a8/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     6256 2024-03-02 00:50:06.000000 cellmaps_hierarchyeval-0.1.0a8/docs/inputs.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1238 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      466 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      820 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       81 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4400 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)     7153 2024-02-14 17:47:38.000000 cellmaps_hierarchyeval-0.1.0a8/docs/outputs.rst
+-rw-r--r--   0 churas     (504) staff       (20)      792 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1733 2024-02-14 17:47:38.000000 cellmaps_hierarchyeval-0.1.0a8/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      405 2024-04-17 01:00:56.078260 cellmaps_hierarchyeval-0.1.0a8/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2371 2024-04-17 00:59:28.000000 cellmaps_hierarchyeval-0.1.0a8/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-17 01:00:56.068229 cellmaps_hierarchyeval-0.1.0a8/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       77 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/tests/__init__.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-17 01:00:56.072011 cellmaps_hierarchyeval-0.1.0a8/tests/data/
+-rw-r--r--   0 churas     (504) staff       (20)    10536 2023-08-07 23:13:47.000000 cellmaps_hierarchyeval-0.1.0a8/tests/data/4nodehierarchy.cx
+-rw-r--r--   0 churas     (504) staff       (20)    17601 2023-11-16 16:55:42.000000 cellmaps_hierarchyeval-0.1.0a8/tests/data/hierarchy.cx
+-rw-r--r--   0 churas     (504) staff       (20)    19898 2023-11-16 16:55:42.000000 cellmaps_hierarchyeval-0.1.0a8/tests/data/hierarchy.cx2
+-rw-r--r--   0 churas     (504) staff       (20)     4327 2024-04-17 00:59:28.000000 cellmaps_hierarchyeval-0.1.0a8/tests/test_cellmaps_hierarchyevalcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     2313 2023-11-16 16:55:42.000000 cellmaps_hierarchyeval-0.1.0a8/tests/test_cellmapshierarchyeval_enrichmentresult.py
+-rw-r--r--   0 churas     (504) staff       (20)     3513 2024-03-02 00:49:56.000000 cellmaps_hierarchyeval-0.1.0a8/tests/test_cellmapshierarchyeval_enrichmentterms.py
+-rw-r--r--   0 churas     (504) staff       (20)     7188 2023-11-16 16:55:42.000000 cellmaps_hierarchyeval-0.1.0a8/tests/test_cellmapshierarchyevalhelpers.py
+-rw-r--r--   0 churas     (504) staff       (20)     8396 2024-04-17 00:59:28.000000 cellmaps_hierarchyeval-0.1.0a8/tests/test_cellmapshierarchyevalrunner.py
+-rw-r--r--   0 churas     (504) staff       (20)      807 2023-02-09 19:06:53.000000 cellmaps_hierarchyeval-0.1.0a8/tests/test_integration_cellmaps_hierarchyeval.py
+-rw-r--r--   0 churas     (504) staff       (20)     2028 2024-04-17 00:59:28.000000 cellmaps_hierarchyeval-0.1.0a8/tests/test_ollamacommandlinegenesetagent.py
```

### Comparing `cellmaps_hierarchyeval-0.1.0a7/CONTRIBUTING.rst` & `cellmaps_hierarchyeval-0.1.0a8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/LICENSE` & `cellmaps_hierarchyeval-0.1.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/README.rst` & `cellmaps_hierarchyeval-0.1.0a8/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval/runner.py` & `cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import logging
 import shutil
 import time
 import json
 import numpy as np
 from datetime import date
+from tqdm import tqdm
 
 from requests import RequestException, JSONDecodeError
 from scipy.stats import hypergeom
 from statsmodels.stats.multitest import multipletests
 import warnings
 import ndex2
 from ndex2.cx2 import CX2Network
@@ -257,14 +258,15 @@
                 for c in annotations:
                     if c in term_genes_dict:
                         term_genes_dict[c].append(node_name)
                     else:
                         term_genes_dict[c] = [node_name]
         return term_genes_dict, all_term_genes
 
+
 class EnrichmentResult(object):
     """
     Base class for representing the results of enrichment analysis.
     It generates a hierarchy that is output in the CX format following the CDAPS style.
     """
 
     def __init__(self,
@@ -468,15 +470,16 @@
 
             # write node attributes
             nodes_dict = hierarchy.get_nodes()
             for node_id, node_data in nodes_dict.items():
                 node_attributes = node_data["v"]
                 for attribute_name in node_attribute_names:
                     value = node_attributes.get(attribute_name, "")
-                    f.write(str(value) + '\t')
+                    cleaned_value = str(value).replace('\n', ' ').replace('\t', ' ')
+                    f.write(cleaned_value + '\t')
                 f.write('\n')
 
 
 class NiceCXNetworkHelper(BaseNetworkHelper):
     """
     Helper class for NiceCX network data manipulation that extends the
     BaseNetworkHelper class with CX-specific logic.
@@ -593,34 +596,100 @@
             for node_id, node_obj in hierarchy.get_nodes():
                 f.write(node_obj['n'] + '\t')
                 for a in hierarchy.get_node_attributes(node_obj):
                     f.write(str(a['v']) + '\t')
                 f.write('\n')
 
 
+class GeneSetAgentAnnotator(object):
+    """
+    Annotates hierarchy with results from one or more
+    :py:class:`~cellmaps_hierarchyeval.analysis.GeneSetAgent` objects
+    """
+    def __init__(self):
+        """
+        Constructor
+        """
+        self._hierarchy_helper = None
+        self._min_comp_size = 4
+
+    def set_hierarchy_helper(self, hierarchy_helper):
+        """
+        Sets HierarchyHelper
+
+        :param hierarchy_helper:
+        :return:
+        """
+        self._hierarchy_helper = hierarchy_helper
+
+    def set_minimum_comparison_size(self, val):
+        """
+        Only examine genesets of size **val** or larger
+        :param val:
+        :type val: int
+        """
+        self._min_comp_size = val
+
+    def annotate_hierarchy(self, geneset_agent=None,
+                           hierarchy=None):
+        """
+        Annotates hierarchy with
+        :py:class:`~cellmaps_hierarchyeval.analysis.GeneSetAgent`
+        by adding new node attributes
+        :param geneset_agent:
+        :param hierarchy:
+        :return:
+        """
+        for node_id, node in tqdm(self._hierarchy_helper.get_nodes(hierarchy).items(), desc='Assemblies'):
+            gene_names = self._hierarchy_helper.get_node_genes(hierarchy, node)
+            if gene_names is None or len(gene_names) == 0:
+                logger.debug('No genes to analyze')
+                hierarchy.set_node_attribute(node_id, f'{geneset_agent.get_attribute_name_prefix()}_process', '')
+                hierarchy.set_node_attribute(node_id, f'{geneset_agent.get_attribute_name_prefix()}_confidence', '')
+                hierarchy.set_node_attribute(node_id, f'{geneset_agent.get_attribute_name_prefix()}_raw', '')
+                continue
+            if len(gene_names) < self._min_comp_size:
+                logger.debug('Skipping node: ' + str(node_id) +
+                             ' has only ' + len(gene_names) +
+                             '  which is below threshold of ' +
+                             str(self._min_comp_size))
+                continue
+            proc_name, \
+                confidence, \
+                output = geneset_agent.annotate_gene_set(gene_names=gene_names)
+            print('Proc name: ' + str(proc_name))
+            print('confidence: ' + str(confidence))
+            hierarchy.set_node_attribute(node_id, f'{geneset_agent.get_attribute_name_prefix()}_process', proc_name)
+            hierarchy.set_node_attribute(node_id, f'{geneset_agent.get_attribute_name_prefix()}_confidence', confidence)
+            hierarchy.set_node_attribute(node_id, f'{geneset_agent.get_attribute_name_prefix()}_raw', output)
+
+
 class CellmapshierarchyevalRunner(object):
     """
     Class to run Hierarchy evaluation
     """
 
     def __init__(self, outdir=None,
                  hierarchy_dir=None,
                  min_comp_size=4,
                  max_fdr=0.05,
                  min_jaccard_index=0.1,
                  corum='764f7471-9b79-11ed-9a1f-005056ae23aa',
                  go_cc='f484e8ee-0b0f-11ee-aa50-005056ae23aa',
                  hpa='a6a88e2d-9c0f-11ed-9a1f-005056ae23aa',
                  ndex_server=None,
+                 geneset_agents=None,
                  name=None,
                  organization_name=None,
                  project_name=None,
                  input_data_dict=None,
+                 skip_term_enrichment=False,
                  skip_logging=True,
-                 provenance_utils=ProvenanceUtil()):
+                 provenance_utils=ProvenanceUtil(),
+                 geneset_annotator=GeneSetAgentAnnotator()):
         """
         Constructor
 
         :param outdir:
         :param hierarchy_dir: Output directory from cellmaps_generate_hierarchy
         :type hierarchy_dir: str
         :param min_comp_size:
@@ -660,24 +729,28 @@
         self._max_fdr = max_fdr
         self._min_jaccard_index = min_jaccard_index
         self._corum = corum
         self._go_cc = go_cc
         self._hpa = hpa
         self._ndex_server = ndex_server
         self._start_time = int(time.time())
+        self._geneset_agents = geneset_agents
         self._name = name
         self._project_name = project_name
         self._organization_name = organization_name
         self._input_data_dict = input_data_dict
         if skip_logging is None:
             self._skip_logging = False
         else:
             self._skip_logging = skip_logging
 
+        self._skip_term_enrichment = skip_term_enrichment
+
         self._provenance_utils = provenance_utils
+        self._geneset_annotator = geneset_annotator
         self._hierarchy_helper = None
         self._hierarchy_real_ids = []
 
     def _term_enrichment_hierarchy(self, hierarchy):
         """
         Performs term enrichment on the given hierarchy.
 
@@ -1090,14 +1163,30 @@
         if os.path.exists(cx2_file_path):
             self._hierarchy_helper = CX2NetworkHelper(cx2_file_path)
             return
 
         raise CellmapshierarchyevalError(f"Input directory '{self._hierarchy_dir}' does not contain neither cx nor cx2 "
                                          f"files.")
 
+    def _annotate_hierarchy_with_geneset_annotators(self, hierarchy=None):
+        """
+        Annotates hierarchy with each GeneSetAgent set in constructor.
+        """
+        if self._geneset_annotator is None:
+            logger.debug('Skipping because geneset_annotator is None')
+            return
+        if self._geneset_agents is None:
+            logger.debug('Skipping because there are no geneset agents')
+            return
+        self._geneset_annotator.set_hierarchy_helper(self._hierarchy_helper)
+        logger.debug('Processing ' + str(len(self._geneset_agents)) + ' geneset agents')
+        for a in tqdm(self._geneset_agents, desc='GeneSet Agents'):
+            self._geneset_annotator.annotate_hierarchy(hierarchy=hierarchy,
+                                                       geneset_agent=a)
+
     def run(self):
         """
         Evaluates CM4AI Hierarchy
 
         :return:
         """
         exitcode = 99
@@ -1123,15 +1212,22 @@
             # Initializes hierarchy helper
             self.initialize_hierarchy_helper()
 
             generated_dataset_ids = []
 
             # annotate hierarchy
             hierarchy = self._hierarchy_helper.get_hierarchy()
-            hierarchy = self._term_enrichment_hierarchy(hierarchy)
+            if self._skip_term_enrichment is None or self._skip_term_enrichment is False:
+                hierarchy = self._term_enrichment_hierarchy(hierarchy)
+            else:
+                logger.info('Skipping term enrichment because '
+                            'skip_term_enrichment flag is True')
+
+            self._annotate_hierarchy_with_geneset_annotators(hierarchy=hierarchy)
+
             self._update_annotate_hierarchy(hierarchy, self._outdir)
 
             # write out annotated hierarchy
             dataset_id = self._write_and_register_annotated_hierarchy(hierarchy)
             generated_dataset_ids.append(dataset_id)
 
             # write out parent network
```

### Comparing `cellmaps_hierarchyeval-0.1.0a7/cellmaps_hierarchyeval.egg-info/SOURCES.txt` & `cellmaps_hierarchyeval-0.1.0a8/cellmaps_hierarchyeval.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 cellmaps_hierarchyeval/__init__.py
+cellmaps_hierarchyeval/analysis.py
 cellmaps_hierarchyeval/cellmaps_hierarchyevalcmd.py
 cellmaps_hierarchyeval/exceptions.py
 cellmaps_hierarchyeval/runner.py
 cellmaps_hierarchyeval.egg-info/PKG-INFO
 cellmaps_hierarchyeval.egg-info/SOURCES.txt
 cellmaps_hierarchyeval.egg-info/dependency_links.txt
 cellmaps_hierarchyeval.egg-info/not-zip-safe
@@ -33,18 +34,18 @@
 docs/outputs.rst
 docs/pypircfile.rst
 docs/usage.rst
 docs/versioningscheme.rst
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
-tests/.DS_Store
 tests/__init__.py
 tests/test_cellmaps_hierarchyevalcmd.py
 tests/test_cellmapshierarchyeval_enrichmentresult.py
 tests/test_cellmapshierarchyeval_enrichmentterms.py
 tests/test_cellmapshierarchyevalhelpers.py
 tests/test_cellmapshierarchyevalrunner.py
 tests/test_integration_cellmaps_hierarchyeval.py
+tests/test_ollamacommandlinegenesetagent.py
 tests/data/4nodehierarchy.cx
 tests/data/hierarchy.cx
 tests/data/hierarchy.cx2
```

### Comparing `cellmaps_hierarchyeval-0.1.0a7/docs/Makefile` & `cellmaps_hierarchyeval-0.1.0a8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/docs/cellmaps_hierarchyeval.rst` & `cellmaps_hierarchyeval-0.1.0a8/docs/cellmaps_hierarchyeval.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 cellmaps\_hierarchyeval package
 ===============================
 
 Submodules
 ----------
 
+cellmaps\_hierarchyeval.analysis module
+---------------------------------------
+
+.. automodule:: cellmaps_hierarchyeval.analysis
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 cellmaps\_hierarchyeval.cellmaps\_hierarchyevalcmd module
 ---------------------------------------------------------
 
 .. automodule:: cellmaps_hierarchyeval.cellmaps_hierarchyevalcmd
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `cellmaps_hierarchyeval-0.1.0a7/docs/conf.py` & `cellmaps_hierarchyeval-0.1.0a8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/docs/index.rst` & `cellmaps_hierarchyeval-0.1.0a8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/docs/inputs.rst` & `cellmaps_hierarchyeval-0.1.0a8/docs/inputs.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/docs/installation.rst` & `cellmaps_hierarchyeval-0.1.0a8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/docs/make.bat` & `cellmaps_hierarchyeval-0.1.0a8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/docs/newrelease.rst` & `cellmaps_hierarchyeval-0.1.0a8/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/docs/outputs.rst` & `cellmaps_hierarchyeval-0.1.0a8/docs/outputs.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/docs/pypircfile.rst` & `cellmaps_hierarchyeval-0.1.0a8/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/docs/usage.rst` & `cellmaps_hierarchyeval-0.1.0a8/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/docs/versioningscheme.rst` & `cellmaps_hierarchyeval-0.1.0a8/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/setup.py` & `cellmaps_hierarchyeval-0.1.0a8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     history = history_file.read()
 
 requirements = ['cellmaps_utils',
                 'statsmodels',
                 'scipy',
                 'tqdm',
                 'numpy',
-                'ndex2>=3.6.0,<4.0.0']
+                'ndex2>=3.6.0,<4.0.0',
+                'requests']
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
     author=author,
@@ -57,14 +58,15 @@
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/x-rst',
     include_package_data=True,
     keywords='cellmaps_hierarchyeval',
     name='cellmaps_hierarchyeval',
     packages=find_packages(include=['cellmaps_hierarchyeval']),
     package_dir={'cellmaps_hierarchyeval': 'cellmaps_hierarchyeval'},
+package_data={'cellmaps_hierarchyeval': ['default_prompt.txt']},
     scripts=['cellmaps_hierarchyeval/cellmaps_hierarchyevalcmd.py'],
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url=repo_url,
     version=version,
     zip_safe=False)
```

### Comparing `cellmaps_hierarchyeval-0.1.0a7/tests/data/4nodehierarchy.cx` & `cellmaps_hierarchyeval-0.1.0a8/tests/data/4nodehierarchy.cx`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/tests/data/hierarchy.cx` & `cellmaps_hierarchyeval-0.1.0a8/tests/data/hierarchy.cx`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/tests/data/hierarchy.cx2` & `cellmaps_hierarchyeval-0.1.0a8/tests/data/hierarchy.cx2`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/tests/test_cellmapshierarchyeval_enrichmentresult.py` & `cellmaps_hierarchyeval-0.1.0a8/tests/test_cellmapshierarchyeval_enrichmentresult.py`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/tests/test_cellmapshierarchyeval_enrichmentterms.py` & `cellmaps_hierarchyeval-0.1.0a8/tests/test_cellmapshierarchyeval_enrichmentterms.py`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/tests/test_cellmapshierarchyevalhelpers.py` & `cellmaps_hierarchyeval-0.1.0a8/tests/test_cellmapshierarchyevalhelpers.py`

 * *Files identical despite different names*

### Comparing `cellmaps_hierarchyeval-0.1.0a7/tests/test_cellmapshierarchyevalrunner.py` & `cellmaps_hierarchyeval-0.1.0a8/tests/test_cellmapshierarchyevalrunner.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 import os
 import tempfile
 import shutil
 import unittest
 from unittest.mock import patch, Mock, MagicMock
 
 import ndex2
+from ndex2.cx2 import CX2Network
 from cellmaps_utils import constants
 from cellmaps_utils.provenance import ProvenanceUtil
 from requests import RequestException
 
+from cellmaps_hierarchyeval.analysis import FakeGeneSetAgent
 from cellmaps_hierarchyeval.exceptions import CellmapshierarchyevalError
 from cellmaps_hierarchyeval.runner import CellmapshierarchyevalRunner, NiceCXNetworkHelper, CX2NetworkHelper
 
-
+@unittest.skipIf(os.getenv('CELLMAPS_HIERARCHYEVAL_BAD_INTERNET') is not None, 'Too slow internet')
 class TestCellmapshierarchyevalrunner(unittest.TestCase):
     """Tests for `cellmaps_hierarchyeval` package."""
 
     def setUp(self):
         """Set up test fixtures, if any."""
         self.runner = CellmapshierarchyevalRunner('outdir')
         self.runner._hierarchy_dir = "mock_hierarchy_dir"
@@ -121,7 +123,58 @@
         node_ids = [1, 2, 3]
         self.runner._add_empty_attr_to_hierarchy(mock_hierarchy, mock_terms, node_ids=node_ids)
         expected_call_count = len(node_ids) * 5
 
         actual_call_count = mock_hierarchy.set_node_attribute.call_count
         self.assertEqual(expected_call_count, actual_call_count,
                          f"Expected set_node_attribute to be called {expected_call_count} times, got {actual_call_count}")
+
+    def test_annotate_hierarchy_with_geneset_annotators(self):
+        gsai = MagicMock()
+        gsai.get_attribute_name_prefix = MagicMock(return_val='foo::')
+        gsai.annotate_gene_set = MagicMock()
+        temp_dir = tempfile.mkdtemp()
+        try:
+            mockannotator = MagicMock()
+            mockannotator.annotate_hierarchy = MagicMock()
+            mockannotator.set_hierarchy_helper = MagicMock()
+            runner = CellmapshierarchyevalRunner(os.path.join(temp_dir, 'foo'),
+                                                 geneset_agents=[gsai],
+                                                 geneset_annotator=mockannotator)
+
+            hierarchy = CX2Network()
+            runner._annotate_hierarchy_with_geneset_annotators(hierarchy=hierarchy)
+            mockannotator.annotate_hierarchy.assert_called()
+            mockannotator.set_hierarchy_helper.assert_called()
+        finally:
+            shutil.rmtree(temp_dir)
+
+    def test_four_node_hierarchy(self):
+        temp_dir = tempfile.mkdtemp()
+        try:
+            agent = FakeGeneSetAgent()
+            runner = CellmapshierarchyevalRunner(os.path.join(temp_dir, 'foo'),
+                                                 geneset_agents=[agent])
+
+            hierhelper = CX2NetworkHelper(os.path.join(os.path.dirname(__file__),
+                                                       'data', 'hierarchy.cx2'))
+            hierarchy = hierhelper.get_hierarchy()
+            runner._hierarchy_helper = hierhelper
+            runner._annotate_hierarchy_with_geneset_annotators(hierarchy=hierarchy)
+            attributes_with_process = []
+            attributes_with_confidence = []
+            attributes_with_raw = []
+
+            for node, attrs in hierarchy.get_nodes().items():
+                for attr in attrs['v']:
+                    if attr.startswith('fake') and attr.endswith('_process'):
+                        attributes_with_process.append(attr)
+                    elif attr.startswith('fake') and attr.endswith('_confidence'):
+                        attributes_with_confidence.append(attr)
+                    elif attr.startswith('fake') and attr.endswith('_raw'):
+                        attributes_with_raw.append(attr)
+
+            self.assertEqual(len(attributes_with_process), len(hierarchy.get_nodes()))
+            self.assertEqual(len(attributes_with_confidence), len(hierarchy.get_nodes()))
+            self.assertEqual(len(attributes_with_raw), len(hierarchy.get_nodes()))
+        finally:
+            shutil.rmtree(temp_dir)
```

### Comparing `cellmaps_hierarchyeval-0.1.0a7/tests/test_integration_cellmaps_hierarchyeval.py` & `cellmaps_hierarchyeval-0.1.0a8/tests/test_integration_cellmaps_hierarchyeval.py`

 * *Files identical despite different names*

