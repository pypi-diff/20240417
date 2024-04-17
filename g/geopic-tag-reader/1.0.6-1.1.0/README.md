# Comparing `tmp/geopic_tag_reader-1.0.6.tar.gz` & `tmp/geopic_tag_reader-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopic_tag_reader-1.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geopic_tag_reader-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geopic_tag_reader-1.0.6.tar` & `geopic_tag_reader-1.1.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0       56 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/.gitignore
--rw-r--r--   0        0        0     1009 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/.gitlab-ci.yml
--rw-r--r--   0        0        0       91 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6218 2024-04-02 12:42:42.379304 geopic_tag_reader-1.0.6/CHANGELOG.md
--rw-r--r--   0        0        0     5468 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1070 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/LICENSE
--rw-r--r--   0        0        0      676 2024-04-02 11:56:01.308379 geopic_tag_reader-1.0.6/Makefile
--rw-r--r--   0        0        0     5243 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/README.md
--rw-r--r--   0        0        0       65 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/docs/.pages
--rw-r--r--   0        0        0     3410 2024-04-02 11:56:01.308379 geopic_tag_reader-1.0.6/docs/API_USAGE.md
--rw-r--r--   0        0        0     1835 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/docs/CLI_USAGE.md
--rw-r--r--   0        0        0      999 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/docs/Develop.md
--rw-r--r--   0        0        0     2015 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/docs/Install.md
--rw-r--r--   0        0        0     1066 2024-03-06 15:09:24.623622 geopic_tag_reader-1.0.6/docs/camera.md
--rw-r--r--   0        0        0      543 2024-04-02 11:56:01.308379 geopic_tag_reader-1.0.6/docs/model.md
--rw-r--r--   0        0        0     8772 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/docs/reader.md
--rw-r--r--   0        0        0     4301 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/docs/writer.md
--rw-r--r--   0        0        0       47 2024-04-02 12:42:42.379304 geopic_tag_reader-1.0.6/geopic_tag_reader/__init__.py
--rw-r--r--   0        0        0     1643 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/geopic_tag_reader/camera.py
--rw-r--r--   0        0        0     3129 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/geopic_tag_reader/main.py
--rw-r--r--   0        0        0      129 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/geopic_tag_reader/model.py
--rw-r--r--   0        0        0        0 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/geopic_tag_reader/py.typed
--rw-r--r--   0        0        0    21325 2024-03-06 15:06:48.384484 geopic_tag_reader-1.0.6/geopic_tag_reader/reader.py
--rw-r--r--   0        0        0     8680 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/geopic_tag_reader/writer.py
--rw-r--r--   0        0        0     1142 2024-04-02 11:56:01.308379 geopic_tag_reader-1.0.6/pyproject.toml
--rw-r--r--   0        0        0       37 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/pytest.ini
--rw-r--r--   0        0        0        0 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/tests/__init__.py
--rw-r--r--   0        0        0      195 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/tests/conftest.py
--rw-r--r--   0        0        0    79729 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/tests/fixtures/1.jpg
--rw-r--r--   0        0        0    24664 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/IMG_20210720_144918.jpg
--rw-r--r--   0        0        0    38766 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/IMG_20210720_161352.jpg
--rw-r--r--   0        0        0    75709 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/a1.jpg
--rw-r--r--   0        0        0    29130 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/b1.jpg
--rw-r--r--   0        0        0    39810 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/broken_makernotes.jpg
--rw-r--r--   0        0        0    69903 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/c1.jpg
--rw-r--r--   0        0        0    30503 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/cropped.jpg
--rw-r--r--   0        0        0    33446 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/d1.jpg
--rw-r--r--   0        0        0     5415 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/datetime_ms_float.jpg
--rw-r--r--   0        0        0    35109 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/datetime_offset.jpg
--rw-r--r--   0        0        0    51474 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/e1.jpg
--rw-r--r--   0        0        0    29141 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/flat.jpg
--rw-r--r--   0        0        0    70264 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/gopromax_flat.jpg
--rw-r--r--   0        0        0     4174 2024-03-06 15:06:48.384484 geopic_tag_reader-1.0.6/tests/fixtures/gps_date_slash.jpg
--rw-r--r--   0        0        0     5237 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/gps_date_time_stamp.jpg
--rw-r--r--   0        0        0    66264 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_Ricoh_Theta.jpg
--rw-r--r--   0        0        0     5360 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_V4MPack.jpg
--rw-r--r--   0        0        0    66961 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_categorisee.jpg
--rw-r--r--   0        0        0   135574 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_datetimeoriginal.jpg
--rw-r--r--   0        0        0    29503 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_gps_date_string.jpg
--rw-r--r--   0        0        0    35282 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_gps_datestamp.jpg
--rw-r--r--   0        0        0    43696 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_gps_sotm.jpg
--rw-r--r--   0        0        0    33170 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/img_invalid_gps_date.jpg
--rw-r--r--   0        0        0    34454 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/img_without_coord.jpg
--rw-r--r--   0        0        0    34518 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/img_without_dt.jpg
--rw-r--r--   0        0        0    12643 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/img_without_exif_tags.jpg
--rw-r--r--   0        0        0    11646 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/insta360_date.jpg
--rw-r--r--   0        0        0    55140 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/int_long_tag.jpg
--rw-r--r--   0        0        0    39169 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/out_of_bounds_lat.jpg
--rw-r--r--   0        0        0    39169 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/out_of_bounds_lon.jpg
--rw-r--r--   0        0        0     9665 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/pic_with_float_lat.jpg
--rw-r--r--   0        0        0     3130 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/ricoh_theta_no_projection.jpg
--rw-r--r--   0        0        0      612 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/test_main.py
--rw-r--r--   0        0        0    21456 2024-04-02 11:56:01.308379 geopic_tag_reader-1.0.6/tests/test_reader.py
--rw-r--r--   0        0        0    11476 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/test_writer.py
--rw-r--r--   0        0        0     6375 1970-01-01 00:00:00.000000 geopic_tag_reader-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0       56 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1009 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0       91 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6697 2024-04-17 06:35:08.457091 geopic_tag_reader-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5468 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1070 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/LICENSE
+-rw-r--r--   0        0        0      676 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/Makefile
+-rw-r--r--   0        0        0     5243 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/README.md
+-rw-r--r--   0        0        0       65 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/docs/.pages
+-rw-r--r--   0        0        0     3393 2024-04-15 10:48:00.708002 geopic_tag_reader-1.1.0/docs/API_USAGE.md
+-rw-r--r--   0        0        0     1835 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/docs/CLI_USAGE.md
+-rw-r--r--   0        0        0      999 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/docs/Develop.md
+-rw-r--r--   0        0        0     2015 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/docs/Install.md
+-rw-r--r--   0        0        0     1066 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/docs/camera.md
+-rw-r--r--   0        0        0      529 2024-04-15 10:48:00.708002 geopic_tag_reader-1.1.0/docs/model.md
+-rw-r--r--   0        0        0     8930 2024-04-16 10:04:34.508732 geopic_tag_reader-1.1.0/docs/reader.md
+-rw-r--r--   0        0        0     4301 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/docs/writer.md
+-rw-r--r--   0        0        0       47 2024-04-17 06:35:08.457091 geopic_tag_reader-1.1.0/geopic_tag_reader/__init__.py
+-rw-r--r--   0        0        0     1643 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/geopic_tag_reader/camera.py
+-rw-r--r--   0        0        0     3141 2024-04-16 10:04:34.508732 geopic_tag_reader-1.1.0/geopic_tag_reader/main.py
+-rw-r--r--   0        0        0      129 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/geopic_tag_reader/model.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/geopic_tag_reader/py.typed
+-rw-r--r--   0        0        0    22867 2024-04-16 10:04:34.508732 geopic_tag_reader-1.1.0/geopic_tag_reader/reader.py
+-rw-r--r--   0        0        0     8672 2024-04-15 10:48:00.708002 geopic_tag_reader-1.1.0/geopic_tag_reader/writer.py
+-rw-r--r--   0        0        0     1142 2024-04-15 10:48:00.708002 geopic_tag_reader-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/pytest.ini
+-rw-r--r--   0        0        0        0 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0    79729 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/tests/fixtures/1.jpg
+-rw-r--r--   0        0        0    24664 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/tests/fixtures/IMG_20210720_144918.jpg
+-rw-r--r--   0        0        0    38766 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/tests/fixtures/IMG_20210720_161352.jpg
+-rw-r--r--   0        0        0    75709 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/tests/fixtures/a1.jpg
+-rw-r--r--   0        0        0    29130 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/b1.jpg
+-rw-r--r--   0        0        0    39810 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/broken_makernotes.jpg
+-rw-r--r--   0        0        0    69903 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/c1.jpg
+-rw-r--r--   0        0        0     4867 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/charset.jpg
+-rw-r--r--   0        0        0    30503 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/cropped.jpg
+-rw-r--r--   0        0        0    33446 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/d1.jpg
+-rw-r--r--   0        0        0     5415 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/datetime_ms_float.jpg
+-rw-r--r--   0        0        0    35109 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/datetime_offset.jpg
+-rw-r--r--   0        0        0    51474 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/e1.jpg
+-rw-r--r--   0        0        0    29141 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/flat.jpg
+-rw-r--r--   0        0        0    70264 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/gopromax_flat.jpg
+-rw-r--r--   0        0        0     4174 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/gps_date_slash.jpg
+-rw-r--r--   0        0        0     5237 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/gps_date_time_stamp.jpg
+-rw-r--r--   0        0        0    66264 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/img_Ricoh_Theta.jpg
+-rw-r--r--   0        0        0     5360 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/img_V4MPack.jpg
+-rw-r--r--   0        0        0    66961 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/img_categorisee.jpg
+-rw-r--r--   0        0        0   135574 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/img_datetimeoriginal.jpg
+-rw-r--r--   0        0        0    29503 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/img_gps_date_string.jpg
+-rw-r--r--   0        0        0    35282 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/img_gps_datestamp.jpg
+-rw-r--r--   0        0        0    43696 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/img_gps_sotm.jpg
+-rw-r--r--   0        0        0    33170 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/img_invalid_gps_date.jpg
+-rw-r--r--   0        0        0    34454 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/img_without_coord.jpg
+-rw-r--r--   0        0        0    34518 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/img_without_dt.jpg
+-rw-r--r--   0        0        0    12643 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/img_without_exif_tags.jpg
+-rw-r--r--   0        0        0    11646 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/insta360_date.jpg
+-rw-r--r--   0        0        0    55140 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/int_long_tag.jpg
+-rw-r--r--   0        0        0    39169 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/out_of_bounds_lat.jpg
+-rw-r--r--   0        0        0    39169 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/out_of_bounds_lon.jpg
+-rw-r--r--   0        0        0     9665 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/pic_with_float_lat.jpg
+-rw-r--r--   0        0        0     3130 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/ricoh_theta_no_projection.jpg
+-rw-r--r--   0        0        0      612 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/test_main.py
+-rw-r--r--   0        0        0    22277 2024-04-16 10:04:34.508732 geopic_tag_reader-1.1.0/tests/test_reader.py
+-rw-r--r--   0        0        0    11365 2024-04-16 10:04:34.508732 geopic_tag_reader-1.1.0/tests/test_writer.py
+-rw-r--r--   0        0        0     6303 1970-01-01 00:00:00.000000 geopic_tag_reader-1.1.0/PKG-INFO
```

### Comparing `geopic_tag_reader-1.0.6/.gitlab-ci.yml` & `geopic_tag_reader-1.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/CHANGELOG.md` & `geopic_tag_reader-1.1.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.1.0] - 2024-04-17
+
+### Changed
+
+- Encoding information (`charset=...`) is now stripped out of text EXIF tags.
+- `GeoPicTags` objects returns `ts` as a Python `datetime` object (instead of decimal epoch).
+- Improved timezone handling in reader, GPS coordinates are used to find appropriate timezone when no timezone is defined in EXIF tags. If a UTC fallback is done, a warning is thrown.
+
 ## [1.0.6] - 2024-04-02
 
 ### Changed
 
 - Bump some dependencies, the most important one being [typer](https://typer.tiangolo.com/) since it removes the need for typer-cli.
 
 ## [1.0.5] - 2024-03-06
@@ -148,15 +156,16 @@
 
 ## [0.0.1] - 2023-03-31
 
 ### Added
 
 - EXIF tag reading methods extracted from [GeoVisio API](https://gitlab.com/geovisio/api)
 
-[Unreleased]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.6...main
+[Unreleased]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.1.0...main
+[1.1.0]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.6...1.1.0
 [1.0.6]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.5...1.0.6
 [1.0.5]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.4...1.0.5
 [1.0.4]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.3...1.0.4
 [1.0.3]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.2...1.0.3
 [1.0.2]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.1...1.0.2
 [1.0.1]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.0...1.0.1
 [1.0.0]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/0.4.1...1.0.0
```

### Comparing `geopic_tag_reader-1.0.6/CODE_OF_CONDUCT.md` & `geopic_tag_reader-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/LICENSE` & `geopic_tag_reader-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/Makefile` & `geopic_tag_reader-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/README.md` & `geopic_tag_reader-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/docs/API_USAGE.md` & `geopic_tag_reader-1.1.0/docs/API_USAGE.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - [`camera`](./camera.md#module-camera)
 - [`model`](./model.md#module-model)
 - [`reader`](./reader.md#module-reader)
 - [`writer`](./writer.md#module-writer)
 
 ## Classes
 
-- [`model.PictureType`](./model.md#class-picturetype): An enumeration.
+- [`model.PictureType`](./model.md#class-picturetype)
 - [`reader.CropValues`](./reader.md#class-cropvalues): Cropped equirectangular pictures metadata
 - [`reader.GeoPicTags`](./reader.md#class-geopictags): Tags associated to a geolocated picture
 - [`reader.InvalidExifException`](./reader.md#class-invalidexifexception): Exception for invalid EXIF information from image
 - [`reader.PartialExifException`](./reader.md#class-partialexifexception): Exception for partial / missing EXIF information from image
 - [`reader.PartialGeoPicTags`](./reader.md#class-partialgeopictags): Tags associated to a geolocated picture when not all tags have been found
 - [`writer.Direction`](./writer.md#class-direction): Direction(value: float, ref: writer.DirectionRef = <DirectionRef.true_north: 'T'>)
 - [`writer.DirectionRef`](./writer.md#class-directionref): Indicates the reference for giving the direction of the image when it is captured.
```

### Comparing `geopic_tag_reader-1.0.6/docs/CLI_USAGE.md` & `geopic_tag_reader-1.1.0/docs/CLI_USAGE.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/docs/Develop.md` & `geopic_tag_reader-1.1.0/docs/Develop.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/docs/Install.md` & `geopic_tag_reader-1.1.0/docs/Install.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/docs/camera.md` & `geopic_tag_reader-1.1.0/docs/camera.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/docs/reader.md` & `geopic_tag_reader-1.1.0/docs/reader.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L114"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L118"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `readPictureMetadata`
 
 ```python
 readPictureMetadata(picture: bytes) → GeoPicTags
 ```
 
@@ -31,56 +31,56 @@
 **Returns:**
  
  - <b>`GeoPicTags`</b>:  Extracted metadata from picture 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L346"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L355"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeMakeModel`
 
 ```python
 decodeMakeModel(value) → str
 ```
 
 Python 2/3 compatible decoding of make/model field. 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L357"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L366"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `isValidManyFractions`
 
 ```python
 isValidManyFractions(value: str) → bool
 ```
 
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L364"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L373"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeManyFractions`
 
 ```python
 decodeManyFractions(value: str) → List[Fraction]
 ```
 
 Try to decode a list of fractions, separated by spaces 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L377"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L386"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeLatLon`
 
 ```python
 decodeLatLon(
     data: dict,
     group: str
@@ -88,63 +88,70 @@
 ```
 
 Reads GPS info from given group to get latitude/longitude as float coordinates 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L432"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L441"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeDateTimeOriginal`
 
 ```python
 decodeDateTimeOriginal(
     data: dict,
-    datetimeField: str
+    datetimeField: str,
+    lat: Optional[float] = None,
+    lon: Optional[float] = None
 ) → Tuple[Optional[datetime], List[str]]
 ```
 
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L464"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L495"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeTimeOffset`
 
 ```python
 decodeTimeOffset(data: dict, offsetTimeField: str) → Optional[tzinfo]
 ```
 
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L470"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L501"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeGPSDateTime`
 
 ```python
-decodeGPSDateTime(data: dict, group: str) → Tuple[Optional[datetime], List[str]]
+decodeGPSDateTime(
+    data: dict,
+    group: str,
+    lat: Optional[float] = None,
+    lon: Optional[float] = None
+) → Tuple[Optional[datetime], List[str]]
 ```
 
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L513"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L552"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeSecondsAndMicroSeconds`
 
 ```python
 decodeSecondsAndMicroSeconds(
     secondsRaw: str,
     microsecondsRaw: str
@@ -154,15 +161,15 @@
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L539"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L578"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `isExifTagUsable`
 
 ```python
 isExifTagUsable(exif, tag, expectedType: Any = <class 'str'>) → bool
 ```
 
@@ -181,15 +188,15 @@
 **Returns:**
  
  - <b>`bool`</b>:  True if not empty 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L16"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L20"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CropValues`
 Cropped equirectangular pictures metadata 
 
 
 
 **Attributes:**
@@ -222,26 +229,26 @@
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L37"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L41"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `GeoPicTags`
 Tags associated to a geolocated picture 
 
 
 
 **Attributes:**
  
  - <b>`lat`</b> (float):  GPS Latitude (in WGS84) 
  - <b>`lon`</b> (float):  GPS Longitude (in WGS84) 
- - <b>`ts`</b> (float):  The capture date (as POSIX timestamp) 
+ - <b>`ts`</b> (datetime):  The capture date (date & time with timezone) 
  - <b>`heading`</b> (int):  Picture heading (in degrees, North = 0°, East = 90°, South = 180°, West = 270°) 
  - <b>`type`</b> (str):  The kind of picture (flat, equirectangular) 
  - <b>`make`</b> (str):  The camera manufacturer name 
  - <b>`model`</b> (str):  The camera model name 
  - <b>`focal_length`</b> (float):  The camera focal length (in mm) 
  - <b>`crop`</b> (CropValues):  The picture cropped area metadata (optional) 
  - <b>`exif`</b> (dict[str, str]):  Raw EXIF tags from picture (following Exiv2 naming scheme, see https://exiv2.org/metadata.html) 
@@ -256,15 +263,15 @@
 
 ### <kbd>method</kbd> `__init__`
 
 ```python
 __init__(
     lat: float,
     lon: float,
-    ts: float,
+    ts: datetime,
     heading: Optional[int],
     type: str,
     make: Optional[str],
     model: Optional[str],
     focal_length: Optional[float],
     crop: Optional[CropValues],
     exif: Dict[str, str] = <factory>,
@@ -279,20 +286,20 @@
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L73"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L77"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `InvalidExifException`
 Exception for invalid EXIF information from image 
 
-<a href="../geopic_tag_reader/reader.py#L76"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L80"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `__init__`
 
 ```python
 __init__(msg)
 ```
 
@@ -302,30 +309,30 @@
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L80"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L84"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PartialGeoPicTags`
 Tags associated to a geolocated picture when not all tags have been found 
 
 Implementation note: this needs to be sync with the GeoPicTags structure 
 
 <a href="../<string>"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `__init__`
 
 ```python
 __init__(
     lat: Optional[float] = None,
     lon: Optional[float] = None,
-    ts: Optional[float] = None,
+    ts: Optional[datetime] = None,
     heading: Optional[int] = None,
     type: Optional[str] = None,
     make: Optional[str] = None,
     model: Optional[str] = None,
     focal_length: Optional[float] = None,
     crop: Optional[CropValues] = None,
     exif: Dict[str, str] = <factory>,
@@ -340,22 +347,22 @@
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L101"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L105"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PartialExifException`
 Exception for partial / missing EXIF information from image 
 
 Contains a PartialGeoPicTags with all tags that have been read and the list of missing tags 
 
-<a href="../geopic_tag_reader/reader.py#L108"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L112"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `__init__`
 
 ```python
 __init__(msg, missing_mandatory_tags: Set[str], partial_tags: PartialGeoPicTags)
 ```
```

#### html2text {}

```diff
@@ -12,68 +12,70 @@
 ```python decodeManyFractions(value: str) â List[Fraction] ``` Try to decode
 a list of fractions, separated by spaces --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
 _s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## function `decodeLatLon` ```python
 decodeLatLon( data: dict, group: str ) â Tuple[Optional[float], Optional
 [float], List[str]] ``` Reads GPS info from given group to get latitude/
 longitude as float coordinates --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
 _c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## function `decodeDateTimeOriginal` ```python
-decodeDateTimeOriginal( data: dict, datetimeField: str ) â Tuple[Optional
-[datetime], List[str]] ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## function `decodeTimeOffset` ```python
-decodeTimeOffset(data: dict, offsetTimeField: str) â Optional[tzinfo] ``` --
+decodeDateTimeOriginal( data: dict, datetimeField: str, lat: Optional[float] =
+None, lon: Optional[float] = None ) â Tuple[Optional[datetime], List[str]]
+``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]##
+function `decodeTimeOffset` ```python decodeTimeOffset(data: dict,
+offsetTimeField: str) â Optional[tzinfo] ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## function `decodeGPSDateTime`
+```python decodeGPSDateTime( data: dict, group: str, lat: Optional[float] =
+None, lon: Optional[float] = None ) â Tuple[Optional[datetime], List[str]]
+``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]##
+function `decodeSecondsAndMicroSeconds` ```python decodeSecondsAndMicroSeconds
+( secondsRaw: str, microsecondsRaw: str ) â Tuple[int, int, List[str]] ``` --
 - _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## function
-`decodeGPSDateTime` ```python decodeGPSDateTime(data: dict, group: str) â
-Tuple[Optional[datetime], List[str]] ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## function `decodeSecondsAndMicroSeconds`
-```python decodeSecondsAndMicroSeconds( secondsRaw: str, microsecondsRaw: str )
-â Tuple[int, int, List[str]] ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## function `isExifTagUsable` ```python
-isExifTagUsable(exif, tag, expectedType: Any =
+`isExifTagUsable` ```python isExifTagUsable(exif, tag, expectedType: Any =
 str'>) â bool ``` Is a given EXIF tag usable (not null and not an empty
 string) **Args:** - ``eexxiiff`` (dict): The EXIF tags - ``ttaagg`` (str): The tag to
 check - ``eexxppeecctteeddTTyyppee`` (class): The expected data type **Returns:** - ``bbooooll``:
 True if not empty --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_]## class `CropValues` Cropped equirectangular pictures metadata
 **Attributes:** - ``ffuullllWWiiddtthh`` (int): Full panorama width - ``ffuullllHHeeiigghhtt`` (int):
 Full panorama height - ``wwiiddtthh`` (int): Cropped area width - ``hheeiigghhtt`` (int):
 Cropped area height - ``lleefftt`` (int): Cropped area left offset - ``ttoopp`` (int):
 Cropped area top offset _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
 _c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `__init__` ```python __init__( fullWidth:
 int, fullHeight: int, width: int, height: int, left: int, top: int ) â None
 ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class
 `GeoPicTags` Tags associated to a geolocated picture **Attributes:** - ``llaatt``
 (float): GPS Latitude (in WGS84) - ``lloonn`` (float): GPS Longitude (in WGS84) -
-``ttss`` (float): The capture date (as POSIX timestamp) - ``hheeaaddiinngg`` (int): Picture
-heading (in degrees, North = 0Â°, East = 90Â°, South = 180Â°, West = 270Â°) -
-``ttyyppee`` (str): The kind of picture (flat, equirectangular) - ``mmaakkee`` (str): The
-camera manufacturer name - ``mmooddeell`` (str): The camera model name -
-``ffooccaall__lleennggtthh`` (float): The camera focal length (in mm) - ``ccrroopp`` (CropValues):
-The picture cropped area metadata (optional) - ``eexxiiff`` (dict[str, str]): Raw
-EXIF tags from picture (following Exiv2 naming scheme, see https://exiv2.org/
-metadata.html) - ``ttaaggrreeaaddeerr__wwaarrnniinnggss`` (list[str]): List of thrown warnings
-during metadata reading - ``aallttiittuuddee`` (float): altitude (in m) (optional)
-Implementation note: this needs to be sync with the PartialGeoPicTags structure
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`__init__` ```python __init__( lat: float, lon: float, ts: float, heading:
-Optional[int], type: str, make: Optional[str], model: Optional[str],
-focal_length: Optional[float], crop: Optional[CropValues], exif: Dict[str, str]
-= , tagreader_warnings: List[str] = , altitude: Optional[float] = None ) â
-None ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]##
-class `InvalidExifException` Exception for invalid EXIF information from image
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`__init__` ```python __init__(msg) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `PartialGeoPicTags` Tags associated to
-a geolocated picture when not all tags have been found Implementation note:
-this needs to be sync with the GeoPicTags structure _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+``ttss`` (datetime): The capture date (date & time with timezone) - ``hheeaaddiinngg``
+(int): Picture heading (in degrees, North = 0Â°, East = 90Â°, South = 180Â°,
+West = 270Â°) - ``ttyyppee`` (str): The kind of picture (flat, equirectangular) -
+``mmaakkee`` (str): The camera manufacturer name - ``mmooddeell`` (str): The camera model
+name - ``ffooccaall__lleennggtthh`` (float): The camera focal length (in mm) - ``ccrroopp``
+(CropValues): The picture cropped area metadata (optional) - ``eexxiiff`` (dict[str,
+str]): Raw EXIF tags from picture (following Exiv2 naming scheme, see https://
+exiv2.org/metadata.html) - ``ttaaggrreeaaddeerr__wwaarrnniinnggss`` (list[str]): List of thrown
+warnings during metadata reading - ``aallttiittuuddee`` (float): altitude (in m)
+(optional) Implementation note: this needs to be sync with the
+PartialGeoPicTags structure _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `__init__` ```python __init__( lat: float,
+lon: float, ts: datetime, heading: Optional[int], type: str, make: Optional
+[str], model: Optional[str], focal_length: Optional[float], crop: Optional
+[CropValues], exif: Dict[str, str] = , tagreader_warnings: List[str] = ,
+altitude: Optional[float] = None ) â None ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `InvalidExifException`
+Exception for invalid EXIF information from image _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `__init__` ```python __init__
-( lat: Optional[float] = None, lon: Optional[float] = None, ts: Optional[float]
-= None, heading: Optional[int] = None, type: Optional[str] = None, make:
-Optional[str] = None, model: Optional[str] = None, focal_length: Optional
-[float] = None, crop: Optional[CropValues] = None, exif: Dict[str, str] = ,
-tagreader_warnings: List[str] = , altitude: Optional[float] = None ) â None
-``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class
-`PartialExifException` Exception for partial / missing EXIF information from
-image Contains a PartialGeoPicTags with all tags that have been read and the
-list of missing tags _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]### method `__init__` ```python __init__(msg, missing_mandatory_tags:
-Set[str], partial_tags: PartialGeoPicTags) ``` --- _This file was automatically
-generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
+(msg) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]##
+class `PartialGeoPicTags` Tags associated to a geolocated picture when not all
+tags have been found Implementation note: this needs to be sync with the
+GeoPicTags structure _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]### method `__init__` ```python __init__( lat: Optional[float] = None,
+lon: Optional[float] = None, ts: Optional[datetime] = None, heading: Optional
+[int] = None, type: Optional[str] = None, make: Optional[str] = None, model:
+Optional[str] = None, focal_length: Optional[float] = None, crop: Optional
+[CropValues] = None, exif: Dict[str, str] = , tagreader_warnings: List[str] = ,
+altitude: Optional[float] = None ) â None ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `PartialExifException`
+Exception for partial / missing EXIF information from image Contains a
+PartialGeoPicTags with all tags that have been read and the list of missing
+tags _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`__init__` ```python __init__(msg, missing_mandatory_tags: Set[str],
+partial_tags: PartialGeoPicTags) ``` --- _This file was automatically generated
+via [lazydocs](https://github.com/ml-tooling/lazydocs)._
```

### Comparing `geopic_tag_reader-1.0.6/docs/writer.md` & `geopic_tag_reader-1.1.0/docs/writer.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/geopic_tag_reader/camera.py` & `geopic_tag_reader-1.1.0/geopic_tag_reader/camera.py`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/geopic_tag_reader/main.py` & `geopic_tag_reader-1.1.0/geopic_tag_reader/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     with open(image, "rb") as img:
         pyexiv2.set_log_level(4 if ignore_exiv2_errors else 2)
 
         metadata = reader.readPictureMetadata(img.read())
 
         print("Latitude:", metadata.lat)
         print("Longitude:", metadata.lon)
-        print("Timestamp:", metadata.ts)
+        print("Timestamp:", metadata.ts.isoformat())
         print("Heading:", metadata.heading)
         print("Type:", metadata.type)
         print("Make:", metadata.make)
         print("Model:", metadata.model)
         print("Focal length:", metadata.focal_length)
         print("Crop parameters:", metadata.crop)
```

### Comparing `geopic_tag_reader-1.0.6/geopic_tag_reader/reader.py` & `geopic_tag_reader-1.1.0/geopic_tag_reader/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,23 @@
 import datetime
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional, Any, Set, Tuple
 import re
 import json
 from fractions import Fraction
 from geopic_tag_reader import camera
+import timezonefinder  # type: ignore
+import pytz
 
 # This is a fix for invalid MakerNotes leading to picture not read at all
 # https://github.com/LeoHsiao1/pyexiv2/issues/58
 pyexiv2.set_log_level(4)
 
+tz_finder = timezonefinder.TimezoneFinder()
+
 
 @dataclass
 class CropValues:
     """Cropped equirectangular pictures metadata
 
     Attributes:
         fullWidth (int): Full panorama width
@@ -37,15 +41,15 @@
 @dataclass
 class GeoPicTags:
     """Tags associated to a geolocated picture
 
     Attributes:
         lat (float): GPS Latitude (in WGS84)
         lon (float): GPS Longitude (in WGS84)
-        ts (float): The capture date (as POSIX timestamp)
+        ts (datetime): The capture date (date & time with timezone)
         heading (int): Picture heading (in degrees, North = 0°, East = 90°, South = 180°, West = 270°)
         type (str): The kind of picture (flat, equirectangular)
         make (str): The camera manufacturer name
         model (str): The camera model name
         focal_length (float): The camera focal length (in mm)
         crop (CropValues): The picture cropped area metadata (optional)
         exif (dict[str, str]): Raw EXIF tags from picture (following Exiv2 naming scheme, see https://exiv2.org/metadata.html)
@@ -54,15 +58,15 @@
 
 
     Implementation note: this needs to be sync with the PartialGeoPicTags structure
     """
 
     lat: float
     lon: float
-    ts: float
+    ts: datetime.datetime
     heading: Optional[int]
     type: str
     make: Optional[str]
     model: Optional[str]
     focal_length: Optional[float]
     crop: Optional[CropValues]
     exif: Dict[str, str] = field(default_factory=lambda: {})
@@ -82,15 +86,15 @@
     """Tags associated to a geolocated picture when not all tags have been found
 
     Implementation note: this needs to be sync with the GeoPicTags structure
     """
 
     lat: Optional[float] = None
     lon: Optional[float] = None
-    ts: Optional[float] = None
+    ts: Optional[datetime.datetime] = None
     heading: Optional[int] = None
     type: Optional[str] = None
     make: Optional[str] = None
     model: Optional[str] = None
     focal_length: Optional[float] = None
     crop: Optional[CropValues] = None
     exif: Dict[str, str] = field(default_factory=lambda: {})
@@ -138,14 +142,19 @@
         imgDesc = data["Exif.Image.ImageDescription"]
         try:
             imgDescJson = json.loads(imgDesc)
             data.update(imgDescJson)
         except:
             pass
 
+    # Sanitize charset information
+    for k, v in data.items():
+        if isinstance(v, str):
+            data[k] = re.sub(r"charset=[^\s]+", "", v).strip()
+
     # Parse latitude/longitude
     lat, lon, llw = decodeLatLon(data, "Exif.GPSInfo")
     if len(llw) > 0:
         warnings.extend(llw)
 
     if lat is None:
         lat, lon, llw = decodeLatLon(data, "Xmp.exif")
@@ -159,32 +168,32 @@
     # Check coordinates validity
     if lat is not None and (lat < -90 or lat > 90):
         raise InvalidExifException("Read latitude is out of WGS84 bounds (should be in [-90, 90])")
     if lon is not None and (lon < -180 or lon > 180):
         raise InvalidExifException("Read longitude is out of WGS84 bounds (should be in [-180, 180])")
 
     # Parse date/time
-    d, llw = decodeGPSDateTime(data, "Exif.GPSInfo")
+    d, llw = decodeGPSDateTime(data, "Exif.GPSInfo", lat, lon)
 
     if len(llw) > 0:
         warnings.extend(llw)
 
     if d is None:
-        d, llw = decodeGPSDateTime(data, "Xmp.exif")
+        d, llw = decodeGPSDateTime(data, "Xmp.exif", lat, lon)
         if len(llw) > 0:
             warnings.extend(llw)
 
     for exifField in [
         "Exif.Image.DateTimeOriginal",
         "Exif.Photo.DateTimeOriginal",
         "Exif.Image.DateTime",
         "Xmp.GPano.SourceImageCreateTime",
     ]:
         if d is None:
-            d, llw = decodeDateTimeOriginal(data, exifField)
+            d, llw = decodeDateTimeOriginal(data, exifField, lat, lon)
             if len(llw) > 0:
                 warnings.extend(llw)
 
         if d is not None:
             break
 
     if d is None and isExifTagUsable(data, "MAPGpsTime"):
@@ -309,15 +318,15 @@
     if errors:
         raise PartialExifException(
             " and ".join(errors),
             missing_fields,
             PartialGeoPicTags(
                 lat,
                 lon,
-                d.timestamp() if d else None,
+                d,
                 heading,
                 pic_type,
                 make,
                 model,
                 focalLength,
                 crop,
                 exif=data,
@@ -326,15 +335,15 @@
             ),
         )
 
     assert lon and lat and d  # at this point all those fields cannot be null
     return GeoPicTags(
         lat,
         lon,
-        d.timestamp(),
+        d,
         heading,
         pic_type,
         make,
         model,
         focalLength,
         crop,
         exif=data,
@@ -425,53 +434,77 @@
 
             lat = latRef * rawLat
             lon = lonRef * rawLon
 
     return (lat, lon, warnings)
 
 
-def decodeDateTimeOriginal(data: dict, datetimeField: str) -> Tuple[Optional[datetime.datetime], List[str]]:
+def decodeDateTimeOriginal(
+    data: dict, datetimeField: str, lat: Optional[float] = None, lon: Optional[float] = None
+) -> Tuple[Optional[datetime.datetime], List[str]]:
     d = None
     warnings = []
 
     if d is None and isExifTagUsable(data, datetimeField):
         try:
             dateRaw = data[datetimeField][:10].replace(":", "-")
             timeRaw = data[datetimeField][11:].split(":")
             hourRaw = int(timeRaw[0])
             minutesRaw = int(timeRaw[1])
             secondsRaw, microsecondsRaw, msw = decodeSecondsAndMicroSeconds(
                 timeRaw[2], data["Exif.Photo.SubSecTimeOriginal"] if isExifTagUsable(data, "Exif.Photo.SubSecTimeOriginal", float) else "0"
             )
-            tz = decodeTimeOffset(data, f"Exif.Photo.OffsetTime{'Original' if 'DateTimeOriginal' in datetimeField else ''}")
             warnings += msw
 
             d = datetime.datetime.combine(
                 datetime.date.fromisoformat(dateRaw),
                 datetime.time(
                     hourRaw,
                     minutesRaw,
                     secondsRaw,
                     microsecondsRaw,
-                    tzinfo=tz or datetime.timezone.utc,
                 ),
             )
+
+            # Timezone handling
+            # Try to read from EXIF
+            tz = decodeTimeOffset(data, f"Exif.Photo.OffsetTime{'Original' if 'DateTimeOriginal' in datetimeField else ''}")
+            if tz is not None:
+                d = d.replace(tzinfo=tz)
+
+            # Otherwise, try to deduct from coordinates
+            elif lon is not None and lat is not None:
+                tz_name = tz_finder.timezone_at(lng=lon, lat=lat)
+                if tz_name is not None:
+                    d = pytz.timezone(tz_name).localize(d)
+                # Otherwise, default to UTC + warning
+                else:
+                    d = d.replace(tzinfo=datetime.timezone.utc)
+                    warnings.append("Precise timezone information not found, fallback to UTC")
+
+            # Otherwise, default to UTC + warning
+            else:
+                d = d.replace(tzinfo=datetime.timezone.utc)
+                warnings.append("Precise timezone information not found (and no GPS coordinates to help), fallback to UTC")
+
         except ValueError as e:
             warnings.append("Skipping original date/time (from " + datetimeField + ") as it was not recognized:\n\t" + str(e))
 
     return (d, warnings)
 
 
 def decodeTimeOffset(data: dict, offsetTimeField: str) -> Optional[datetime.tzinfo]:
     if isExifTagUsable(data, offsetTimeField, datetime.tzinfo):
         return datetime.datetime.fromisoformat(f"2020-01-01T00:00:00{data[offsetTimeField]}").tzinfo
     return None
 
 
-def decodeGPSDateTime(data: dict, group: str) -> Tuple[Optional[datetime.datetime], List[str]]:
+def decodeGPSDateTime(
+    data: dict, group: str, lat: Optional[float] = None, lon: Optional[float] = None
+) -> Tuple[Optional[datetime.datetime], List[str]]:
     d = None
     warnings = []
 
     if d is None and isExifTagUsable(data, f"{group}.GPSDateStamp"):
         try:
             dateRaw = data[f"{group}.GPSDateStamp"].replace(":", "-").replace("\x00", "").replace("/", "-")
 
@@ -500,14 +533,20 @@
                         int(float(timeRaw[1])),
                         seconds,
                         microseconds,
                         tzinfo=datetime.timezone.utc,
                     ),
                 )
 
+                # Set timezone from coordinates
+                if lon is not None and lat is not None:
+                    tz_name = tz_finder.timezone_at(lng=lon, lat=lat)
+                    if tz_name is not None:
+                        d = d.astimezone(pytz.timezone(tz_name))
+
         except ValueError as e:
             warnings.append(f"Skipping GPS date/time ({group} group) as it was not recognized:\n\t{str(e)}")
 
     return (d, warnings)
 
 
 def decodeSecondsAndMicroSeconds(secondsRaw: str, microsecondsRaw: str) -> Tuple[int, int, List[str]]:
```

### Comparing `geopic_tag_reader-1.0.6/geopic_tag_reader/writer.py` & `geopic_tag_reader-1.1.0/geopic_tag_reader/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Optional, Tuple, Dict, Any
 from datetime import datetime, timedelta
 from dataclasses import dataclass
 from geopic_tag_reader.model import PictureType
 from enum import Enum
+import timezonefinder  # type: ignore
+import pytz
 
 try:
     import pyexiv2  # type: ignore
-    import timezonefinder  # type: ignore
-    import pytz
 except ImportError:
     raise Exception(
         """Impossible to write the exif tags without the '[write-exif]' dependency (that will need to install libexiv2).
 Install this package with `pip install geopic-tag-reader[write-exif]` to use this function"""
     )
 
 tz_finder = timezonefinder.TimezoneFinder()
```

### Comparing `geopic_tag_reader-1.0.6/pyproject.toml` & `geopic_tag_reader-1.1.0/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 dependencies = [
     "typer ~= 0.12",
     "xmltodict ~= 0.13",
     "pyexiv2 == 2.8.3",
+    "timezonefinder == 6.2.0",
+    "pytz ~= 2023.3",
+    "types-pytz ~= 2023.3.0.1",
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 Home = "https://gitlab.com/geovisio/geo-picture-tag-reader"
 
 [project.scripts]
@@ -29,17 +32,14 @@
     "lazydocs ~= 0.4.8",
     "types-xmltodict ~= 0.13",
     "pre-commit ~= 3.3.3",
 ]
 build = ["flit ~= 3.8.0"]
 # optional dependencies to be able to write exif tags
 write-exif = [
-    "timezonefinder == 6.2.0",
-    "pytz ~= 2023.3",
-    "types-pytz ~= 2023.3.0.1",
     "python-dateutil ~= 2.8.2",
 ]
 
 
 [build-system]
 requires = ["flit_core ~= 3.8,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/1.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/IMG_20210720_144918.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/IMG_20210720_144918.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/IMG_20210720_161352.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/IMG_20210720_161352.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/a1.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/a1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/b1.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/b1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/broken_makernotes.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/broken_makernotes.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/c1.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/c1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/cropped.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/cropped.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/d1.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/d1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/datetime_ms_float.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/datetime_ms_float.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/datetime_offset.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/datetime_offset.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/e1.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/e1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/flat.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/flat.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/gopromax_flat.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/gopromax_flat.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/gps_date_slash.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/gps_date_slash.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/gps_date_time_stamp.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/gps_date_time_stamp.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/img_Ricoh_Theta.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/img_Ricoh_Theta.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/img_V4MPack.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/img_V4MPack.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/img_categorisee.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/img_categorisee.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/img_datetimeoriginal.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/img_datetimeoriginal.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/img_gps_date_string.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/img_gps_date_string.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/img_gps_datestamp.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/img_gps_datestamp.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/img_gps_sotm.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/img_gps_sotm.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/img_invalid_gps_date.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/img_invalid_gps_date.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/img_without_coord.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/img_without_coord.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/img_without_dt.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/img_without_dt.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/img_without_exif_tags.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/img_without_exif_tags.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/insta360_date.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/insta360_date.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/int_long_tag.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/int_long_tag.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/out_of_bounds_lat.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/out_of_bounds_lat.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/out_of_bounds_lon.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/out_of_bounds_lon.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/pic_with_float_lat.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/pic_with_float_lat.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/fixtures/ricoh_theta_no_projection.jpg` & `geopic_tag_reader-1.1.0/tests/fixtures/ricoh_theta_no_projection.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/test_main.py` & `geopic_tag_reader-1.1.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.6/tests/test_reader.py` & `geopic_tag_reader-1.1.0/tests/test_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,29 @@
 from geopic_tag_reader import reader
 from .conftest import FIXTURE_DIR, openImg
 
 
 def assertGeoPicTagsEquals(gpt, expectedDict):
     assert gpt.lat == expectedDict.get("lat")
     assert gpt.lon == expectedDict.get("lon")
-    assert gpt.ts == expectedDict.get("ts")
     assert gpt.heading == expectedDict.get("heading")
     assert gpt.type == expectedDict.get("type")
     assert gpt.make == expectedDict.get("make")
     assert gpt.model == expectedDict.get("model")
     assert gpt.focal_length == expectedDict.get("focal_length")
     assert gpt.altitude == expectedDict.get("altitude")
     assert gpt.tagreader_warnings == expectedDict.get("tagreader_warnings", [])
     assert len(gpt.exif) > 0
 
+    if expectedDict.get("ts") is not None:
+        assert gpt.ts is not None
+        assert gpt.ts.isoformat() == expectedDict["ts"]
+    else:
+        assert gpt.ts is None
+
     if gpt.crop:
         assert expectedDict.get("crop") is not None
         assert gpt.crop.fullWidth == expectedDict["crop"].get("fullWidth")
         assert gpt.crop.fullHeight == expectedDict["crop"].get("fullHeight")
         assert gpt.crop.width == expectedDict["crop"].get("width")
         assert gpt.crop.height == expectedDict["crop"].get("height")
         assert gpt.crop.left == expectedDict["crop"].get("left")
@@ -33,15 +38,15 @@
 def test_readPictureMetadata(datafiles):
     result = reader.readPictureMetadata(openImg(str(datafiles) + "/1.jpg"))
     assertGeoPicTagsEquals(
         result,
         {
             "lat": 49.00688961988304,
             "lon": 1.9191854417991367,
-            "ts": 1627550214.0,
+            "ts": "2021-07-29T11:16:54+02:00",
             "heading": 349,
             "type": "equirectangular",
             "make": "GoPro",
             "model": "Max",
             "focal_length": 3,
             "altitude": 93,
         },
@@ -52,15 +57,15 @@
 def test_readPictureMetadata_negCoords(datafiles):
     result = reader.readPictureMetadata(openImg(str(datafiles) + "/a1.jpg"))
     assertGeoPicTagsEquals(
         result,
         {
             "lat": 48.33756428166505,
             "lon": -1.9331088333333333,
-            "ts": 1652453580.0,
+            "ts": "2022-05-13T16:53:00+02:00",
             "heading": 32,
             "type": "equirectangular",
             "make": "GoPro",
             "model": "Max",
             "focal_length": 3,
             "altitude": 79,
         },
@@ -71,15 +76,15 @@
 def test_readPictureMetadata_flat(datafiles):
     result = reader.readPictureMetadata(openImg(str(datafiles) + "/b1.jpg"))
     assertGeoPicTagsEquals(
         result,
         {
             "lat": 48.139852239480945,
             "lon": -1.9499731060073981,
-            "ts": 1429976268.0,
+            "ts": "2015-04-25T15:37:48+02:00",
             "heading": 155,
             "type": "flat",
             "make": "OLYMPUS IMAGING CORP.",
             "model": "SP-720UZ",
             "focal_length": 4.66,
         },
     )
@@ -89,15 +94,15 @@
 def test_readPictureMetadata_flat2(datafiles):
     result = reader.readPictureMetadata(openImg(str(datafiles) + "/c1.jpg"))
     assertGeoPicTagsEquals(
         result,
         {
             "lat": 48.85779642035038,
             "lon": 2.3392783047650747,
-            "ts": 1430744932.0,
+            "ts": "2015-05-04T13:08:52+02:00",
             "heading": 302,
             "type": "flat",
             "make": "Canon",
             "model": "EOS 6D0",
             "focal_length": 35.0,
         },
     )
@@ -107,15 +112,15 @@
 def test_readPictureMetadata_xmpHeading(datafiles):
     result = reader.readPictureMetadata(openImg(str(datafiles) + "/d1.jpg"))
     assertGeoPicTagsEquals(
         result,
         {
             "lat": 50.87070833333333,
             "lon": -1.5260916666666666,
-            "ts": 1600008019.767,
+            "ts": "2020-09-13T15:40:19.767000+01:00",
             "heading": 67,
             "type": "equirectangular",
             "make": "Google",
             "model": "Pixel 3",
             "focal_length": None,
             "altitude": 68,
         },
@@ -126,15 +131,15 @@
 def test_readPictureMetadata_noHeading(datafiles):
     result = reader.readPictureMetadata(openImg(str(datafiles) + "/e1.jpg"))
     assertGeoPicTagsEquals(
         result,
         {
             "lat": 48.15506638888889,
             "lon": -1.6844680555555556,
-            "ts": 1666166194.0,
+            "ts": "2022-10-19T09:56:34+02:00",
             "heading": None,
             "type": "flat",
             "make": "SONY",
             "model": "FDR-X1000V",
             "focal_length": 2.8,
             "altitude": 34,
         },
@@ -150,15 +155,15 @@
             {
                 "focal_length": 0.75,
                 "heading": 270,
                 "lat": 48.83930905577957,
                 "lon": 2.3205357914890987,
                 "make": "RICOH",
                 "model": "THETA m15",
-                "ts": 1458911533.0,
+                "ts": "2016-03-25T14:12:13+01:00",
                 "type": "equirectangular",
             },
         )
 
 
 @pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "img_V4MPack.jpg"))
 def test_readPictureMetadata_v4mpack(datafiles):
@@ -169,15 +174,15 @@
             {
                 "focal_length": None,
                 "heading": 64,
                 "lat": 47.08506017299737,
                 "lon": -1.2761512389983616,
                 "make": "STFMANI",
                 "model": "V4MPOD 1",
-                "ts": 1555417213.0,
+                "ts": "2019-04-16T14:20:13+02:00",
                 "type": "equirectangular",
                 "altitude": 34,
             },
         )
 
 
 @pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "IMG_20210720_161352.jpg"))
@@ -188,15 +193,15 @@
         {
             "focal_length": 4.103,
             "heading": 355,
             "lat": 48.96280504578332,
             "lon": 2.51197323068765,
             "make": "OnePlus",
             "model": "ONEPLUS A5000",
-            "ts": 1626797632.199995,
+            "ts": "2021-07-20T16:13:52.199995+02:00",
             "type": "flat",
             "altitude": 0,
         },
     )
 
 
 @pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "IMG_20210720_144918.jpg"))
@@ -223,15 +228,15 @@
         {
             "focal_length": None,
             "heading": 255,
             "lat": 44.09732280555556,
             "lon": 4.700622,
             "make": None,
             "model": None,
-            "ts": 1673515020.0,
+            "ts": "2023-01-12T09:17:00+01:00",
             "type": "flat",
             "tagreader_warnings": ["GPSLongitudeRef not found, assuming GPSLongitudeRef is East"],
         },
     )
 
 
 @pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "img_invalid_gps_date.jpg"))
@@ -245,15 +250,15 @@
         {
             "focal_length": 4.2,
             "heading": 202,
             "lat": 48.88026828330809,
             "lon": 2.358506155368721,
             "make": "samsung",
             "model": None,
-            "ts": 1631101437.0754,
+            "ts": "2021-09-08T11:43:57.075400+02:00",
             "type": "flat",
             "altitude": 73,
             "tagreader_warnings": [
                 "Skipping GPS date/time (Exif.GPSInfo group) as it was not recognized:\n\tInvalid isoformat string: '2021-09-08H'"
             ],
         },
     )
@@ -267,15 +272,15 @@
         {
             "focal_length": 4.2,
             "heading": 138,
             "lat": 48.80334166666666,
             "lon": 2.4833194444444446,
             "make": "Apple",
             "model": "iPhone 12 Pro",
-            "ts": 1682785851.565,
+            "ts": "2023-04-29T18:30:51.565000+02:00",
             "type": "flat",
             "altitude": 36,
             "tagreader_warnings": [
                 "Microseconds read from decimal seconds value (3000) is not matching value from EXIF field (565000). Max value will be kept."
             ],
         },
     )
@@ -289,15 +294,15 @@
         {
             "focal_length": 3.99,
             "heading": 182,
             "lat": 45.624741666666665,
             "lon": -1.0015555555555555,
             "make": "Apple",
             "model": "iPhone 8 Plus",
-            "ts": 1564313142.529,
+            "ts": "2019-07-28T13:25:42.529000+02:00",
             "type": "flat",
             "altitude": 19,
             "tagreader_warnings": [
                 "Microseconds read from decimal seconds value (529000) is not matching value from EXIF field (506000). Max value will be kept."
             ],
         },
     )
@@ -318,15 +323,15 @@
         result,
         {
             "heading": 349,
             "lat": 49.00688961988304,
             "lon": 1.919185441804927,
             "make": "GoPro",
             "model": "Max",
-            "ts": 1627550214.0,
+            "ts": "2021-07-29T11:16:54+02:00",
             "type": "equirectangular",
             "altitude": 93,
             "crop": {"fullWidth": 4032, "fullHeight": 2016, "width": 2150, "height": 1412, "top": 134, "left": 538},
         },
     )
 
 
@@ -337,15 +342,15 @@
         result,
         {
             "heading": 228,
             "lat": 47.05369676823944,
             "lon": -1.382302762883527,
             "make": "Motorola",
             "model": "XT1052",
-            "ts": 1598866588.0,
+            "ts": "2020-08-31T09:36:28+02:00",
             "type": "flat",
             "altitude": 72,
             "tagreader_warnings": [
                 "Skipping GPS date/time (Exif.GPSInfo group) as it was not recognized:\n\tGPSTimeStamp and GPSDateTime don't contain supported time format (in Exif.GPSInfo group)"
             ],
         },
     )
@@ -358,15 +363,15 @@
         result,
         {
             "heading": 62,
             "lat": 14.527860666666667,
             "lon": 121.15072633333334,
             "make": "BlackVue",
             "model": "DR900S-1CH",
-            "ts": 1699748719.023,
+            "ts": "2023-11-12T00:25:19.023000+08:00",
             "type": "flat",
             "altitude": 29,
             "tagreader_warnings": [],
         },
     )
 
 
@@ -397,15 +402,15 @@
         {
             "focal_length": 4.2,
             "heading": 138,
             "lat": None,  # but lat/lon should be None
             "lon": None,
             "make": "Apple",
             "model": "iPhone 12 Pro",
-            "ts": 1682785851.565,
+            "ts": "2023-04-29T16:30:51.565000+00:00",
             "type": "flat",
             "altitude": 36,
             "tagreader_warnings": [
                 "Microseconds read from decimal seconds value (3000) is not matching value from EXIF field (565000). Max value will be kept."
             ],
         },
     )
@@ -468,15 +473,15 @@
         result,
         {
             "heading": 6,
             "lat": 48.553668,
             "lon": 7.683081,
             "make": None,
             "model": "PULSAR",
-            "ts": 1637075896.89,
+            "ts": "2021-11-16T16:18:16.890000+01:00",
             "type": "equirectangular",
             "altitude": None,
             "tagreader_warnings": [],
         },
     )
 
 
@@ -488,15 +493,15 @@
         result,
         {
             "heading": 6,
             "lat": 48.553668,
             "lon": 7.683081,
             "make": None,
             "model": "PULSAR",
-            "ts": 1637075896.89,
+            "ts": "2021-11-16T16:18:16.890000+01:00",
             "type": "equirectangular",
             "altitude": None,
             "tagreader_warnings": [],
         },
     )
 
 
@@ -508,15 +513,15 @@
         result,
         {
             "heading": None,
             "lat": 43.29976944444444,
             "lon": 3.482755555555556,
             "make": "Insta360",
             "model": "One X2.PHOTO_NORMAL",
-            "ts": 1700662669.0,
+            "ts": "2023-11-22T14:17:49+01:00",
             "type": "equirectangular",
             "altitude": 84,
             "tagreader_warnings": [],
         },
     )
 
 
@@ -528,15 +533,15 @@
         result,
         {
             "heading": None,
             "lat": 48.23105138608521,
             "lon": -1.5464416503906249,
             "make": "Ricoh",
             "model": "Theta S",
-            "ts": 1672575342.0,
+            "ts": "2023-01-01T13:15:42+01:00",
             "type": "equirectangular",
             "altitude": None,
             "tagreader_warnings": [],
         },
     )
 
 
@@ -545,15 +550,15 @@
     result = reader.readPictureMetadata(openImg(str(datafiles) + "/gopromax_flat.jpg"))
 
     assertGeoPicTagsEquals(
         result,
         {
             "lat": 47.22555109997222,
             "lon": -1.5631604999722222,
-            "ts": 1708173992.0,
+            "ts": "2024-02-17T13:46:32+01:00",
             "heading": None,
             "type": "flat",
             "make": "GoPro",
             "model": "Max",
             "focal_length": 3,
             "altitude": 78,
         },
@@ -568,15 +573,15 @@
         result,
         {
             "heading": 33,
             "lat": 48.24849805555556,
             "lon": -1.7841980555555554,
             "make": "SONY",
             "model": "FDR-X1000V",
-            "ts": 1599115820.0,
+            "ts": "2020-09-03T08:50:20+02:00",
             "type": "flat",
             "altitude": 99,
             "focal_length": 2.8,
             "tagreader_warnings": [],
         },
     )
 
@@ -586,15 +591,15 @@
     result = reader.readPictureMetadata(openImg(str(datafiles) + "/datetime_offset.jpg"))
 
     assertGeoPicTagsEquals(
         result,
         {
             "lat": 48.33756428166505,
             "lon": -1.9331088333333333,
-            "ts": 1652453651.0,
+            "ts": "2022-05-13T16:54:11+02:00",
             "heading": 32,
             "type": "equirectangular",
             "make": "GoPro",
             "model": "Max",
             "focal_length": 3,
             "altitude": 79,
         },
@@ -606,20 +611,26 @@
     result = reader.readPictureMetadata(openImg(str(datafiles) + "/gps_date_slash.jpg"))
 
     assertGeoPicTagsEquals(
         result,
         {
             "lat": 43.42541569992266,
             "lon": 1.3766216000638112,
-            "ts": 1686640500.0,
+            "ts": "2023-06-13T09:15:00+02:00",
             "heading": None,
             "type": "flat",
             "make": None,
             "model": None,
             "focal_length": None,
             "altitude": None,
             "tagreader_warnings": [
                 "GPSLatitudeRef not found, assuming GPSLatitudeRef is North",
                 "GPSLongitudeRef not found, assuming GPSLongitudeRef is East",
             ],
         },
     )
+
+
+@pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "charset.jpg"))
+def test_readPictureMetadata_charset(datafiles):
+    result = reader.readPictureMetadata(openImg(str(datafiles) + "/charset.jpg"))
+    assert result.exif["Exif.Photo.UserComment"] == "CD31 31_D0003_51_600"
```

### Comparing `geopic_tag_reader-1.0.6/tests/test_writer.py` & `geopic_tag_reader-1.1.0/tests/test_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def test_writePictureMetadata_capture_time(datafiles):
     capture_time = datetime(year=2023, month=6, day=1, hour=12, minute=48, second=1, microsecond=500000, tzinfo=pytz.UTC)
 
     img_orig = openImg(str(datafiles / "1.jpg"))
     image_file_upd = writer.writePictureMetadata(img_orig, writer.PictureMetadata(capture_time=capture_time))
     tags = reader.readPictureMetadata(image_file_upd)
 
-    assert datetime.fromtimestamp(tags.ts, tz=pytz.UTC) == capture_time
+    assert tags.ts == capture_time
 
     # we also check specific tags:
     assert tags.exif["Exif.Photo.DateTimeOriginal"] == "2023-06-01 12:48:01"
     assert tags.exif["Exif.GPSInfo.GPSDateStamp"] == "2023-06-01"
     assert tags.exif["Exif.GPSInfo.GPSTimeStamp"] == "12/1 48/1 1/1"
     assert tags.exif["Exif.Photo.SubSecTimeOriginal"] == "500000"
 
@@ -32,15 +32,15 @@
     capture_time = datetime(year=2023, month=6, day=1, hour=12, minute=48, second=1, tzinfo=None)
 
     img_orig = openImg(str(datafiles / "1.jpg"))
     image_file_upd = writer.writePictureMetadata(img_orig, writer.PictureMetadata(capture_time=capture_time))
     tags = reader.readPictureMetadata(image_file_upd)
 
     paris = pytz.timezone("Europe/Paris")
-    assert datetime.fromtimestamp(tags.ts, tz=pytz.UTC) == paris.localize(capture_time).astimezone(pytz.UTC)
+    assert tags.ts == paris.localize(capture_time).astimezone(pytz.UTC)
 
     # DateTimeOriginal should be a local time, so 12:48:01 localized in Europe/Paris timezome (since it's where the picture has been taken)
     assert tags.exif["Exif.Photo.DateTimeOriginal"] == "2023-06-01 12:48:01"
     assert tags.exif["Exif.GPSInfo.GPSDateStamp"] == "2023-06-01"
     # GPSTimeStamp should always be in UTC
     assert tags.exif["Exif.GPSInfo.GPSTimeStamp"] == "10/1 48/1 1/1"
     assert tags.exif["Exif.Photo.OffsetTimeOriginal"] == "+02:00"
@@ -74,15 +74,15 @@
     img_orig = openImg(str(datafiles / "img_without_coord.jpg"))
     image_file_upd = writer.writePictureMetadata(
         img_orig, writer.PictureMetadata(capture_time=capture_time, latitude=48.866667, longitude=2.333333)
     )
     tags = reader.readPictureMetadata(image_file_upd)
 
     paris = pytz.timezone("Europe/Paris")
-    assert datetime.fromtimestamp(tags.ts, tz=pytz.UTC) == paris.localize(capture_time).astimezone(pytz.UTC)
+    assert tags.ts == paris.localize(capture_time).astimezone(pytz.UTC)
 
     # DateTimeOriginal should be a local time, so 12:48:01 localized in Europe/Paris timezome (since it's where the picture has been taken)
     assert tags.exif["Exif.Photo.DateTimeOriginal"] == "2023-06-01 12:48:01"
     assert tags.exif["Exif.Photo.OffsetTimeOriginal"] == "+02:00"
     assert tags.exif["Exif.GPSInfo.GPSDateStamp"] == "2023-06-01"
     # GPSTimeStamp should always be in UTC
     assert tags.exif["Exif.GPSInfo.GPSTimeStamp"] == "10/1 48/1 1/1"
```

### Comparing `geopic_tag_reader-1.0.6/PKG-INFO` & `geopic_tag_reader-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: geopic-tag-reader
-Version: 1.0.6
+Version: 1.1.0
 Summary: GeoPicTagReader
 Author-email: Adrien PAVIE <panieravide@riseup.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: typer ~= 0.12
 Requires-Dist: xmltodict ~= 0.13
 Requires-Dist: pyexiv2 == 2.8.3
+Requires-Dist: timezonefinder == 6.2.0
+Requires-Dist: pytz ~= 2023.3
+Requires-Dist: types-pytz ~= 2023.3.0.1
 Requires-Dist: flit ~= 3.8.0 ; extra == "build"
 Requires-Dist: black ~= 24.3 ; extra == "dev"
 Requires-Dist: mypy ~= 1.9 ; extra == "dev"
 Requires-Dist: pytest ~= 7.2.0 ; extra == "dev"
 Requires-Dist: pytest-datafiles ~= 3.0 ; extra == "dev"
 Requires-Dist: lazydocs ~= 0.4.8 ; extra == "dev"
 Requires-Dist: types-xmltodict ~= 0.13 ; extra == "dev"
 Requires-Dist: pre-commit ~= 3.3.3 ; extra == "dev"
-Requires-Dist: timezonefinder == 6.2.0 ; extra == "write-exif"
-Requires-Dist: pytz ~= 2023.3 ; extra == "write-exif"
-Requires-Dist: types-pytz ~= 2023.3.0.1 ; extra == "write-exif"
 Requires-Dist: python-dateutil ~= 2.8.2 ; extra == "write-exif"
 Project-URL: Home, https://gitlab.com/geovisio/geo-picture-tag-reader
 Provides-Extra: build
 Provides-Extra: dev
 Provides-Extra: write-exif
 
 # ![GeoVisio](https://gitlab.com/geovisio/api/-/raw/develop/images/logo_full.png)
```

