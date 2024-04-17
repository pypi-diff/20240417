# Comparing `tmp/medialibrary-0.2.1.tar.gz` & `tmp/medialibrary-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medialibrary-0.2.1.tar", last modified: Sun Dec 10 23:24:45 2023, max compression
+gzip compressed data, was "medialibrary-0.2.3.tar", last modified: Wed Apr 17 01:06:30 2024, max compression
```

## Comparing `medialibrary-0.2.1.tar` & `medialibrary-0.2.3.tar`

### file list

```diff
@@ -1,137 +1,144 @@
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.264908 medialibrary-0.2.1/
--rw-r--r--   0 chrisj     (102) other        (1)     1071 2021-09-05 20:32:22.000000 medialibrary-0.2.1/LICENSE
--rw-r--r--   0 chrisj     (102) other        (1)     3293 2023-12-10 23:24:45.264817 medialibrary-0.2.1/PKG-INFO
--rw-r--r--   0 chrisj     (102) other        (1)     2388 2023-12-10 23:20:51.000000 medialibrary-0.2.1/README.md
--rw-r--r--   0 chrisj     (102) other        (1)     1055 2023-12-10 23:23:13.000000 medialibrary-0.2.1/pyproject.toml
--rw-r--r--   0 chrisj     (102) other        (1)      150 2023-12-10 23:24:45.265469 medialibrary-0.2.1/setup.cfg
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.223509 medialibrary-0.2.1/src/
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.225224 medialibrary-0.2.1/src/media/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.226379 medialibrary-0.2.1/src/media/data/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     2182 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/dates.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.227168 medialibrary-0.2.1/src/media/data/media/
--rw-r--r--   0 chrisj     (102) other        (1)     1259 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.227558 medialibrary-0.2.1/src/media/data/media/contents/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/contents/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.228839 medialibrary-0.2.1/src/media/data/media/contents/generic/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/contents/generic/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     5671 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/contents/generic/catalog.py
--rw-r--r--   0 chrisj     (102) other        (1)     8487 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/data/media/contents/generic/keywords.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.230127 medialibrary-0.2.1/src/media/data/media/contents/generic/story/
--rw-r--r--   0 chrisj     (102) other        (1)     1172 2023-05-29 21:03:24.000000 medialibrary-0.2.1/src/media/data/media/contents/generic/story/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     4319 2023-05-29 21:03:24.000000 medialibrary-0.2.1/src/media/data/media/contents/generic/story/characters.py
--rw-r--r--   0 chrisj     (102) other        (1)     2783 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/data/media/contents/generic/story/internal.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.230965 medialibrary-0.2.1/src/media/data/media/contents/genericv/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/contents/genericv/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.232288 medialibrary-0.2.1/src/media/data/media/contents/genericv/crew/
--rw-r--r--   0 chrisj     (102) other        (1)     1198 2023-05-29 21:03:24.000000 medialibrary-0.2.1/src/media/data/media/contents/genericv/crew/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     8627 2023-05-29 21:03:24.000000 medialibrary-0.2.1/src/media/data/media/contents/genericv/crew/cast.py
--rw-r--r--   0 chrisj     (102) other        (1)     5667 2023-05-29 21:03:24.000000 medialibrary-0.2.1/src/media/data/media/contents/genericv/crew/internal.py
--rw-r--r--   0 chrisj     (102) other        (1)     3332 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/contents/genericv/technical.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.233542 medialibrary-0.2.1/src/media/data/media/contents/movie/
--rw-r--r--   0 chrisj     (102) other        (1)     1171 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/contents/movie/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     3810 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/contents/movie/classification.py
--rw-r--r--   0 chrisj     (102) other        (1)     6100 2023-05-29 21:03:24.000000 medialibrary-0.2.1/src/media/data/media/contents/movie/internal.py
--rw-r--r--   0 chrisj     (102) other        (1)     3863 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/data/media/internal.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.235181 medialibrary-0.2.1/src/media/data/media/library/
--rw-r--r--   0 chrisj     (102) other        (1)     1259 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/library/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     1853 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/library/filing.py
--rw-r--r--   0 chrisj     (102) other        (1)     5007 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/library/instances.py
--rw-r--r--   0 chrisj     (102) other        (1)     2070 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/library/internal.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.237593 medialibrary-0.2.1/src/media/data/media/medium/
--rw-r--r--   0 chrisj     (102) other        (1)     1259 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/medium/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     2498 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/medium/internal.py
--rw-r--r--   0 chrisj     (102) other        (1)     8439 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/medium/inventory.py
--rw-r--r--   0 chrisj     (102) other        (1)     3590 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/medium/productid.py
--rw-r--r--   0 chrisj     (102) other        (1)     4650 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/medium/productspecs.py
--rw-r--r--   0 chrisj     (102) other        (1)     3318 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/data/media/medium/release.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.238416 medialibrary-0.2.1/src/media/data/media/meta/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/data/media/meta/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)    12864 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/data/media/meta/authorship.py
--rw-r--r--   0 chrisj     (102) other        (1)     9141 2023-05-29 21:03:24.000000 medialibrary-0.2.1/src/media/data/nouns.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.240336 medialibrary-0.2.1/src/media/fileops/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/fileops/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     1564 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/fileops/filenames.py
--rw-r--r--   0 chrisj     (102) other        (1)     2013 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/fileops/loader.py
--rw-r--r--   0 chrisj     (102) other        (1)     3282 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/fileops/repo.py
--rw-r--r--   0 chrisj     (102) other        (1)     2977 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/fileops/scanner.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.240700 medialibrary-0.2.1/src/media/fmt/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/fmt/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.242286 medialibrary-0.2.1/src/media/fmt/text/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/fmt/text/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     4058 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/fmt/text/basics.py
--rw-r--r--   0 chrisj     (102) other        (1)     8180 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/fmt/text/media.py
--rw-r--r--   0 chrisj     (102) other        (1)     8922 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/fmt/text/movie.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.243039 medialibrary-0.2.1/src/media/generic/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/generic/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.244238 medialibrary-0.2.1/src/media/generic/sorting/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/generic/sorting/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     5470 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/generic/sorting/groups.py
--rw-r--r--   0 chrisj     (102) other        (1)     4307 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/generic/sorting/lists.py
--rw-r--r--   0 chrisj     (102) other        (1)     2351 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/generic/stringtools.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.245071 medialibrary-0.2.1/src/media/tools/
--rw-r--r--   0 chrisj     (102) other        (1)     1145 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/tools/__init__.py
--rwxr-xr-x   0 chrisj     (102) other        (1)     1846 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/tools/common.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.246988 medialibrary-0.2.1/src/media/tools/media/
--rw-r--r--   0 chrisj     (102) other        (1)     1150 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/tools/media/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     2645 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/tools/media/authorrecords.py
--rw-r--r--   0 chrisj     (102) other        (1)     2433 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/tools/media/list.py
--rw-r--r--   0 chrisj     (102) other        (1)     2390 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/tools/media/show.py
--rw-r--r--   0 chrisj     (102) other        (1)     7157 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/tools/media/validate.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.247768 medialibrary-0.2.1/src/media/tools/meta/
--rw-r--r--   0 chrisj     (102) other        (1)     1149 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/tools/meta/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     2291 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/tools/meta/authorship.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.251685 medialibrary-0.2.1/src/media/tools/movies/
--rw-r--r--   0 chrisj     (102) other        (1)     1151 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/tools/movies/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     8026 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/tools/movies/castlist.py
--rw-r--r--   0 chrisj     (102) other        (1)     3096 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/tools/movies/debuglist.py
--rw-r--r--   0 chrisj     (102) other        (1)     9675 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/tools/movies/genrebreakdown.py
--rw-r--r--   0 chrisj     (102) other        (1)     4230 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/tools/movies/keywordlist.py
--rw-r--r--   0 chrisj     (102) other        (1)     3808 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/tools/movies/list.py
--rw-r--r--   0 chrisj     (102) other        (1)     5766 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/tools/movies/namelist.py
--rwxr-xr-x   0 chrisj     (102) other        (1)     3431 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/tools/movies/show.py
--rwxr-xr-x   0 chrisj     (102) other        (1)     8688 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/tools/movies/timebuckets.py
--rw-r--r--   0 chrisj     (102) other        (1)     6459 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/tools/movies/validate.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.252079 medialibrary-0.2.1/src/media/validation/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.254396 medialibrary-0.2.1/src/media/validation/core/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/core/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     2042 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/core/faults.py
--rw-r--r--   0 chrisj     (102) other        (1)     1606 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/core/results.py
--rw-r--r--   0 chrisj     (102) other        (1)    13173 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/core/status.py
--rw-r--r--   0 chrisj     (102) other        (1)     1362 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/core/tests.py
--rw-r--r--   0 chrisj     (102) other        (1)     2280 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/core/validator.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.255184 medialibrary-0.2.1/src/media/validation/suites/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/suites/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     1740 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/suites/default.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.255559 medialibrary-0.2.1/src/media/validation/tests/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.256342 medialibrary-0.2.1/src/media/validation/tests/media/
--rw-r--r--   0 chrisj     (102) other        (1)     1169 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/media/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.257195 medialibrary-0.2.1/src/media/validation/tests/media/contents/
--rw-r--r--   0 chrisj     (102) other        (1)     1178 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/media/contents/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.258901 medialibrary-0.2.1/src/media/validation/tests/media/contents/generic/
--rw-r--r--   0 chrisj     (102) other        (1)     1169 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/media/contents/generic/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     4391 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/media/contents/generic/catalog.py
--rw-r--r--   0 chrisj     (102) other        (1)     1152 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/media/contents/generic/internal.py
--rw-r--r--   0 chrisj     (102) other        (1)     4873 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/media/contents/generic/story.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.259748 medialibrary-0.2.1/src/media/validation/tests/media/contents/genericv/
--rw-r--r--   0 chrisj     (102) other        (1)     1144 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/media/contents/genericv/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     4132 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/media/contents/genericv/technical.py
--rw-r--r--   0 chrisj     (102) other        (1)     1971 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/media/contents/internal.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.261036 medialibrary-0.2.1/src/media/validation/tests/media/contents/movie/
--rw-r--r--   0 chrisj     (102) other        (1)     1189 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/media/contents/movie/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     2573 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/media/contents/movie/internal.py
--rw-r--r--   0 chrisj     (102) other        (1)     3193 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/media/contents/movie/technical.py
--rw-r--r--   0 chrisj     (102) other        (1)     6910 2023-12-10 23:20:51.000000 medialibrary-0.2.1/src/media/validation/tests/media/internal.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.262557 medialibrary-0.2.1/src/media/xml/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/xml/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     1546 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/xml/functions.py
--rw-r--r--   0 chrisj     (102) other        (1)     1751 2023-03-16 00:41:46.000000 medialibrary-0.2.1/src/media/xml/namespaces.py
--rw-r--r--   0 chrisj     (102) other        (1)     2365 2022-11-30 03:32:25.000000 medialibrary-0.2.1/src/media/xml/parser.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-12-10 23:24:45.264402 medialibrary-0.2.1/src/medialibrary.egg-info/
--rw-r--r--   0 chrisj     (102) other        (1)     3293 2023-12-10 23:24:45.000000 medialibrary-0.2.1/src/medialibrary.egg-info/PKG-INFO
--rw-r--r--   0 chrisj     (102) other        (1)     3958 2023-12-10 23:24:45.000000 medialibrary-0.2.1/src/medialibrary.egg-info/SOURCES.txt
--rw-r--r--   0 chrisj     (102) other        (1)        1 2023-12-10 23:24:45.000000 medialibrary-0.2.1/src/medialibrary.egg-info/dependency_links.txt
--rw-r--r--   0 chrisj     (102) other        (1)        6 2023-12-10 23:24:45.000000 medialibrary-0.2.1/src/medialibrary.egg-info/top_level.txt
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.534866 medialibrary-0.2.3/
+-rw-r--r--   0 chrisj     (102) other        (1)     1071 2021-09-05 20:32:22.000000 medialibrary-0.2.3/LICENSE
+-rw-r--r--   0 chrisj     (102) other        (1)     3458 2024-04-17 01:06:30.534728 medialibrary-0.2.3/PKG-INFO
+-rw-r--r--   0 chrisj     (102) other        (1)     2388 2023-12-10 23:58:09.000000 medialibrary-0.2.3/README.md
+-rw-r--r--   0 chrisj     (102) other        (1)     1202 2024-04-17 01:00:34.000000 medialibrary-0.2.3/pyproject.toml
+-rw-r--r--   0 chrisj     (102) other        (1)      150 2024-04-17 01:06:30.535723 medialibrary-0.2.3/setup.cfg
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.414706 medialibrary-0.2.3/src/
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.428155 medialibrary-0.2.3/src/media/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.429299 medialibrary-0.2.3/src/media/data/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2182 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/dates.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.430074 medialibrary-0.2.3/src/media/data/media/
+-rw-r--r--   0 chrisj     (102) other        (1)     1259 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.430854 medialibrary-0.2.3/src/media/data/media/contents/
+-rw-r--r--   0 chrisj     (102) other        (1)     1203 2024-04-17 00:57:58.000000 medialibrary-0.2.3/src/media/data/media/contents/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.432073 medialibrary-0.2.3/src/media/data/media/contents/generic/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/contents/generic/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5671 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/contents/generic/catalog.py
+-rw-r--r--   0 chrisj     (102) other        (1)     8487 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/data/media/contents/generic/keywords.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.433340 medialibrary-0.2.3/src/media/data/media/contents/generic/story/
+-rw-r--r--   0 chrisj     (102) other        (1)     1172 2023-05-29 21:03:24.000000 medialibrary-0.2.3/src/media/data/media/contents/generic/story/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4319 2023-05-29 21:03:24.000000 medialibrary-0.2.3/src/media/data/media/contents/generic/story/characters.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2783 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/data/media/contents/generic/story/internal.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.434161 medialibrary-0.2.3/src/media/data/media/contents/genericv/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/contents/genericv/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.460372 medialibrary-0.2.3/src/media/data/media/contents/genericv/crew/
+-rw-r--r--   0 chrisj     (102) other        (1)     1198 2023-05-29 21:03:24.000000 medialibrary-0.2.3/src/media/data/media/contents/genericv/crew/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     8627 2023-05-29 21:03:24.000000 medialibrary-0.2.3/src/media/data/media/contents/genericv/crew/cast.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5667 2023-05-29 21:03:24.000000 medialibrary-0.2.3/src/media/data/media/contents/genericv/crew/internal.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3332 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/contents/genericv/technical.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2962 2024-04-17 00:57:58.000000 medialibrary-0.2.3/src/media/data/media/contents/internal.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.461684 medialibrary-0.2.3/src/media/data/media/contents/movie/
+-rw-r--r--   0 chrisj     (102) other        (1)     1171 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/contents/movie/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3810 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/contents/movie/classification.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4626 2024-04-17 00:57:58.000000 medialibrary-0.2.3/src/media/data/media/contents/movie/internal.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3863 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/data/media/internal.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.463359 medialibrary-0.2.3/src/media/data/media/library/
+-rw-r--r--   0 chrisj     (102) other        (1)     1259 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/library/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1853 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/library/filing.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5007 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/library/instances.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2070 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/library/internal.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.465835 medialibrary-0.2.3/src/media/data/media/medium/
+-rw-r--r--   0 chrisj     (102) other        (1)     1259 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/medium/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2498 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/medium/internal.py
+-rw-r--r--   0 chrisj     (102) other        (1)     8439 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/medium/inventory.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3590 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/medium/productid.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4650 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/medium/productspecs.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3318 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/data/media/medium/release.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.466649 medialibrary-0.2.3/src/media/data/media/meta/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/data/media/meta/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)    12864 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/data/media/meta/authorship.py
+-rw-r--r--   0 chrisj     (102) other        (1)     9141 2023-05-29 21:03:24.000000 medialibrary-0.2.3/src/media/data/nouns.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.468624 medialibrary-0.2.3/src/media/fileops/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/fileops/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1564 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/fileops/filenames.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2013 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/fileops/loader.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3282 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/fileops/repo.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2977 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/fileops/scanner.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.469013 medialibrary-0.2.3/src/media/fmt/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/fmt/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.470606 medialibrary-0.2.3/src/media/fmt/text/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/fmt/text/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4058 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/fmt/text/basics.py
+-rw-r--r--   0 chrisj     (102) other        (1)     8180 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/fmt/text/media.py
+-rw-r--r--   0 chrisj     (102) other        (1)     8922 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/fmt/text/movie.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.472167 medialibrary-0.2.3/src/media/generic/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/generic/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.472965 medialibrary-0.2.3/src/media/generic/compare/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-04-17 00:57:58.000000 medialibrary-0.2.3/src/media/generic/compare/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     7959 2024-04-17 00:57:58.000000 medialibrary-0.2.3/src/media/generic/compare/movie.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1313 2024-04-17 00:57:58.000000 medialibrary-0.2.3/src/media/generic/language.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.474162 medialibrary-0.2.3/src/media/generic/sorting/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/generic/sorting/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5470 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/generic/sorting/groups.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4307 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/generic/sorting/lists.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2255 2024-04-17 00:57:58.000000 medialibrary-0.2.3/src/media/generic/stringtools.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4570 2024-04-17 00:57:58.000000 medialibrary-0.2.3/src/media/generic/titletools.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.474955 medialibrary-0.2.3/src/media/tools/
+-rw-r--r--   0 chrisj     (102) other        (1)     1145 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/tools/__init__.py
+-rwxr-xr-x   0 chrisj     (102) other        (1)     1846 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/tools/common.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.477025 medialibrary-0.2.3/src/media/tools/media/
+-rw-r--r--   0 chrisj     (102) other        (1)     1150 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/tools/media/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2645 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/tools/media/authorrecords.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2433 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/tools/media/list.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2390 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/tools/media/show.py
+-rw-r--r--   0 chrisj     (102) other        (1)     7157 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/tools/media/validate.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.477829 medialibrary-0.2.3/src/media/tools/meta/
+-rw-r--r--   0 chrisj     (102) other        (1)     1149 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/tools/meta/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2291 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/tools/meta/authorship.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.482208 medialibrary-0.2.3/src/media/tools/movies/
+-rw-r--r--   0 chrisj     (102) other        (1)     1151 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/tools/movies/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     8026 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/tools/movies/castlist.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1791 2024-04-17 00:57:58.000000 medialibrary-0.2.3/src/media/tools/movies/compare.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3096 2023-12-30 00:58:47.000000 medialibrary-0.2.3/src/media/tools/movies/debuglist.py
+-rw-r--r--   0 chrisj     (102) other        (1)     9675 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/tools/movies/genrebreakdown.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4230 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/tools/movies/keywordlist.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3808 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/tools/movies/list.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5766 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/tools/movies/namelist.py
+-rwxr-xr-x   0 chrisj     (102) other        (1)     3431 2023-03-16 00:41:46.000000 medialibrary-0.2.3/src/media/tools/movies/show.py
+-rwxr-xr-x   0 chrisj     (102) other        (1)     8688 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/tools/movies/timebuckets.py
+-rw-r--r--   0 chrisj     (102) other        (1)     6459 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/tools/movies/validate.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.482603 medialibrary-0.2.3/src/media/validation/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.484966 medialibrary-0.2.3/src/media/validation/core/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/core/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2042 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/core/faults.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1606 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/core/results.py
+-rw-r--r--   0 chrisj     (102) other        (1)    13173 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/core/status.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1362 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/core/tests.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2280 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/core/validator.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.485779 medialibrary-0.2.3/src/media/validation/suites/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/suites/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1740 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/suites/default.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.507130 medialibrary-0.2.3/src/media/validation/tests/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.508430 medialibrary-0.2.3/src/media/validation/tests/media/
+-rw-r--r--   0 chrisj     (102) other        (1)     1169 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/media/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.509286 medialibrary-0.2.3/src/media/validation/tests/media/contents/
+-rw-r--r--   0 chrisj     (102) other        (1)     1178 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/media/contents/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.511038 medialibrary-0.2.3/src/media/validation/tests/media/contents/generic/
+-rw-r--r--   0 chrisj     (102) other        (1)     1169 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/media/contents/generic/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4391 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/media/contents/generic/catalog.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1152 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/media/contents/generic/internal.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4873 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/media/contents/generic/story.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.511922 medialibrary-0.2.3/src/media/validation/tests/media/contents/genericv/
+-rw-r--r--   0 chrisj     (102) other        (1)     1144 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/media/contents/genericv/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4132 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/media/contents/genericv/technical.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1971 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/media/contents/internal.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.528992 medialibrary-0.2.3/src/media/validation/tests/media/contents/movie/
+-rw-r--r--   0 chrisj     (102) other        (1)     1189 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/media/contents/movie/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2573 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/media/contents/movie/internal.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3193 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/media/contents/movie/technical.py
+-rw-r--r--   0 chrisj     (102) other        (1)     6910 2023-12-10 23:58:09.000000 medialibrary-0.2.3/src/media/validation/tests/media/internal.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.531329 medialibrary-0.2.3/src/media/xml/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/xml/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1546 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/xml/functions.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1863 2024-04-17 00:57:58.000000 medialibrary-0.2.3/src/media/xml/namespaces.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2365 2022-11-30 03:32:25.000000 medialibrary-0.2.3/src/media/xml/parser.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-17 01:06:30.534111 medialibrary-0.2.3/src/medialibrary.egg-info/
+-rw-r--r--   0 chrisj     (102) other        (1)     3458 2024-04-17 01:06:30.000000 medialibrary-0.2.3/src/medialibrary.egg-info/PKG-INFO
+-rw-r--r--   0 chrisj     (102) other        (1)     4169 2024-04-17 01:06:30.000000 medialibrary-0.2.3/src/medialibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisj     (102) other        (1)        1 2024-04-17 01:06:30.000000 medialibrary-0.2.3/src/medialibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisj     (102) other        (1)        6 2024-04-17 01:06:30.000000 medialibrary-0.2.3/src/medialibrary.egg-info/top_level.txt
```

### Comparing `medialibrary-0.2.1/LICENSE` & `medialibrary-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/PKG-INFO` & `medialibrary-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: medialibrary
-Version: 0.2.1
-Summary: Library for reading vtmedia XML files
+Version: 0.2.3
+Summary: Package for reading vtmedia XML files describing a movie/music media library
 Author-email: Chris J <cjcodeproj@fastmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/cjcodeproj/medialibrary
 Project-URL: bug tracker, https://github.com/cjcodeproj/medialibrary/issues
 Project-URL: repository, https://github.com/cjcodeproj/medialibrary
 Project-URL: changelog, https://github.com/cjcodeproj/medialibrary/blob/main/CHANGELOG.md
-Keywords: xml,movies,dvds
+Keywords: xml,movies,dvds,music
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: XML
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Video
 Requires-Python: >3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Media Library Reader
 
 The `medialibrary` module is a Python module for reading files containing entertainment media
```

### Comparing `medialibrary-0.2.1/README.md` & `medialibrary-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/pyproject.toml` & `medialibrary-0.2.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [project]
 name = "medialibrary"
-version = "0.2.1"
-description = "Library for reading vtmedia XML files"
+version = "0.2.3"
+description = "Package for reading vtmedia XML files describing a movie/music media library"
 readme = "README.md"
 requires-python = ">3.8"
 license = {text = "MIT License"}
-keywords = ["xml", "movies", "dvds"]
+keywords = ["xml", "movies", "dvds", "music"]
 authors = [
   {email = "cjcodeproj@fastmail.com", name = "Chris J"}
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
-  "Topic :: Text Processing :: Markup :: XML"
+  "Topic :: Text Processing :: Markup :: XML",
+  "Topic :: Multimedia",
+  "Topic :: Multimedia :: Sound/Audio",
+  "Topic :: Multimedia :: Video"
 ]
 
 [project.urls]
 homepage = "https://github.com/cjcodeproj/medialibrary"
 "bug tracker" = "https://github.com/cjcodeproj/medialibrary/issues"
 repository = "https://github.com/cjcodeproj/medialibrary"
 changelog = "https://github.com/cjcodeproj/medialibrary/blob/main/CHANGELOG.md"
```

### Comparing `medialibrary-0.2.1/src/media/__init__.py` & `medialibrary-0.2.3/src/media/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/__init__.py` & `medialibrary-0.2.3/src/media/data/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/dates.py` & `medialibrary-0.2.3/src/media/data/dates.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/__init__.py` & `medialibrary-0.2.3/src/media/data/media/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/__init__.py` & `medialibrary-0.2.3/src/media/data/media/contents/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/generic/__init__.py` & `medialibrary-0.2.3/src/media/data/media/contents/genericv/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/generic/catalog.py` & `medialibrary-0.2.3/src/media/data/media/contents/generic/catalog.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/generic/keywords.py` & `medialibrary-0.2.3/src/media/data/media/contents/generic/keywords.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/generic/story/__init__.py` & `medialibrary-0.2.3/src/media/data/media/contents/generic/story/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/generic/story/characters.py` & `medialibrary-0.2.3/src/media/data/media/contents/generic/story/characters.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/generic/story/internal.py` & `medialibrary-0.2.3/src/media/data/media/contents/generic/story/internal.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/genericv/__init__.py` & `medialibrary-0.2.3/src/media/fileops/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/genericv/crew/__init__.py` & `medialibrary-0.2.3/src/media/data/media/contents/genericv/crew/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/genericv/crew/cast.py` & `medialibrary-0.2.3/src/media/data/media/contents/genericv/crew/cast.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/genericv/crew/internal.py` & `medialibrary-0.2.3/src/media/data/media/contents/genericv/crew/internal.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/genericv/technical.py` & `medialibrary-0.2.3/src/media/data/media/contents/genericv/technical.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/movie/__init__.py` & `medialibrary-0.2.3/src/media/data/media/contents/movie/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/movie/classification.py` & `medialibrary-0.2.3/src/media/data/media/contents/movie/classification.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/contents/movie/internal.py` & `medialibrary-0.2.3/src/media/data/media/contents/movie/internal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 #
-# Copyright 2023 Chris Josephes
+# Copyright 2024 Chris Josephes
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -25,88 +25,51 @@
 '''Main module file for the Movie() and Title() objects'''
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=too-many-instance-attributes
 
 from datetime import timedelta
 from media.xml.namespaces import Namespaces
-from media.data.media.contents.generic.catalog import (
-        Title, TitleValueException, Catalog
-        )
+from media.data.media.contents import AbstractContent, ContentException
 from media.data.media.contents.generic.story import Story
 from media.data.media.contents.genericv.crew import Crew
 from media.data.media.contents.genericv.technical import Technical
 from media.data.media.contents.movie.classification import Classification
 from media.generic.sorting.lists import ContentIndex
 
 
-class Movie():
+class Movie(AbstractContent):
     '''Movie object'''
-    def __init__(self, in_chunk):
-        self.title = None
-        self.catalog = None
+    def __init__(self, in_element):
+        super().__init__()
         self.technical = None
         self.crew = None
-        self.sort_title = ""
-        self.unique_key = ""
-        self._process(in_chunk)
+        self._process(in_element)
 
     def build_index_object(self):
         """
         Build an index object to make grouping and
         sorting operations easier.
         """
         return MovieIndexEntry(self)
 
-    def _process(self, in_chunk):
-        for child in in_chunk:
-            if child.tag == Namespaces.nsf('movie') + 'title':
-                try:
-                    self.title = Title(child.text)
-                except TitleValueException as tve:
-                    raise MovieException(tve.message) from tve
-            if child.tag == Namespaces.nsf('movie') + 'catalog':
-                self.catalog = Catalog(child)
+    def _process(self, in_element):
+        super()._process(in_element)
+        for child in in_element:
             if child.tag == Namespaces.nsf('movie') + 'classification':
                 self.classification = Classification(child)
             if child.tag == Namespaces.nsf('movie') + 'technical':
                 self.technical = Technical(child)
             if child.tag == Namespaces.nsf('movie') + 'story':
                 self.story = Story(child)
             if child.tag == Namespaces.nsf('movie') + 'description':
                 self.story = Story(child)
             if child.tag == Namespaces.nsf('movie') + 'crew':
                 self.crew = Crew(child)
-        if self.title is not None:
-            self._build_unique_key()
-
-    def _build_unique_key(self):
-        ukv = None
-        cpy = None
-        if self.catalog is not None:
-            if self.catalog.alt_titles is not None:
-                if self.catalog.alt_titles.variant_sort is True:
-                    self.sort_title = \
-                            self.catalog.alt_titles.variant_title.sort_title
-                    self.unique_key = self.sort_title
-                else:
-                    self.sort_title = self.title.sort_title
-                    self.unique_key = self.sort_title
-            if self.catalog.copyright is not None:
-                cpy = str(self.catalog.copyright.year)
-            else:
-                cpy = "0000"
-            if self.catalog.unique_index is not None:
-                ukv = str(self.catalog.unique_index.index)
-            else:
-                ukv = "1"
-            self.unique_key += "-" + cpy + "-" + ukv
-        else:
-            self.sort_title = self.title.sort_title
-            self.unique_key = self.sort_title + "-0000-1"
+        self._post_load_process()
 
     def __hash__(self):
         return hash(self.unique_key)
 
     def __lt__(self, other):
         return self.unique_key < other.unique_key
 
@@ -153,15 +116,15 @@
                     self.runtime = tch.runtime.overall
         if not self.runtime:
             self.runtime = timedelta(seconds=0)
         self.sort_title = self.movie.sort_title
         self.first_letter = self.sort_title[0]
 
 
-class MovieException(Exception):
+class MovieException(ContentException):
     '''Exception raised when there is an issue with a movie.'''
     def __init__(self, message):
         super().__init__(message)
         self.message = message
 
     def __str__(self):
         return self.message
```

### Comparing `medialibrary-0.2.1/src/media/data/media/internal.py` & `medialibrary-0.2.3/src/media/data/media/internal.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/library/__init__.py` & `medialibrary-0.2.3/src/media/data/media/library/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/library/filing.py` & `medialibrary-0.2.3/src/media/data/media/library/filing.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/library/instances.py` & `medialibrary-0.2.3/src/media/data/media/library/instances.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/library/internal.py` & `medialibrary-0.2.3/src/media/data/media/library/internal.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/medium/__init__.py` & `medialibrary-0.2.3/src/media/data/media/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/medium/internal.py` & `medialibrary-0.2.3/src/media/data/media/medium/internal.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/medium/inventory.py` & `medialibrary-0.2.3/src/media/data/media/medium/inventory.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/medium/productid.py` & `medialibrary-0.2.3/src/media/data/media/medium/productid.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/medium/productspecs.py` & `medialibrary-0.2.3/src/media/data/media/medium/productspecs.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/medium/release.py` & `medialibrary-0.2.3/src/media/data/media/medium/release.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/meta/__init__.py` & `medialibrary-0.2.3/src/media/data/media/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/media/meta/authorship.py` & `medialibrary-0.2.3/src/media/data/media/meta/authorship.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/data/nouns.py` & `medialibrary-0.2.3/src/media/data/nouns.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/fileops/__init__.py` & `medialibrary-0.2.3/src/media/fmt/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/fileops/filenames.py` & `medialibrary-0.2.3/src/media/fileops/filenames.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/fileops/loader.py` & `medialibrary-0.2.3/src/media/fileops/loader.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/fileops/repo.py` & `medialibrary-0.2.3/src/media/fileops/repo.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/fileops/scanner.py` & `medialibrary-0.2.3/src/media/fileops/scanner.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/fmt/__init__.py` & `medialibrary-0.2.3/src/media/fmt/text/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/fmt/text/__init__.py` & `medialibrary-0.2.3/src/media/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/fmt/text/basics.py` & `medialibrary-0.2.3/src/media/fmt/text/basics.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/fmt/text/media.py` & `medialibrary-0.2.3/src/media/fmt/text/media.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/fmt/text/movie.py` & `medialibrary-0.2.3/src/media/fmt/text/movie.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/generic/__init__.py` & `medialibrary-0.2.3/src/media/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/generic/sorting/__init__.py` & `medialibrary-0.2.3/src/media/generic/compare/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/generic/sorting/groups.py` & `medialibrary-0.2.3/src/media/generic/sorting/groups.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/generic/sorting/lists.py` & `medialibrary-0.2.3/src/media/generic/sorting/lists.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/generic/stringtools.py` & `medialibrary-0.2.3/src/media/generic/stringtools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 #
-# Copyright 2022 Chris Josephes
+# Copyright 2024 Chris Josephes
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,17 +20,16 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 '''Common code related to sorting operations.'''
 
-# pylint: disable=too-few-public-methods
-
 import string
+from media.generic.language import LanguageHelpers
 
 
 def transform_string(in_value):
     '''Low level change to remove all punctuation from a string.'''
     if in_value is not None:
         no_punctuation = in_value.translate(
             in_value.maketrans("", "", string.punctuation))
@@ -53,12 +52,7 @@
     '''Build a string suitable for sorting, accounting for language rules.'''
     level1 = transform_string(in_value)
     word_split = level1.split()
     if word_split[0] in LanguageHelpers.Articles_English:
         article = word_split.pop(0)
         word_split.append('+'+article)
     return '_'.join(word_split)
-
-
-class LanguageHelpers():
-    '''Static data on languages.'''
-    Articles_English = ['a', 'an', 'the']
```

### Comparing `medialibrary-0.2.1/src/media/tools/__init__.py` & `medialibrary-0.2.3/src/media/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/common.py` & `medialibrary-0.2.3/src/media/tools/common.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/media/__init__.py` & `medialibrary-0.2.3/src/media/tools/media/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/media/authorrecords.py` & `medialibrary-0.2.3/src/media/tools/media/authorrecords.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/media/list.py` & `medialibrary-0.2.3/src/media/tools/media/list.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/media/show.py` & `medialibrary-0.2.3/src/media/tools/media/show.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/media/validate.py` & `medialibrary-0.2.3/src/media/tools/media/validate.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/meta/__init__.py` & `medialibrary-0.2.3/src/media/tools/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/meta/authorship.py` & `medialibrary-0.2.3/src/media/tools/meta/authorship.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/movies/__init__.py` & `medialibrary-0.2.3/src/media/tools/movies/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/movies/castlist.py` & `medialibrary-0.2.3/src/media/tools/movies/castlist.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/movies/debuglist.py` & `medialibrary-0.2.3/src/media/tools/movies/debuglist.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/movies/genrebreakdown.py` & `medialibrary-0.2.3/src/media/tools/movies/genrebreakdown.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/movies/keywordlist.py` & `medialibrary-0.2.3/src/media/tools/movies/keywordlist.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/movies/list.py` & `medialibrary-0.2.3/src/media/tools/movies/list.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/movies/namelist.py` & `medialibrary-0.2.3/src/media/tools/movies/namelist.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/movies/show.py` & `medialibrary-0.2.3/src/media/tools/movies/show.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/movies/timebuckets.py` & `medialibrary-0.2.3/src/media/tools/movies/timebuckets.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/tools/movies/validate.py` & `medialibrary-0.2.3/src/media/tools/movies/validate.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/__init__.py` & `medialibrary-0.2.3/src/media/generic/sorting/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/core/__init__.py` & `medialibrary-0.2.3/src/media/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/core/faults.py` & `medialibrary-0.2.3/src/media/validation/core/faults.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/core/results.py` & `medialibrary-0.2.3/src/media/validation/core/results.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/core/status.py` & `medialibrary-0.2.3/src/media/validation/core/status.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/core/tests.py` & `medialibrary-0.2.3/src/media/validation/core/tests.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/core/validator.py` & `medialibrary-0.2.3/src/media/validation/core/validator.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/suites/__init__.py` & `medialibrary-0.2.3/src/media/validation/core/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/suites/default.py` & `medialibrary-0.2.3/src/media/validation/suites/default.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/__init__.py` & `medialibrary-0.2.3/src/media/validation/suites/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/media/__init__.py` & `medialibrary-0.2.3/src/media/validation/tests/media/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/media/contents/__init__.py` & `medialibrary-0.2.3/src/media/validation/tests/media/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/media/contents/generic/__init__.py` & `medialibrary-0.2.3/src/media/validation/tests/media/contents/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/media/contents/generic/catalog.py` & `medialibrary-0.2.3/src/media/validation/tests/media/contents/generic/catalog.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/media/contents/generic/internal.py` & `medialibrary-0.2.3/src/media/validation/tests/media/contents/generic/internal.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/media/contents/generic/story.py` & `medialibrary-0.2.3/src/media/validation/tests/media/contents/generic/story.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/media/contents/genericv/__init__.py` & `medialibrary-0.2.3/src/media/validation/tests/media/contents/genericv/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/media/contents/genericv/technical.py` & `medialibrary-0.2.3/src/media/validation/tests/media/contents/genericv/technical.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/media/contents/internal.py` & `medialibrary-0.2.3/src/media/validation/tests/media/contents/internal.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/media/contents/movie/__init__.py` & `medialibrary-0.2.3/src/media/validation/tests/media/contents/movie/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/media/contents/movie/internal.py` & `medialibrary-0.2.3/src/media/validation/tests/media/contents/movie/internal.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/media/contents/movie/technical.py` & `medialibrary-0.2.3/src/media/validation/tests/media/contents/movie/technical.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/validation/tests/media/internal.py` & `medialibrary-0.2.3/src/media/validation/tests/media/internal.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/xml/__init__.py` & `medialibrary-0.2.3/src/media/validation/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 #
-# Copyright 2022 Chris Josephes
+# Copyright 2023 Chris Josephes
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `medialibrary-0.2.1/src/media/xml/functions.py` & `medialibrary-0.2.3/src/media/xml/functions.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/media/xml/namespaces.py` & `medialibrary-0.2.3/src/media/xml/namespaces.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 #
-# Copyright 2023 Chris Josephes
+# Copyright 2024 Chris Josephes
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -24,17 +24,19 @@
 
 '''XML Namespace Constants'''
 
 
 class Namespaces():
     '''Static data on XML Namespaces'''
     ns = {
-            "media": "http://vectortron.com/xml/media/media",
-            "movie": "http://vectortron.com/xml/media/movie",
-            "authorship": "http://vectortron.com/xml/media/meta/authorship"
+            'media': 'http://vectortron.com/xml/media/media',
+            'movie': 'http://vectortron.com/xml/media/movie',
+            'authorship': 'http://vectortron.com/xml/media/meta/authorship',
+            'xml': 'http://www.w3.org/XML/1998/namespace',
+            'xlink': 'http://www.w3.org/1999/xlink'
         }
 
     @classmethod
     def nsf(cls, in_tag):
         '''return the fully qualified namespace to the prefix format'''
         return '{' + Namespaces.ns[in_tag] + '}'
```

### Comparing `medialibrary-0.2.1/src/media/xml/parser.py` & `medialibrary-0.2.3/src/media/xml/parser.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.2.1/src/medialibrary.egg-info/PKG-INFO` & `medialibrary-0.2.3/src/medialibrary.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: medialibrary
-Version: 0.2.1
-Summary: Library for reading vtmedia XML files
+Version: 0.2.3
+Summary: Package for reading vtmedia XML files describing a movie/music media library
 Author-email: Chris J <cjcodeproj@fastmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/cjcodeproj/medialibrary
 Project-URL: bug tracker, https://github.com/cjcodeproj/medialibrary/issues
 Project-URL: repository, https://github.com/cjcodeproj/medialibrary
 Project-URL: changelog, https://github.com/cjcodeproj/medialibrary/blob/main/CHANGELOG.md
-Keywords: xml,movies,dvds
+Keywords: xml,movies,dvds,music
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: XML
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Video
 Requires-Python: >3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Media Library Reader
 
 The `medialibrary` module is a Python module for reading files containing entertainment media
```

### Comparing `medialibrary-0.2.1/src/medialibrary.egg-info/SOURCES.txt` & `medialibrary-0.2.3/src/medialibrary.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/media/__init__.py
 src/media/data/__init__.py
 src/media/data/dates.py
 src/media/data/nouns.py
 src/media/data/media/__init__.py
 src/media/data/media/internal.py
 src/media/data/media/contents/__init__.py
+src/media/data/media/contents/internal.py
 src/media/data/media/contents/generic/__init__.py
 src/media/data/media/contents/generic/catalog.py
 src/media/data/media/contents/generic/keywords.py
 src/media/data/media/contents/generic/story/__init__.py
 src/media/data/media/contents/generic/story/characters.py
 src/media/data/media/contents/generic/story/internal.py
 src/media/data/media/contents/genericv/__init__.py
@@ -42,29 +43,34 @@
 src/media/fileops/scanner.py
 src/media/fmt/__init__.py
 src/media/fmt/text/__init__.py
 src/media/fmt/text/basics.py
 src/media/fmt/text/media.py
 src/media/fmt/text/movie.py
 src/media/generic/__init__.py
+src/media/generic/language.py
 src/media/generic/stringtools.py
+src/media/generic/titletools.py
+src/media/generic/compare/__init__.py
+src/media/generic/compare/movie.py
 src/media/generic/sorting/__init__.py
 src/media/generic/sorting/groups.py
 src/media/generic/sorting/lists.py
 src/media/tools/__init__.py
 src/media/tools/common.py
 src/media/tools/media/__init__.py
 src/media/tools/media/authorrecords.py
 src/media/tools/media/list.py
 src/media/tools/media/show.py
 src/media/tools/media/validate.py
 src/media/tools/meta/__init__.py
 src/media/tools/meta/authorship.py
 src/media/tools/movies/__init__.py
 src/media/tools/movies/castlist.py
+src/media/tools/movies/compare.py
 src/media/tools/movies/debuglist.py
 src/media/tools/movies/genrebreakdown.py
 src/media/tools/movies/keywordlist.py
 src/media/tools/movies/list.py
 src/media/tools/movies/namelist.py
 src/media/tools/movies/show.py
 src/media/tools/movies/timebuckets.py
```

