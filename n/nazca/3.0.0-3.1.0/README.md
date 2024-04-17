# Comparing `tmp/nazca-3.0.0.tar.gz` & `tmp/nazca-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nazca-3.0.0.tar", last modified: Wed Jul  5 14:11:52 2023, max compression
+gzip compressed data, was "nazca-3.1.0.tar", last modified: Wed Apr 17 12:05:30 2024, max compression
```

## Comparing `nazca-3.0.0.tar` & `nazca-3.1.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.366472 nazca-3.0.0/
--rw-r--r--   0 schabot   (1000) schabot   (1000)    20883 2023-07-05 13:54:58.000000 nazca-3.0.0/CHANGELOG.md
--rw-r--r--   0 schabot   (1000) schabot   (1000)      381 2023-07-05 13:18:11.000000 nazca-3.0.0/MANIFEST.in
--rw-r--r--   0 schabot   (1000) schabot   (1000)      668 2023-07-05 14:11:52.366472 nazca-3.0.0/PKG-INFO
--rw-r--r--   0 schabot   (1000) schabot   (1000)       83 2023-07-05 13:28:03.000000 nazca-3.0.0/README.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.358472 nazca-3.0.0/doc/
--rw-r--r--   0 schabot   (1000) schabot   (1000)    54838 2019-04-19 14:35:24.000000 nazca-3.0.0/doc/nazca-logo.svg
--rw-r--r--   0 schabot   (1000) schabot   (1000)    22785 2019-04-19 14:35:24.000000 nazca-3.0.0/doc.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.358472 nazca-3.0.0/examples/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-04-19 14:35:24.000000 nazca-3.0.0/examples/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6653 2023-07-05 13:28:03.000000 nazca-3.0.0/examples/demo.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2305 2019-04-19 14:35:24.000000 nazca-3.0.0/examples/goncourt.csv
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.358472 nazca-3.0.0/nazca/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-04-19 14:35:24.000000 nazca-3.0.0/nazca/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1912 2023-07-05 13:54:13.000000 nazca-3.0.0/nazca/__pkginfo__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.362472 nazca-3.0.0/nazca/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      216 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/data/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    32441 2020-05-07 07:41:53.000000 nazca-3.0.0/nazca/data/countries.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4882 2019-04-19 14:35:24.000000 nazca-3.0.0/nazca/data/countries_iso_3166.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)  4246181 2019-04-19 14:35:24.000000 nazca-3.0.0/nazca/data/french_lemmas.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)    24612 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/data/stopwords.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5376 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/data/us_states.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.362472 nazca-3.0.0/nazca/ner/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2681 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/ner/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3755 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/ner/filters.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2699 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/ner/preprocessors.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3892 2023-07-05 13:31:15.000000 nazca-3.0.0/nazca/ner/sources.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.362472 nazca-3.0.0/nazca/rl/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-04-19 14:35:24.000000 nazca-3.0.0/nazca/rl/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    15110 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/rl/aligner.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    26824 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/rl/blocking.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.362472 nazca-3.0.0/nazca/utils/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-06-03 13:28:47.000000 nazca-3.0.0/nazca/utils/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    12047 2023-07-05 13:31:49.000000 nazca-3.0.0/nazca/utils/dataio.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    22287 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/utils/distances.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8679 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/utils/minhashing.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    15394 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/utils/normalize.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2655 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/utils/tokenizer.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.358472 nazca-3.0.0/nazca.egg-info/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      668 2023-07-05 14:11:52.000000 nazca-3.0.0/nazca.egg-info/PKG-INFO
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1122 2023-07-05 14:11:52.000000 nazca-3.0.0/nazca.egg-info/SOURCES.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2023-07-05 14:11:52.000000 nazca-3.0.0/nazca.egg-info/dependency_links.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2019-04-19 14:38:35.000000 nazca-3.0.0/nazca.egg-info/not-zip-safe
--rw-r--r--   0 schabot   (1000) schabot   (1000)       53 2023-07-05 14:11:52.000000 nazca-3.0.0/nazca.egg-info/requires.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)        6 2023-07-05 14:11:52.000000 nazca-3.0.0/nazca.egg-info/top_level.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)       38 2023-07-05 14:11:52.366472 nazca-3.0.0/setup.cfg
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2461 2023-07-05 13:28:03.000000 nazca-3.0.0/setup.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.362472 nazca-3.0.0/test/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.366472 nazca-3.0.0/test/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       83 2019-04-19 14:35:24.000000 nazca-3.0.0/test/data/alignfile.csv
--rw-r--r--   0 schabot   (1000) schabot   (1000)       86 2019-04-19 14:35:24.000000 nazca-3.0.0/test/data/file2parse
--rw-r--r--   0 schabot   (1000) schabot   (1000)    20618 2019-04-19 14:35:24.000000 nazca-3.0.0/test/data/file2split
--rw-r--r--   0 schabot   (1000) schabot   (1000)       63 2019-04-19 14:35:24.000000 nazca-3.0.0/test/data/targetfile.csv
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10516 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_alignment.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    16831 2023-07-05 13:43:33.000000 nazca-3.0.0/test/test_blocking.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    13276 2023-07-05 13:32:27.000000 nazca-3.0.0/test/test_dataio.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10180 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_distances.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7225 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_filters.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2667 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_minhashing.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    15678 2023-07-05 13:30:48.000000 nazca-3.0.0/test/test_ner.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8590 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_normalize.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4454 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_preprocessors.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3923 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_tokenizer.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      871 2023-07-05 13:28:03.000000 nazca-3.0.0/tox.ini
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-17 12:05:30.106469 nazca-3.1.0/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    21106 2024-04-17 11:57:32.000000 nazca-3.1.0/CHANGELOG.md
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      381 2023-07-05 13:18:11.000000 nazca-3.1.0/MANIFEST.in
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      627 2024-04-17 12:05:30.106469 nazca-3.1.0/PKG-INFO
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       83 2023-07-05 13:28:03.000000 nazca-3.1.0/README.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-17 12:05:30.098469 nazca-3.1.0/doc/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    54838 2019-04-19 14:35:24.000000 nazca-3.1.0/doc/nazca-logo.svg
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    22785 2019-04-19 14:35:24.000000 nazca-3.1.0/doc.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-17 12:05:30.098469 nazca-3.1.0/examples/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-04-19 14:35:24.000000 nazca-3.1.0/examples/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6655 2024-04-17 10:40:01.000000 nazca-3.1.0/examples/demo.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2305 2019-04-19 14:35:24.000000 nazca-3.1.0/examples/goncourt.csv
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-17 12:05:30.098469 nazca-3.1.0/nazca/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-04-19 14:35:24.000000 nazca-3.1.0/nazca/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1935 2024-04-17 11:57:25.000000 nazca-3.1.0/nazca/__pkginfo__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-17 12:05:30.102469 nazca-3.1.0/nazca/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      217 2024-04-17 10:40:01.000000 nazca-3.1.0/nazca/data/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    32441 2020-05-07 07:41:53.000000 nazca-3.1.0/nazca/data/countries.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4882 2019-04-19 14:35:24.000000 nazca-3.1.0/nazca/data/countries_iso_3166.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)  4246181 2019-04-19 14:35:24.000000 nazca-3.1.0/nazca/data/french_lemmas.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    24612 2023-07-05 13:28:03.000000 nazca-3.1.0/nazca/data/stopwords.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5376 2023-07-05 13:28:03.000000 nazca-3.1.0/nazca/data/us_states.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-17 12:05:30.102469 nazca-3.1.0/nazca/ner/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2682 2024-04-17 10:40:01.000000 nazca-3.1.0/nazca/ner/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3756 2024-04-17 10:40:01.000000 nazca-3.1.0/nazca/ner/filters.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2700 2024-04-17 10:40:01.000000 nazca-3.1.0/nazca/ner/preprocessors.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3893 2024-04-17 10:40:01.000000 nazca-3.1.0/nazca/ner/sources.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-17 12:05:30.102469 nazca-3.1.0/nazca/rl/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-04-19 14:35:24.000000 nazca-3.1.0/nazca/rl/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15110 2023-07-05 13:28:03.000000 nazca-3.1.0/nazca/rl/aligner.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    26824 2024-04-17 10:21:28.000000 nazca-3.1.0/nazca/rl/blocking.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-17 12:05:30.102469 nazca-3.1.0/nazca/utils/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-06-03 13:28:47.000000 nazca-3.1.0/nazca/utils/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    12065 2024-04-17 11:56:10.000000 nazca-3.1.0/nazca/utils/dataio.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    22287 2024-04-17 10:21:28.000000 nazca-3.1.0/nazca/utils/distances.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8679 2023-07-05 13:28:03.000000 nazca-3.1.0/nazca/utils/minhashing.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15394 2023-07-05 13:28:03.000000 nazca-3.1.0/nazca/utils/normalize.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2656 2024-04-17 10:40:01.000000 nazca-3.1.0/nazca/utils/tokenizer.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-17 12:05:30.098469 nazca-3.1.0/nazca.egg-info/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      627 2024-04-17 12:05:29.000000 nazca-3.1.0/nazca.egg-info/PKG-INFO
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1122 2024-04-17 12:05:30.000000 nazca-3.1.0/nazca.egg-info/SOURCES.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2024-04-17 12:05:29.000000 nazca-3.1.0/nazca.egg-info/dependency_links.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2019-04-19 14:38:35.000000 nazca-3.1.0/nazca.egg-info/not-zip-safe
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       60 2024-04-17 12:05:29.000000 nazca-3.1.0/nazca.egg-info/requires.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        6 2024-04-17 12:05:29.000000 nazca-3.1.0/nazca.egg-info/top_level.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       38 2024-04-17 12:05:30.106469 nazca-3.1.0/setup.cfg
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2461 2023-07-05 13:28:03.000000 nazca-3.1.0/setup.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-17 12:05:30.106469 nazca-3.1.0/test/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-17 12:05:30.106469 nazca-3.1.0/test/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       83 2019-04-19 14:35:24.000000 nazca-3.1.0/test/data/alignfile.csv
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       86 2019-04-19 14:35:24.000000 nazca-3.1.0/test/data/file2parse
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    20618 2019-04-19 14:35:24.000000 nazca-3.1.0/test/data/file2split
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       63 2019-04-19 14:35:24.000000 nazca-3.1.0/test/data/targetfile.csv
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10516 2023-07-05 13:28:03.000000 nazca-3.1.0/test/test_alignment.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    16831 2023-07-05 13:43:33.000000 nazca-3.1.0/test/test_blocking.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    13276 2023-07-05 13:32:27.000000 nazca-3.1.0/test/test_dataio.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10180 2023-07-05 13:28:03.000000 nazca-3.1.0/test/test_distances.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7225 2023-07-05 13:28:03.000000 nazca-3.1.0/test/test_filters.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2667 2023-07-05 13:28:03.000000 nazca-3.1.0/test/test_minhashing.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15678 2023-07-05 13:30:48.000000 nazca-3.1.0/test/test_ner.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8590 2023-07-05 13:28:03.000000 nazca-3.1.0/test/test_normalize.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4454 2023-07-05 13:28:03.000000 nazca-3.1.0/test/test_preprocessors.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3923 2023-07-05 13:28:03.000000 nazca-3.1.0/test/test_tokenizer.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1092 2024-04-17 12:04:21.000000 nazca-3.1.0/tox.ini
```

### Comparing `nazca-3.0.0/CHANGELOG.md` & `nazca-3.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+## Version 3.1.0 (2024-04-17)
+### 👷 Bug fixes
+
+- allow html validation to use remote dtd
+
+### 🤖 Continuous integration
+
+- update .gitlab-ci to use templates
+
+### 🤷 Various changes
+
+- update the url of the project
+
 ## Version 3.0.0 (2023-07-05)
 ### 🎉 New features
 
 - *BREAKING CHANGE*: remove RQL related functions
 - correctly process OPTIONAL values in SPARQL
 - improve logging messages about statistics
```

### Comparing `nazca-3.0.0/doc/nazca-logo.svg` & `nazca-3.1.0/doc/nazca-logo.svg`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/doc.rst` & `nazca-3.1.0/doc.rst`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/examples/demo.py` & `nazca-3.1.0/examples/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     alignset = parsefile(dpath("frenchbnf"), indexes=[0, 2, (14, 12)], nbmax=1000)
 
     # Let's define the processings to apply on the location's name
     tr_name = {
         "normalization": [aln.simplify],  # Simply all the names (remove
         #   punctuation, lower case, etc)
         "metric": ald.levenshtein,  # Use the levenshtein distance
-        "weighting": 1  # Use 1 a name-distance matrix
+        "weighting": 1,  # Use 1 a name-distance matrix
         #   weighting coefficient
     }
     tr_geo = {
         "normalization": [],  # No normalization needed
         "metric": ald.geographical,  # Use the geographical distance
         "metric_params": {"units": "km"},  # Arguments given the
         #   distance function. Here,
@@ -127,15 +127,15 @@
     neighbours = findneighbours(alignset, targetset, indexes=(2, 2), mode="minibatch")
 
     # Let's define the processings to apply on the location's name
     tr_name = {
         "normalization": [aln.simplify],  # Simply all the names (remove
         #   punctuation, lower case, etc)
         "metric": ald.levenshtein,  # Use the levenshtein distance
-        "weighting": 1  # Use 1 a name-distance matrix
+        "weighting": 1,  # Use 1 a name-distance matrix
         #   weighting coefficient
     }
 
     processings = {1: tr_name}
     print("Start computation")
     for ind, (alignid, targetid) in enumerate(neighbours):
         print("%3d" % ind, len(alignid), "x", len(targetid))
```

### Comparing `nazca-3.0.0/examples/goncourt.csv` & `nazca-3.1.0/examples/goncourt.csv`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/nazca/__pkginfo__.py` & `nazca-3.1.0/nazca/__pkginfo__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,35 +20,35 @@
 __docformat__ = "restructuredtext en"
 from os.path import join
 import sys
 
 distname = "nazca"
 modname = "nazca"
 
-numversion = (3, 0, 0)
+numversion = (3, 1, 0)
 version = ".".join([str(num) for num in numversion])
 
 license = "LGPL"  # 2.1 or later
 description = "Python library for data alignment"
-web = "https://www.logilab.org/project/nazca"
+web = "https://forge.extranet.logilab.fr/open-source/nazca"
 author = "Logilab"
 author_email = "contact@logilab.fr"
 
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing",
 ]
 
 __depends__ = {
     "python-dateutil": None,
-    "lxml": "<= 4.9.2",
+    "lxml": ">= 4.0.0, < 6.0.0",
     "numpy": None,
     "scipy": None,
     "scikit-learn": None,
 }
 
 __recommends__ = {
     "sparqlwrapper": None,
```

### Comparing `nazca-3.0.0/nazca/data/countries.py` & `nazca-3.1.0/nazca/data/countries.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/nazca/data/countries_iso_3166.txt` & `nazca-3.1.0/nazca/data/countries_iso_3166.txt`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/nazca/data/french_lemmas.txt` & `nazca-3.1.0/nazca/data/french_lemmas.txt`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/nazca/data/stopwords.py` & `nazca-3.1.0/nazca/data/stopwords.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/nazca/data/us_states.py` & `nazca-3.1.0/nazca/data/us_states.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/nazca/ner/__init__.py` & `nazca-3.1.0/nazca/ner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Process/Core functions for Named Entities Recognition.
 """
+
 from nazca.utils.tokenizer import RichStringTokenizer
 
 
 ###############################################################################
 # NER PROCESS #################################################################
 ###############################################################################
 class NerProcess:
```

### Comparing `nazca-3.0.0/nazca/ner/filters.py` & `nazca-3.1.0/nazca/ner/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Filters for Named Entities Recognition.
 """
+
 from nazca.utils.dataio import sparqlquery
 
 
 ###############################################################################
 # NER FILTERS #################################################################
 ###############################################################################
 class AbstractNerFilter:
```

### Comparing `nazca-3.0.0/nazca/ner/preprocessors.py` & `nazca-3.1.0/nazca/ner/preprocessors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Preprocessors for Named Entities Recognition.
 """
+
 from nazca.utils.tokenizer import Token
 from nazca.data.stopwords import FRENCH_STOPWORDS, ENGLISH_STOPWORDS
 
 STOPWORDS = {"fr": FRENCH_STOPWORDS, "en": ENGLISH_STOPWORDS}
 
 
 ###############################################################################
```

### Comparing `nazca-3.0.0/nazca/ner/sources.py` & `nazca-3.1.0/nazca/ner/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Sources for Named Entities Recognition.
 """
+
 from nazca.utils.dataio import sparqlquery
 
 
 ###############################################################################
 # NER SOURCE ##################################################################
 ###############################################################################
 class AbstractNerSource:
```

### Comparing `nazca-3.0.0/nazca/rl/aligner.py` & `nazca-3.1.0/nazca/rl/aligner.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/nazca/rl/blocking.py` & `nazca-3.1.0/nazca/rl/blocking.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/nazca/utils/dataio.py` & `nazca-3.1.0/nazca/utils/dataio.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,12 +341,12 @@
 
     def is_valid(self, html):
         if isinstance(html, str):
             html = html.encode("utf-8")
         try:
             etree.fromstring(
                 self.XHTML_DOC_TEMPLATE % html,
-                parser=etree.XMLParser(dtd_validation=True),
+                parser=etree.XMLParser(dtd_validation=True, no_network=False),
             )
         except etree.XMLSyntaxError:
             return False
         return True
```

### Comparing `nazca-3.0.0/nazca/utils/distances.py` & `nazca-3.1.0/nazca/utils/distances.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/nazca/utils/minhashing.py` & `nazca-3.1.0/nazca/utils/minhashing.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/nazca/utils/normalize.py` & `nazca-3.1.0/nazca/utils/normalize.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/nazca/utils/tokenizer.py` & `nazca-3.1.0/nazca/utils/tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Tokenizer for sentences/words segmentation.
 """
+
 import collections
 import re
 
 try:
     from nltk.tokenize.punkt import PunktSentenceTokenizer
 except ImportError:
     NLTK_AVAILABLE = False
```

### Comparing `nazca-3.0.0/nazca.egg-info/SOURCES.txt` & `nazca-3.1.0/nazca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/setup.py` & `nazca-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/test/data/file2split` & `nazca-3.1.0/test/data/file2split`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/test/test_alignment.py` & `nazca-3.1.0/test/test_alignment.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/test/test_blocking.py` & `nazca-3.1.0/test/test_blocking.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/test/test_dataio.py` & `nazca-3.1.0/test/test_dataio.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/test/test_distances.py` & `nazca-3.1.0/test/test_distances.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/test/test_filters.py` & `nazca-3.1.0/test/test_filters.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/test/test_minhashing.py` & `nazca-3.1.0/test/test_minhashing.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/test/test_ner.py` & `nazca-3.1.0/test/test_ner.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/test/test_normalize.py` & `nazca-3.1.0/test/test_normalize.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/test/test_preprocessors.py` & `nazca-3.1.0/test/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/test/test_tokenizer.py` & `nazca-3.1.0/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nazca-3.0.0/tox.ini` & `nazca-3.1.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 [testenv]
 deps =
   pytest
   nltk
   SPARQLWrapper
   mock
-  git+https://github.com/psycojoker/pytest-capture-deprecatedwarnings
 commands =
   {envpython} -m pytest {posargs:test}
 
 [testenv:flake8]
 skip_install = true
 whitelist_externals =
   flake8
@@ -45,7 +44,22 @@
 [testenv:check-manifest]
 skip_install = true
 skipsdist = true
 deps =
   check-manifest
 commands =
   {envpython} -m check_manifest
+
+[testenv:pypi-publish]
+basepython = python3
+skip_install = true
+allowlist_externals = rm
+deps =
+  twine
+passenv =
+  TWINE_USERNAME
+  TWINE_PASSWORD
+commands =
+  rm -rf build dist .egg .egg-info
+  python3 setup.py sdist bdist_wheel
+  twine check dist/*
+  twine upload --skip-existing dist/*
```

