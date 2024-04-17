# Comparing `tmp/meeteval-0.2.1.tar.gz` & `tmp/meeteval-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meeteval-0.2.1.tar", last modified: Tue Feb  6 09:59:37 2024, max compression
+gzip compressed data, was "meeteval-0.3.0.tar", last modified: Wed Apr 17 03:50:04 2024, max compression
```

## Comparing `meeteval-0.2.1.tar` & `meeteval-0.3.0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:59:37.755278 meeteval-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-02-06 09:59:26.000000 meeteval-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17609 2024-02-06 09:59:37.755278 meeteval-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15420 2024-02-06 09:59:26.000000 meeteval-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:59:37.739278 meeteval-0.2.1/meeteval/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:59:37.739278 meeteval-0.2.1/meeteval/der/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/der/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/der/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/der/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/der/md_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:59:37.743278 meeteval-0.2.1/meeteval/io/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15784 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/io/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/io/chime7.py
--rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/io/ctm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/io/keyed_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/io/load_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/io/pbjson.py
--rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/io/py.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/io/rttm.py
--rw-r--r--   0 runner    (1001) docker     (127)    23011 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/io/seglst.py
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/io/stm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/io/uem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:59:37.743278 meeteval-0.2.1/meeteval/viz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/viz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/viz/file_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/viz/visualize.css
--rw-r--r--   0 runner    (1001) docker     (127)    71415 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/viz/visualize.js
--rw-r--r--   0 runner    (1001) docker     (127)    20964 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/viz/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:59:37.743278 meeteval-0.2.1/meeteval/wer/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20525 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:59:37.751278 meeteval-0.2.1/meeteval/wer/matching/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1412126 2024-02-06 09:59:36.000000 meeteval-0.2.1/meeteval/wer/matching/cy_levenshtein.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13387 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/matching/cy_levenshtein.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   530566 2024-02-06 09:59:36.000000 meeteval-0.2.1/meeteval/wer/matching/cy_mimo_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14310 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/matching/cy_mimo_matching.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   393287 2024-02-06 09:59:37.000000 meeteval-0.2.1/meeteval/wer/matching/cy_orc_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/matching/cy_orc_matching.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   481230 2024-02-06 09:59:37.000000 meeteval-0.2.1/meeteval/wer/matching/cy_time_constrained_orc_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/matching/cy_time_constrained_orc_matching.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    19088 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/matching/levenshtein.h
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/matching/mimo_matching.h
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/matching/mimo_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/matching/orc_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    22255 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/matching/time_constrained_orc_matching.h
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:59:37.751278 meeteval-0.2.1/meeteval/wer/wer/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/wer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17597 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/wer/cp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/wer/error_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/wer/mimo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/wer/orc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/wer/siso.py
--rw-r--r--   0 runner    (1001) docker     (127)    41636 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/wer/time_constrained.py
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/wer/time_constrained_orc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-02-06 09:59:26.000000 meeteval-0.2.1/meeteval/wer/wer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:59:37.755278 meeteval-0.2.1/meeteval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17609 2024-02-06 09:59:37.000000 meeteval-0.2.1/meeteval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-02-06 09:59:37.000000 meeteval-0.2.1/meeteval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 09:59:37.000000 meeteval-0.2.1/meeteval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-06 09:59:37.000000 meeteval-0.2.1/meeteval.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-06 09:59:37.000000 meeteval-0.2.1/meeteval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-06 09:59:37.000000 meeteval-0.2.1/meeteval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-06 09:59:26.000000 meeteval-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 09:59:37.755278 meeteval-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-02-06 09:59:26.000000 meeteval-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:59:37.755278 meeteval-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-02-06 09:59:26.000000 meeteval-0.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-02-06 09:59:26.000000 meeteval-0.2.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-06 09:59:26.000000 meeteval-0.2.1/tests/test_levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-02-06 09:59:26.000000 meeteval-0.2.1/tests/test_mimo_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-02-06 09:59:26.000000 meeteval-0.2.1/tests/test_orc_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-02-06 09:59:26.000000 meeteval-0.2.1/tests/test_python_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-06 09:59:26.000000 meeteval-0.2.1/tests/test_shell_vs_py.py
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-02-06 09:59:26.000000 meeteval-0.2.1/tests/test_time_constrained.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-02-06 09:59:26.000000 meeteval-0.2.1/tests/test_time_constrained_orc_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:50:04.224740 meeteval-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-17 03:49:57.000000 meeteval-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17801 2024-04-17 03:50:04.224740 meeteval-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15251 2024-04-17 03:49:57.000000 meeteval-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:50:04.204740 meeteval-0.3.0/meeteval/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:50:04.208740 meeteval-0.3.0/meeteval/der/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/der/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/der/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/der/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/der/md_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:50:04.208740 meeteval-0.3.0/meeteval/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15784 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/io/chime7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/io/ctm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/io/keyed_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/io/load_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/io/pbjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/io/py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/io/rttm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26269 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/io/seglst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/io/stm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/io/uem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:50:04.212740 meeteval-0.3.0/meeteval/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/viz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/viz/file_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/viz/side_by_side_sync.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/viz/visualize.css
+-rw-r--r--   0 runner    (1001) docker     (127)    99277 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/viz/visualize.js
+-rw-r--r--   0 runner    (1001) docker     (127)    28486 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/viz/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:50:04.212740 meeteval-0.3.0/meeteval/wer/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21771 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:50:04.216740 meeteval-0.3.0/meeteval/wer/matching/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1412614 2024-04-17 03:50:03.000000 meeteval-0.3.0/meeteval/wer/matching/cy_levenshtein.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13387 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/matching/cy_levenshtein.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   531036 2024-04-17 03:50:03.000000 meeteval-0.3.0/meeteval/wer/matching/cy_mimo_matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14310 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/matching/cy_mimo_matching.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   393757 2024-04-17 03:50:03.000000 meeteval-0.3.0/meeteval/wer/matching/cy_orc_matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/matching/cy_orc_matching.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   482920 2024-04-17 03:50:03.000000 meeteval-0.3.0/meeteval/wer/matching/cy_time_constrained_orc_matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/matching/cy_time_constrained_orc_matching.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    19088 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/matching/levenshtein.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/matching/mimo_matching.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/matching/mimo_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/matching/orc_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22255 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/matching/time_constrained_orc_matching.h
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:50:04.216740 meeteval-0.3.0/meeteval/wer/wer/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/wer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20404 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/wer/cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/wer/error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/wer/mimo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/wer/orc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/wer/siso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41676 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/wer/time_constrained.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/wer/time_constrained_orc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-17 03:49:57.000000 meeteval-0.3.0/meeteval/wer/wer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:50:04.220740 meeteval-0.3.0/meeteval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17801 2024-04-17 03:50:04.000000 meeteval-0.3.0/meeteval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-17 03:50:04.000000 meeteval-0.3.0/meeteval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 03:50:04.000000 meeteval-0.3.0/meeteval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-17 03:50:04.000000 meeteval-0.3.0/meeteval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-17 03:50:04.000000 meeteval-0.3.0/meeteval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 03:50:04.000000 meeteval-0.3.0/meeteval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-17 03:49:57.000000 meeteval-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 03:50:04.224740 meeteval-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-17 03:49:57.000000 meeteval-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:50:04.220740 meeteval-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-17 03:49:57.000000 meeteval-0.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-17 03:49:57.000000 meeteval-0.3.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-17 03:49:57.000000 meeteval-0.3.0/tests/test_levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-17 03:49:57.000000 meeteval-0.3.0/tests/test_mimo_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-17 03:49:57.000000 meeteval-0.3.0/tests/test_orc_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-17 03:49:57.000000 meeteval-0.3.0/tests/test_python_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 03:49:57.000000 meeteval-0.3.0/tests/test_shell_vs_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10383 2024-04-17 03:49:57.000000 meeteval-0.3.0/tests/test_time_constrained.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-04-17 03:49:57.000000 meeteval-0.3.0/tests/test_time_constrained_orc_matching.py
```

### Comparing `meeteval-0.2.1/LICENSE` & `meeteval-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/PKG-INFO` & `meeteval-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meeteval
-Version: 0.2.1
+Version: 0.3.0
 Home-page: https://github.com/fgnt/meeteval/
 Author: Department of Communications Engineering, Paderborn University
 Author-email: sek@nt.upb.de
 License: MIT
 Keywords: speech recognition,word error rate,evaluation,meeting,ASR,WER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -24,44 +24,53 @@
 Requires-Dist: Cython
 Provides-Extra: cli
 Requires-Dist: pyyaml; extra == "cli"
 Requires-Dist: fire; extra == "cli"
 Requires-Dist: simplejson; extra == "cli"
 Requires-Dist: aiohttp; extra == "cli"
 Requires-Dist: soundfile; extra == "cli"
+Requires-Dist: tqdm; extra == "cli"
+Requires-Dist: yattag; extra == "cli"
+Requires-Dist: platformdirs; extra == "cli"
 Provides-Extra: test
 Requires-Dist: editdistance; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
-Requires-Dist: click; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: ipython; extra == "test"
 Requires-Dist: pyyaml; extra == "test"
+Requires-Dist: fire; extra == "test"
 Requires-Dist: simplejson; extra == "test"
 Requires-Dist: aiohttp; extra == "test"
 Requires-Dist: soundfile; extra == "test"
+Requires-Dist: tqdm; extra == "test"
+Requires-Dist: yattag; extra == "test"
+Requires-Dist: platformdirs; extra == "test"
 Provides-Extra: all
+Requires-Dist: lazy_dataset; extra == "all"
+Requires-Dist: ipywidgets; extra == "all"
 Requires-Dist: pyyaml; extra == "all"
 Requires-Dist: fire; extra == "all"
 Requires-Dist: simplejson; extra == "all"
 Requires-Dist: aiohttp; extra == "all"
 Requires-Dist: soundfile; extra == "all"
+Requires-Dist: tqdm; extra == "all"
+Requires-Dist: yattag; extra == "all"
+Requires-Dist: platformdirs; extra == "all"
 Requires-Dist: editdistance; extra == "all"
 Requires-Dist: pytest; extra == "all"
 Requires-Dist: hypothesis; extra == "all"
-Requires-Dist: click; extra == "all"
 Requires-Dist: coverage; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
 Requires-Dist: ipython; extra == "all"
-Requires-Dist: lazy_dataset; extra == "all"
 
 <h1 align="center">MeetEval</h1> 
 <h3 align="center">A meeting transcription evaluation toolkit</h3>
-<div align="center"><a href="#features">Features</a> | <a href="#installation">Installation</a> | <a href="#python-interface">Python Interface</a> | <a href="#command-line-interface">Command Line Interface</a> | <a href="#visualization-wip">Visualization (WIP)</a> | <a href="#cite">Cite</a></div>
+<div align="center"><a href="#features">Features</a> | <a href="#installation">Installation</a> | <a href="#python-interface">Python Interface</a> | <a href="#command-line-interface">Command Line Interface</a> | <a href="#visualization">Visualization</a> | <a href="#cite">Cite</a></div>
 <br>
 <a href="https://github.com/fgnt/meeteval/actions"><img src="https://github.com/fgnt/meeteval/actions/workflows/pytest.yml/badge.svg"/></a>
 
 
 ## Features
 MeetEval supports the following metrics for meeting transcription evaluation:
 
@@ -76,15 +85,15 @@
 - **Time-Constrained minimum-Permutation Word Error Rate (tcpWER)**<br>
   `meeteval-wer tcpwer -r ref.stm -h hyp.stm --collar 5`
 - **Time-Constrained Optimal Reference Combination Word Error Rate (tcORC WER)**<br>
   `meeteval-wer tcorcwer -r ref.stm -h hyp.stm --collar 5`
 - **Diarization Error Rate (DER)** by wrapping [mdeval](https://github.com/nryant/dscore/raw/master/scorelib/md-eval-22.pl)<br>
   `meeteval-der md_eval_22 -r ref.stm -h hyp.stm --collar .25`
 
-Additionally (WIP), MeetEval contains a [visualization](#visualization-wip) tool for cpWER and tcpWER alignments that help spot errors in system outputs.
+Additionally, MeetEval contains a [visualization](#visualization) tool for cpWER and tcpWER alignments that helps to spot errors in system outputs.
 
 ## Installation
 
 ### From PyPI
 
 ```shell
 pip install meeteval
@@ -99,15 +108,15 @@
 
 ## Command-line interface
 
 `MeetEval` supports the following file formats as input:
  - [Segmental Time Mark](https://github.com/usnistgov/SCTK/blob/master/doc/infmts.htm#L75) (`STM`)
  - [Time Marked Conversation](https://github.com/usnistgov/SCTK/blob/master/doc/infmts.htm#L286) (`CTM`)
  - [SEGment-wise Long-form Speech Transcription annotation](#segment-wise-long-form-speech-transcription-annotation-seglst) (`SegLST`), the file format used in the [CHiME challenges](https://www.chimechallenge.org)
- - [Rich Transcription Time Marked](https://github.com/nryant/dscore?tab=readme-ov-file#rttm) (`RTTM`) files (only for Diarizaiton Error Rate)
+ - [Rich Transcription Time Marked](https://github.com/nryant/dscore?tab=readme-ov-file#rttm) (`RTTM`) files (only for Diarization Error Rate)
 
 
 > [!NOTE]
 > `MeetEval` does not support alternate transcripts (e.g., `"i've { um / uh / @ } as far as i'm concerned"`).
 
 The command-line interface is available as `meeteval-wer` or `python -m meeteval.wer` with the following signature:
 
@@ -325,20 +334,18 @@
 Sequences can be aligned, similar to `kaldialign.align`, using the tcpWER matching:
 ```python
 import meeteval
 meeteval.wer.wer.time_constrained.align([{'words': 'a b', 'start_time': 0, 'end_time': 1}], [{'words': 'a c', 'start_time': 0, 'end_time': 1}, {'words': 'd', 'start_time': 2, 'end_time': 3}])
 # [('a', 'a'), ('b', 'c'), ('*', 'd')]
 ```
 
-## Visualization [WIP]
+## Visualization
 
-> [!IMPORTANT]
-> The visualization is under development! <br>
-> Preview: https://groups.uni-paderborn.de/nt/meeteval/viz.html<br>
-> Interactive notebook: https://fgnt.github.io/meeteval_jupyterlite/lab?path=Demo.ipynb
+> [!TIP]
+> Try it in the browser! https://fgnt.github.com/meeteval_viz
 
 ```python
 import meeteval
 from meeteval.viz.visualize import AlignmentVisualization
 
 folder = r'https://raw.githubusercontent.com/fgnt/meeteval/main/'
 av = AlignmentVisualization(
```

#### html2text {}

```diff
@@ -1,40 +1,45 @@
-Metadata-Version: 2.1 Name: meeteval Version: 0.2.1 Home-page: https://
+Metadata-Version: 2.1 Name: meeteval Version: 0.3.0 Home-page: https://
 github.com/fgnt/meeteval/ Author: Department of Communications Engineering,
 Paderborn University Author-email: sek@nt.upb.de License: MIT Keywords: speech
 recognition,word error rate,evaluation,meeting,ASR,WER Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Python: >=3.5 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: kaldialign Requires-Dist: scipy Requires-
 Dist: typing_extensions; python_version < "3.8" Requires-Dist: cached_property;
 python_version < "3.8" Requires-Dist: Cython Provides-Extra: cli Requires-Dist:
 pyyaml; extra == "cli" Requires-Dist: fire; extra == "cli" Requires-Dist:
 simplejson; extra == "cli" Requires-Dist: aiohttp; extra == "cli" Requires-
-Dist: soundfile; extra == "cli" Provides-Extra: test Requires-Dist:
-editdistance; extra == "test" Requires-Dist: pytest; extra == "test" Requires-
-Dist: hypothesis; extra == "test" Requires-Dist: click; extra == "test"
+Dist: soundfile; extra == "cli" Requires-Dist: tqdm; extra == "cli" Requires-
+Dist: yattag; extra == "cli" Requires-Dist: platformdirs; extra == "cli"
+Provides-Extra: test Requires-Dist: editdistance; extra == "test" Requires-
+Dist: pytest; extra == "test" Requires-Dist: hypothesis; extra == "test"
 Requires-Dist: coverage; extra == "test" Requires-Dist: pytest-cov; extra ==
 "test" Requires-Dist: ipython; extra == "test" Requires-Dist: pyyaml; extra ==
-"test" Requires-Dist: simplejson; extra == "test" Requires-Dist: aiohttp; extra
-== "test" Requires-Dist: soundfile; extra == "test" Provides-Extra: all
-Requires-Dist: pyyaml; extra == "all" Requires-Dist: fire; extra == "all"
+"test" Requires-Dist: fire; extra == "test" Requires-Dist: simplejson; extra ==
+"test" Requires-Dist: aiohttp; extra == "test" Requires-Dist: soundfile; extra
+== "test" Requires-Dist: tqdm; extra == "test" Requires-Dist: yattag; extra ==
+"test" Requires-Dist: platformdirs; extra == "test" Provides-Extra: all
+Requires-Dist: lazy_dataset; extra == "all" Requires-Dist: ipywidgets; extra ==
+"all" Requires-Dist: pyyaml; extra == "all" Requires-Dist: fire; extra == "all"
 Requires-Dist: simplejson; extra == "all" Requires-Dist: aiohttp; extra ==
-"all" Requires-Dist: soundfile; extra == "all" Requires-Dist: editdistance;
-extra == "all" Requires-Dist: pytest; extra == "all" Requires-Dist: hypothesis;
-extra == "all" Requires-Dist: click; extra == "all" Requires-Dist: coverage;
-extra == "all" Requires-Dist: pytest-cov; extra == "all" Requires-Dist:
-ipython; extra == "all" Requires-Dist: lazy_dataset; extra == "all"
+"all" Requires-Dist: soundfile; extra == "all" Requires-Dist: tqdm; extra ==
+"all" Requires-Dist: yattag; extra == "all" Requires-Dist: platformdirs; extra
+== "all" Requires-Dist: editdistance; extra == "all" Requires-Dist: pytest;
+extra == "all" Requires-Dist: hypothesis; extra == "all" Requires-Dist:
+coverage; extra == "all" Requires-Dist: pytest-cov; extra == "all" Requires-
+Dist: ipython; extra == "all"
                             ************ MMeeeettEEvvaall ************
              ******** AA mmeeeettiinngg ttrraannssccrriippttiioonn eevvaalluuaattiioonn ttoooollkkiitt ********
      _F_e_a_t_u_r_e_s | _I_n_s_t_a_l_l_a_t_i_o_n | _P_y_t_h_o_n_ _I_n_t_e_r_f_a_c_e | _C_o_m_m_a_n_d_ _L_i_n_e_ _I_n_t_e_r_f_a_c_e |
-                          _V_i_s_u_a_l_i_z_a_t_i_o_n_ _(_W_I_P_) | _C_i_t_e
+                             _V_i_s_u_a_l_i_z_a_t_i_o_n | _C_i_t_e
 
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_f_g_n_t_/_m_e_e_t_e_v_a_l_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_p_y_t_e_s_t_._y_m_l_/_b_a_d_g_e_._s_v_g_]##
 Features MeetEval supports the following metrics for meeting transcription
 evaluation: - **Standard WER** for single utterances (Called SISO WER in
 MeetEval)
 `meeteval-wer wer -r ref -h hyp` - **Concatenated minimum-Permutation Word
 Error Rate (cpWER)**
@@ -45,28 +50,28 @@
 `meeteval-wer mimower -r ref.stm -h hyp.stm` - **Time-Constrained minimum-
 Permutation Word Error Rate (tcpWER)**
 `meeteval-wer tcpwer -r ref.stm -h hyp.stm --collar 5` - **Time-Constrained
 Optimal Reference Combination Word Error Rate (tcORC WER)**
 `meeteval-wer tcorcwer -r ref.stm -h hyp.stm --collar 5` - **Diarization Error
 Rate (DER)** by wrapping [mdeval](https://github.com/nryant/dscore/raw/master/
 scorelib/md-eval-22.pl)
-`meeteval-der md_eval_22 -r ref.stm -h hyp.stm --collar .25` Additionally
-(WIP), MeetEval contains a [visualization](#visualization-wip) tool for cpWER
-and tcpWER alignments that help spot errors in system outputs. ## Installation
-### From PyPI ```shell pip install meeteval ``` ### From source ```shell git
-clone https://github.com/fgnt/meeteval pip install -e ./meeteval ``` ##
-Command-line interface `MeetEval` supports the following file formats as input:
-- [Segmental Time Mark](https://github.com/usnistgov/SCTK/blob/master/doc/
-infmts.htm#L75) (`STM`) - [Time Marked Conversation](https://github.com/
-usnistgov/SCTK/blob/master/doc/infmts.htm#L286) (`CTM`) - [SEGment-wise Long-
-form Speech Transcription annotation](#segment-wise-long-form-speech-
-transcription-annotation-seglst) (`SegLST`), the file format used in the [CHiME
-challenges](https://www.chimechallenge.org) - [Rich Transcription Time Marked]
-(https://github.com/nryant/dscore?tab=readme-ov-file#rttm) (`RTTM`) files (only
-for Diarizaiton Error Rate) > [!NOTE] > `MeetEval` does not support alternate
+`meeteval-der md_eval_22 -r ref.stm -h hyp.stm --collar .25` Additionally,
+MeetEval contains a [visualization](#visualization) tool for cpWER and tcpWER
+alignments that helps to spot errors in system outputs. ## Installation ###
+From PyPI ```shell pip install meeteval ``` ### From source ```shell git clone
+https://github.com/fgnt/meeteval pip install -e ./meeteval ``` ## Command-line
+interface `MeetEval` supports the following file formats as input: - [Segmental
+Time Mark](https://github.com/usnistgov/SCTK/blob/master/doc/infmts.htm#L75)
+(`STM`) - [Time Marked Conversation](https://github.com/usnistgov/SCTK/blob/
+master/doc/infmts.htm#L286) (`CTM`) - [SEGment-wise Long-form Speech
+Transcription annotation](#segment-wise-long-form-speech-transcription-
+annotation-seglst) (`SegLST`), the file format used in the [CHiME challenges]
+(https://www.chimechallenge.org) - [Rich Transcription Time Marked](https://
+github.com/nryant/dscore?tab=readme-ov-file#rttm) (`RTTM`) files (only for
+Diarization Error Rate) > [!NOTE] > `MeetEval` does not support alternate
 transcripts (e.g., `"i've { um / uh / @ } as far as i'm concerned"`). The
 command-line interface is available as `meeteval-wer` or `python -
 m meeteval.wer` with the following signature: ```shell python -m meeteval.wer
 [orcwer|mimower|cpwer|tcpwer|tcorcwer] -h example_files/hyp.stm -
 r example_files/ref.stm # or meeteval-wer
 [orcwer|mimower|cpwer|tcpwer|tcorcwer] -h example_files/hyp.stm -
 r example_files/ref.stm ``` You can add `--help` to any command to get more
@@ -199,21 +204,18 @@
 hypothesis_self_overlap=SelfOverlap(overlap_rate=Decimal('0'), overlap_time=0,
 total_time=Decimal('2')), missed_speaker=0, falarm_speaker=0, scored_speaker=2)
 ``` ### Aligning sequences Sequences can be aligned, similar to
 `kaldialign.align`, using the tcpWER matching: ```python import meeteval
 meeteval.wer.wer.time_constrained.align([{'words': 'a b', 'start_time': 0,
 'end_time': 1}], [{'words': 'a c', 'start_time': 0, 'end_time': 1}, {'words':
 'd', 'start_time': 2, 'end_time': 3}]) # [('a', 'a'), ('b', 'c'), ('*', 'd')]
-``` ## Visualization [WIP] > [!IMPORTANT] > The visualization is under
-development!
-> Preview: https://groups.uni-paderborn.de/nt/meeteval/viz.html
-> Interactive notebook: https://fgnt.github.io/meeteval_jupyterlite/
-lab?path=Demo.ipynb ```python import meeteval from meeteval.viz.visualize
-import AlignmentVisualization folder = r'https://raw.githubusercontent.com/
-fgnt/meeteval/main/' av = AlignmentVisualization( meeteval.io.load(folder +
+``` ## Visualization > [!TIP] > Try it in the browser! https://fgnt.github.com/
+meeteval_viz ```python import meeteval from meeteval.viz.visualize import
+AlignmentVisualization folder = r'https://raw.githubusercontent.com/fgnt/
+meeteval/main/' av = AlignmentVisualization( meeteval.io.load(folder +
 'example_files/ref.stm').groupby('filename')['recordingA'], meeteval.io.load
 (folder + 'example_files/hyp.stm').groupby('filename')['recordingA'] ) #
 display(av) # Jupyter # av.dump('viz.html') # Create standalone HTML file ```
 ## Cite The toolkit and the tcpWER were presented at the CHiME-2023 workshop
 (Computational Hearing in Multisource Environments) with the paper ["MeetEval:
 A Toolkit for Computation of Word Error Rates for Meeting Transcription
 Systems"](https://arxiv.org/abs/2307.11394). ```bibtex @InProceedings
```

### Comparing `meeteval-0.2.1/README.md` & `meeteval-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <h1 align="center">MeetEval</h1> 
 <h3 align="center">A meeting transcription evaluation toolkit</h3>
-<div align="center"><a href="#features">Features</a> | <a href="#installation">Installation</a> | <a href="#python-interface">Python Interface</a> | <a href="#command-line-interface">Command Line Interface</a> | <a href="#visualization-wip">Visualization (WIP)</a> | <a href="#cite">Cite</a></div>
+<div align="center"><a href="#features">Features</a> | <a href="#installation">Installation</a> | <a href="#python-interface">Python Interface</a> | <a href="#command-line-interface">Command Line Interface</a> | <a href="#visualization">Visualization</a> | <a href="#cite">Cite</a></div>
 <br>
 <a href="https://github.com/fgnt/meeteval/actions"><img src="https://github.com/fgnt/meeteval/actions/workflows/pytest.yml/badge.svg"/></a>
 
 
 ## Features
 MeetEval supports the following metrics for meeting transcription evaluation:
 
@@ -19,15 +19,15 @@
 - **Time-Constrained minimum-Permutation Word Error Rate (tcpWER)**<br>
   `meeteval-wer tcpwer -r ref.stm -h hyp.stm --collar 5`
 - **Time-Constrained Optimal Reference Combination Word Error Rate (tcORC WER)**<br>
   `meeteval-wer tcorcwer -r ref.stm -h hyp.stm --collar 5`
 - **Diarization Error Rate (DER)** by wrapping [mdeval](https://github.com/nryant/dscore/raw/master/scorelib/md-eval-22.pl)<br>
   `meeteval-der md_eval_22 -r ref.stm -h hyp.stm --collar .25`
 
-Additionally (WIP), MeetEval contains a [visualization](#visualization-wip) tool for cpWER and tcpWER alignments that help spot errors in system outputs.
+Additionally, MeetEval contains a [visualization](#visualization) tool for cpWER and tcpWER alignments that helps to spot errors in system outputs.
 
 ## Installation
 
 ### From PyPI
 
 ```shell
 pip install meeteval
@@ -42,15 +42,15 @@
 
 ## Command-line interface
 
 `MeetEval` supports the following file formats as input:
  - [Segmental Time Mark](https://github.com/usnistgov/SCTK/blob/master/doc/infmts.htm#L75) (`STM`)
  - [Time Marked Conversation](https://github.com/usnistgov/SCTK/blob/master/doc/infmts.htm#L286) (`CTM`)
  - [SEGment-wise Long-form Speech Transcription annotation](#segment-wise-long-form-speech-transcription-annotation-seglst) (`SegLST`), the file format used in the [CHiME challenges](https://www.chimechallenge.org)
- - [Rich Transcription Time Marked](https://github.com/nryant/dscore?tab=readme-ov-file#rttm) (`RTTM`) files (only for Diarizaiton Error Rate)
+ - [Rich Transcription Time Marked](https://github.com/nryant/dscore?tab=readme-ov-file#rttm) (`RTTM`) files (only for Diarization Error Rate)
 
 
 > [!NOTE]
 > `MeetEval` does not support alternate transcripts (e.g., `"i've { um / uh / @ } as far as i'm concerned"`).
 
 The command-line interface is available as `meeteval-wer` or `python -m meeteval.wer` with the following signature:
 
@@ -268,20 +268,18 @@
 Sequences can be aligned, similar to `kaldialign.align`, using the tcpWER matching:
 ```python
 import meeteval
 meeteval.wer.wer.time_constrained.align([{'words': 'a b', 'start_time': 0, 'end_time': 1}], [{'words': 'a c', 'start_time': 0, 'end_time': 1}, {'words': 'd', 'start_time': 2, 'end_time': 3}])
 # [('a', 'a'), ('b', 'c'), ('*', 'd')]
 ```
 
-## Visualization [WIP]
+## Visualization
 
-> [!IMPORTANT]
-> The visualization is under development! <br>
-> Preview: https://groups.uni-paderborn.de/nt/meeteval/viz.html<br>
-> Interactive notebook: https://fgnt.github.io/meeteval_jupyterlite/lab?path=Demo.ipynb
+> [!TIP]
+> Try it in the browser! https://fgnt.github.com/meeteval_viz
 
 ```python
 import meeteval
 from meeteval.viz.visualize import AlignmentVisualization
 
 folder = r'https://raw.githubusercontent.com/fgnt/meeteval/main/'
 av = AlignmentVisualization(
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                             ************ MMeeeettEEvvaall ************
              ******** AA mmeeeettiinngg ttrraannssccrriippttiioonn eevvaalluuaattiioonn ttoooollkkiitt ********
      _F_e_a_t_u_r_e_s | _I_n_s_t_a_l_l_a_t_i_o_n | _P_y_t_h_o_n_ _I_n_t_e_r_f_a_c_e | _C_o_m_m_a_n_d_ _L_i_n_e_ _I_n_t_e_r_f_a_c_e |
-                          _V_i_s_u_a_l_i_z_a_t_i_o_n_ _(_W_I_P_) | _C_i_t_e
+                             _V_i_s_u_a_l_i_z_a_t_i_o_n | _C_i_t_e
 
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_f_g_n_t_/_m_e_e_t_e_v_a_l_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_p_y_t_e_s_t_._y_m_l_/_b_a_d_g_e_._s_v_g_]##
 Features MeetEval supports the following metrics for meeting transcription
 evaluation: - **Standard WER** for single utterances (Called SISO WER in
 MeetEval)
 `meeteval-wer wer -r ref -h hyp` - **Concatenated minimum-Permutation Word
 Error Rate (cpWER)**
@@ -16,28 +16,28 @@
 `meeteval-wer mimower -r ref.stm -h hyp.stm` - **Time-Constrained minimum-
 Permutation Word Error Rate (tcpWER)**
 `meeteval-wer tcpwer -r ref.stm -h hyp.stm --collar 5` - **Time-Constrained
 Optimal Reference Combination Word Error Rate (tcORC WER)**
 `meeteval-wer tcorcwer -r ref.stm -h hyp.stm --collar 5` - **Diarization Error
 Rate (DER)** by wrapping [mdeval](https://github.com/nryant/dscore/raw/master/
 scorelib/md-eval-22.pl)
-`meeteval-der md_eval_22 -r ref.stm -h hyp.stm --collar .25` Additionally
-(WIP), MeetEval contains a [visualization](#visualization-wip) tool for cpWER
-and tcpWER alignments that help spot errors in system outputs. ## Installation
-### From PyPI ```shell pip install meeteval ``` ### From source ```shell git
-clone https://github.com/fgnt/meeteval pip install -e ./meeteval ``` ##
-Command-line interface `MeetEval` supports the following file formats as input:
-- [Segmental Time Mark](https://github.com/usnistgov/SCTK/blob/master/doc/
-infmts.htm#L75) (`STM`) - [Time Marked Conversation](https://github.com/
-usnistgov/SCTK/blob/master/doc/infmts.htm#L286) (`CTM`) - [SEGment-wise Long-
-form Speech Transcription annotation](#segment-wise-long-form-speech-
-transcription-annotation-seglst) (`SegLST`), the file format used in the [CHiME
-challenges](https://www.chimechallenge.org) - [Rich Transcription Time Marked]
-(https://github.com/nryant/dscore?tab=readme-ov-file#rttm) (`RTTM`) files (only
-for Diarizaiton Error Rate) > [!NOTE] > `MeetEval` does not support alternate
+`meeteval-der md_eval_22 -r ref.stm -h hyp.stm --collar .25` Additionally,
+MeetEval contains a [visualization](#visualization) tool for cpWER and tcpWER
+alignments that helps to spot errors in system outputs. ## Installation ###
+From PyPI ```shell pip install meeteval ``` ### From source ```shell git clone
+https://github.com/fgnt/meeteval pip install -e ./meeteval ``` ## Command-line
+interface `MeetEval` supports the following file formats as input: - [Segmental
+Time Mark](https://github.com/usnistgov/SCTK/blob/master/doc/infmts.htm#L75)
+(`STM`) - [Time Marked Conversation](https://github.com/usnistgov/SCTK/blob/
+master/doc/infmts.htm#L286) (`CTM`) - [SEGment-wise Long-form Speech
+Transcription annotation](#segment-wise-long-form-speech-transcription-
+annotation-seglst) (`SegLST`), the file format used in the [CHiME challenges]
+(https://www.chimechallenge.org) - [Rich Transcription Time Marked](https://
+github.com/nryant/dscore?tab=readme-ov-file#rttm) (`RTTM`) files (only for
+Diarization Error Rate) > [!NOTE] > `MeetEval` does not support alternate
 transcripts (e.g., `"i've { um / uh / @ } as far as i'm concerned"`). The
 command-line interface is available as `meeteval-wer` or `python -
 m meeteval.wer` with the following signature: ```shell python -m meeteval.wer
 [orcwer|mimower|cpwer|tcpwer|tcorcwer] -h example_files/hyp.stm -
 r example_files/ref.stm # or meeteval-wer
 [orcwer|mimower|cpwer|tcpwer|tcorcwer] -h example_files/hyp.stm -
 r example_files/ref.stm ``` You can add `--help` to any command to get more
@@ -170,21 +170,18 @@
 hypothesis_self_overlap=SelfOverlap(overlap_rate=Decimal('0'), overlap_time=0,
 total_time=Decimal('2')), missed_speaker=0, falarm_speaker=0, scored_speaker=2)
 ``` ### Aligning sequences Sequences can be aligned, similar to
 `kaldialign.align`, using the tcpWER matching: ```python import meeteval
 meeteval.wer.wer.time_constrained.align([{'words': 'a b', 'start_time': 0,
 'end_time': 1}], [{'words': 'a c', 'start_time': 0, 'end_time': 1}, {'words':
 'd', 'start_time': 2, 'end_time': 3}]) # [('a', 'a'), ('b', 'c'), ('*', 'd')]
-``` ## Visualization [WIP] > [!IMPORTANT] > The visualization is under
-development!
-> Preview: https://groups.uni-paderborn.de/nt/meeteval/viz.html
-> Interactive notebook: https://fgnt.github.io/meeteval_jupyterlite/
-lab?path=Demo.ipynb ```python import meeteval from meeteval.viz.visualize
-import AlignmentVisualization folder = r'https://raw.githubusercontent.com/
-fgnt/meeteval/main/' av = AlignmentVisualization( meeteval.io.load(folder +
+``` ## Visualization > [!TIP] > Try it in the browser! https://fgnt.github.com/
+meeteval_viz ```python import meeteval from meeteval.viz.visualize import
+AlignmentVisualization folder = r'https://raw.githubusercontent.com/fgnt/
+meeteval/main/' av = AlignmentVisualization( meeteval.io.load(folder +
 'example_files/ref.stm').groupby('filename')['recordingA'], meeteval.io.load
 (folder + 'example_files/hyp.stm').groupby('filename')['recordingA'] ) #
 display(av) # Jupyter # av.dump('viz.html') # Create standalone HTML file ```
 ## Cite The toolkit and the tcpWER were presented at the CHiME-2023 workshop
 (Computational Hearing in Multisource Environments) with the paper ["MeetEval:
 A Toolkit for Computation of Word Error Rates for Meeting Transcription
 Systems"](https://arxiv.org/abs/2307.11394). ```bibtex @InProceedings
```

### Comparing `meeteval-0.2.1/meeteval/der/api.py` & `meeteval-0.3.0/meeteval/der/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 ]
 
 
 def md_eval_22(
         reference,
         hypothesis,
         collar=0,
+        regions='all',
         regex=None,
         uem=None,
 ):
     r, h = _load_texts(reference, hypothesis, regex)
     from meeteval.der.md_eval import md_eval_22_multifile
     if uem is not None:
         from meeteval.io.uem import UEM
         if isinstance(uem, (str, Path, list, tuple)):
             uem = UEM.load(uem)
 
-    results = md_eval_22_multifile(r, h, collar, uem=uem)
+    results = md_eval_22_multifile(
+        r, h, collar, regions=regions, uem=uem
+    )
     return results
```

### Comparing `meeteval-0.2.1/meeteval/der/md_eval.py` & `meeteval-0.3.0/meeteval/der/md_eval.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,15 +73,37 @@
             scored_speaker_time=self.scored_speaker_time + other.scored_speaker_time,
             missed_speaker_time=self.missed_speaker_time + other.missed_speaker_time,
             falarm_speaker_time=self.falarm_speaker_time + other.falarm_speaker_time,
             speaker_error_time=self.speaker_error_time + other.speaker_error_time,
         )
 
 
-def md_eval_22_multifile(reference, hypothesis, collar=0, uem=None):
+def md_eval_22_multifile(
+        reference, hypothesis, collar=0, regions='all',
+        uem=None
+):
+    """
+    Computes the Diarization Error Rate (DER) and statistics using
+    md-eval-22.pl.
+
+    Args:
+        reference: The reference in a format convertible to RTTM.
+        hypothesis: The hypothesis in a format convertible to RTTM.
+        collar: The collar in seconds.
+        regions: The regions to score. Either 'all' or 'nooverlap'.
+            'nooverlap' limits scoring to single-speaker regions by appending
+            `-1` to the md-eval-22.pl command.
+        uem: The UEM file.
+    """
+    if regions not in {'all', 'nooverlap'}:
+        raise ValueError(
+            f'Invalid regions: {regions}. '
+            f'Select from "all" or "nooverlap".'
+        )
+
     from meeteval.io.rttm import RTTM
     reference = RTTM.new(reference)
     hypothesis = RTTM.new(hypothesis)
 
     reference = _fix_channel(reference)
     hypothesis = _fix_channel(hypothesis)
 
@@ -115,14 +137,17 @@
         cmd = [
             'perl', f'{md_eval_22}',
             '-c', f'{collar}',
             '-r', f'{r_file}',
             '-s', f'{h_file}',
         ]
 
+        if regions == 'nooverlap':
+            cmd.append('-1')
+
         if uem:
             uem_file = tmpdir / f'{key}.uem'
             uem.dump(uem_file)
             cmd.extend(['-u', f'{uem_file}'])
 
         cp = subprocess.run(cmd, stdout=subprocess.PIPE,
                             check=True, universal_newlines=True)
@@ -171,17 +196,19 @@
                 f'({summary.error_rate})\n'
                 f'does not match the average error rate of md-eval-22.pl '
                 f'applied to each recording ({md_eval.error_rate}).'
             )
     return per_reco
 
 
-def md_eval_22(reference, hypothesis, collar=0, uem=None):
+def md_eval_22(reference, hypothesis, collar=0, regions='all', uem=None):
     from meeteval.io.rttm import RTTM
     reference = RTTM.new(reference, filename='dummy')
     hypothesis = RTTM.new(hypothesis, filename='dummy')
 
     assert len(reference.filenames()) == 1, reference.filenames()
     assert len(hypothesis.filenames()) == 1, hypothesis.filenames()
     assert reference.filenames() == hypothesis.filenames(), (reference.filenames(), hypothesis.filenames())
 
-    return md_eval_22_multifile(reference, hypothesis, collar, uem=uem)[reference.filenames()[0]]
+    return md_eval_22_multifile(
+        reference, hypothesis, collar, regions=regions, uem=uem
+    )[reference.filenames()[0]]
```

### Comparing `meeteval-0.2.1/meeteval/io/base.py` & `meeteval-0.3.0/meeteval/io/base.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/io/chime7.py` & `meeteval-0.3.0/meeteval/io/chime7.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/io/ctm.py` & `meeteval-0.3.0/meeteval/io/ctm.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/io/keyed_text.py` & `meeteval-0.3.0/meeteval/io/keyed_text.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/io/load_wrapper.py` & `meeteval-0.3.0/meeteval/io/load_wrapper.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/io/pbjson.py` & `meeteval-0.3.0/meeteval/io/pbjson.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/io/py.py` & `meeteval-0.3.0/meeteval/io/py.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/io/rttm.py` & `meeteval-0.3.0/meeteval/io/rttm.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/io/seglst.py` & `meeteval-0.3.0/meeteval/io/seglst.py`

 * *Files 12% similar despite different names*

```diff
@@ -161,30 +161,44 @@
         The name `T` is inspired by the `T` in `pandas.DataFrame.T` and
         `numpy.ndarray.T`.
         """
 
         def __init__(self, outer):
             self._outer = outer
 
-        def keys(self):
+        def keys(self, *, all=False):
             """
-            The keys that are common among all segments
+            The keys that are common among all segments (all=False) or all
+            keys (all=True).
+
+            Use the get method to fill defaults for missing values.
             """
             if len(self._outer) == 0:
                 return set()
-            return set.intersection(
+            if all:
+                op = set.union
+            else:
+                op = set.intersection
+            return op(
                 *[set(s.keys()) for s in self._outer.segments]
             )
 
         def __getitem__(self, key: _SegLstSegment_keys):
             """
             Returns the values for `key` of all segments as a list.
             """
             return [s[key] for s in self._outer.segments]
 
+        def get(self, key, default=None):
+            """
+            Returns the values for `key` of all segments as a list, or default,
+            when key is not present.
+            """
+            return [s.get(key, default) for s in self._outer.segments]
+
         def __class_getitem__(cls, item: _SegLstSegment_keys) -> 'list':
             """
             This is a dummy for type annotation.
 
             PyCharm doesn't get it, what a property on the class definition
             does and thinks `__class_getitem__` is called, while `__getitem__`
             gets called.
@@ -264,14 +278,15 @@
     def filter(self, fn: 'Callable[[SegLstSegment], bool]') -> 'SegLST':
         """
         Applies `fn` to all segments and returns a new `SegLST` object with the
         segments for which `fn` returns true.
         """
         return SegLST([s for s in self.segments if fn(s)])
 
+
     @classmethod
     def merge(cls, *t) -> 'SegLST':
         """
         Merges multiple `SegLST` objects into one by concatenating all segments.
         """
         return SegLST([s for t_ in t for s in t_.segments])
 
@@ -535,22 +550,43 @@
     return _seglst_map
 
 
 def apply_multi_file(
         fn: 'Callable[[SegLST, SegLST], ErrorRate]',
         reference, hypothesis,
         *,
-        allowed_empty_examples_ratio=0.1
+        allowed_empty_examples_ratio=0.1,
+        partial=False
 ):
     """
     Applies a function individually to all sessions / files.
 
     `reference` and `hypothesis` must be convertible to `SegLST`. If they are a
     Python structure, the first level is interpreted as the session / file key.
 
+    Reference and hypothesis should have the same keys. If a hypothesis key is
+    missing, it interpreted as silence. The ratio of allowed missing hypothesis
+    keys is limited by `allowed_empty_examples_ratio`. If the amount of missing
+    hypothesis keys exceeds `allowed_empty_examples_ratio`, a `RuntimeError` is
+    raised.
+
+    Reference keys are only allowed to be missing if `partial=True`. Then,
+    it is assumed that the user only evaluates a subset and the corresponding
+    hypothesis segments are dropped.
+
+    Args:
+        fn: Function that takes two `SegLST` objects as input and returns an
+            `ErrorRate` object.
+        reference: Reference data. Must contain session IDs
+        hypothesis: Hypothesis data. Must contain session IDs
+        allowed_empty_examples_ratio: Ratio of allowed missing hypothesis keys.
+        partial: If True, the function returns the results for all sessions
+            where the reference sessions. If False, the function raises an
+            exception when session IDs are missing in the reference.
+
     >>> from meeteval.wer.wer.cp import cp_word_error_rate
     >>> from pprint import pprint
     >>> ref = [['a b c', 'd e f'], ['g h i']]
     >>> hyp = [['a b c'], ['d e f', 'g h i']]
     >>> er = apply_multi_file(cp_word_error_rate, ref, hyp)
     >>> pprint(er)
     {0: CPErrorRate(error_rate=0.5, errors=3, length=6, insertions=0, deletions=3, substitutions=0, missed_speaker=1, falarm_speaker=0, scored_speaker=2, assignment=((0, 0), (1, None))),
@@ -559,64 +595,93 @@
     import logging
     reference = asseglst(
         reference, required_keys=('session_id',),
         py_convert=lambda p: NestedStructure(
             p, ('session_id', 'speaker', 'segment_id')
         )
     ).groupby('session_id')
+
+    if len(reference) == 0:
+        raise RuntimeError(f'Empty reference.')
+
     hypothesis = asseglst(
         hypothesis, required_keys=('session_id',),
         py_convert=lambda p: NestedStructure(
             p, ('session_id', 'speaker', 'segment_id')
         )
     ).groupby('session_id')
 
     # Check session keys. Print a warning if they differ and raise an exception
     # when they differ too much
     if reference.keys() != hypothesis.keys():
         h_minus_r = list(set(hypothesis.keys()) - set(reference.keys()))
         r_minus_h = list(set(reference.keys()) - set(hypothesis.keys()))
 
-        ratio = len(r_minus_h) / len(reference.keys())
-
         if h_minus_r:
-            # This is a warning, because missing in reference is not a problem,
-            # we can safely ignore it. Missing in hypothesis is a problem,
-            # because we cannot distinguish between silence and missing.
+            # Keys are missing in the reference.
+            if not partial:
+                raise RuntimeError(
+                    f'{len(h_minus_r)} of {len(hypothesis)} session IDs are '
+                    f'present in the hypothesis but missing in the reference.\n'
+                    f'Missing (showing first 5): {h_minus_r[:5]}\n'
+                    f'If this is intentional, consider setting `partial=True`.'
+                )
+
+            # The user set partial=True.
+            # Assume that the user only wants to evaluate a sub-set defined by
+            # the keys present in the reference. Still inform the user about
+            # the missing keys.
             logging.warning(
-                f'Keys of reference and hypothesis differ\n'
-                f'hypothesis - reference: e.g. {h_minus_r[:5]} (Total: '
-                f'{len(h_minus_r)} of {len(reference)})\n'
-                f'Drop them.',
+                f'{len(h_minus_r)} of {len(hypothesis)} keys are present in '
+                f'the hypothesis but missing in the reference. \n'
+                f'Missing (showing first 5): {h_minus_r[:5]}\n'
+                f'`partial=True`, so the computation continues with the '
+                f'assumption that only the sub-set of sessions present in the '
+                f'reference should be evaluated.',
             )
             hypothesis = {
                 k: v
                 for k, v in hypothesis.items()
                 if k not in h_minus_r
             }
 
-        if len(r_minus_h) == 0:
-            pass
-        elif ratio <= allowed_empty_examples_ratio:
-            logging.warning(
-                f'Missing {ratio * 100:.3} % = '
-                f'{len(r_minus_h)}/{len(reference.keys())} of recordings in'
-                f' hypothesis.\n'
-                f'Please check your system, if it ignored some recordings or '
-                f'predicted no transcriptions for some recordings.\n'
-                f'Continue with the assumption, that the system predicted '
-                f'silence for the missing recordings.',
-            )
-        else:
-            raise RuntimeError(
-                'Keys of reference and hypothesis differ\n'
-                f'hypothesis - reference: e.g. {h_minus_r[:5]} '
-                f'(Total: {len(h_minus_r)} of {len(hypothesis)})\n'
-                f'reference - hypothesis: e.g. {r_minus_h[:5]} '
-                f'(Total: {len(r_minus_h)} of {len(reference)})'
-            )
+        # The following if statement is active when keys are missing in the
+        # hypothesis. We assume that the system didn't produce any output for
+        # the missing examples but throw an exception when a threshold is
+        # exceeded
+        if len(r_minus_h):
+            # len(reference.keys)) can't be 0 here
+            ratio = len(r_minus_h) / len(reference.keys())
+            if ratio <= allowed_empty_examples_ratio:
+                logging.warning(
+                    f'Missing {ratio * 100:.3f} % = '
+                    f'{len(r_minus_h)}/{len(reference.keys())} of recordings in '
+                    f'hypothesis. An exception will be raised when this number '
+                    f'exceeds {allowed_empty_examples_ratio * 100:3} %.\n'
+                    f'Please check if your system ignored recordings. '
+                    f'It is recommended to output an empty transcript if silence '
+                    f'was recognized in order to reliably detect errors.\n'
+                    f'Missing (showing first 5): {r_minus_h[:5]}\n'
+                    f'The computation continues with the assumption that the system '
+                    f'predicted silence for the missing recordings.',
+                )
+            else:
+                raise RuntimeError(
+                    f'Missing {ratio * 100:.3f} % = '
+                    f'{len(r_minus_h)}/{len(reference.keys())} of recordings in '
+                    f'hypothesis. This exceeds the threshold of '
+                    f'{allowed_empty_examples_ratio * 100:3} %.\n'
+                    f'Please check if your system ignored recordings. '
+                    f'It is recommended to output an empty transcript if silence '
+                    f'was recognized in order to reliably detect errors.\n'
+                    f'Missing (showing first 5): {r_minus_h[:5]}'
+                )
 
     results = {}
     for session in reference.keys():
-        results[session] = fn(reference[session], hypothesis[session])
+        try:
+            results[session] = fn(reference[session], hypothesis.get(session, SegLST([])))
+        except:
+            logging.error(f'Error in session {session}')
+            raise
 
     return results
```

### Comparing `meeteval-0.2.1/meeteval/io/stm.py` & `meeteval-0.3.0/meeteval/io/stm.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/io/uem.py` & `meeteval-0.3.0/meeteval/io/uem.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/viz/__main__.py` & `meeteval-0.3.0/meeteval/viz/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 from pathlib import Path
 import collections
+import itertools
 
 import meeteval
 from meeteval.viz.visualize import AlignmentVisualization
 from meeteval.wer.api import _load_texts
 import tqdm
 
 
 def create_viz_folder(
         reference,
         hypothesiss,
         out,
-        alignment='tcp',
+        alignments='tcp',
         regex=None,
+        normalizer=None,
+        js_debug=False,
 ):
     out = Path(out)
     out.mkdir(parents=True, exist_ok=True)
 
     avs = {}
-    for i, hypothesis in tqdm.tqdm(hypothesiss.items()):
+    for (i, hypothesis), alignment in tqdm.tqdm(list(itertools.product(
+            hypothesiss.items(),
+            alignments.split(','),
+    ))):
 
         r, h = _load_texts(
             reference, hypothesis, regex=regex,
             reference_sort='segment',
             hypothesis_sort='segment',
+            normalizer=normalizer,
         )
 
         r = r.groupby('session_id')
         h = h.groupby('session_id')
 
         session_ids = set(r.keys()) & set(h.keys())
         xor = set(r.keys()) ^ set(h.keys())
         if xor:
             print(f'Ignore {xor}, because they are not available in reference and hypothesis.')
 
-        for session_id in session_ids:
+        for session_id in tqdm.tqdm(session_ids):
             av = AlignmentVisualization(r[session_id],
                                         h[session_id],
-                                        alignment=alignment)
-            av.dump(out / f'{session_id}_{i}.html')
-            avs.setdefault(i, {})[session_id] = av
+                                        alignment=alignment,
+                                        js_debug=js_debug,
+                                        sync_id=1)
+            av.dump(out / f'{session_id}_{i}_{alignment}.html')
+            avs.setdefault((i, alignment), {})[session_id] = av
 
     ###########################################################################
 
     from yattag import Doc
     from yattag import indent
 
     avs_T = collections.defaultdict(lambda: {k: None for k in avs.keys()})
@@ -55,19 +64,19 @@
     for session_id, v in avs_T.items():
         doc, tag, text = Doc().tagtext()
         doc.asis('<!DOCTYPE html>')
 
         # With 100 % there is a scroll bar -> use 99 %
         with tag('html', style="height: 99%; margin: 0;"):
             with tag('body', style="width: 100%; height: 100%; margin: 0; display: flex;"):
-                for i, av in v.items():
+                for (i, alignment), av in v.items():
                     with tag('div', style='flex-grow: 1'):
-                        with tag('iframe', src=f'{session_id}_{i}.html',
+                        with tag('iframe', src=f'{session_id}_{i}_{alignment}.html',
                                  title="right", width="100%",
-                                 height="100%"):
+                                 height="100%", style="border-width: 0"):
                             pass
 
         file = out / f"{session_id}.html"
         file.write_text(indent(doc.getvalue()))
         print(f'Wrote {file.absolute()}')
 
     ###########################################################################
@@ -83,118 +92,141 @@
         ]).error_rate
         return f'{error_rate * 100:.2f} %'
 
     doc, tag, text = Doc().tagtext()
     doc.asis('<!DOCTYPE html>')
     with tag('html'):
         with tag('head'):
+            # When offline, the page will still work.
+            # The sort will break and the table style rested.
             with tag('script', src='https://code.jquery.com/jquery-3.6.4.min.js'):
                 pass
             with tag('script', src='https://cdnjs.cloudflare.com/ajax/libs/jquery.tablesorter/2.31.2/js/jquery.tablesorter.min.js'):
                 pass
             doc.asis('<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/jquery.tablesorter/2.31.2/css/theme.default.min.css">')
         with tag('body'):
-            with tag('table', klass='tablesorter', id='myTable'):
+            with tag('table', klass='tablesorter', id='myTable', style='width: auto;'):
                 with tag('thead'), tag('tr'):
                     for s in [
                         'Session ID',
                         *[
                             col
-                            for k, v in avs.items()
-                            for col in [k, f'WER: {get_wer(v)}']
+                            for (k, alignment), v in avs.items()
+                            for col in [k, f'{alignment}WER: {get_wer(v)}']
                         ]
                     ]:
                         with tag('th'):
                             doc.text(s)
 
                 with tag('tbody'):
                     for session_id, v in avs_T.items():
                         with tag('tr'):
                             with tag('td'):
                                 doc.text(f'{session_id}')
-                            for i, av in v.items():
+                            for (i, alignment), av in v.items():
                                 with tag('td'):
                                     with tag('a',
-                                             href=f'{session_id}_{i}.html'):
-                                        doc.text('viz')
+                                             href=f'{session_id}_{i}_{alignment}.html'):
+                                        doc.text('View')
                                 with tag('td'):
                                     wer = av.data['info']['wer']['hypothesis']['error_rate']
                                     doc.text(f"{wer * 100:.2f} %")
 
-                            with tag('td'):
-                                with tag('a', href=f'{session_id}.html'):
-                                    doc.text('SideBySide viz')
+                            if len(v) > 1:
+                                with tag('td'):
+                                    with tag('a', href=f'{session_id}.html'):
+                                        doc.text('View SideBySide')
+                                with tag('td'):
+                                    tags = '&'.join(f'{session_id}_{i}_{a}' for i, a in v.keys())
+                                    with tag('a', href=f'side_by_side_sync.html?{tags}'):
+                                        doc.text('View SydeBySide Synced')
             doc.asis('''
 <script>
     $(document).ready(function() {
         // Initialize tablesorter on the table
         $("#myTable").tablesorter();
     });
 </script>
             ''')
 
+    import shutil
+    shutil.copy(Path(__file__).parent / 'side_by_side_sync.html', out / 'side_by_side_sync.html')
+
     with open(out / "index.html", "w") as text_file:
         text_file.write(indent(doc.getvalue()))
     print(f'Open {(out / "index.html").absolute()}')
 
 
 def html(
         reference,
         hypothesis,
         alignment='tcp',
         regex=None,
+        normalizer=None,
         out='viz',
+        js_debug=False,
 ):
     def prepare(i: int, h: str):
         if ':' in h and not Path(h).exists():
             # inspired by tensorboard from the --logdir_spec argument.
             name, path = h.split(':', maxsplit=1)
             return name, path
         else:
-            return f'sys{i}', h
+            if len(hypothesis) > 1:
+                return f'System {i}', h
+            else:
+                return f'System', h
 
     assert len(reference) == 1, (len(reference), 'At the moment only shared reference is supported.')
 
     hypothesis = dict([
         prepare(i, h)
         for i, h in enumerate(hypothesis)
     ])
 
     create_viz_folder(
         reference=reference,
         hypothesiss=hypothesis,
         out=out,
-        alignment=alignment,
+        alignments=alignment,
         regex=regex,
+        normalizer=normalizer,
+        js_debug=js_debug,
     )
 
 
 def cli():
     from meeteval.wer.__main__ import CLI
 
     class VizCLI(CLI):
 
         def add_argument(self, command_parser, name, p):
             if name == 'alignment':
                 command_parser.add_argument(
                     '--alignment',
-                    choices=['tcp', 'cp'],
+                    choices=['tcp', 'cp', 'tcp,cp', 'cp,tcp', 'tcorc', 'orc'],
                     help='Specifies which alignment is used.\n'
                          '- cp: Find the permutation that minimizes the cpWER and use the "classical" alignment.\n'
                          '- tcp: Find the permutation that minimizes the tcpWER and use a time constraint alignment.'
                 )
             elif name == 'hypothesis':
                 command_parser.add_argument(
                     '-h', '--hypothesis',
                     help='Hypothesis file(s) in SegLST, STM or CTM format. '
                          'Multiple files can be provided for a side by side view. '
                          'Optionally prefixed with system name, e.g. mysystem:/path/to/hyp.stm',
                     nargs='+', action=self.extend_action,
                     required=True,
                 )
+            elif name == 'js_debug':
+                command_parser.add_argument(
+                    '--js-debug',
+                    action='store_true',
+                    help='Add a debug flag to the HTML output to enable debugging in the browser.'
+                )
             else:
                 return super().add_argument(command_parser, name, p)
 
     cli = VizCLI()
     cli.add_command(html)
     cli.run()
```

### Comparing `meeteval-0.2.1/meeteval/viz/file_server.py` & `meeteval-0.3.0/meeteval/viz/file_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,16 @@
  - Normalizes the audio files (Useful for far-field recordings that typically have a low volume)
 
 python -m meeteval.viz.file_server
 """
 
 import io
 import functools
+import os
+import sys
 from pathlib import Path
 from aiohttp import web
 
 import numpy as np
 import soundfile
 
 
@@ -49,50 +51,67 @@
                 num = round(num * samplerate)
             elif isinstance(num, str):
                 num = round(float(num) * samplerate) if '.' in num else int(num)
             else:
                 raise TypeError(type(num), num)
             yield num
 
+    def get_sample_rate(path):
+        try:
+            return soundfile.info(os.fspath(path)).samplerate
+        except RuntimeError:
+            if Path(path).exists():
+                raise
+            else:
+                raise FileNotFoundError(path) from None
+
     if '::' in path:
         path, slice = path.split('::')
-        samplerate = soundfile.info(path).samplerate
+        samplerate = get_sample_rate(path)
         start, stop = to_number(start, stop)
         assert slice[0] == '[' and slice[-1] == ']', slice
         start_, stop_ = to_number(*slice[1:-1].split(':'))
         if start is None and stop is None:
             start, stop = start_, stop_
         else:
             # Arguments are applied on the [...:...]
             start, stop = start + start_, stop + start_
     else:
-        samplerate = soundfile.info(path).samplerate
+        samplerate = get_sample_rate(path)
         start, stop = to_number(start, stop)
 
-    assert (stop - start) < samplerate * 120, ('For stability: Limit the max duration to 2 min', start, stop, samplerate)
+    if start is not None and start is not None:
+        assert (stop - start) < samplerate * 120, ('For stability: Limit the max duration to 2 min', start, stop, samplerate)
     return path, start, stop
 
 
 class Backend:
     def __init__(self):
         pass
 
     async def handle(self, request: web.Request):
         try:
             name = request.match_info.get('name', "Anonymous")
             name = '/' + name
+            print(f'Requested: {name}')
 
             start = request.query.get('start', None)
             stop = request.query.get('stop', None)
 
             name, start, stop = _parse_audio_slice(name, start, stop)
             name = Path(name)
 
-            if name.suffix in ['.wav']:
-                data, sample_rate = soundfile.read(str(name), start=start, stop=stop)
+            if name.suffix in ['.wav', '.flac']:
+                try:
+                    data, sample_rate = soundfile.read(str(name), start=start, stop=stop)
+                except RuntimeError:
+                    if Path(name).exists():
+                        raise
+                    else:
+                        raise FileNotFoundError(name) from None
                 data = data * 0.95 / np.amax(np.abs(data))
                 bytes = io.BytesIO()
                 # Wav files produce in some browsers artefacts in the audio.
                 # This is undesired, because it is not clear, that it is caused
                 # by the browser or by the enhancement system of the user.
                 # Ogg doesn't has this issue.
                 # ToDo: Does ogg remove user artefacts?
@@ -101,16 +120,18 @@
                 soundfile.write(bytes, data, samplerate=sample_rate, format='ogg')
                 return web.Response(body=bytes.getvalue())
                 # cp = subprocess.run([
                 #     'sox', '--norm', str(name), '-t', 'ogg', '-'
                 # ], stdout=subprocess.PIPE, check=True)
                 # return web.Response(body=cp.stdout)
         except Exception:
-            import traceback
-            traceback.print_exc()
+            import traceback, textwrap
+            print(textwrap.indent(
+                traceback.format_exc(), ' | ',
+            ))
         return web.Response(status=web.HTTPUnauthorized().status_code)
 
     def main(self):
         app = web.Application()
         app.add_routes([web.get('/', self.handle),
                         web.get('/{name:.*}', self.handle),
                         ])
```

### Comparing `meeteval-0.2.1/meeteval/viz/visualize.py` & `meeteval-0.3.0/meeteval/viz/visualize.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 import os
 import json
 
+import urllib.request
+
 import meeteval
 from meeteval.wer import ErrorRate
 
 logging.basicConfig(level=logging.ERROR)
 import dataclasses
 import functools
 import shutil
@@ -22,56 +24,82 @@
 from meeteval.io.stm import STM
 from meeteval.wer.wer.time_constrained import get_pseudo_word_level_timings
 
 from meeteval.io.seglst import asseglst, SegLST
 
 
 def dumps_json(
-        obj, *, indent=2, sort_keys=True, **kwargs):
+        obj, *, indent=2, sort_keys=True,
+        float_round=None,
+        **kwargs,
+):
     import io
     fd = io.StringIO()
     dump_json(
         obj,
         path=fd,
         indent=indent,
         create_path=False,
         sort_keys=sort_keys,
+        float_round=float_round,
         **kwargs,
     )
     return fd.getvalue()
 
 
 def dump_json(
-        obj, path, *, indent=2, create_path=True, sort_keys=False, **kwargs):
+        obj, path, *, indent=2, create_path=True, sort_keys=False,
+        float_round=None,
+        **kwargs,
+):
     """
     Numpy types will be converted to the equivalent Python type for dumping the
     object.
 
     :param obj: Arbitrary object that is JSON serializable,
         where Numpy is allowed.
     :param path: String or ``pathlib.Path`` object.
     :param indent: See ``json.dump()``.
     :param kwargs: See ``json.dump()``.
 
     """
     import io
     import simplejson
 
+    if float_round is not None:
+        import decimal
+
+        def nested_round(obj):
+            if isinstance(obj, (tuple, list)):
+                return [nested_round(e) for e in obj]
+            elif isinstance(obj, dict):
+                return {nested_round(k): nested_round(v) for k, v in
+                        obj.items()}
+            elif isinstance(obj, (float, decimal.Decimal)):
+                return round(obj, float_round)
+            elif type(obj) in [int, str, type(None)]:
+                return obj
+            else:
+                raise TypeError(type(obj))
+        obj = nested_round(obj)
+
     if isinstance(path, io.IOBase):
         simplejson.dump(obj, path, indent=indent,
                         sort_keys=sort_keys, **kwargs)
     elif isinstance(path, (str, Path)):
         path = Path(path).expanduser()
 
         if create_path:
             path.parent.mkdir(parents=True, exist_ok=True)
 
         with path.open('w') as f:
             simplejson.dump(obj, f, indent=indent,
-                            sort_keys=sort_keys, **kwargs)
+                            sort_keys=sort_keys,
+                            for_json=True,
+                            **kwargs)
     else:
         raise TypeError(path)
 
 
 def get_wer(t: SegLST, assignment_type, collar=5, hypothesis_key='hypothesis'):
     """
     Compute the WER with the given assignment type and collar between the segments with `s['source'] = 'reference'`
@@ -209,18 +237,55 @@
                 r.setdefault('matches', []).append((h['word_index'], 'substitution'))
 
 
 def get_visualization_data(ref: SegLST, *hyp: SegLST, assignment='tcp', alignment_transform=None):
     ref = asseglst(ref)
     hyp = [asseglst(h) for h in hyp]
 
+    data = {
+        'info': {
+            'filename': ref[0]['session_id'],
+            'alignment_type': assignment,
+            'length': max([e['end_time'] for e in hyp[0] + ref]) - min([e['start_time'] for e in hyp[0] + ref]),
+        }
+    }
+
+    # Solve assignment when assignment is tcorc or orc
+    if assignment == 'tcorc':
+        assert len(hyp) == 1, len(hyp)
+        from meeteval.wer.wer.time_constrained_orc import time_constrained_orc_wer
+        # The visualization looks wrong if we don't sort segments
+        wer = time_constrained_orc_wer(
+            ref, *hyp,
+            collar=5,
+            reference_sort='segment',
+            hypothesis_sort='segment',
+            reference_pseudo_word_level_timing='character_based',
+            hypothesis_pseudo_word_level_timing='character_based_points',
+        )
+        ref, hyp = wer.apply_assignment(ref, *hyp)
+        hyp = (hyp,)
+        assignment = 'tcp'
+    elif assignment == 'orc':
+        assert len(hyp) == 1, len(hyp)
+        from meeteval.wer.wer.orc import orc_word_error_rate
+        wer = orc_word_error_rate(ref, *hyp)
+        ref, hyp = wer.apply_assignment(ref, *hyp)
+        hyp = (hyp,)
+        assignment = 'cp'
+
     assert len(hyp) > 0, hyp
     if alignment_transform is None:
         alignment_transform = lambda x: x
 
+    ref_session_ids = set(ref.T['session_id'])
+    for h in hyp:
+        hyp_session_ids = set(h.T['session_id'])
+        assert 1 == len(ref_session_ids) and ref_session_ids == hyp_session_ids, f'Expect a single session ID/filename and the same for reference an hypothesis, got {ref_session_ids} and {hyp_session_ids}.'
+
     # Add information about ref/hyp to each utterance
     ref = ref.map(lambda s: {**s, 'source': 'reference'})
     # TODO: how to encode hypothesis correctly? I want to be able to name them from outside.
     #  Use a new key, "system_name"?
     if len(hyp) > 1:
         hypothesis_keys = [f'hypothesis-{i}' for i in range(len(hyp))]
     else:
@@ -228,24 +293,14 @@
     hyp = SegLST.merge(*[
         h.map(lambda s: {**s, 'source': hypothesis_keys[i]})
         for i, h in enumerate(hyp)
     ])
 
     u = ref + hyp
 
-    data = {
-        'info': {
-            'filename': ref[0]['session_id'],
-            'speakers': list(ref.unique('speaker')),
-            'alignment_type': assignment,
-            'length': max([e['end_time'] for e in u]) - min([e['start_time'] for e in u]),
-            'num_hypotheses': len(hyp),
-        }
-    }
-
     # Sort by begin time. Otherwise, the alignment will be unintuitive and likely not what the user wanted
     u = u.sorted('start_time')
 
     # Convert to words so that the transformation can be applied
     w = get_pseudo_word_level_timings(u, 'character_based')
     w = w.map(lambda w: {**w, 'words': call_with_args(alignment_transform, w), 'original_words': w['words']})
 
@@ -271,17 +326,48 @@
 
     # Map back to original_words
     # and pre-compute things that are required in the visualization
     words = words.map(lambda w: {
         **w,
         'words': w['original_words'],
         'transformed_words': w['words'],
-        'center_time': (w['start_time'] + w['end_time']) / 2,  # Point where the stitches attach
+        'duration': w['end_time'] - w['start_time'],
     })
-    data['words'] = words.segments
+
+    compress = True
+    if compress:
+        data['words'] = {k: words.T.get(k) for k in words.T.keys(all=True)}
+        data['words'] = {
+            k: data['words'][k]
+            for k in [
+                'words',
+                'source',
+                'matches',
+                'speaker',
+                'start_time',
+                'duration',
+            ]
+        }
+        def compress(m):
+            if not m:
+                return m
+            if isinstance(m, (tuple, list)):
+                return [compress(e) for e in m]
+            if isinstance(m, str):
+                return {
+                    'insertion': 'i',
+                    'deletion': 'd',
+                    'substitution': 's',
+                    'correct': 'c',
+                }[m]
+            return m
+        data['words']['matches'] = [compress(m) for m in data['words']['matches']]
+        data['words']['source'] = [{'hypothesis': 'h', 'reference': 'r'}[s] for s in data['words']['source']]
+    else:
+        data['words'] = words.segments
 
     # Add utterances to data. Add total number of words to each utterance
     data['utterances'] = [{**l, 'total': len(l['words'].split())} for l in u]
 
     data['info']['wer'] = {k: dataclasses.asdict(wer) for k, wer in wers.items()}
 
     def wer_by_speaker(hypothesis_key, speaker):
@@ -311,15 +397,15 @@
             reference_self_overlap=None,
             hypothesis_self_overlap=None,
         ))
 
     data['info']['wer_by_speakers'] = {
         k: {
             speaker: wer_by_speaker(k, speaker)
-            for speaker in data['info']['speakers']
+            for speaker in list(ref.unique('speaker'))
         }
         for k in hypothesis_keys
     }
     return data
 
 
 def call_with_args(fn, d):
@@ -351,14 +437,16 @@
             num_minimaps=2,
             show_details=True,
             show_legend=True,
             highlight_regex=None,
             alignment_transform=None,
             markers=None,
             recording_file: 'str | Path | dict[str, str | Path]' = None,
+            js_debug=False,  # If True, don't embed js (and css) code and use absolute paths
+            sync_id=None,
     ):
         if isinstance(reference, (str, Path)):
             reference = meeteval.io.load(reference)
         if isinstance(hypothesis, (str, Path)):
             hypothesis = meeteval.io.load(hypothesis)
         self.reference = reference
         self.hypothesis = hypothesis
@@ -368,22 +456,24 @@
         self.barplot_scale_exclude_total = barplot_scale_exclude_total
         self.num_minimaps = num_minimaps
         self.show_details = show_details
         self.show_legend = show_legend
         self.highlight_regex = highlight_regex
         self.alignment_transform = alignment_transform
         self.markers = markers
+        self.js_debug = js_debug
         if recording_file:
             if not isinstance(recording_file, dict):
                 recording_file = {"": os.fspath(recording_file)}
             for k, v in recording_file.items():
                 assert os.path.exists(v), (k, v, recording_file)
         else:
             recording_file = {'': ''}
         self.recording_file = recording_file
+        self.sync_id = sync_id
 
     def _get_colormap(self):
         if isinstance(self.colormap, str):
             if not self.colormap in self.available_colormaps:
                 raise ValueError(
                     f'Unknown colormap: {self.colormap}. Use one of '
                     f'{self.available_colormaps} or a custom mapping from '
@@ -404,54 +494,142 @@
     def data(self):
         d = get_visualization_data(
             self.reference, self.hypothesis, assignment=self.alignment,
                                    alignment_transform=self.alignment_transform)
         d['markers'] = self.markers
         return d
 
-    def _repr_html_(self):
+    def _iypnb_html_(self):
         """
         Be aware that this writes _a lot of data_ in json format into the
         output cell. This can cause the browser to hang/crash and may produce
         large ipynb files.
         """
-        return self.html()
+        return f'''
+            <html>
+            <style>
+                /* Styles for notebook view */
+                body {{
+                    margin: 1px;
+                    padding: 0;
+                    overflow: hidden;
+                }}
+                
+                .meeteval-viz {{
+                    width: 100%;
+                    height: 80vh; /* 80% of the window height roughly aligns with the visible height in a typical notebook setup */
+                }}
+            </style>
+            {self.html(encode_url=False)}
+            </html>
+            '''
+
+    def _ipython_display_(self):
+        from IPython.display import HTML, display
+
+        reference = meeteval.io.asseglst(self.reference)
+        hypothesis = meeteval.io.asseglst(self.hypothesis)
+
+        ref_session_ids = reference.unique('session_id')
+        hyp_session_ids = hypothesis.unique('session_id')
+
+        if self.js_debug:
+            print('WARNING: js_debug is not supported in ipynb.')
+            self.js_debug = False
+
+        if len(ref_session_ids) > 1 or len(hyp_session_ids) > 1:
+            session_ids = sorted(ref_session_ids & hyp_session_ids)
+            assert len(session_ids) >= 1, (session_ids, ref_session_ids, hyp_session_ids)
+            import ipywidgets
+
+            r = reference.groupby('session_id')
+            h = hypothesis.groupby('session_id')
+
+            cache = {}
+            def func(session_id, alignment):
+                key = (session_id, alignment)
+                if key not in cache:
+                    try:
+                        self.reference = r[session_id]
+                        self.hypothesis = h[session_id]
+                        self.alignment = alignment
+                        cache[key] = self._iypnb_html_()
+                        del self.data
+                    finally:
+                        self.reference = reference
+                        self.hypothesis = hypothesis
+                return HTML(cache[key])
+
+            session_id = ipywidgets.Dropdown(
+                options=session_ids, value=session_ids[0])
+            alignment = ipywidgets.Dropdown(
+                options=['tcp', 'cp'], value=self.alignment)
+            ipywidgets.interact(func, session_id=session_id, alignment=alignment)
+        else:
+            display(HTML(self._iypnb_html_()))
 
-    def html(self):
+    def html(self, encode_url=True):
         """
         Creates a visualization in HTML format.
 
         Note: This HTML contains script and link tags that load external
             libraries, so the visualization will not work offline!
             TODO: Add an option to embed the dependencies into the HTML file.
         """
+        import platformdirs
+
         # Generate data
         element_id = 'viz-' + str(uuid.uuid4())
 
         # Generate HTML and JS for data
-        visualize_js = (Path(__file__).parent / 'visualize.js').read_text()
-        css = (Path(__file__).parent / 'visualize.css').read_text()
+        visualize_js = Path(__file__).parent / 'visualize.js'
+        if self.js_debug:
+            visualize_js = f'''<script src="{visualize_js}" charset="utf-8"></script>'''
+        else:
+            visualize_js = f'<script>{visualize_js.read_text()}</script>'
+
+        css = (Path(__file__).parent / 'visualize.css')
+        if self.js_debug:
+            css = f'<link rel="stylesheet" href="{css}"/>'
+        else:
+            css = f'<style>{css.read_text()}</style>'
+
         highlight_regex = f'"{self.highlight_regex}"' if self.highlight_regex else 'null'
+
+        cdn = {
+            'd3': 'https://cdn.jsdelivr.net/npm/d3@7',
+            # 'font_awesome': 'https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css',
+        }
+
+        cache_dir = Path(platformdirs.user_data_dir('meeteval'))
+        def load_cdn(name, url):
+            file = cache_dir / name
+            try:
+                return file.read_text()
+            except FileNotFoundError:
+                cache_dir.mkdir(parents=True, exist_ok=True)
+                urllib.request.urlretrieve(url, file)
+                return file.read_text()
+
+        d3 = f'<script>{load_cdn("d3.js", cdn["d3"])}</script>'
+        # font_awesome = f'<style>{load_cdn("d3font_awesome.css", cdn["font_awesome"])}</style>'
+
+        font_awesome = ''
         html = f'''
-            <script src="https://cdn.jsdelivr.net/npm/d3@7"></script>
-            <script src="https://cdnjs.cloudflare.com/ajax/libs/howler/2.2.4/howler.min.js"></script>
-            <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" integrity="sha512-z3gLpd7yknf1YoNbCzqRKc4qyor8gaKU1qmn+CShxbuBusANI9QpRohGBreCFkKxLhei6S9CQXFEbbKuqLg0DA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
-            <style>
-                {css}
-            </style>
-            <div style="margin: auto" class="meeteval-viz">
-                <div id='{element_id}'></div>
-            <div>
+            {d3}
+            {font_awesome}
+            {css}
+            <div class="meeteval-viz" id='{element_id}'><div>
+            {visualize_js}
             <script>
-                {visualize_js}
 
                 function exec() {{
                     // Wait for d3 to load
                     if (typeof d3 !== 'undefined') alignment_visualization(
-                        {dumps_json(self.data, indent=None, sort_keys=False)}, 
+                        {dumps_json(self.data, indent=None, sort_keys=False, separators=(',', ':'), float_round=4)},
                         "#{element_id}",
                         {{
                             colors: {self._get_colormap()},
                             barplot: {{
                                 style: "{self.barplot_style}",
                                 scaleExcludeCorrect: {'true' if self.barplot_scale_exclude_total else 'false'}
                             }},
@@ -459,27 +637,65 @@
                                 number: {self.num_minimaps}
                             }},
                             show_details: {'true' if self.show_details else 'false'},
                             show_legend: {'true' if self.show_legend else 'false'},
                             search_bar: {{
                                 initial_query: {highlight_regex}
                             }},
-                            recording_file: {json.dumps(self.recording_file, default=os.fspath)}
+                            recording_file: {dumps_json(self.recording_file, default=os.fspath)},
+                            match_width: 0.1,
+                            syncID: {dumps_json(self.sync_id, default='null')},
+                            audio_server: 'http://localhost:7777',
+                            encodeURL: {'true' if encode_url else 'false'},
                         }}
                     );
                     else setTimeout(exec, 100);
                 }}
                 exec();
                 
             </script>
         '''
         return html
 
     def dump(self, filename):
-        Path(filename).write_text(self.html())
+        # For standalone HTML, we have to
+        #   - disable zooming for mobile devices (viewport setting)
+        #   - Scale the visualization to the full window size
+        Path(filename).write_text(
+            f'''
+            <!DOCTYPE html>
+            <html lang="en">
+            <meta charset="utf-8">
+            <meta name="viewport" content="width=device-width, user-scalable=no" />
+            <style>
+                /* Styles for full-screen view */
+                html {{
+                    height: 100%;
+                    width: 100%;
+                }}
+
+                body {{
+                    height: 100%;
+                    width: 100%;
+                    margin: 1px;
+                    padding: 0;
+                    /* Make sure that no scroll bars appear */
+                    overflow: hidden;
+                    font-family: Arial, Helvetica, sans-serif;
+                }}
+                
+                .meeteval-viz {{
+                    width: 100%;
+                    height: 100%;
+                }}
+            </style>
+            {self.html()}
+            </html>
+            '''
+        )
 
 
 def cli():
     import argparse
     parser = argparse.ArgumentParser(add_help=False)
     parser.add_argument(
         '--help', help='show this help message and exit',
```

### Comparing `meeteval-0.2.1/meeteval/wer/__main__.py` & `meeteval-0.3.0/meeteval/wer/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -164,56 +164,64 @@
         reference, hypothesis,
         average_out='{parent}/{stem}_orcwer.json',
         per_reco_out='{parent}/{stem}_orcwer_per_reco.json',
         regex=None,
         reference_sort='segment',
         hypothesis_sort='segment',
         uem=None,
+        partial=False,
+        normalizer=None,
 ):
     """Computes the Optimal Reference Combination Word Error Rate (ORC WER)"""
     results = meeteval.wer.orcwer(
         reference, hypothesis, regex=regex,
         reference_sort=reference_sort, hypothesis_sort=hypothesis_sort,
         uem=uem,
+        partial=partial,
+        normalizer=normalizer,
     )
     _save_results(results, hypothesis, per_reco_out, average_out)
 
 
 def cpwer(
         reference, hypothesis,
         average_out='{parent}/{stem}_cpwer.json',
         per_reco_out='{parent}/{stem}_cpwer_per_reco.json',
         regex=None,
         reference_sort='segment',
         hypothesis_sort='segment',
         uem=None,
+        normalizer=None,
+        partial=False,
 ):
     """Computes the Concatenated minimum-Permutation Word Error Rate (cpWER)"""
     results = meeteval.wer.cpwer(
         reference, hypothesis, regex=regex,
         reference_sort=reference_sort, hypothesis_sort=hypothesis_sort,
-        uem=uem,
+        uem=uem, partial=partial, normalizer=normalizer,
     )
     _save_results(results, hypothesis, per_reco_out, average_out)
 
 
 def mimower(
         reference, hypothesis,
         average_out='{parent}/{stem}_mimower.json',
         per_reco_out='{parent}/{stem}_mimower_per_reco.json',
         regex=None,
         reference_sort='segment',
         hypothesis_sort='segment',
         uem=None,
+        normalizer=None,
+        partial=False,
 ):
     """Computes the MIMO WER"""
     results = meeteval.wer.mimower(
         reference, hypothesis, regex=regex,
         reference_sort=reference_sort, hypothesis_sort=hypothesis_sort,
-        uem=uem,
+        uem=uem, partial=partial, normalizer=normalizer,
     )
     _save_results(results, hypothesis, per_reco_out, average_out)
 
 
 def tcpwer(
         reference, hypothesis,
         average_out='{parent}/{stem}_tcpwer.json',
@@ -221,24 +229,26 @@
         collar=0,
         hyp_pseudo_word_timing='character_based_points',
         ref_pseudo_word_timing='character_based',
         regex=None,
         reference_sort='segment',
         hypothesis_sort='segment',
         uem=None,
+        normalizer=None,
+        partial=False,
 ):
     """Computes the time-constrained minimum permutation WER"""
     results = meeteval.wer.tcpwer(
         reference, hypothesis, regex=regex,
         ref_pseudo_word_timing=ref_pseudo_word_timing,
         hyp_pseudo_word_timing=hyp_pseudo_word_timing,
         collar=collar,
         reference_sort=reference_sort,
         hypothesis_sort=hypothesis_sort,
-        uem=uem,
+        uem=uem, normalizer=normalizer, partial=partial,
     )
     _save_results(results, hypothesis, per_reco_out, average_out)
 
 
 def tcorcwer(
         reference, hypothesis,
         average_out='{parent}/{stem}_tcorcwer.json',
@@ -246,24 +256,27 @@
         regex=None,
         collar=0,
         hyp_pseudo_word_timing='character_based_points',
         ref_pseudo_word_timing='character_based',
         hypothesis_sort='segment',
         reference_sort='segment',
         uem=None,
+        normalizer=None,
+        partial=False,
 ):
     """Computes the time-constrained ORC WER (tcORC WER)"""
     results = meeteval.wer.tcorcwer(
         reference, hypothesis, regex=regex,
         collar=collar,
         hyp_pseudo_word_timing=hyp_pseudo_word_timing,
         ref_pseudo_word_timing=ref_pseudo_word_timing,
         hypothesis_sort=hypothesis_sort,
         reference_sort=reference_sort,
-        uem=uem,
+        uem=uem, partial=partial,
+        normalizer=normalizer,
     )
     _save_results(results, hypothesis, per_reco_out, average_out)
 
 
 def _merge(
         files: 'list[str]',
         out: str = '-',
@@ -491,18 +504,34 @@
                      '- True: Sort by segment start time and assert that the word-level timings are sorted by start '
                      'time. Only supported for time-constrained WERs\n'
                      '- word: sort words by start time. Only supported for time-constrained WERs'
             )
         elif name == 'uem':
             command_parser.add_argument(
                 '--uem',
-                help='UEM file that defines the scoring regions. Only supported when reference and hypothesis files'
+                help='UEM file that defines the scoring regions. Only supported when reference and hypothesis files '
                      'contain time-stamps.',
                 nargs='+', action=self.extend_action,
             )
+        elif name == 'normalizer':
+            command_parser.add_argument(
+                '--normalizer',
+                help='A normalizer that is applied to the transcript.\n'
+                     'Choices:\n'
+                     '- None: Do nothing (default)\n'
+                     '- lower,rm(.?!,): Lowercase the transcript and remove punctuations (.,?!).',
+                choices=[None, 'lower,rm(.?!,)'],
+            )
+        elif name == 'partial':
+            command_parser.add_argument(
+                '--partial',
+                action='store_true',
+                help='Compute the metrics on the subset of sessions defined in the reference files.'
+                     'Ignore any sessions present in the hypothesis but not in the reference.'
+            )
         elif name == 'files':
             command_parser.add_argument('files', nargs='+')
         else:
             raise AssertionError("Error in command definition", name)
 
     def add_command(self, fn, command_name=None):
         if command_name is None:
```

### Comparing `meeteval-0.2.1/meeteval/wer/api.py` & `meeteval-0.3.0/meeteval/wer/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 def _load_texts(
         reference_paths: 'list[str]',
         hypothesis_paths: 'list[str]',
         regex,
         reference_sort: 'bool | str' = False,
         hypothesis_sort: 'bool | str' = False,
         file_format=None,
+        normalizer=None,
         uem=None,
 ) -> 'tuple[meeteval.io.SegLST, meeteval.io.SegLST]':
     """Load and validate reference and hypothesis texts.
 
     Validation checks that reference and hypothesis have the same example IDs.
     """
     # Load input files
@@ -122,91 +123,110 @@
             f'time-constrained WERs.'
         )
     else:
         raise ValueError(
             f'Unknown choice for hypothesis_sort: {hypothesis_sort}'
         )
 
+    if normalizer is not None:
+        if normalizer == 'lower,rm(.?!,)':
+            def normalizer(seg):
+                seg['words'] = seg['words'].lower().replace('.', '').replace('?', '').replace('!', '').replace(',', '')
+                return seg
+        else:
+            raise NotImplementedError(normalizer)
+        reference = reference.map(normalizer)
+        hypothesis = hypothesis.map(normalizer)
+
     return reference, hypothesis
 
 
 def orcwer(
         reference, hypothesis,
         regex=None,
         reference_sort='segment',
         hypothesis_sort='segment',
         uem=None,
+        partial=False,
+        normalizer=None,
 ):
     """Computes the Optimal Reference Combination Word Error Rate (ORC WER)"""
     from meeteval.wer.wer.orc import orc_word_error_rate_multifile
     reference, hypothesis = _load_texts(
         reference, hypothesis, regex=regex,
         reference_sort=reference_sort, hypothesis_sort=hypothesis_sort,
-        uem=uem,
+        uem=uem, normalizer=normalizer,
     )
-    results = orc_word_error_rate_multifile(reference, hypothesis)
+    results = orc_word_error_rate_multifile(reference, hypothesis, partial=partial)
     return results
 
 
 def cpwer(
         reference, hypothesis,
         regex=None,
         reference_sort='segment',
         hypothesis_sort='segment',
         uem=None,
+        normalizer=None,
+        partial=False
 ):
     """Computes the Concatenated minimum-Permutation Word Error Rate (cpWER)"""
     from meeteval.wer.wer.cp import cp_word_error_rate_multifile
     reference, hypothesis = _load_texts(
         reference, hypothesis, regex=regex,
         reference_sort=reference_sort, hypothesis_sort=hypothesis_sort,
-        uem=uem,
+        uem=uem, normalizer=normalizer,
     )
-    results = cp_word_error_rate_multifile(reference, hypothesis)
+    results = cp_word_error_rate_multifile(reference, hypothesis, partial=partial)
     return results
 
 
 def mimower(
         reference, hypothesis,
         regex=None,
         reference_sort='segment',
         hypothesis_sort='segment',
         uem=None,
+        normalizer=None,
+        partial=False,
 ):
     """Computes the MIMO WER"""
     from meeteval.wer.wer.mimo import mimo_word_error_rate_multifile
     reference, hypothesis = _load_texts(
         reference, hypothesis, regex=regex,
         reference_sort=reference_sort, hypothesis_sort=hypothesis_sort,
-        uem=uem,
+        uem=uem, normalizer=normalizer
     )
-    results = mimo_word_error_rate_multifile(reference, hypothesis)
+    results = mimo_word_error_rate_multifile(reference, hypothesis, partial=partial)
     return results
 
 
 def tcpwer(
         reference, hypothesis,
         collar=0,
         hyp_pseudo_word_timing='character_based_points',
         ref_pseudo_word_timing='character_based',
         regex=None,
         reference_sort='segment',
         hypothesis_sort='segment',
         uem=None,
+        normalizer=None,
+        partial=False,
 ):
     """Computes the time-constrained minimum permutation WER"""
     from meeteval.wer.wer.time_constrained import tcp_word_error_rate_multifile
-    reference, hypothesis = _load_texts(reference, hypothesis, regex=regex, uem=uem)
+    reference, hypothesis = _load_texts(reference, hypothesis, regex=regex, uem=uem, normalizer=normalizer)
     results = tcp_word_error_rate_multifile(
         reference, hypothesis,
         reference_pseudo_word_level_timing=ref_pseudo_word_timing,
         hypothesis_pseudo_word_level_timing=hyp_pseudo_word_timing,
         collar=collar,
         reference_sort=reference_sort,
         hypothesis_sort=hypothesis_sort,
+        partial=partial,
     )
     from meeteval.wer import combine_error_rates
     average: ErrorRate = combine_error_rates(results)
     if average.hypothesis_self_overlap is not None:
         average.hypothesis_self_overlap.warn('hypothesis')
     if average.reference_self_overlap is not None:
         average.reference_self_overlap.warn('reference')
@@ -218,25 +238,28 @@
         regex=None,
         collar=0,
         hyp_pseudo_word_timing='character_based_points',
         ref_pseudo_word_timing='character_based',
         hypothesis_sort='segment',
         reference_sort='segment',
         uem=None,
+        normalizer=None,
+        partial=False,
 ):
     """Computes the time-constrained ORC WER"""
     from meeteval.wer.wer.time_constrained_orc import time_constrained_orc_wer_multifile
-    reference, hypothesis = _load_texts(reference, hypothesis, regex=regex, uem=uem)
+    reference, hypothesis = _load_texts(reference, hypothesis, regex=regex, uem=uem, normalizer=normalizer)
     results = time_constrained_orc_wer_multifile(
         reference, hypothesis,
         reference_pseudo_word_level_timing=ref_pseudo_word_timing,
         hypothesis_pseudo_word_level_timing=hyp_pseudo_word_timing,
         collar=collar,
         hypothesis_sort=hypothesis_sort,
         reference_sort=reference_sort,
+        partial=partial,
     )
     from meeteval.wer import combine_error_rates
     average: ErrorRate = combine_error_rates(results)
     if average.hypothesis_self_overlap is not None:
         average.hypothesis_self_overlap.warn('hypothesis')
     if average.reference_self_overlap is not None:
         average.reference_self_overlap.warn('reference')
```

### Comparing `meeteval-0.2.1/meeteval/wer/matching/cy_levenshtein.cpp` & `meeteval-0.3.0/meeteval/wer/matching/cy_levenshtein.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "meeteval/wer/matching/levenshtein.h"
         ],
@@ -45,18 +45,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -140,14 +140,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -201,14 +203,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -262,60 +266,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -398,14 +425,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -757,16 +787,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1110,15 +1145,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1197,15 +1232,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1318,32 +1353,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -24759,24 +24777,26 @@
   __Pyx_XDECREF(__pyx_v_reference_);
   __Pyx_XDECREF(__pyx_v_hypothesis_);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr *__pyx_freelist_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr[8];
 static int __pyx_freecount_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr)))) {
     o = (PyObject*)__pyx_freelist_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr[--__pyx_freecount_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -24796,15 +24816,15 @@
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_t);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr)))) {
     __pyx_freelist_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr[__pyx_freecount_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr++] = ((struct __pyx_obj_8meeteval_3wer_8matching_14cy_levenshtein___pyx_scope_struct__genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -31919,15 +31939,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `meeteval-0.2.1/meeteval/wer/matching/cy_levenshtein.pyx` & `meeteval-0.3.0/meeteval/wer/matching/cy_levenshtein.pyx`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/wer/matching/cy_mimo_matching.cpp` & `meeteval-0.3.0/meeteval/wer/matching/cy_mimo_matching.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "meeteval/wer/matching/mimo_matching.h"
         ],
@@ -45,18 +45,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -140,14 +140,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -201,14 +203,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -262,60 +266,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -398,14 +425,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -757,16 +787,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1110,15 +1145,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1197,15 +1232,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1317,32 +1352,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -10571,15 +10589,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `meeteval-0.2.1/meeteval/wer/matching/cy_mimo_matching.pyx` & `meeteval-0.3.0/meeteval/wer/matching/cy_mimo_matching.pyx`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/wer/matching/cy_orc_matching.cpp` & `meeteval-0.3.0/meeteval/wer/matching/cy_orc_matching.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-std=c++11"
@@ -40,18 +40,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -135,14 +135,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -196,14 +198,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -257,60 +261,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -393,14 +420,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -752,16 +782,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1105,15 +1140,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1192,15 +1227,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1298,32 +1333,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -7679,15 +7697,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `meeteval-0.2.1/meeteval/wer/matching/cy_orc_matching.pyx` & `meeteval-0.3.0/meeteval/wer/matching/cy_orc_matching.pyx`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/wer/matching/cy_time_constrained_orc_matching.cpp` & `meeteval-0.3.0/meeteval/wer/matching/cy_time_constrained_orc_matching.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "meeteval/wer/matching/time_constrained_orc_matching.h"
         ],
@@ -46,18 +46,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -141,14 +141,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -202,14 +204,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -263,60 +267,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -399,14 +426,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -758,16 +788,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1111,15 +1146,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1198,15 +1233,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1316,32 +1351,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1528,35 +1546,35 @@
 /* #### Code section: complex_type_declarations ### */
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr;
 struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr;
 
-/* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":32
+/* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":36
  *     # Shortcuts for trivial cases
  *     if len(reference) == 0:
  *         return sum(len(h) for h in hypothesis), []             # <<<<<<<<<<<<<<
  *     if len(hypothesis) == 0:
- *         return sum(len(r) for r in reference), []
+ *         # 0 is a dummy stream index
  */
 struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr {
   PyObject_HEAD
   PyObject *__pyx_genexpr_arg_0;
   PyObject *__pyx_v_h;
   PyObject *__pyx_t_0;
   Py_ssize_t __pyx_t_1;
   PyObject *(*__pyx_t_2)(PyObject *);
 };
 
 
-/* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":34
- *         return sum(len(h) for h in hypothesis), []
+/* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":39
  *     if len(hypothesis) == 0:
- *         return sum(len(r) for r in reference), []             # <<<<<<<<<<<<<<
+ *         # 0 is a dummy stream index
+ *         return sum(len(r) for r in reference), [0] * len(reference)             # <<<<<<<<<<<<<<
  * 
  *     # Translate symbols/words to integers for the cpp code
  */
 struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr {
   PyObject_HEAD
   PyObject *__pyx_genexpr_arg_0;
   PyObject *__pyx_v_r;
@@ -2537,14 +2555,15 @@
   PyObject *__pyx_n_s_sym2int;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_throw;
   PyObject *__pyx_n_s_time_constrained_orc_levenshtein;
   PyObject *__pyx_n_s_time_constrained_orc_levenshtein_2;
   PyObject *__pyx_n_s_update;
   PyObject *__pyx_n_s_v;
+  PyObject *__pyx_int_0;
   PyObject *__pyx_tuple_;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__3;
   PyObject *__pyx_codeobj__4;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
@@ -2628,14 +2647,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_sym2int);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_throw);
   Py_CLEAR(clear_module_state->__pyx_n_s_time_constrained_orc_levenshtein);
   Py_CLEAR(clear_module_state->__pyx_n_s_time_constrained_orc_levenshtein_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
   Py_CLEAR(clear_module_state->__pyx_n_s_v);
+  Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_tuple_);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__3);
   Py_CLEAR(clear_module_state->__pyx_codeobj__4);
   return 0;
 }
 #endif
@@ -2697,14 +2717,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_sym2int);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_throw);
   Py_VISIT(traverse_module_state->__pyx_n_s_time_constrained_orc_levenshtein);
   Py_VISIT(traverse_module_state->__pyx_n_s_time_constrained_orc_levenshtein_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
   Py_VISIT(traverse_module_state->__pyx_n_s_v);
+  Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_tuple_);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__3);
   Py_VISIT(traverse_module_state->__pyx_codeobj__4);
   return 0;
 }
 #endif
@@ -2782,14 +2803,15 @@
 #define __pyx_n_s_sym2int __pyx_mstate_global->__pyx_n_s_sym2int
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_throw __pyx_mstate_global->__pyx_n_s_throw
 #define __pyx_n_s_time_constrained_orc_levenshtein __pyx_mstate_global->__pyx_n_s_time_constrained_orc_levenshtein
 #define __pyx_n_s_time_constrained_orc_levenshtein_2 __pyx_mstate_global->__pyx_n_s_time_constrained_orc_levenshtein_2
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
 #define __pyx_n_s_v __pyx_mstate_global->__pyx_n_s_v
+#define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
 #define __pyx_codeobj__4 __pyx_mstate_global->__pyx_codeobj__4
 /* #### Code section: module_code ### */
 
 /* "vector.from_py":45
@@ -3682,15 +3704,16 @@
 static PyObject *__pyx_pw_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_1time_constrained_orc_levenshtein_distance(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_1time_constrained_orc_levenshtein_distance = {"time_constrained_orc_levenshtein_distance", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_1time_constrained_orc_levenshtein_distance, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+PyDoc_STRVAR(__pyx_doc_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_time_constrained_orc_levenshtein_distance, "\n    Compute the time-constrained ORC Levenshtein distance between two sequences of \n    symbols and returns the distance and the alignment.\n    ");
+static PyMethodDef __pyx_mdef_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_1time_constrained_orc_levenshtein_distance = {"time_constrained_orc_levenshtein_distance", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_1time_constrained_orc_levenshtein_distance, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_time_constrained_orc_levenshtein_distance};
 static PyObject *__pyx_pw_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_1time_constrained_orc_levenshtein_distance(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
@@ -3816,43 +3839,43 @@
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_41time_constrained_orc_levenshtein_distance_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":32
+/* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":36
  *     # Shortcuts for trivial cases
  *     if len(reference) == 0:
  *         return sum(len(h) for h in hypothesis), []             # <<<<<<<<<<<<<<
  *     if len(hypothesis) == 0:
- *         return sum(len(r) for r in reference), []
+ *         # 0 is a dummy stream index
  */
 
 static PyObject *__pyx_pf_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_41time_constrained_orc_levenshtein_distance_genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0) {
   struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr *)__pyx_tp_new_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr(__pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 32, __pyx_L1_error)
+    __PYX_ERR(0, 36, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_41time_constrained_orc_levenshtein_distance_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_time_constrained_orc_levenshtein, __pyx_n_s_meeteval_wer_matching_cy_time_co); if (unlikely(!gen)) __PYX_ERR(0, 32, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_41time_constrained_orc_levenshtein_distance_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_time_constrained_orc_levenshtein, __pyx_n_s_meeteval_wer_matching_cy_time_co); if (unlikely(!gen)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3882,74 +3905,74 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 32, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 32, __pyx_L1_error) }
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 36, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 36, __pyx_L1_error) }
   if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) {
     __pyx_t_1 = __pyx_cur_scope->__pyx_genexpr_arg_0; __Pyx_INCREF(__pyx_t_1);
     __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 32, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 32, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 36, __pyx_L1_error)
           #endif
           if (__pyx_t_2 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 32, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 36, __pyx_L1_error)
         #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 32, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 36, __pyx_L1_error)
           #endif
           if (__pyx_t_2 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 32, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 36, __pyx_L1_error)
         #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 32, __pyx_L1_error)
+          else __PYX_ERR(0, 36, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_h);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_h, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_5 = PyObject_Length(__pyx_cur_scope->__pyx_v_h); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 32, __pyx_L1_error)
-    __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+    __pyx_t_5 = PyObject_Length(__pyx_cur_scope->__pyx_v_h); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 36, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     __Pyx_XGIVEREF(__pyx_t_1);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_2;
     __pyx_cur_scope->__pyx_t_2 = __pyx_t_3;
@@ -3961,15 +3984,15 @@
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 32, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 36, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -3986,18 +4009,18 @@
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_41time_constrained_orc_levenshtein_distance_5generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":34
- *         return sum(len(h) for h in hypothesis), []
+/* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":39
  *     if len(hypothesis) == 0:
- *         return sum(len(r) for r in reference), []             # <<<<<<<<<<<<<<
+ *         # 0 is a dummy stream index
+ *         return sum(len(r) for r in reference), [0] * len(reference)             # <<<<<<<<<<<<<<
  * 
  *     # Translate symbols/words to integers for the cpp code
  */
 
 static PyObject *__pyx_pf_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_41time_constrained_orc_levenshtein_distance_3genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0) {
   struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
@@ -4006,23 +4029,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr *)__pyx_tp_new_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr(__pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 34, __pyx_L1_error)
+    __PYX_ERR(0, 39, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_41time_constrained_orc_levenshtein_distance_5generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_time_constrained_orc_levenshtein, __pyx_n_s_meeteval_wer_matching_cy_time_co); if (unlikely(!gen)) __PYX_ERR(0, 34, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_41time_constrained_orc_levenshtein_distance_5generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_time_constrained_orc_levenshtein, __pyx_n_s_meeteval_wer_matching_cy_time_co); if (unlikely(!gen)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4052,74 +4075,74 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 34, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 34, __pyx_L1_error) }
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 39, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 39, __pyx_L1_error) }
   if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) {
     __pyx_t_1 = __pyx_cur_scope->__pyx_genexpr_arg_0; __Pyx_INCREF(__pyx_t_1);
     __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 34, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 39, __pyx_L1_error)
           #endif
           if (__pyx_t_2 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 34, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 39, __pyx_L1_error)
         #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 39, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 34, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 39, __pyx_L1_error)
           #endif
           if (__pyx_t_2 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 34, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 39, __pyx_L1_error)
         #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 39, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 34, __pyx_L1_error)
+          else __PYX_ERR(0, 39, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_r);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_r, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_5 = PyObject_Length(__pyx_cur_scope->__pyx_v_r); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 34, __pyx_L1_error)
-    __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
+    __pyx_t_5 = PyObject_Length(__pyx_cur_scope->__pyx_v_r); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 39, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     __Pyx_XGIVEREF(__pyx_t_1);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_2;
     __pyx_cur_scope->__pyx_t_2 = __pyx_t_3;
@@ -4131,15 +4154,15 @@
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 34, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 39, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -4204,782 +4227,790 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("time_constrained_orc_levenshtein_distance", 0);
   __Pyx_INCREF(__pyx_v_reference);
   __Pyx_INCREF(__pyx_v_hypothesis);
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":25
- * ):
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":29
+ *     """
  *     # Validate inputs
  *     if len(reference) != len(reference_timings):             # <<<<<<<<<<<<<<
  *         raise ValueError("reference and reference_timings must have the same length")
  *     if len(hypothesis) != len(hypothesis_timings):
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_reference); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 25, __pyx_L1_error)
-  __pyx_t_2 = PyObject_Length(__pyx_v_reference_timings); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_reference); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_v_reference_timings); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 29, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_1 != __pyx_t_2);
   if (unlikely(__pyx_t_3)) {
 
-    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":26
+    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":30
  *     # Validate inputs
  *     if len(reference) != len(reference_timings):
  *         raise ValueError("reference and reference_timings must have the same length")             # <<<<<<<<<<<<<<
  *     if len(hypothesis) != len(hypothesis_timings):
  *         raise ValueError("hypothesis and hypothesis_timings must have the same length")
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 26, __pyx_L1_error)
+    __PYX_ERR(0, 30, __pyx_L1_error)
 
-    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":25
- * ):
+    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":29
+ *     """
  *     # Validate inputs
  *     if len(reference) != len(reference_timings):             # <<<<<<<<<<<<<<
  *         raise ValueError("reference and reference_timings must have the same length")
  *     if len(hypothesis) != len(hypothesis_timings):
  */
   }
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":27
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":31
  *     if len(reference) != len(reference_timings):
  *         raise ValueError("reference and reference_timings must have the same length")
  *     if len(hypothesis) != len(hypothesis_timings):             # <<<<<<<<<<<<<<
  *         raise ValueError("hypothesis and hypothesis_timings must have the same length")
  * 
  */
-  __pyx_t_2 = PyObject_Length(__pyx_v_hypothesis); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 27, __pyx_L1_error)
-  __pyx_t_1 = PyObject_Length(__pyx_v_hypothesis_timings); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_v_hypothesis); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_hypothesis_timings); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 31, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_2 != __pyx_t_1);
   if (unlikely(__pyx_t_3)) {
 
-    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":28
+    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":32
  *         raise ValueError("reference and reference_timings must have the same length")
  *     if len(hypothesis) != len(hypothesis_timings):
  *         raise ValueError("hypothesis and hypothesis_timings must have the same length")             # <<<<<<<<<<<<<<
  * 
  *     # Shortcuts for trivial cases
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 28, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 28, __pyx_L1_error)
+    __PYX_ERR(0, 32, __pyx_L1_error)
 
-    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":27
+    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":31
  *     if len(reference) != len(reference_timings):
  *         raise ValueError("reference and reference_timings must have the same length")
  *     if len(hypothesis) != len(hypothesis_timings):             # <<<<<<<<<<<<<<
  *         raise ValueError("hypothesis and hypothesis_timings must have the same length")
  * 
  */
   }
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":31
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":35
  * 
  *     # Shortcuts for trivial cases
  *     if len(reference) == 0:             # <<<<<<<<<<<<<<
  *         return sum(len(h) for h in hypothesis), []
  *     if len(hypothesis) == 0:
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_reference); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_reference); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 35, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_1 == 0);
   if (__pyx_t_3) {
 
-    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":32
+    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":36
  *     # Shortcuts for trivial cases
  *     if len(reference) == 0:
  *         return sum(len(h) for h in hypothesis), []             # <<<<<<<<<<<<<<
  *     if len(hypothesis) == 0:
- *         return sum(len(r) for r in reference), []
+ *         # 0 is a dummy stream index
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __pyx_pf_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_41time_constrained_orc_levenshtein_distance_genexpr(NULL, __pyx_v_hypothesis); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+    __pyx_t_4 = __pyx_pf_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_41time_constrained_orc_levenshtein_distance_genexpr(NULL, __pyx_v_hypothesis); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 32, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 32, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_5);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5)) __PYX_ERR(0, 32, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_4);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error);
     __pyx_t_5 = 0;
     __pyx_t_4 = 0;
     __pyx_r = __pyx_t_6;
     __pyx_t_6 = 0;
     goto __pyx_L0;
 
-    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":31
+    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":35
  * 
  *     # Shortcuts for trivial cases
  *     if len(reference) == 0:             # <<<<<<<<<<<<<<
  *         return sum(len(h) for h in hypothesis), []
  *     if len(hypothesis) == 0:
  */
   }
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":33
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":37
  *     if len(reference) == 0:
  *         return sum(len(h) for h in hypothesis), []
  *     if len(hypothesis) == 0:             # <<<<<<<<<<<<<<
- *         return sum(len(r) for r in reference), []
- * 
+ *         # 0 is a dummy stream index
+ *         return sum(len(r) for r in reference), [0] * len(reference)
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_hypothesis); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_hypothesis); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 37, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_1 == 0);
   if (__pyx_t_3) {
 
-    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":34
- *         return sum(len(h) for h in hypothesis), []
+    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":39
  *     if len(hypothesis) == 0:
- *         return sum(len(r) for r in reference), []             # <<<<<<<<<<<<<<
+ *         # 0 is a dummy stream index
+ *         return sum(len(r) for r in reference), [0] * len(reference)             # <<<<<<<<<<<<<<
  * 
  *     # Translate symbols/words to integers for the cpp code
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_6 = __pyx_pf_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_41time_constrained_orc_levenshtein_distance_3genexpr(NULL, __pyx_v_reference); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 34, __pyx_L1_error)
+    __pyx_t_6 = __pyx_pf_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching_41time_constrained_orc_levenshtein_distance_3genexpr(NULL, __pyx_v_reference); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 34, __pyx_L1_error)
+    __pyx_t_1 = PyObject_Length(__pyx_v_reference); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 39, __pyx_L1_error)
+    __pyx_t_6 = PyList_New(1 * ((__pyx_t_1<0) ? 0:__pyx_t_1)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 34, __pyx_L1_error)
+    { Py_ssize_t __pyx_temp;
+      for (__pyx_temp=0; __pyx_temp < __pyx_t_1; __pyx_temp++) {
+        __Pyx_INCREF(__pyx_int_0);
+        __Pyx_GIVEREF(__pyx_int_0);
+        if (__Pyx_PyList_SET_ITEM(__pyx_t_6, __pyx_temp, __pyx_int_0)) __PYX_ERR(0, 39, __pyx_L1_error);
+      }
+    }
+    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_4);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4)) __PYX_ERR(0, 39, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_6);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_6)) __PYX_ERR(0, 34, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_6)) __PYX_ERR(0, 39, __pyx_L1_error);
     __pyx_t_4 = 0;
     __pyx_t_6 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":33
+    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":37
  *     if len(reference) == 0:
  *         return sum(len(h) for h in hypothesis), []
  *     if len(hypothesis) == 0:             # <<<<<<<<<<<<<<
- *         return sum(len(r) for r in reference), []
- * 
+ *         # 0 is a dummy stream index
+ *         return sum(len(r) for r in reference), [0] * len(reference)
  */
   }
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":37
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":42
  * 
  *     # Translate symbols/words to integers for the cpp code
  *     all_symbols = set()             # <<<<<<<<<<<<<<
  *     for r in reference:
  *         all_symbols.update(set(list(r)))
  */
-  __pyx_t_5 = PySet_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_5 = PySet_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_v_all_symbols = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":38
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":43
  *     # Translate symbols/words to integers for the cpp code
  *     all_symbols = set()
  *     for r in reference:             # <<<<<<<<<<<<<<
  *         all_symbols.update(set(list(r)))
  *     for h in hypothesis:
  */
   if (likely(PyList_CheckExact(__pyx_v_reference)) || PyTuple_CheckExact(__pyx_v_reference)) {
     __pyx_t_5 = __pyx_v_reference; __Pyx_INCREF(__pyx_t_5);
     __pyx_t_1 = 0;
     __pyx_t_7 = NULL;
   } else {
-    __pyx_t_1 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_reference); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 38, __pyx_L1_error)
+    __pyx_t_1 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_reference); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 38, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 43, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_5))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 38, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 43, __pyx_L1_error)
           #endif
           if (__pyx_t_1 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_1); __Pyx_INCREF(__pyx_t_6); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 38, __pyx_L1_error)
+        __pyx_t_6 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_1); __Pyx_INCREF(__pyx_t_6); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 43, __pyx_L1_error)
         #else
-        __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 38, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 43, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_5);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 38, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 43, __pyx_L1_error)
           #endif
           if (__pyx_t_1 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_1); __Pyx_INCREF(__pyx_t_6); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 38, __pyx_L1_error)
+        __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_1); __Pyx_INCREF(__pyx_t_6); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 43, __pyx_L1_error)
         #else
-        __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 38, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 43, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         #endif
       }
     } else {
       __pyx_t_6 = __pyx_t_7(__pyx_t_5);
       if (unlikely(!__pyx_t_6)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 38, __pyx_L1_error)
+          else __PYX_ERR(0, 43, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_6);
     }
     __Pyx_XDECREF_SET(__pyx_v_r, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":39
+    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":44
  *     all_symbols = set()
  *     for r in reference:
  *         all_symbols.update(set(list(r)))             # <<<<<<<<<<<<<<
  *     for h in hypothesis:
  *         all_symbols.update(set(list(h)))
  */
-    __pyx_t_6 = PySequence_List(__pyx_v_r); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 39, __pyx_L1_error)
+    __pyx_t_6 = PySequence_List(__pyx_v_r); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 44, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = PySet_New(__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 39, __pyx_L1_error)
+    __pyx_t_4 = PySet_New(__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PySet_Type_update, __pyx_v_all_symbols, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 39, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PySet_Type_update, __pyx_v_all_symbols, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 44, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":38
+    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":43
  *     # Translate symbols/words to integers for the cpp code
  *     all_symbols = set()
  *     for r in reference:             # <<<<<<<<<<<<<<
  *         all_symbols.update(set(list(r)))
  *     for h in hypothesis:
  */
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":40
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":45
  *     for r in reference:
  *         all_symbols.update(set(list(r)))
  *     for h in hypothesis:             # <<<<<<<<<<<<<<
  *         all_symbols.update(set(list(h)))
  *     int2sym = dict(enumerate(sorted(all_symbols)))
  */
   if (likely(PyList_CheckExact(__pyx_v_hypothesis)) || PyTuple_CheckExact(__pyx_v_hypothesis)) {
     __pyx_t_5 = __pyx_v_hypothesis; __Pyx_INCREF(__pyx_t_5);
     __pyx_t_1 = 0;
     __pyx_t_7 = NULL;
   } else {
-    __pyx_t_1 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_hypothesis); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __pyx_t_1 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_hypothesis); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 45, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 45, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_5))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 40, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 45, __pyx_L1_error)
           #endif
           if (__pyx_t_1 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_1); __Pyx_INCREF(__pyx_t_6); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 40, __pyx_L1_error)
+        __pyx_t_6 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_1); __Pyx_INCREF(__pyx_t_6); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 45, __pyx_L1_error)
         #else
-        __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 40, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 45, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_5);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 40, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 45, __pyx_L1_error)
           #endif
           if (__pyx_t_1 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_1); __Pyx_INCREF(__pyx_t_6); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 40, __pyx_L1_error)
+        __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_1); __Pyx_INCREF(__pyx_t_6); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 45, __pyx_L1_error)
         #else
-        __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 40, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 45, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         #endif
       }
     } else {
       __pyx_t_6 = __pyx_t_7(__pyx_t_5);
       if (unlikely(!__pyx_t_6)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 40, __pyx_L1_error)
+          else __PYX_ERR(0, 45, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_6);
     }
     __Pyx_XDECREF_SET(__pyx_v_h, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":41
+    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":46
  *         all_symbols.update(set(list(r)))
  *     for h in hypothesis:
  *         all_symbols.update(set(list(h)))             # <<<<<<<<<<<<<<
  *     int2sym = dict(enumerate(sorted(all_symbols)))
  *     sym2int = {v: k for k, v in int2sym.items()}
  */
-    __pyx_t_6 = PySequence_List(__pyx_v_h); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __pyx_t_6 = PySequence_List(__pyx_v_h); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = PySet_New(__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __pyx_t_4 = PySet_New(__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PySet_Type_update, __pyx_v_all_symbols, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PySet_Type_update, __pyx_v_all_symbols, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":40
+    /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":45
  *     for r in reference:
  *         all_symbols.update(set(list(r)))
  *     for h in hypothesis:             # <<<<<<<<<<<<<<
  *         all_symbols.update(set(list(h)))
  *     int2sym = dict(enumerate(sorted(all_symbols)))
  */
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":42
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":47
  *     for h in hypothesis:
  *         all_symbols.update(set(list(h)))
  *     int2sym = dict(enumerate(sorted(all_symbols)))             # <<<<<<<<<<<<<<
  *     sym2int = {v: k for k, v in int2sym.items()}
  * 
  */
-  __pyx_t_6 = PySequence_List(__pyx_v_all_symbols); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_6 = PySequence_List(__pyx_v_all_symbols); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_5 = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_8 = PyList_Sort(__pyx_t_5); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 42, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_enumerate, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_8 = PyList_Sort(__pyx_t_5); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_enumerate, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_int2sym = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":43
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":48
  *         all_symbols.update(set(list(h)))
  *     int2sym = dict(enumerate(sorted(all_symbols)))
  *     sym2int = {v: k for k, v in int2sym.items()}             # <<<<<<<<<<<<<<
  * 
  *     reference = [[sym2int[h_] for h_ in h] for h in reference]
  */
   { /* enter inner scope */
-    __pyx_t_5 = PyDict_New(); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 43, __pyx_L15_error)
+    __pyx_t_5 = PyDict_New(); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L15_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_1 = 0;
-    __pyx_t_4 = __Pyx_dict_iterator(__pyx_v_int2sym, 1, __pyx_n_s_items, (&__pyx_t_2), (&__pyx_t_9)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 43, __pyx_L15_error)
+    __pyx_t_4 = __Pyx_dict_iterator(__pyx_v_int2sym, 1, __pyx_n_s_items, (&__pyx_t_2), (&__pyx_t_9)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 48, __pyx_L15_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6);
     __pyx_t_6 = __pyx_t_4;
     __pyx_t_4 = 0;
     while (1) {
       __pyx_t_11 = __Pyx_dict_iter_next(__pyx_t_6, __pyx_t_2, &__pyx_t_1, &__pyx_t_4, &__pyx_t_10, NULL, __pyx_t_9);
       if (unlikely(__pyx_t_11 == 0)) break;
-      if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 43, __pyx_L15_error)
+      if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 48, __pyx_L15_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_k, __pyx_t_4);
       __pyx_t_4 = 0;
       __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_v, __pyx_t_10);
       __pyx_t_10 = 0;
-      if (unlikely(PyDict_SetItem(__pyx_t_5, (PyObject*)__pyx_8genexpr2__pyx_v_v, (PyObject*)__pyx_8genexpr2__pyx_v_k))) __PYX_ERR(0, 43, __pyx_L15_error)
+      if (unlikely(PyDict_SetItem(__pyx_t_5, (PyObject*)__pyx_8genexpr2__pyx_v_v, (PyObject*)__pyx_8genexpr2__pyx_v_k))) __PYX_ERR(0, 48, __pyx_L15_error)
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_k); __pyx_8genexpr2__pyx_v_k = 0;
     __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_v); __pyx_8genexpr2__pyx_v_v = 0;
     goto __pyx_L18_exit_scope;
     __pyx_L15_error:;
     __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_k); __pyx_8genexpr2__pyx_v_k = 0;
     __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_v); __pyx_8genexpr2__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L18_exit_scope:;
   } /* exit inner scope */
   __pyx_v_sym2int = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":45
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":50
  *     sym2int = {v: k for k, v in int2sym.items()}
  * 
  *     reference = [[sym2int[h_] for h_ in h] for h in reference]             # <<<<<<<<<<<<<<
  *     hypothesis = [[sym2int[h_] for h_ in h] for h in hypothesis]
  * 
  */
   { /* enter inner scope */
-    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 45, __pyx_L21_error)
+    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L21_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (likely(PyList_CheckExact(__pyx_v_reference)) || PyTuple_CheckExact(__pyx_v_reference)) {
       __pyx_t_6 = __pyx_v_reference; __Pyx_INCREF(__pyx_t_6);
       __pyx_t_2 = 0;
       __pyx_t_7 = NULL;
     } else {
-      __pyx_t_2 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_reference); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 45, __pyx_L21_error)
+      __pyx_t_2 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_reference); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 50, __pyx_L21_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 45, __pyx_L21_error)
+      __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 50, __pyx_L21_error)
     }
     for (;;) {
       if (likely(!__pyx_t_7)) {
         if (likely(PyList_CheckExact(__pyx_t_6))) {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_6);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 45, __pyx_L21_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 50, __pyx_L21_error)
             #endif
             if (__pyx_t_2 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_10 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_2); __Pyx_INCREF(__pyx_t_10); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 45, __pyx_L21_error)
+          __pyx_t_10 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_2); __Pyx_INCREF(__pyx_t_10); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 50, __pyx_L21_error)
           #else
-          __pyx_t_10 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 45, __pyx_L21_error)
+          __pyx_t_10 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 50, __pyx_L21_error)
           __Pyx_GOTREF(__pyx_t_10);
           #endif
         } else {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_6);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 45, __pyx_L21_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 50, __pyx_L21_error)
             #endif
             if (__pyx_t_2 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_10 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_2); __Pyx_INCREF(__pyx_t_10); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 45, __pyx_L21_error)
+          __pyx_t_10 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_2); __Pyx_INCREF(__pyx_t_10); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 50, __pyx_L21_error)
           #else
-          __pyx_t_10 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 45, __pyx_L21_error)
+          __pyx_t_10 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 50, __pyx_L21_error)
           __Pyx_GOTREF(__pyx_t_10);
           #endif
         }
       } else {
         __pyx_t_10 = __pyx_t_7(__pyx_t_6);
         if (unlikely(!__pyx_t_10)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 45, __pyx_L21_error)
+            else __PYX_ERR(0, 50, __pyx_L21_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_10);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_h, __pyx_t_10);
       __pyx_t_10 = 0;
       { /* enter inner scope */
-        __pyx_t_10 = PyList_New(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 45, __pyx_L26_error)
+        __pyx_t_10 = PyList_New(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 50, __pyx_L26_error)
         __Pyx_GOTREF(__pyx_t_10);
         if (likely(PyList_CheckExact(__pyx_8genexpr3__pyx_v_h)) || PyTuple_CheckExact(__pyx_8genexpr3__pyx_v_h)) {
           __pyx_t_4 = __pyx_8genexpr3__pyx_v_h; __Pyx_INCREF(__pyx_t_4);
           __pyx_t_1 = 0;
           __pyx_t_12 = NULL;
         } else {
-          __pyx_t_1 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_8genexpr3__pyx_v_h); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 45, __pyx_L26_error)
+          __pyx_t_1 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_8genexpr3__pyx_v_h); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 50, __pyx_L26_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 45, __pyx_L26_error)
+          __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 50, __pyx_L26_error)
         }
         for (;;) {
           if (likely(!__pyx_t_12)) {
             if (likely(PyList_CheckExact(__pyx_t_4))) {
               {
                 Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_4);
                 #if !CYTHON_ASSUME_SAFE_MACROS
-                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 45, __pyx_L26_error)
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 50, __pyx_L26_error)
                 #endif
                 if (__pyx_t_1 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_13 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_13); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 45, __pyx_L26_error)
+              __pyx_t_13 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_13); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 50, __pyx_L26_error)
               #else
-              __pyx_t_13 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 45, __pyx_L26_error)
+              __pyx_t_13 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 50, __pyx_L26_error)
               __Pyx_GOTREF(__pyx_t_13);
               #endif
             } else {
               {
                 Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_4);
                 #if !CYTHON_ASSUME_SAFE_MACROS
-                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 45, __pyx_L26_error)
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 50, __pyx_L26_error)
                 #endif
                 if (__pyx_t_1 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_13 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_13); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 45, __pyx_L26_error)
+              __pyx_t_13 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_13); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 50, __pyx_L26_error)
               #else
-              __pyx_t_13 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 45, __pyx_L26_error)
+              __pyx_t_13 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 50, __pyx_L26_error)
               __Pyx_GOTREF(__pyx_t_13);
               #endif
             }
           } else {
             __pyx_t_13 = __pyx_t_12(__pyx_t_4);
             if (unlikely(!__pyx_t_13)) {
               PyObject* exc_type = PyErr_Occurred();
               if (exc_type) {
                 if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                else __PYX_ERR(0, 45, __pyx_L26_error)
+                else __PYX_ERR(0, 50, __pyx_L26_error)
               }
               break;
             }
             __Pyx_GOTREF(__pyx_t_13);
           }
           __Pyx_XDECREF_SET(__pyx_8genexpr4__pyx_v_h_, __pyx_t_13);
           __pyx_t_13 = 0;
-          __pyx_t_13 = __Pyx_PyDict_GetItem(__pyx_v_sym2int, __pyx_8genexpr4__pyx_v_h_); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 45, __pyx_L26_error)
+          __pyx_t_13 = __Pyx_PyDict_GetItem(__pyx_v_sym2int, __pyx_8genexpr4__pyx_v_h_); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 50, __pyx_L26_error)
           __Pyx_GOTREF(__pyx_t_13);
-          if (unlikely(__Pyx_ListComp_Append(__pyx_t_10, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 45, __pyx_L26_error)
+          if (unlikely(__Pyx_ListComp_Append(__pyx_t_10, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 50, __pyx_L26_error)
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_h_); __pyx_8genexpr4__pyx_v_h_ = 0;
         goto __pyx_L30_exit_scope;
         __pyx_L26_error:;
         __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_h_); __pyx_8genexpr4__pyx_v_h_ = 0;
         goto __pyx_L21_error;
         __pyx_L30_exit_scope:;
       } /* exit inner scope */
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_10))) __PYX_ERR(0, 45, __pyx_L21_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_10))) __PYX_ERR(0, 50, __pyx_L21_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_h); __pyx_8genexpr3__pyx_v_h = 0;
     goto __pyx_L32_exit_scope;
     __pyx_L21_error:;
     __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_h); __pyx_8genexpr3__pyx_v_h = 0;
     goto __pyx_L1_error;
     __pyx_L32_exit_scope:;
   } /* exit inner scope */
   __Pyx_DECREF_SET(__pyx_v_reference, __pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":46
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":51
  * 
  *     reference = [[sym2int[h_] for h_ in h] for h in reference]
  *     hypothesis = [[sym2int[h_] for h_ in h] for h in hypothesis]             # <<<<<<<<<<<<<<
  * 
  *     return time_constrained_orc_levenshtein_distance_(
  */
   { /* enter inner scope */
-    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 46, __pyx_L35_error)
+    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L35_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (likely(PyList_CheckExact(__pyx_v_hypothesis)) || PyTuple_CheckExact(__pyx_v_hypothesis)) {
       __pyx_t_6 = __pyx_v_hypothesis; __Pyx_INCREF(__pyx_t_6);
       __pyx_t_2 = 0;
       __pyx_t_7 = NULL;
     } else {
-      __pyx_t_2 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_hypothesis); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 46, __pyx_L35_error)
+      __pyx_t_2 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_hypothesis); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 51, __pyx_L35_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 46, __pyx_L35_error)
+      __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 51, __pyx_L35_error)
     }
     for (;;) {
       if (likely(!__pyx_t_7)) {
         if (likely(PyList_CheckExact(__pyx_t_6))) {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_6);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 46, __pyx_L35_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 51, __pyx_L35_error)
             #endif
             if (__pyx_t_2 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_10 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_2); __Pyx_INCREF(__pyx_t_10); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 46, __pyx_L35_error)
+          __pyx_t_10 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_2); __Pyx_INCREF(__pyx_t_10); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 51, __pyx_L35_error)
           #else
-          __pyx_t_10 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 46, __pyx_L35_error)
+          __pyx_t_10 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 51, __pyx_L35_error)
           __Pyx_GOTREF(__pyx_t_10);
           #endif
         } else {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_6);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 46, __pyx_L35_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 51, __pyx_L35_error)
             #endif
             if (__pyx_t_2 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_10 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_2); __Pyx_INCREF(__pyx_t_10); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 46, __pyx_L35_error)
+          __pyx_t_10 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_2); __Pyx_INCREF(__pyx_t_10); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 51, __pyx_L35_error)
           #else
-          __pyx_t_10 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 46, __pyx_L35_error)
+          __pyx_t_10 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 51, __pyx_L35_error)
           __Pyx_GOTREF(__pyx_t_10);
           #endif
         }
       } else {
         __pyx_t_10 = __pyx_t_7(__pyx_t_6);
         if (unlikely(!__pyx_t_10)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 46, __pyx_L35_error)
+            else __PYX_ERR(0, 51, __pyx_L35_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_10);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr5__pyx_v_h, __pyx_t_10);
       __pyx_t_10 = 0;
       { /* enter inner scope */
-        __pyx_t_10 = PyList_New(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 46, __pyx_L40_error)
+        __pyx_t_10 = PyList_New(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 51, __pyx_L40_error)
         __Pyx_GOTREF(__pyx_t_10);
         if (likely(PyList_CheckExact(__pyx_8genexpr5__pyx_v_h)) || PyTuple_CheckExact(__pyx_8genexpr5__pyx_v_h)) {
           __pyx_t_4 = __pyx_8genexpr5__pyx_v_h; __Pyx_INCREF(__pyx_t_4);
           __pyx_t_1 = 0;
           __pyx_t_12 = NULL;
         } else {
-          __pyx_t_1 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_8genexpr5__pyx_v_h); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 46, __pyx_L40_error)
+          __pyx_t_1 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_8genexpr5__pyx_v_h); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L40_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 46, __pyx_L40_error)
+          __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 51, __pyx_L40_error)
         }
         for (;;) {
           if (likely(!__pyx_t_12)) {
             if (likely(PyList_CheckExact(__pyx_t_4))) {
               {
                 Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_4);
                 #if !CYTHON_ASSUME_SAFE_MACROS
-                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 46, __pyx_L40_error)
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 51, __pyx_L40_error)
                 #endif
                 if (__pyx_t_1 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_13 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_13); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 46, __pyx_L40_error)
+              __pyx_t_13 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_13); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 51, __pyx_L40_error)
               #else
-              __pyx_t_13 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 46, __pyx_L40_error)
+              __pyx_t_13 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 51, __pyx_L40_error)
               __Pyx_GOTREF(__pyx_t_13);
               #endif
             } else {
               {
                 Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_4);
                 #if !CYTHON_ASSUME_SAFE_MACROS
-                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 46, __pyx_L40_error)
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 51, __pyx_L40_error)
                 #endif
                 if (__pyx_t_1 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_13 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_13); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 46, __pyx_L40_error)
+              __pyx_t_13 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_13); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 51, __pyx_L40_error)
               #else
-              __pyx_t_13 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 46, __pyx_L40_error)
+              __pyx_t_13 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 51, __pyx_L40_error)
               __Pyx_GOTREF(__pyx_t_13);
               #endif
             }
           } else {
             __pyx_t_13 = __pyx_t_12(__pyx_t_4);
             if (unlikely(!__pyx_t_13)) {
               PyObject* exc_type = PyErr_Occurred();
               if (exc_type) {
                 if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                else __PYX_ERR(0, 46, __pyx_L40_error)
+                else __PYX_ERR(0, 51, __pyx_L40_error)
               }
               break;
             }
             __Pyx_GOTREF(__pyx_t_13);
           }
           __Pyx_XDECREF_SET(__pyx_8genexpr6__pyx_v_h_, __pyx_t_13);
           __pyx_t_13 = 0;
-          __pyx_t_13 = __Pyx_PyDict_GetItem(__pyx_v_sym2int, __pyx_8genexpr6__pyx_v_h_); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 46, __pyx_L40_error)
+          __pyx_t_13 = __Pyx_PyDict_GetItem(__pyx_v_sym2int, __pyx_8genexpr6__pyx_v_h_); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 51, __pyx_L40_error)
           __Pyx_GOTREF(__pyx_t_13);
-          if (unlikely(__Pyx_ListComp_Append(__pyx_t_10, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 46, __pyx_L40_error)
+          if (unlikely(__Pyx_ListComp_Append(__pyx_t_10, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 51, __pyx_L40_error)
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_h_); __pyx_8genexpr6__pyx_v_h_ = 0;
         goto __pyx_L44_exit_scope;
         __pyx_L40_error:;
         __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_h_); __pyx_8genexpr6__pyx_v_h_ = 0;
         goto __pyx_L35_error;
         __pyx_L44_exit_scope:;
       } /* exit inner scope */
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_10))) __PYX_ERR(0, 46, __pyx_L35_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_10))) __PYX_ERR(0, 51, __pyx_L35_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_h); __pyx_8genexpr5__pyx_v_h = 0;
     goto __pyx_L46_exit_scope;
     __pyx_L35_error:;
     __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_h); __pyx_8genexpr5__pyx_v_h = 0;
     goto __pyx_L1_error;
     __pyx_L46_exit_scope:;
   } /* exit inner scope */
   __Pyx_DECREF_SET(__pyx_v_hypothesis, __pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":48
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":53
  *     hypothesis = [[sym2int[h_] for h_ in h] for h in hypothesis]
  * 
  *     return time_constrained_orc_levenshtein_distance_(             # <<<<<<<<<<<<<<
  *         reference,
  *         hypothesis,
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":49
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":54
  * 
  *     return time_constrained_orc_levenshtein_distance_(
  *         reference,             # <<<<<<<<<<<<<<
  *         hypothesis,
  *         reference_timings,
  */
-  __pyx_t_14 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_unsigned_int_3e___(__pyx_v_reference); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_14 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_unsigned_int_3e___(__pyx_v_reference); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L1_error)
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":50
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":55
  *     return time_constrained_orc_levenshtein_distance_(
  *         reference,
  *         hypothesis,             # <<<<<<<<<<<<<<
  *         reference_timings,
  *         hypothesis_timings
  */
-  __pyx_t_15 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_unsigned_int_3e___(__pyx_v_hypothesis); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_15 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_unsigned_int_3e___(__pyx_v_hypothesis); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 55, __pyx_L1_error)
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":51
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":56
  *         reference,
  *         hypothesis,
  *         reference_timings,             # <<<<<<<<<<<<<<
  *         hypothesis_timings
  *     )
  */
-  __pyx_t_16 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_double_2c_double_3e____3e___(__pyx_v_reference_timings); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_16 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_double_2c_double_3e____3e___(__pyx_v_reference_timings); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 56, __pyx_L1_error)
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":52
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":57
  *         hypothesis,
  *         reference_timings,
  *         hypothesis_timings             # <<<<<<<<<<<<<<
  *     )
  */
-  __pyx_t_17 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_double_2c_double_3e____3e___(__pyx_v_hypothesis_timings); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_17 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_double_2c_double_3e____3e___(__pyx_v_hypothesis_timings); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L1_error)
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":48
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":53
  *     hypothesis = [[sym2int[h_] for h_ in h] for h in hypothesis]
  * 
  *     return time_constrained_orc_levenshtein_distance_(             # <<<<<<<<<<<<<<
  *         reference,
  *         hypothesis,
  */
   try {
     __pyx_t_18 = time_constrained_orc_levenshtein_distance_(__PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_14), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_15), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_16), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_17));
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 48, __pyx_L1_error)
+    __PYX_ERR(0, 53, __pyx_L1_error)
   }
-  __pyx_t_5 = __pyx_convert_pair_to_py_unsigned_int____std_3a__3a_vector_3c_unsigned_int_3e___(__pyx_t_18); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_5 = __pyx_convert_pair_to_py_unsigned_int____std_3a__3a_vector_3c_unsigned_int_3e___(__pyx_t_18); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
   /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":18
  *     ) except +
@@ -5015,24 +5046,26 @@
   __Pyx_XDECREF(__pyx_v_reference);
   __Pyx_XDECREF(__pyx_v_hypothesis);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr *__pyx_freelist_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr[8];
 static int __pyx_freecount_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr)))) {
     o = (PyObject*)__pyx_freelist_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr[--__pyx_freecount_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -5053,15 +5086,15 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_h);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr)))) {
     __pyx_freelist_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr[__pyx_freecount_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr++] = ((struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -5182,24 +5215,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr *__pyx_freelist_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr[8];
 static int __pyx_freecount_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr)))) {
     o = (PyObject*)__pyx_freelist_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr[--__pyx_freecount_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -5220,15 +5255,15 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_r);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr)))) {
     __pyx_freelist_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr[__pyx_freecount_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr++] = ((struct __pyx_obj_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -5412,48 +5447,48 @@
     {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 26, __pyx_L1_error)
-  __pyx_builtin_sum = __Pyx_GetBuiltinName(__pyx_n_s_sum); if (!__pyx_builtin_sum) __PYX_ERR(0, 32, __pyx_L1_error)
-  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_builtin_sum = __Pyx_GetBuiltinName(__pyx_n_s_sum); if (!__pyx_builtin_sum) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 47, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 68, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 76, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":26
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":30
  *     # Validate inputs
  *     if len(reference) != len(reference_timings):
  *         raise ValueError("reference and reference_timings must have the same length")             # <<<<<<<<<<<<<<
  *     if len(hypothesis) != len(hypothesis_timings):
  *         raise ValueError("hypothesis and hypothesis_timings must have the same length")
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_reference_and_reference_timings); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_reference_and_reference_timings); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":28
+  /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":32
  *         raise ValueError("reference and reference_timings must have the same length")
  *     if len(hypothesis) != len(hypothesis_timings):
  *         raise ValueError("hypothesis and hypothesis_timings must have the same length")             # <<<<<<<<<<<<<<
  * 
  *     # Shortcuts for trivial cases
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_hypothesis_and_hypothesis_timing); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_hypothesis_and_hypothesis_timing); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "meeteval/wer/matching/cy_time_constrained_orc_matching.pyx":18
  *     ) except +
  * 
  * def time_constrained_orc_levenshtein_distance(             # <<<<<<<<<<<<<<
@@ -5472,14 +5507,15 @@
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   __pyx_umethod_PySet_Type_update.type = (PyObject*)&PySet_Type;
   __pyx_umethod_PySet_Type_update.method_name = &__pyx_n_s_update;
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_globals ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
@@ -5523,42 +5559,42 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr_spec, NULL); if (unlikely(!__pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr)) __PYX_ERR(0, 32, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr_spec, __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr_spec, NULL); if (unlikely(!__pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr)) __PYX_ERR(0, 36, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr_spec, __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
   #else
   __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr = &__pyx_type_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr->tp_dictoffset && __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct__genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr)) __PYX_ERR(0, 34, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr_spec, __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr)) __PYX_ERR(0, 39, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr_spec, __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
   #else
   __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr = &__pyx_type_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr->tp_dictoffset && __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_8meeteval_3wer_8matching_32cy_time_constrained_orc_matching___pyx_scope_struct_1_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -8838,15 +8874,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `meeteval-0.2.1/meeteval/wer/matching/cy_time_constrained_orc_matching.pyx` & `meeteval-0.3.0/meeteval/wer/matching/cy_time_constrained_orc_matching.pyx`

 * *Files 11% similar despite different names*

```diff
@@ -17,25 +17,30 @@
 
 def time_constrained_orc_levenshtein_distance(
         reference,  # List (utterances) of list of symbols
         hypothesis, # List (streams) of list of symbols
         reference_timings,
         hypothesis_timings
 ):
+    """
+    Compute the time-constrained ORC Levenshtein distance between two sequences of 
+    symbols and returns the distance and the alignment.
+    """
     # Validate inputs
     if len(reference) != len(reference_timings):
         raise ValueError("reference and reference_timings must have the same length")
     if len(hypothesis) != len(hypothesis_timings):
         raise ValueError("hypothesis and hypothesis_timings must have the same length")
 
     # Shortcuts for trivial cases
     if len(reference) == 0:
         return sum(len(h) for h in hypothesis), []
     if len(hypothesis) == 0:
-        return sum(len(r) for r in reference), []
+        # 0 is a dummy stream index
+        return sum(len(r) for r in reference), [0] * len(reference)
 
     # Translate symbols/words to integers for the cpp code
     all_symbols = set()
     for r in reference:
         all_symbols.update(set(list(r)))
     for h in hypothesis:
         all_symbols.update(set(list(h)))
```

### Comparing `meeteval-0.2.1/meeteval/wer/matching/levenshtein.h` & `meeteval-0.3.0/meeteval/wer/matching/levenshtein.h`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/wer/matching/mimo_matching.h` & `meeteval-0.3.0/meeteval/wer/matching/mimo_matching.h`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/wer/matching/mimo_matching.py` & `meeteval-0.3.0/meeteval/wer/matching/mimo_matching.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/wer/matching/orc_matching.py` & `meeteval-0.3.0/meeteval/wer/matching/orc_matching.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/wer/matching/time_constrained_orc_matching.h` & `meeteval-0.3.0/meeteval/wer/matching/time_constrained_orc_matching.h`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/wer/utils.py` & `meeteval-0.3.0/meeteval/wer/utils.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/wer/wer/__init__.py` & `meeteval-0.3.0/meeteval/wer/wer/__init__.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/wer/wer/cp.py` & `meeteval-0.3.0/meeteval/wer/wer/cp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dataclasses
 import itertools
 import string
 from typing import Optional, Any, Iterable
 
+import meeteval
 from meeteval._typing import Literal
-from meeteval.io.seglst import SegLST, asseglst
+from meeteval.io.seglst import SegLST, asseglst, asseglistconvertible
 
 from meeteval.wer.wer.error_rate import ErrorRate
 
 __all__ = [
     'CPErrorRate',
     'cp_word_error_rate',
     'apply_cp_assignment',
@@ -170,23 +171,23 @@
                 for w in (s['words'].split() if s['words'].strip() else [''])
             ])
 
     return cp_error_rate(split_words(reference), split_words(hypothesis))
 
 
 def cp_word_error_rate_multifile(
-        reference, hypothesis
+        reference, hypothesis, partial=False
 ) -> 'dict[str, CPErrorRate]':
     """
     Computes the cpWER for each example in the reference and hypothesis STM files.
 
     To compute the overall WER, use `sum(cp_word_error_rate_multifile(r, h).values())`.
     """
     from meeteval.io.seglst import apply_multi_file
-    return apply_multi_file(cp_word_error_rate, reference, hypothesis)
+    return apply_multi_file(cp_word_error_rate, reference, hypothesis, partial=partial)
 
 
 def _cp_error_rate(
         reference: SegLST,
         hypothesis: SegLST,
         distance_fn: callable,
         siso_error_rate: callable,
@@ -275,23 +276,22 @@
         reference_self_overlap=None,
         hypothesis_self_overlap=None,
     )
 
 
 def apply_cp_assignment(
         assignment: 'list[tuple[Any, ...]] | tuple[tuple[Any, ...], ...]',
-        reference: dict,
-        hypothesis: dict,
+        reference: 'dict | list | tuple | SegLST',
+        hypothesis: 'dict | list | tuple | SegLST',
         style: 'Literal["hyp", "ref"]' = 'ref',
         fallback_keys=string.ascii_letters,
         missing='',
 ):
     """
-    Apply the assignment, so that reference and hypothesis have the same
-    keys.
+    Apply the assignment so that reference and hypothesis have the same keys.
 
     The code is roughly:
         if style == 'ref':
             hypothesis = {
                 r_key: hypothesis[h_key]
                 for r_key, h_key in assignment
             }
@@ -349,17 +349,94 @@
     (['0ref'], ['0hyp'])
     >>> test_list([(0, 0), (1, None)])
     (['0ref', '1ref'], ['0hyp', ''])
     (['0ref', '1ref'], ['0hyp', ''])
     >>> test_list([(0, 0), (None, 1)])
     (['0ref', ''], ['0hyp', '1hyp'])
     (['0ref', ''], ['0hyp', '1hyp'])
+
+    Also works for anything convertible to SegLST
+    >>> r, h = apply_cp_assignment(
+    ...     [('rA', 'hB'), ('rB', 'hA')],
+    ...     meeteval.io.STM.parse(
+    ...         'file1 0 rA 0 1 Hello World\\n'
+    ...         'file1 0 rB 0 1 Goodbye'
+    ...     ),
+    ...     meeteval.io.STM.parse(
+    ...         'file1 0 hB 0 1 Hello World\\n'
+    ...         'file1 0 hA 0 1 Goodbye'
+    ...     ),
+    ...     style='ref'
+    ... )
+    >>> print(r.dumps())
+    file1 0 rA 0 1 Hello World
+    file1 0 rB 0 1 Goodbye
+    <BLANKLINE>
+    >>> print(h.dumps())
+    file1 0 rA 0 1 Hello World
+    file1 0 rB 0 1 Goodbye
+    <BLANKLINE>
     """
     assert assignment, assignment
 
+    try:
+        r_conv = asseglistconvertible(reference, py_convert=None)
+        h_conv = asseglistconvertible(hypothesis, py_convert=None)
+    except Exception:
+        # This is a Python structure
+        pass
+    else:
+        reference = r_conv.to_seglst()
+        hypothesis = h_conv.to_seglst()
+
+        # Check for valid keys
+        r_keys, h_keys = zip(*assignment)
+        r_keys = set(r_keys) - {None}
+        h_keys = set(h_keys) - {None}
+        assert r_keys == reference.unique('speaker'), (r_keys, reference.unique('speaker'), assignment)
+        assert h_keys == hypothesis.unique('speaker'), (h_keys, hypothesis.unique('speaker'), assignment)
+
+        fallback_keys_iter = iter([
+            k
+            for k in fallback_keys
+            if k not in r_keys
+            if k not in h_keys
+        ])
+
+        try:
+            if style == 'hyp':
+                assignment = {
+                    r: h if h is not None else next(fallback_keys_iter)
+                    for r, h in assignment
+                    if r is not None
+                }
+                # Change the keys of the reference to those of the hypothesis
+                reference = reference.map(lambda s: {
+                    **s, 'speaker': assignment[s['speaker']]
+                })
+            elif style == 'ref':
+                assignment = {
+                    h: r if r is not None else next(fallback_keys_iter)
+                    for r, h in assignment
+                    if h is not None
+                }
+                hypothesis = hypothesis.map(lambda s: {
+                    **s, 'speaker': assignment[s['speaker']]
+                })
+            else:
+                raise ValueError(f'{style!r} not in ["ref", "hyp"]')
+        except StopIteration:
+            raise RuntimeError(
+                f'Too few fallback keys provided! '
+                f'There are more over-/under-estimated speakers '
+                f'than fallback_keys in {fallback_keys}'
+            )
+
+        return r_conv.new(reference), h_conv.new(hypothesis)
+
     if isinstance(reference, dict) and isinstance(hypothesis, dict):
         # Check for valid keys
         assert None not in reference, reference.keys()
         assert None not in hypothesis, hypothesis.keys()
 
         r_keys, h_keys = zip(*assignment)
         # CB: Why do we need to remove None?
```

### Comparing `meeteval-0.2.1/meeteval/wer/wer/error_rate.py` & `meeteval-0.3.0/meeteval/wer/wer/error_rate.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/meeteval/wer/wer/mimo.py` & `meeteval-0.3.0/meeteval/wer/wer/mimo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import dataclasses
 from typing import Iterable, Any
 
-from meeteval.io.seglst import asseglst
+from meeteval.io.seglst import asseglst, asseglistconvertible
 from meeteval.wer.wer.error_rate import ErrorRate
 from meeteval.wer.wer.siso import _siso_error_rate
 from meeteval.wer.utils import _keys, _items, _values
 
 __all__ = [
     'MimoErrorRate', 'mimo_word_error_rate', 'apply_mimo_assignment',
     'mimo_word_error_rate_multifile'
@@ -121,25 +121,26 @@
 
     # Call core function
     return mimo_error_rate(reference, hypothesis)
 
 
 def mimo_word_error_rate_multifile(
         reference,
-        hypothesis
+        hypothesis,
+        partial=False,
 ) -> 'dict[str, MimoErrorRate]':
     """
     Computes the MIMO WER for each example in the reference and hypothesis
     files.
 
     To compute the overall WER, use
     `sum(mimo_word_error_rate_multifile(r, h).values())`.
     """
     from meeteval.io.seglst import apply_multi_file
-    return apply_multi_file(mimo_word_error_rate, reference, hypothesis)
+    return apply_multi_file(mimo_word_error_rate, reference, hypothesis, partial=partial)
 
 
 def apply_mimo_assignment(
         assignment: 'list[tuple]',
         reference: 'list[list[Any]] | dict[list[Any]]',
         hypothesis: 'list[Any] | dict[Any, Any]',
 ):
@@ -157,15 +158,46 @@
     ([['c d'], ['a b', 'e f']], ['c d', 'a b e f'])
 
     >>> assignment = [('A', 'O1'), ('A', 'O1')]
     >>> reference = {'A': ['a b', 'c d']}
     >>> hypothesis = {'O1': 'c d', 'O2': 'a b e f'}
     >>> apply_mimo_assignment(assignment, reference, hypothesis)
     ({'O1': ['a b', 'c d'], 'O2': []}, {'O1': 'c d', 'O2': 'a b e f'})
-    """
+
+    >>> reference = STM.parse('X 1 A 0.0 1.0 a b\\nX 1 A 1.0 2.0 c d\\n')
+    >>> hypothesis = STM.parse('X 1 O1 0.0 2.0 c d\\nX 1 O0 0.0 2.0 a b e f\\n')
+    >>> reference, hypothesis = apply_mimo_assignment(assignment, reference, hypothesis)
+    >>> print(reference.dumps())
+    X 1 O1 0.0 1.0 a b
+    X 1 O1 1.0 2.0 c d
+    <BLANKLINE>
+    >>> print(hypothesis.dumps())
+    X 1 O1 0.0 2.0 c d
+    X 1 O0 0.0 2.0 a b e f
+    <BLANKLINE>
+    """
+
+    try:
+        r_conv = asseglistconvertible(reference, py_convert=None)
+    except Exception:
+        pass
+    else:
+        reference = r_conv.to_seglst().sorted('start_time')
+        reference = {
+            k: list(v)
+            for k, v in reference.groupby('speaker').items()
+        }
+
+        reference_new = [
+            {**reference[r].pop(0), 'speaker': h}
+            for r, h in assignment
+        ]
+
+        return r_conv.new(reference_new), hypothesis
+
     reference_new = {k: [] for k in _keys(hypothesis)}
     # convert to list and copy
     reference = {k: list(v) for k, v in _items(reference)}
 
     for r, h in assignment:
         reference_new[h].append(reference[r].pop(0))
```

### Comparing `meeteval-0.2.1/meeteval/wer/wer/siso.py` & `meeteval-0.3.0/meeteval/wer/wer/siso.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing
 from typing import Hashable
 
 from meeteval.io.py import NestedStructure
 from meeteval.wer.wer.error_rate import ErrorRate
+from meeteval.wer.wer.utils import kaldialign_edit_distance
 from meeteval.io.seglst import asseglst
 
 if typing.TYPE_CHECKING:
     from meeteval.io.stm import STM
     from meeteval.io.seglst import SegLST
 
 __all__ = [
@@ -38,18 +39,16 @@
 
     return levenshtein_distance(reference, hypothesis)
 
 
 def _siso_error_rate(
         reference: 'list[Hashable]', hypothesis: 'list[Hashable]'
 ) -> ErrorRate:
-    import kaldialign
-
     try:
-        result = kaldialign.edit_distance(reference, hypothesis)
+        result = kaldialign_edit_distance(reference, hypothesis)
     except TypeError:
         raise TypeError(
             type(reference), type(hypothesis), type(reference[0]),
             type(hypothesis[0]), reference[0], hypothesis[0]
         )
 
     return ErrorRate(
```

### Comparing `meeteval-0.2.1/meeteval/wer/wer/time_constrained.py` & `meeteval-0.3.0/meeteval/wer/wer/time_constrained.py`

 * *Files 1% similar despite different names*

```diff
@@ -821,14 +821,15 @@
 def tcp_word_error_rate_multifile(
         reference, hypothesis,
         reference_pseudo_word_level_timing='character_based',
         hypothesis_pseudo_word_level_timing='character_based_points',
         collar: int = 0,
         reference_sort='segment',
         hypothesis_sort='segment',
+        partial=False,
 ) -> 'dict[str, CPErrorRate]':
     """
     Computes the tcpWER for each example in the reference and hypothesis files.
     See `time_constrained_minimum_permutation_word_error_rate` for details.
     
     To compute the overall WER, use
     `sum(tcp_word_error_rate_multifile(r, h).values())`.
@@ -837,15 +838,15 @@
     r = apply_multi_file(lambda r, h: time_constrained_minimum_permutation_word_error_rate(
         r, h,
         reference_pseudo_word_level_timing=reference_pseudo_word_level_timing,
         hypothesis_pseudo_word_level_timing=hypothesis_pseudo_word_level_timing,
         collar=collar,
         reference_sort=reference_sort,
         hypothesis_sort=hypothesis_sort,
-    ), reference, hypothesis)
+    ), reference, hypothesis, partial=partial)
     return r
 
 
 def index_alignment_to_kaldi_alignment(alignment, reference, hypothesis, eps='*'):
     return [
         (eps if a is None else reference[a], eps if b is None else hypothesis[b])
         for a, b in alignment
```

### Comparing `meeteval-0.2.1/meeteval/wer/wer/time_constrained_orc.py` & `meeteval-0.3.0/meeteval/wer/wer/time_constrained_orc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import meeteval
-from meeteval.wer import ErrorRate, combine_error_rates
-from meeteval.wer.wer.error_rate import SelfOverlap
-from meeteval.wer.wer.orc import OrcErrorRate
+from meeteval.wer import combine_error_rates
+from meeteval.wer.wer.orc import OrcErrorRate, apply_orc_assignment
 from meeteval.wer.wer.time_constrained import get_self_overlap
 from meeteval.wer.wer.utils import check_single_filename
 
 import typing
 
 if typing.TYPE_CHECKING:
     from meeteval.io import STM
@@ -31,30 +30,37 @@
 
     Special cases where the reference or hypothesis is empty
     >>> time_constrained_orc_wer([], [])
     OrcErrorRate(errors=0, length=0, insertions=0, deletions=0, substitutions=0, assignment=())
     >>> time_constrained_orc_wer([], [{'session_id': 'a', 'start_time': 0, 'end_time': 1, 'words': 'a', 'speaker': 'A'}])
     OrcErrorRate(errors=1, length=0, insertions=1, deletions=0, substitutions=0, hypothesis_self_overlap=SelfOverlap(overlap_rate=0.0, overlap_time=0, total_time=1), assignment=())
     >>> time_constrained_orc_wer([{'session_id': 'a', 'start_time': 0, 'end_time': 1, 'words': 'a', 'speaker': 'A'}], [])
-    OrcErrorRate(error_rate=1.0, errors=1, length=1, insertions=0, deletions=1, substitutions=0, reference_self_overlap=SelfOverlap(overlap_rate=0.0, overlap_time=0, total_time=1), assignment=())
+    OrcErrorRate(error_rate=1.0, errors=1, length=1, insertions=0, deletions=1, substitutions=0, reference_self_overlap=SelfOverlap(overlap_rate=0.0, overlap_time=0, total_time=1), assignment=('dummy',))
+    >>> time_constrained_orc_wer([{'session_id': 'a', 'start_time': 0, 'end_time': 1, 'words': '', 'speaker': 'A'}], [{'session_id': 'a', 'start_time': 0, 'end_time': 1, 'words': 'a', 'speaker': 'A'}])
+    OrcErrorRate(errors=1, length=0, insertions=1, deletions=0, substitutions=0, reference_self_overlap=SelfOverlap(overlap_rate=0.0, overlap_time=0, total_time=1), hypothesis_self_overlap=SelfOverlap(overlap_rate=0.0, overlap_time=0, total_time=1), assignment=('A',))
+    >>> time_constrained_orc_wer([{'session_id': 'a', 'start_time': 0, 'end_time': 1, 'words': 'a b', 'speaker': 'A'}], [{'session_id': 'a', 'start_time': 0, 'end_time': 1, 'words': 'a d', 'speaker': 'A'}])
+    OrcErrorRate(error_rate=0.5, errors=1, length=2, insertions=0, deletions=0, substitutions=1, reference_self_overlap=SelfOverlap(overlap_rate=0.0, overlap_time=0, total_time=1), hypothesis_self_overlap=SelfOverlap(overlap_rate=0.0, overlap_time=0, total_time=1), assignment=('A',))
+
     """
     if reference_sort == 'word':
         raise ValueError(
             'reference_sort="word" is not supported for time-constrained '
             'ORC-WER because the ORC-WER assumes that an utterance appears'
             'continuously in the reference.'
         )
 
     # Convert to seglst
-    reference = meeteval.io.asseglst(reference)
-    hypothesis = meeteval.io.asseglst(hypothesis)
+    original_reference = reference = meeteval.io.asseglst(reference)
+    original_hypothesis = hypothesis = meeteval.io.asseglst(hypothesis)
     check_single_filename(reference, hypothesis)
 
     # Add a segment index to the reference so that we can later find words that
-    # come from the same segment
+    # come from the same segment. Do this before removing empty segments so that
+    # we can still find the original segments in the reference after the
+    # assignment.
     for i, s in enumerate(reference):
         s['segment_index'] = i
 
     # Group by stream. For ORC-WER, only hypothesis must be grouped
     hypothesis = hypothesis.groupby('speaker')
 
     # Calculate self-overlap before modifying the segments
@@ -62,14 +68,15 @@
         [get_self_overlap(h) for h in reference.groupby('speaker').values()]
     ) if len(reference) > 0 else None
     hypothesis_self_overlap = sum(
         [get_self_overlap(h) for h in hypothesis.values()]
     ) if len(hypothesis) > 0 else None
 
     # Remove empty segments
+    reference_missing_segments = reference.filter(lambda s: s['words'] == '')
     reference = reference.filter(lambda s: s['words'] != '')
     hypothesis = {
         k: h.filter(lambda s: s['words'] != '')
         for k, h in hypothesis.items()
     }
 
     # Time-constrained preprocessing
@@ -102,35 +109,54 @@
         [stream.T['words'] for stream in hypothesis.values()],
         [list(zip(segment.T['start_time'], segment.T['end_time'])) for segment in
          reference.groupby('segment_index').values()],
         [list(zip(stream.T['start_time'], stream.T['end_time'])) for stream in hypothesis.values()],
     )
 
     # Translate the assignment from hypothesis index to stream id
-    hypothesis_keys = list(hypothesis.keys())
+    hypothesis_keys = list(hypothesis.keys()) or ['dummy']
     assignment = [hypothesis_keys[h] for h in assignment]
 
-    # Apply assignment in seglst format
-    r_ = list(reference.groupby('segment_index').values())  # Shallow copy because we pop later
-    if assignment:
-        reference_new = []
-        for h in assignment:
-            for w in r_.pop(0):
-                reference_new.append({**w, 'speaker': h})
-        reference_new = meeteval.io.SegLST(reference_new).groupby('speaker')
-    else:
-        reference_new = reference.groupby('speaker')
+    # Apply assignment
+    reference_new, _ = apply_orc_assignment(assignment, reference, hypothesis)
+
+    # Put the original segments back by inserting empty segments that were
+    # removed in the beginning. Sort by segment_index to get the assignment in
+    # the same order as the input to this function.
+    # TODO: Estimate the stream for the missing segments
+    reference_missing_segments = reference_missing_segments.map(
+        lambda s: {**s, 'speaker': hypothesis_keys[0]}
+    )
+    reference_new = meeteval.io.SegLST.merge(
+        reference_new, reference_missing_segments
+    ).sorted('segment_index')
+    assignment = tuple([
+        v[0]['speaker']
+        for v in reference_new.groupby('segment_index').values()
+    ])
+
+    # Apply the assignment to the original reference for the consistency check.
+    original_reference, _ = apply_orc_assignment(assignment, original_reference, original_hypothesis)
+
+    # Group by speaker
+    reference_new = original_reference.groupby('speaker')
+    original_hypothesis = original_hypothesis.groupby('speaker')
 
     # Consistency check: Compute WER with the siso algorithm after applying the
     # assignment and compare the result with the distance from the ORC algorithm
-    from meeteval.wer.wer.time_constrained import _time_constrained_siso_error_rate
+    from meeteval.wer.wer.time_constrained import time_constrained_siso_word_error_rate
     er = combine_error_rates(*[
-        _time_constrained_siso_error_rate(
+        time_constrained_siso_word_error_rate(
             reference_new.get(k, meeteval.io.SegLST([])),
-            hypothesis.get(k, meeteval.io.SegLST([])),
+            original_hypothesis.get(k, meeteval.io.SegLST([])),
+            reference_pseudo_word_level_timing=reference_pseudo_word_level_timing,
+            hypothesis_pseudo_word_level_timing=hypothesis_pseudo_word_level_timing,
+            collar=collar,
+            reference_sort=reference_sort,
+            hypothesis_sort=hypothesis_sort,
         )
         for k in set(hypothesis.keys()) | set(reference_new.keys())
     ])
     length = len(reference)
     assert er.length == length, (length, er)
     assert er.errors == distance, (distance, er, assignment)
 
@@ -148,18 +174,19 @@
 def time_constrained_orc_wer_multifile(
         reference: 'STM', hypothesis: 'STM',
         reference_pseudo_word_level_timing='character_based',
         hypothesis_pseudo_word_level_timing='character_based_points',
         collar: int = 0,
         hypothesis_sort='segment',
         reference_sort='segment',
+        partial=False,
 ) -> 'dict[str, CPErrorRate]':
     from meeteval.io.seglst import apply_multi_file
     r = apply_multi_file(lambda r, h: time_constrained_orc_wer(
         r, h,
         reference_pseudo_word_level_timing=reference_pseudo_word_level_timing,
         hypothesis_pseudo_word_level_timing=hypothesis_pseudo_word_level_timing,
         collar=collar,
         hypothesis_sort=hypothesis_sort,
         reference_sort=reference_sort,
-    ), reference, hypothesis)
+    ), reference, hypothesis, partial=partial)
     return r
```

### Comparing `meeteval-0.2.1/meeteval.egg-info/PKG-INFO` & `meeteval-0.3.0/meeteval.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meeteval
-Version: 0.2.1
+Version: 0.3.0
 Home-page: https://github.com/fgnt/meeteval/
 Author: Department of Communications Engineering, Paderborn University
 Author-email: sek@nt.upb.de
 License: MIT
 Keywords: speech recognition,word error rate,evaluation,meeting,ASR,WER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -24,44 +24,53 @@
 Requires-Dist: Cython
 Provides-Extra: cli
 Requires-Dist: pyyaml; extra == "cli"
 Requires-Dist: fire; extra == "cli"
 Requires-Dist: simplejson; extra == "cli"
 Requires-Dist: aiohttp; extra == "cli"
 Requires-Dist: soundfile; extra == "cli"
+Requires-Dist: tqdm; extra == "cli"
+Requires-Dist: yattag; extra == "cli"
+Requires-Dist: platformdirs; extra == "cli"
 Provides-Extra: test
 Requires-Dist: editdistance; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
-Requires-Dist: click; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: ipython; extra == "test"
 Requires-Dist: pyyaml; extra == "test"
+Requires-Dist: fire; extra == "test"
 Requires-Dist: simplejson; extra == "test"
 Requires-Dist: aiohttp; extra == "test"
 Requires-Dist: soundfile; extra == "test"
+Requires-Dist: tqdm; extra == "test"
+Requires-Dist: yattag; extra == "test"
+Requires-Dist: platformdirs; extra == "test"
 Provides-Extra: all
+Requires-Dist: lazy_dataset; extra == "all"
+Requires-Dist: ipywidgets; extra == "all"
 Requires-Dist: pyyaml; extra == "all"
 Requires-Dist: fire; extra == "all"
 Requires-Dist: simplejson; extra == "all"
 Requires-Dist: aiohttp; extra == "all"
 Requires-Dist: soundfile; extra == "all"
+Requires-Dist: tqdm; extra == "all"
+Requires-Dist: yattag; extra == "all"
+Requires-Dist: platformdirs; extra == "all"
 Requires-Dist: editdistance; extra == "all"
 Requires-Dist: pytest; extra == "all"
 Requires-Dist: hypothesis; extra == "all"
-Requires-Dist: click; extra == "all"
 Requires-Dist: coverage; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
 Requires-Dist: ipython; extra == "all"
-Requires-Dist: lazy_dataset; extra == "all"
 
 <h1 align="center">MeetEval</h1> 
 <h3 align="center">A meeting transcription evaluation toolkit</h3>
-<div align="center"><a href="#features">Features</a> | <a href="#installation">Installation</a> | <a href="#python-interface">Python Interface</a> | <a href="#command-line-interface">Command Line Interface</a> | <a href="#visualization-wip">Visualization (WIP)</a> | <a href="#cite">Cite</a></div>
+<div align="center"><a href="#features">Features</a> | <a href="#installation">Installation</a> | <a href="#python-interface">Python Interface</a> | <a href="#command-line-interface">Command Line Interface</a> | <a href="#visualization">Visualization</a> | <a href="#cite">Cite</a></div>
 <br>
 <a href="https://github.com/fgnt/meeteval/actions"><img src="https://github.com/fgnt/meeteval/actions/workflows/pytest.yml/badge.svg"/></a>
 
 
 ## Features
 MeetEval supports the following metrics for meeting transcription evaluation:
 
@@ -76,15 +85,15 @@
 - **Time-Constrained minimum-Permutation Word Error Rate (tcpWER)**<br>
   `meeteval-wer tcpwer -r ref.stm -h hyp.stm --collar 5`
 - **Time-Constrained Optimal Reference Combination Word Error Rate (tcORC WER)**<br>
   `meeteval-wer tcorcwer -r ref.stm -h hyp.stm --collar 5`
 - **Diarization Error Rate (DER)** by wrapping [mdeval](https://github.com/nryant/dscore/raw/master/scorelib/md-eval-22.pl)<br>
   `meeteval-der md_eval_22 -r ref.stm -h hyp.stm --collar .25`
 
-Additionally (WIP), MeetEval contains a [visualization](#visualization-wip) tool for cpWER and tcpWER alignments that help spot errors in system outputs.
+Additionally, MeetEval contains a [visualization](#visualization) tool for cpWER and tcpWER alignments that helps to spot errors in system outputs.
 
 ## Installation
 
 ### From PyPI
 
 ```shell
 pip install meeteval
@@ -99,15 +108,15 @@
 
 ## Command-line interface
 
 `MeetEval` supports the following file formats as input:
  - [Segmental Time Mark](https://github.com/usnistgov/SCTK/blob/master/doc/infmts.htm#L75) (`STM`)
  - [Time Marked Conversation](https://github.com/usnistgov/SCTK/blob/master/doc/infmts.htm#L286) (`CTM`)
  - [SEGment-wise Long-form Speech Transcription annotation](#segment-wise-long-form-speech-transcription-annotation-seglst) (`SegLST`), the file format used in the [CHiME challenges](https://www.chimechallenge.org)
- - [Rich Transcription Time Marked](https://github.com/nryant/dscore?tab=readme-ov-file#rttm) (`RTTM`) files (only for Diarizaiton Error Rate)
+ - [Rich Transcription Time Marked](https://github.com/nryant/dscore?tab=readme-ov-file#rttm) (`RTTM`) files (only for Diarization Error Rate)
 
 
 > [!NOTE]
 > `MeetEval` does not support alternate transcripts (e.g., `"i've { um / uh / @ } as far as i'm concerned"`).
 
 The command-line interface is available as `meeteval-wer` or `python -m meeteval.wer` with the following signature:
 
@@ -325,20 +334,18 @@
 Sequences can be aligned, similar to `kaldialign.align`, using the tcpWER matching:
 ```python
 import meeteval
 meeteval.wer.wer.time_constrained.align([{'words': 'a b', 'start_time': 0, 'end_time': 1}], [{'words': 'a c', 'start_time': 0, 'end_time': 1}, {'words': 'd', 'start_time': 2, 'end_time': 3}])
 # [('a', 'a'), ('b', 'c'), ('*', 'd')]
 ```
 
-## Visualization [WIP]
+## Visualization
 
-> [!IMPORTANT]
-> The visualization is under development! <br>
-> Preview: https://groups.uni-paderborn.de/nt/meeteval/viz.html<br>
-> Interactive notebook: https://fgnt.github.io/meeteval_jupyterlite/lab?path=Demo.ipynb
+> [!TIP]
+> Try it in the browser! https://fgnt.github.com/meeteval_viz
 
 ```python
 import meeteval
 from meeteval.viz.visualize import AlignmentVisualization
 
 folder = r'https://raw.githubusercontent.com/fgnt/meeteval/main/'
 av = AlignmentVisualization(
```

#### html2text {}

```diff
@@ -1,40 +1,45 @@
-Metadata-Version: 2.1 Name: meeteval Version: 0.2.1 Home-page: https://
+Metadata-Version: 2.1 Name: meeteval Version: 0.3.0 Home-page: https://
 github.com/fgnt/meeteval/ Author: Department of Communications Engineering,
 Paderborn University Author-email: sek@nt.upb.de License: MIT Keywords: speech
 recognition,word error rate,evaluation,meeting,ASR,WER Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Python: >=3.5 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: kaldialign Requires-Dist: scipy Requires-
 Dist: typing_extensions; python_version < "3.8" Requires-Dist: cached_property;
 python_version < "3.8" Requires-Dist: Cython Provides-Extra: cli Requires-Dist:
 pyyaml; extra == "cli" Requires-Dist: fire; extra == "cli" Requires-Dist:
 simplejson; extra == "cli" Requires-Dist: aiohttp; extra == "cli" Requires-
-Dist: soundfile; extra == "cli" Provides-Extra: test Requires-Dist:
-editdistance; extra == "test" Requires-Dist: pytest; extra == "test" Requires-
-Dist: hypothesis; extra == "test" Requires-Dist: click; extra == "test"
+Dist: soundfile; extra == "cli" Requires-Dist: tqdm; extra == "cli" Requires-
+Dist: yattag; extra == "cli" Requires-Dist: platformdirs; extra == "cli"
+Provides-Extra: test Requires-Dist: editdistance; extra == "test" Requires-
+Dist: pytest; extra == "test" Requires-Dist: hypothesis; extra == "test"
 Requires-Dist: coverage; extra == "test" Requires-Dist: pytest-cov; extra ==
 "test" Requires-Dist: ipython; extra == "test" Requires-Dist: pyyaml; extra ==
-"test" Requires-Dist: simplejson; extra == "test" Requires-Dist: aiohttp; extra
-== "test" Requires-Dist: soundfile; extra == "test" Provides-Extra: all
-Requires-Dist: pyyaml; extra == "all" Requires-Dist: fire; extra == "all"
+"test" Requires-Dist: fire; extra == "test" Requires-Dist: simplejson; extra ==
+"test" Requires-Dist: aiohttp; extra == "test" Requires-Dist: soundfile; extra
+== "test" Requires-Dist: tqdm; extra == "test" Requires-Dist: yattag; extra ==
+"test" Requires-Dist: platformdirs; extra == "test" Provides-Extra: all
+Requires-Dist: lazy_dataset; extra == "all" Requires-Dist: ipywidgets; extra ==
+"all" Requires-Dist: pyyaml; extra == "all" Requires-Dist: fire; extra == "all"
 Requires-Dist: simplejson; extra == "all" Requires-Dist: aiohttp; extra ==
-"all" Requires-Dist: soundfile; extra == "all" Requires-Dist: editdistance;
-extra == "all" Requires-Dist: pytest; extra == "all" Requires-Dist: hypothesis;
-extra == "all" Requires-Dist: click; extra == "all" Requires-Dist: coverage;
-extra == "all" Requires-Dist: pytest-cov; extra == "all" Requires-Dist:
-ipython; extra == "all" Requires-Dist: lazy_dataset; extra == "all"
+"all" Requires-Dist: soundfile; extra == "all" Requires-Dist: tqdm; extra ==
+"all" Requires-Dist: yattag; extra == "all" Requires-Dist: platformdirs; extra
+== "all" Requires-Dist: editdistance; extra == "all" Requires-Dist: pytest;
+extra == "all" Requires-Dist: hypothesis; extra == "all" Requires-Dist:
+coverage; extra == "all" Requires-Dist: pytest-cov; extra == "all" Requires-
+Dist: ipython; extra == "all"
                             ************ MMeeeettEEvvaall ************
              ******** AA mmeeeettiinngg ttrraannssccrriippttiioonn eevvaalluuaattiioonn ttoooollkkiitt ********
      _F_e_a_t_u_r_e_s | _I_n_s_t_a_l_l_a_t_i_o_n | _P_y_t_h_o_n_ _I_n_t_e_r_f_a_c_e | _C_o_m_m_a_n_d_ _L_i_n_e_ _I_n_t_e_r_f_a_c_e |
-                          _V_i_s_u_a_l_i_z_a_t_i_o_n_ _(_W_I_P_) | _C_i_t_e
+                             _V_i_s_u_a_l_i_z_a_t_i_o_n | _C_i_t_e
 
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_f_g_n_t_/_m_e_e_t_e_v_a_l_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_p_y_t_e_s_t_._y_m_l_/_b_a_d_g_e_._s_v_g_]##
 Features MeetEval supports the following metrics for meeting transcription
 evaluation: - **Standard WER** for single utterances (Called SISO WER in
 MeetEval)
 `meeteval-wer wer -r ref -h hyp` - **Concatenated minimum-Permutation Word
 Error Rate (cpWER)**
@@ -45,28 +50,28 @@
 `meeteval-wer mimower -r ref.stm -h hyp.stm` - **Time-Constrained minimum-
 Permutation Word Error Rate (tcpWER)**
 `meeteval-wer tcpwer -r ref.stm -h hyp.stm --collar 5` - **Time-Constrained
 Optimal Reference Combination Word Error Rate (tcORC WER)**
 `meeteval-wer tcorcwer -r ref.stm -h hyp.stm --collar 5` - **Diarization Error
 Rate (DER)** by wrapping [mdeval](https://github.com/nryant/dscore/raw/master/
 scorelib/md-eval-22.pl)
-`meeteval-der md_eval_22 -r ref.stm -h hyp.stm --collar .25` Additionally
-(WIP), MeetEval contains a [visualization](#visualization-wip) tool for cpWER
-and tcpWER alignments that help spot errors in system outputs. ## Installation
-### From PyPI ```shell pip install meeteval ``` ### From source ```shell git
-clone https://github.com/fgnt/meeteval pip install -e ./meeteval ``` ##
-Command-line interface `MeetEval` supports the following file formats as input:
-- [Segmental Time Mark](https://github.com/usnistgov/SCTK/blob/master/doc/
-infmts.htm#L75) (`STM`) - [Time Marked Conversation](https://github.com/
-usnistgov/SCTK/blob/master/doc/infmts.htm#L286) (`CTM`) - [SEGment-wise Long-
-form Speech Transcription annotation](#segment-wise-long-form-speech-
-transcription-annotation-seglst) (`SegLST`), the file format used in the [CHiME
-challenges](https://www.chimechallenge.org) - [Rich Transcription Time Marked]
-(https://github.com/nryant/dscore?tab=readme-ov-file#rttm) (`RTTM`) files (only
-for Diarizaiton Error Rate) > [!NOTE] > `MeetEval` does not support alternate
+`meeteval-der md_eval_22 -r ref.stm -h hyp.stm --collar .25` Additionally,
+MeetEval contains a [visualization](#visualization) tool for cpWER and tcpWER
+alignments that helps to spot errors in system outputs. ## Installation ###
+From PyPI ```shell pip install meeteval ``` ### From source ```shell git clone
+https://github.com/fgnt/meeteval pip install -e ./meeteval ``` ## Command-line
+interface `MeetEval` supports the following file formats as input: - [Segmental
+Time Mark](https://github.com/usnistgov/SCTK/blob/master/doc/infmts.htm#L75)
+(`STM`) - [Time Marked Conversation](https://github.com/usnistgov/SCTK/blob/
+master/doc/infmts.htm#L286) (`CTM`) - [SEGment-wise Long-form Speech
+Transcription annotation](#segment-wise-long-form-speech-transcription-
+annotation-seglst) (`SegLST`), the file format used in the [CHiME challenges]
+(https://www.chimechallenge.org) - [Rich Transcription Time Marked](https://
+github.com/nryant/dscore?tab=readme-ov-file#rttm) (`RTTM`) files (only for
+Diarization Error Rate) > [!NOTE] > `MeetEval` does not support alternate
 transcripts (e.g., `"i've { um / uh / @ } as far as i'm concerned"`). The
 command-line interface is available as `meeteval-wer` or `python -
 m meeteval.wer` with the following signature: ```shell python -m meeteval.wer
 [orcwer|mimower|cpwer|tcpwer|tcorcwer] -h example_files/hyp.stm -
 r example_files/ref.stm # or meeteval-wer
 [orcwer|mimower|cpwer|tcpwer|tcorcwer] -h example_files/hyp.stm -
 r example_files/ref.stm ``` You can add `--help` to any command to get more
@@ -199,21 +204,18 @@
 hypothesis_self_overlap=SelfOverlap(overlap_rate=Decimal('0'), overlap_time=0,
 total_time=Decimal('2')), missed_speaker=0, falarm_speaker=0, scored_speaker=2)
 ``` ### Aligning sequences Sequences can be aligned, similar to
 `kaldialign.align`, using the tcpWER matching: ```python import meeteval
 meeteval.wer.wer.time_constrained.align([{'words': 'a b', 'start_time': 0,
 'end_time': 1}], [{'words': 'a c', 'start_time': 0, 'end_time': 1}, {'words':
 'd', 'start_time': 2, 'end_time': 3}]) # [('a', 'a'), ('b', 'c'), ('*', 'd')]
-``` ## Visualization [WIP] > [!IMPORTANT] > The visualization is under
-development!
-> Preview: https://groups.uni-paderborn.de/nt/meeteval/viz.html
-> Interactive notebook: https://fgnt.github.io/meeteval_jupyterlite/
-lab?path=Demo.ipynb ```python import meeteval from meeteval.viz.visualize
-import AlignmentVisualization folder = r'https://raw.githubusercontent.com/
-fgnt/meeteval/main/' av = AlignmentVisualization( meeteval.io.load(folder +
+``` ## Visualization > [!TIP] > Try it in the browser! https://fgnt.github.com/
+meeteval_viz ```python import meeteval from meeteval.viz.visualize import
+AlignmentVisualization folder = r'https://raw.githubusercontent.com/fgnt/
+meeteval/main/' av = AlignmentVisualization( meeteval.io.load(folder +
 'example_files/ref.stm').groupby('filename')['recordingA'], meeteval.io.load
 (folder + 'example_files/hyp.stm').groupby('filename')['recordingA'] ) #
 display(av) # Jupyter # av.dump('viz.html') # Create standalone HTML file ```
 ## Cite The toolkit and the tcpWER were presented at the CHiME-2023 workshop
 (Computational Hearing in Multisource Environments) with the paper ["MeetEval:
 A Toolkit for Computation of Word Error Rates for Meeting Transcription
 Systems"](https://arxiv.org/abs/2307.11394). ```bibtex @InProceedings
```

### Comparing `meeteval-0.2.1/meeteval.egg-info/SOURCES.txt` & `meeteval-0.3.0/meeteval.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 meeteval/io/rttm.py
 meeteval/io/seglst.py
 meeteval/io/stm.py
 meeteval/io/uem.py
 meeteval/viz/__init__.py
 meeteval/viz/__main__.py
 meeteval/viz/file_server.py
+meeteval/viz/side_by_side_sync.html
 meeteval/viz/visualize.css
 meeteval/viz/visualize.js
 meeteval/viz/visualize.py
 meeteval/wer/__init__.py
 meeteval/wer/__main__.py
 meeteval/wer/api.py
 meeteval/wer/utils.py
```

### Comparing `meeteval-0.2.1/setup.py` & `meeteval-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,40 +29,42 @@
             ['meeteval/wer/matching/cy_time_constrained_orc_matching.pyx'],
             extra_compile_args=['-std=c++11', '-O3'],
             extra_link_args=['-std=c++11'],
         ),
      ]
 )
 
+extras_require = {}
+extras_require['cli'] = [
+    'pyyaml',
+    'fire',
+    'simplejson',
+    'aiohttp',
+    'soundfile',
+    'tqdm',  # Used in meeteval.viz.__main__.py
+    'yattag',  # Used in meeteval.viz.__main__.py
+    'platformdirs',  # Used in meeteval.viz.visualize.py
+]
+extras_require['test'] = [
+    'editdistance',     # Faulty for long sequences, but useful for testing
+    'pytest',
+    'hypothesis',
+    'coverage',
+    'pytest-cov',
+    'ipython',  # IPython.lib.pretty.pprint
+    *extras_require['cli'],
+]
+extras_require['all'] = [
+    'lazy_dataset',
+    'ipywidgets',  # Used to provide dropdown menu in ipynb
+    *sum(extras_require.values(), []),
+]
 extras_require = {
-    'cli': [
-        'pyyaml',
-        'fire',
-        'simplejson',
-        'aiohttp',
-        'soundfile',
-    ],
-    'test': [
-        'editdistance',     # Faulty for long sequences, but useful for testing
-        'pytest',
-        'hypothesis',
-        'click',
-        'coverage',
-        'pytest-cov',
-        'ipython',  # IPython.lib.pretty.pprint
-        'pyyaml',
-        'simplejson',
-        'aiohttp',
-        'soundfile',
-    ],
-    'all': [  # List only missing from the other lists
-        'lazy_dataset',
-    ],
-}
-extras_require['all'] = list(dict.fromkeys(sum(extras_require.values(), [])))
+    k: list(dict.fromkeys(v))  # Drop duplicates
+    for k, v in extras_require.items()}
 
 # Get the long description from the relevant file
 try:
     from os import path
 
     here = path.abspath(path.dirname(__file__))
     with open(path.join(here, 'README.md'), encoding='utf-8') as f:
@@ -70,15 +72,15 @@
 except FileNotFoundError:
     long_description = ''
 
 setup(
     name="meeteval",
 
     # Versions should comply with PEP440.
-    version='0.2.1',
+    version='0.3.0',
 
     # The project's main homepage.
     url='https://github.com/fgnt/meeteval/',
 
     # Choose your license
     license='MIT',
 
@@ -118,15 +120,15 @@
         'kaldialign',
         'scipy',  # scipy.optimize.linear_sum_assignment
         "typing_extensions; python_version<'3.8'",  # Missing Literal in py37
         "cached_property; python_version<'3.8'",  # Missing functools.cached_property in py37
         'Cython'
     ],
     extras_require=extras_require,
-    package_data={'meeteval': ['**/*.pyx', '**/*.h', '**/*.js', '**/*.css']},  # https://stackoverflow.com/a/60751886
+    package_data={'meeteval': ['**/*.pyx', '**/*.h', '**/*.js', '**/*.css', '**/*.html']},  # https://stackoverflow.com/a/60751886
     entry_points={
         'console_scripts': [
             'meeteval-wer=meeteval.wer.__main__:cli',
             'meeteval-der=meeteval.der.__main__:cli',
         ]
     }
 )
```

### Comparing `meeteval-0.2.1/tests/test_cli.py` & `meeteval-0.3.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,16 @@
 
 
 def test_burn_md_eval_22():
     run(f'python -m meeteval.der md_eval_22 -h hyp.stm -r ref.stm')
     run(f'meeteval-der md_eval_22 -h hyp.stm -r ref.stm')
     run(f'python -m meeteval.der md_eval_22 -h hyp.stm -r ref.stm --collar 0.25')
     run(f'python -m meeteval.der md_eval_22 -h hyp.rttm -r ref.rttm')
+    run(f'python -m meeteval.der md_eval_22 -h hyp.rttm -r ref.rttm --regions all')
+    run(f'python -m meeteval.der md_eval_22 -h hyp.rttm -r ref.rttm --regions nooverlap')
     run(f'python -m meeteval.der md_eval_22 -h hyp.rttm -r ref.rttm --regex ".*A"')
     run(f'python -m meeteval.der md_eval_22 -h hyp.seglst.json -r ref.seglst.json')
     # examples for collar:
     #    0:    CHiME-6
     #    0.25: CHiME-7 DASR
     # ToDo: Table 2 of https://arxiv.org/pdf/2312.04324.pdf lists collars for
     #       datsets. Add them here.
@@ -151,7 +153,15 @@
     run(f'python -m meeteval.wer average hypA_cpwer_per_reco.json hypB_cpwer_per_reco.json')
 
     run(f'python -m meeteval.wer average hypA_cpwer_per_reco.json hypB_cpwer_per_reco.json')
 
 
 def test_burn_siso():
     run(f'python -m meeteval.wer wer -h text_hyp -r text_ref')
+
+
+def test_viz_html():
+    run(f'python -m meeteval.viz html -h hyp.stm -r ref.stm')
+    run(f'python -m meeteval.viz html -h hyp.stm -r ref.stm --normalizer="lower,rm(.?!,)"')
+    run(f'python -m meeteval.viz html -h hyp.stm -r ref.stm --alignment=tcp')
+    run(f'python -m meeteval.viz html -h hyp.stm -r ref.stm --alignment=cp')
+    run(f'python -m meeteval.viz html -h hyp.stm -r ref.stm --out=viz')
```

### Comparing `meeteval-0.2.1/tests/test_io.py` & `meeteval-0.3.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/tests/test_levenshtein.py` & `meeteval-0.3.0/tests/test_levenshtein.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/tests/test_mimo_matching.py` & `meeteval-0.3.0/tests/test_mimo_matching.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/tests/test_orc_matching.py` & `meeteval-0.3.0/tests/test_orc_matching.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/tests/test_shell_vs_py.py` & `meeteval-0.3.0/tests/test_shell_vs_py.py`

 * *Files identical despite different names*

### Comparing `meeteval-0.2.1/tests/test_time_constrained.py` & `meeteval-0.3.0/tests/test_time_constrained.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,23 +94,24 @@
     assert len([a for a in s['alignment'] if a[0] is None or a[1] is None]) <= distance
 
 
 @given(string, string)
 @settings(deadline=None)
 def test_time_constrained_levenshtein_distance_with_alignment_against_kaldialign(a, b):
     """Check that the returned alignment matches kaldialign then the time intervals span the full length"""
-    from kaldialign import align as kaldi_align, edit_distance
+    from kaldialign import align as kaldi_align
+    from meeteval.wer.wer.utils import kaldialign_edit_distance
     from meeteval.wer.wer.time_constrained import index_alignment_to_kaldi_alignment
     from meeteval.wer.matching import time_constrained_levenshtein_distance_with_alignment
 
     a_timing = [(0, 1)] * len(a)
     b_timing = [(0, 1)] * len(b)
 
     kaldialign_alignment = kaldi_align(a, b, '*')
-    kaldialign_statistics = edit_distance(a, b)
+    kaldialign_statistics = kaldialign_edit_distance(a, b)
     statistics = time_constrained_levenshtein_distance_with_alignment(a, b, a_timing, b_timing)
     alignment = statistics.pop('alignment')
     alignment = index_alignment_to_kaldi_alignment(alignment, a, b)
     assert alignment == kaldialign_alignment, (alignment, kaldialign_alignment)
     assert kaldialign_statistics['ins'] == statistics['insertions'], (kaldialign_statistics, statistics)
     assert kaldialign_statistics['sub'] == statistics['substitutions'], (kaldialign_statistics, statistics)
     assert kaldialign_statistics['total'] == statistics['total'], (kaldialign_statistics, statistics)
```

### Comparing `meeteval-0.2.1/tests/test_time_constrained_orc_matching.py` & `meeteval-0.3.0/tests/test_time_constrained_orc_matching.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,15 +52,16 @@
     """
     from meeteval.wer.wer.orc import orc_word_error_rate
     from meeteval.wer.wer.time_constrained_orc import time_constrained_orc_wer
 
     orc = orc_word_error_rate(reference, hypothesis)
 
     # Without time constraint (collar is larger than the maximum length)
-    tcorc = time_constrained_orc_wer(reference, hypothesis, collar=1000)
+    # and without sorting because the low-level ORC-WER doesn't sort
+    tcorc = time_constrained_orc_wer(reference, hypothesis, collar=1000, reference_sort=False, hypothesis_sort=False)
     assert orc.error_rate == tcorc.error_rate
     assert orc.errors == tcorc.errors
     # TODO: make sure that the following are equal
     # assert orc.insertions == tcorc.insertions
     # assert orc.deletions == tcorc.deletions
     # assert orc.substitutions == tcorc.substitutions
 
@@ -71,15 +72,15 @@
 )
 def test_orc_bound_by_tcorc(reference, hypothesis):
     """Tests that tcORC-WER is never lower than ORC-WER"""
     from meeteval.wer.wer.orc import orc_word_error_rate
     from meeteval.wer.wer.time_constrained_orc import time_constrained_orc_wer
 
     orc = orc_word_error_rate(reference, hypothesis)
-    tcorc = time_constrained_orc_wer(reference, hypothesis, collar=0.1)
+    tcorc = time_constrained_orc_wer(reference, hypothesis, collar=0.1, reference_sort=False, hypothesis_sort=False)
 
     # error_rate can be None when length is None
     assert orc.error_rate is None and tcorc.error_rate is None or orc.error_rate <= tcorc.error_rate
 
 
 @given(
     seglst(max_speakers=1, min_segments=1),
@@ -131,7 +132,27 @@
     example_files = (Path(__file__).parent.parent / 'example_files').absolute()
 
     from meeteval.wer import tcorcwer
     wers = tcorcwer(example_files / 'ref.stm', example_files / 'hyp.stm', collar=5)
     for k, wer in wers.items():
         assert wer.reference_self_overlap.overlap_time == 0, (k, wer)
         assert wer.hypothesis_self_overlap.overlap_time == 0, (k, wer)
+
+
+def test_assignment_keeps_order():
+    from meeteval.wer.wer.time_constrained_orc import time_constrained_orc_wer
+
+    tcorc = time_constrained_orc_wer(
+        SegLST([
+            {'words': 'a1', 'session_id': 'a', 'speaker': 'A', 'start_time': 2, 'end_time': 3},
+            {'words': '', 'session_id': 'a', 'speaker': 'A', 'start_time': 1, 'end_time': 2},
+            {'words': 'a2', 'session_id': 'a', 'speaker': 'A', 'start_time': 0, 'end_time': 1}
+        ]),
+        SegLST([
+            {'words': 'a1', 'session_id': 'a', 'speaker': 'A1', 'start_time': 2, 'end_time': 3},
+            {'words': 'a2', 'session_id': 'a', 'speaker': 'A2', 'start_time': 0, 'end_time': 1}
+        ]),
+        reference_sort='segment',
+    )
+    assert tcorc.assignment == ('A1', 'A1', 'A2')
+
+
```

