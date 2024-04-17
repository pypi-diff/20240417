# Comparing `tmp/aind-metadata-mapper-0.6.2.tar.gz` & `tmp/aind_metadata_mapper-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-metadata-mapper-0.6.2.tar", last modified: Wed Apr 10 20:05:35 2024, max compression
+gzip compressed data, was "aind_metadata_mapper-0.6.3.tar", last modified: Wed Apr 17 16:59:39 2024, max compression
```

## Comparing `aind-metadata-mapper-0.6.2.tar` & `aind_metadata_mapper-0.6.3.tar`

### file list

```diff
@@ -1,110 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.373698 aind-metadata-mapper-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.353698 aind-metadata-mapper-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.357698 aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.357698 aind-metadata-mapper-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-10 20:05:35.373698 aind-metadata-mapper-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.357698 aind-metadata-mapper-0.6.2/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.357698 aind-metadata-mapper-0.6.2/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/examples/bergamo_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/mismatched_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/rig.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:05:35.373698 aind-metadata-mapper-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.353698 aind-metadata-mapper-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23421 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/bergamo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/ephys/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/fib/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/fib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/fib/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/mesoscope/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.365698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.373698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-10 20:05:35.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-10 20:05:35.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:05:35.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 20:05:35.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 20:05:35.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.365698 aind-metadata-mapper-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.357698 aind-metadata-mapper-0.6.2/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.365698 aind-metadata-mapper-0.6.2/tests/resources/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/bergamo/cropped_neuron50_00001.tif
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/bergamo/example_description0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/bergamo/example_metadata.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/bergamo/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.365698 aind-metadata-mapper-0.6.2/tests/resources/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/ephys/ephys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/ephys/newscale_main.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/ephys/newscale_surface_finding.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/ephys/settings_main.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/ephys/settings_surface_finding.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.369698 aind-metadata-mapper-0.6.2/tests/resources/fib/
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/fib/000000_ophys_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/fib/000000_ophys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/fib/example_from_teensy.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.369698 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/example_extract.json
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/example_platform.json
--rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.373698 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/base-missing-probe_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/base_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/mvr.ini
--rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/mvr_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/open-ephys-inferred_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/open-ephys_rig.json
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/settings.mislabeled-probes-0.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/settings.mislabeled-probes-1.xml
--rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/sync.yml
--rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/sync_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_bergamo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_ephys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_fib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_legacy_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_mesoscope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.373698 aind-metadata-mapper-0.6.2/tests/test_neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_open_ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_open_ephys_rig_inferrred.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.529946 aind_metadata_mapper-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.505946 aind_metadata_mapper-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.509946 aind_metadata_mapper-0.6.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.513946 aind_metadata_mapper-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-17 16:59:39.529946 aind_metadata_mapper-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.513946 aind_metadata_mapper-0.6.3/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.513946 aind_metadata_mapper-0.6.3/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.513946 aind_metadata_mapper-0.6.3/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.513946 aind_metadata_mapper-0.6.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/examples/bergamo_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.513946 aind_metadata_mapper-0.6.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/scripts/singularity_build.def
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:59:39.529946 aind_metadata_mapper-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.505946 aind_metadata_mapper-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.513946 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 16:59:27.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.513946 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23421 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/bergamo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.517946 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/ephys/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.517946 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/fib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/fib/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10639 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/gather_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.517946 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/mesoscope/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.517946 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/neuropixels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/neuropixels/mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/neuropixels/sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/neuropixels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.529946 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-17 16:59:39.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-17 16:59:39.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:59:39.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 16:59:39.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 16:59:39.000000 aind_metadata_mapper-0.6.3/src/aind_metadata_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.517946 aind_metadata_mapper-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.509946 aind_metadata_mapper-0.6.3/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.517946 aind_metadata_mapper-0.6.3/tests/resources/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/bergamo/cropped_neuron50_00001.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/bergamo/example_description0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/bergamo/example_metadata.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/bergamo/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.521946 aind_metadata_mapper-0.6.3/tests/resources/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/ephys/ephys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/ephys/newscale_main.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/ephys/newscale_surface_finding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/ephys/settings_main.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/ephys/settings_surface_finding.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.521946 aind_metadata_mapper-0.6.3/tests/resources/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/fib/000000_ophys_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/fib/000000_ophys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/fib/example_from_teensy.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.521946 aind_metadata_mapper-0.6.3/tests/resources/gather_metadata_job/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/gather_metadata_job/example_procedures_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/gather_metadata_job/example_subject_response.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.521946 aind_metadata_mapper-0.6.3/tests/resources/gather_metadata_job/metadata_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/gather_metadata_job/metadata_files/data_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/gather_metadata_job/metadata_files/procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/gather_metadata_job/metadata_files/processing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/gather_metadata_job/metadata_files/subject.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.521946 aind_metadata_mapper-0.6.3/tests/resources/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/mesoscope/example_extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/mesoscope/example_platform.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/mesoscope/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.525946 aind_metadata_mapper-0.6.3/tests/resources/neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/neuropixels/base-missing-probe_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/neuropixels/base_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/neuropixels/mvr.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/neuropixels/mvr_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/neuropixels/open-ephys-inferred_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/neuropixels/open-ephys_rig.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/neuropixels/settings.mislabeled-probes-0.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/neuropixels/settings.mislabeled-probes-1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/neuropixels/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/neuropixels/sync.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/resources/neuropixels/sync_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/test_bergamo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/test_ephys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/test_fib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15172 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/test_gather_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/test_legacy_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/test_mesoscope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:39.529946 aind_metadata_mapper-0.6.3/tests/test_neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/test_neuropixels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/test_neuropixels/test_mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/test_neuropixels/test_neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/test_neuropixels/test_open_ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/test_neuropixels/test_open_ephys_rig_inferrred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/test_neuropixels/test_sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-17 16:59:26.000000 aind_metadata_mapper-0.6.3/tests/test_neuropixels/utils.py
```

### Comparing `aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_mapper-0.6.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_mapper-0.6.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_mapper-0.6.3/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/.github/workflows/test_and_lint.yml` & `aind_metadata_mapper-0.6.3/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/.gitignore` & `aind_metadata_mapper-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/LICENSE` & `aind_metadata_mapper-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/PKG-INFO` & `aind_metadata_mapper-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.6.2
+Version: 0.6.3
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind-metadata-mapper-0.6.2/README.md` & `aind_metadata_mapper-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/doc_template/Makefile` & `aind_metadata_mapper-0.6.3/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/doc_template/make.bat` & `aind_metadata_mapper-0.6.3/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/doc_template/source/_static/dark-logo.svg` & `aind_metadata_mapper-0.6.3/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/doc_template/source/_static/favicon.ico` & `aind_metadata_mapper-0.6.3/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/doc_template/source/_static/light-logo.svg` & `aind_metadata_mapper-0.6.3/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/doc_template/source/conf.py` & `aind_metadata_mapper-0.6.3/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/examples/bergamo_session.py` & `aind_metadata_mapper-0.6.3/examples/bergamo_session.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/mismatched_rig.json` & `aind_metadata_mapper-0.6.3/tests/resources/neuropixels/base-missing-probe_rig.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/pyproject.toml` & `aind_metadata_mapper-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/rig.json` & `aind_metadata_mapper-0.6.3/tests/resources/neuropixels/base_rig.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9942528735632183%*

 * *Differences: {"'modalities'": "{0: {'name': 'Behavior videos', 'abbreviation': 'behavior-videos'}, 1: {'name': "*

 * *                 "'Extracellular electrophysiology', 'abbreviation': 'ecephys'}}"}*

```diff
@@ -979,22 +979,22 @@
             "serial_number": null,
             "wavelength": 633,
             "wavelength_unit": "nanometer"
         }
     ],
     "modalities": [
         {
-            "abbreviation": "ecephys",
-            "name": "Extracellular electrophysiology"
-        },
-        {
             "abbreviation": "behavior-videos",
             "name": "Behavior videos"
         },
         {
+            "abbreviation": "ecephys",
+            "name": "Extracellular electrophysiology"
+        },
+        {
             "abbreviation": "behavior",
             "name": "Behavior"
         }
     ],
     "modification_date": "2024-04-01",
     "mouse_platform": {
         "additional_settings": {},
```

### Comparing `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/bergamo/session.py` & `aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/bergamo/session.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/core.py` & `aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/core.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/ephys/session.py` & `aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/ephys/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         ephys_session["data_streams"] = []
 
         for stage, data_stream in zip(
             stage_logs, experiment_data["data_streams"]
         ):
             session_stream = {}
             session_stream["stream_start_time"] = datetime.strptime(
-               stage[0][0], "%Y/%m/%d %H:%M:%S.%f"
+                stage[0][0], "%Y/%m/%d %H:%M:%S.%f"
             )
             session_stream["stream_end_time"] = datetime.strptime(
                 stage[-1][0], "%Y/%m/%d %H:%M:%S.%f"
             )
             session_stream["stream_modalities"] = [Modality.ECEPHYS]
             session_stream["stick_microscopes"] = stick_microscopes
             session_stream["camera_names"] = camera_names
```

### Comparing `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/fib/session.py` & `aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/fib/session.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/mesoscope/session.py` & `aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/mesoscope/session.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/mvr_rig.py` & `aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/neuropixels/mvr_rig.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py` & `aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Base ETL class for neuropixels rigs."""
 
 import logging
+from datetime import date
 from pathlib import Path
 from typing import Optional
-from datetime import date
 
 from aind_data_schema.core.rig import Rig  # type: ignore
 from pydantic import BaseModel
 
 from aind_metadata_mapper.core import BaseEtl
 
 logger = logging.getLogger(__name__)
@@ -51,17 +51,17 @@
         """Transforms extracted rig context into aind-data-schema rig.Rig
         instance.
         """
         return extracted_source
 
     @classmethod
     def update_modification_date(
-            cls,
-            extracted_source: Rig,
-            modification_date: Optional[date] = None,
+        cls,
+        extracted_source: Rig,
+        modification_date: Optional[date] = None,
     ) -> Rig:
         """Updates modification date and rig id."""
         room_id, rig_name, _ = extracted_source.rig_id.split("_")
         if modification_date is None:
             modification_date = date.today()
 
         extracted_source.rig_id = (
```

### Comparing `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py` & `aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ETL for the Open Ephys config."""
 
 import logging
+from datetime import date
 from pathlib import Path
 from typing import List, Optional, Tuple
 from xml.etree import ElementTree
-from datetime import date
 
 from aind_data_schema.core.rig import Rig  # type: ignore
 from pydantic import BaseModel
 
 from aind_metadata_mapper.neuropixels import utils
 from aind_metadata_mapper.neuropixels.neuropixels_rig import (
     NeuropixelsRigContext,
@@ -156,10 +156,11 @@
                     model=probe.model,
                     serial_number=probe.serial_number,
                 )
                 if updated:
                     break
 
         self.update_modification_date(
-            extracted_source.current, self.modification_date)
+            extracted_source.current, self.modification_date
+        )
 
         return super()._transform(extracted_source.current)
```

### Comparing `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/sync_rig.py` & `aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/neuropixels/sync_rig.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/utils.py` & `aind_metadata_mapper-0.6.3/src/aind_metadata_mapper/neuropixels/utils.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/PKG-INFO` & `aind_metadata_mapper-0.6.3/src/aind_metadata_mapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.6.2
+Version: 0.6.3
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/SOURCES.txt` & `aind_metadata_mapper-0.6.3/src/aind_metadata_mapper.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 .flake8
 .gitignore
 LICENSE
 README.md
-mismatched_rig.json
 pyproject.toml
-rig.json
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/user-story.md
 .github/workflows/tag_and_publish.yml
 .github/workflows/test_and_lint.yml
 doc_template/Makefile
 doc_template/make.bat
 doc_template/source/conf.py
 doc_template/source/index.rst
 doc_template/source/_static/dark-logo.svg
 doc_template/source/_static/favicon.ico
 doc_template/source/_static/light-logo.svg
 examples/bergamo_session.py
+scripts/singularity_build.def
 src/aind_metadata_mapper/__init__.py
 src/aind_metadata_mapper/core.py
+src/aind_metadata_mapper/gather_metadata.py
 src/aind_metadata_mapper.egg-info/PKG-INFO
 src/aind_metadata_mapper.egg-info/SOURCES.txt
 src/aind_metadata_mapper.egg-info/dependency_links.txt
 src/aind_metadata_mapper.egg-info/requires.txt
 src/aind_metadata_mapper.egg-info/top_level.txt
 src/aind_metadata_mapper/bergamo/__init__.py
 src/aind_metadata_mapper/bergamo/session.py
@@ -40,28 +40,35 @@
 src/aind_metadata_mapper/neuropixels/open_ephys_rig.py
 src/aind_metadata_mapper/neuropixels/sync_rig.py
 src/aind_metadata_mapper/neuropixels/utils.py
 tests/__init__.py
 tests/test_bergamo.py
 tests/test_ephys.py
 tests/test_fib.py
+tests/test_gather_metadata.py
 tests/test_legacy_core.py
 tests/test_mesoscope.py
 tests/resources/bergamo/cropped_neuron50_00001.tif
 tests/resources/bergamo/example_description0.txt
 tests/resources/bergamo/example_metadata.txt.gz
 tests/resources/bergamo/expected_session.json
 tests/resources/ephys/ephys_session.json
 tests/resources/ephys/newscale_main.csv
 tests/resources/ephys/newscale_surface_finding.csv
 tests/resources/ephys/settings_main.xml
 tests/resources/ephys/settings_surface_finding.xml
 tests/resources/fib/000000_ophys_rig.json
 tests/resources/fib/000000_ophys_session.json
 tests/resources/fib/example_from_teensy.txt
+tests/resources/gather_metadata_job/example_procedures_response.json
+tests/resources/gather_metadata_job/example_subject_response.json
+tests/resources/gather_metadata_job/metadata_files/data_description.json
+tests/resources/gather_metadata_job/metadata_files/procedures.json
+tests/resources/gather_metadata_job/metadata_files/processing.json
+tests/resources/gather_metadata_job/metadata_files/subject.json
 tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
 tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
 tests/resources/mesoscope/0123456789_Face_20240212T091444.json
 tests/resources/mesoscope/example_extract.json
 tests/resources/mesoscope/example_platform.json
 tests/resources/mesoscope/expected_session.json
 tests/resources/neuropixels/base-missing-probe_rig.json
```

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/bergamo/cropped_neuron50_00001.tif` & `aind_metadata_mapper-0.6.3/tests/resources/bergamo/cropped_neuron50_00001.tif`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/bergamo/example_description0.txt` & `aind_metadata_mapper-0.6.3/tests/resources/bergamo/example_description0.txt`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/bergamo/example_metadata.txt.gz` & `aind_metadata_mapper-0.6.3/tests/resources/bergamo/example_metadata.txt.gz`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/bergamo/expected_session.json` & `aind_metadata_mapper-0.6.3/tests/resources/bergamo/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/ephys/ephys_session.json` & `aind_metadata_mapper-0.6.3/tests/resources/ephys/ephys_session.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/ephys/newscale_main.csv` & `aind_metadata_mapper-0.6.3/tests/resources/ephys/newscale_main.csv`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/ephys/newscale_surface_finding.csv` & `aind_metadata_mapper-0.6.3/tests/resources/ephys/newscale_surface_finding.csv`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/ephys/settings_main.xml` & `aind_metadata_mapper-0.6.3/tests/resources/ephys/settings_main.xml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/ephys/settings_surface_finding.xml` & `aind_metadata_mapper-0.6.3/tests/resources/ephys/settings_surface_finding.xml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/fib/000000_ophys_rig.json` & `aind_metadata_mapper-0.6.3/tests/resources/fib/000000_ophys_rig.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/fib/000000_ophys_session.json` & `aind_metadata_mapper-0.6.3/tests/resources/fib/000000_ophys_session.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json` & `aind_metadata_mapper-0.6.3/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json` & `aind_metadata_mapper-0.6.3/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/mesoscope/0123456789_Face_20240212T091444.json` & `aind_metadata_mapper-0.6.3/tests/resources/mesoscope/0123456789_Face_20240212T091444.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/mesoscope/example_extract.json` & `aind_metadata_mapper-0.6.3/tests/resources/mesoscope/example_extract.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/mesoscope/example_platform.json` & `aind_metadata_mapper-0.6.3/tests/resources/mesoscope/example_platform.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/mesoscope/expected_session.json` & `aind_metadata_mapper-0.6.3/tests/resources/mesoscope/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/neuropixels/base-missing-probe_rig.json` & `aind_metadata_mapper-0.6.3/tests/resources/neuropixels/mvr_rig.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9884634888438133%*

 * *Differences: {"'cameras'": "{0: {'camera': {'serial_number': '50-0536905703', 'recording_software': {replace: "*

 * *              "OrderedDict([('name', 'MVR'), ('version', 'Not detected/provided.'), ('url', None), "*

 * *              "('parameters', OrderedDict())])}}}, 1: {'camera': {'serial_number': "*

 * *              "'50-0536876074', 'recording_software': {replace: OrderedDict([('name', 'MVR'), "*

 * *              "('version', 'Not detected/provided.'), ('url', None), ('parameters', "*

 * *              "OrderedDict())])}}}, 2: {'came […]*

```diff
@@ -71,20 +71,25 @@
                 },
                 "max_frame_rate": "102",
                 "model": "G-032",
                 "name": "Forward camera",
                 "notes": "Max frame rate is at maximum resolution.",
                 "path_to_cad": null,
                 "port_index": null,
-                "recording_software": null,
+                "recording_software": {
+                    "name": "MVR",
+                    "parameters": {},
+                    "url": null,
+                    "version": "Not detected/provided."
+                },
                 "sensor_format": null,
                 "sensor_format_unit": null,
                 "sensor_height": 7400,
                 "sensor_width": 7400,
-                "serial_number": null,
+                "serial_number": "50-0536905703",
                 "size_unit": "nanometer"
             },
             "camera_target": "Face forward",
             "filter": {
                 "additional_settings": {},
                 "center_wavelength": null,
                 "cut_off_wavelength": null,
@@ -213,20 +218,25 @@
                 },
                 "max_frame_rate": "102",
                 "model": "G-032",
                 "name": "Side camera",
                 "notes": "Max frame rate is at maximum resolution.",
                 "path_to_cad": null,
                 "port_index": null,
-                "recording_software": null,
+                "recording_software": {
+                    "name": "MVR",
+                    "parameters": {},
+                    "url": null,
+                    "version": "Not detected/provided."
+                },
                 "sensor_format": null,
                 "sensor_format_unit": null,
                 "sensor_height": 7400,
                 "sensor_width": 7400,
-                "serial_number": null,
+                "serial_number": "50-0536876074",
                 "size_unit": "nanometer"
             },
             "camera_target": "Body",
             "filter": {
                 "additional_settings": {},
                 "center_wavelength": null,
                 "cut_off_wavelength": null,
@@ -352,20 +362,25 @@
                 },
                 "max_frame_rate": "102",
                 "model": "G-032",
                 "name": "Eye camera",
                 "notes": "Max frame rate is at maximum resolution.",
                 "path_to_cad": null,
                 "port_index": null,
-                "recording_software": null,
+                "recording_software": {
+                    "name": "MVR",
+                    "parameters": {},
+                    "url": null,
+                    "version": "Not detected/provided."
+                },
                 "sensor_format": null,
                 "sensor_format_unit": null,
                 "sensor_height": 7400,
                 "sensor_width": 7400,
-                "serial_number": null,
+                "serial_number": "50-0536905703",
                 "size_unit": "nanometer"
             },
             "camera_target": "Eye",
             "filter": {
                 "additional_settings": {},
                 "center_wavelength": null,
                 "cut_off_wavelength": null,
@@ -821,14 +836,57 @@
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
                     "serial_number": null
                 }
             ]
+        },
+        {
+            "manipulator": {
+                "additional_settings": {},
+                "device_type": "Manipulator",
+                "manufacturer": {
+                    "abbreviation": null,
+                    "name": "New Scale Technologies",
+                    "registry": null,
+                    "registry_identifier": null
+                },
+                "model": "06591-M-0004",
+                "name": "Ephys Assembly F Manipulator",
+                "notes": null,
+                "path_to_cad": null,
+                "port_index": null,
+                "serial_number": null
+            },
+            "name": "Ephys Assembly F",
+            "probes": [
+                {
+                    "additional_settings": {},
+                    "device_type": "Ephys probe",
+                    "headstage": null,
+                    "lasers": [],
+                    "manufacturer": {
+                        "abbreviation": "IMEC",
+                        "name": "Interuniversity Microelectronics Center",
+                        "registry": {
+                            "abbreviation": "ROR",
+                            "name": "Research Organization Registry"
+                        },
+                        "registry_identifier": "02kcbn207"
+                    },
+                    "model": null,
+                    "name": "ProbeF",
+                    "notes": null,
+                    "path_to_cad": null,
+                    "port_index": null,
+                    "probe_model": "Neuropixels 1.0",
+                    "serial_number": null
+                }
+            ]
         }
     ],
     "fiber_assemblies": [],
     "filters": [],
     "laser_assemblies": [],
     "lenses": [],
     "light_sources": [
@@ -936,24 +994,24 @@
             "serial_number": null,
             "wavelength": 633,
             "wavelength_unit": "nanometer"
         }
     ],
     "modalities": [
         {
+            "abbreviation": "behavior",
+            "name": "Behavior"
+        },
+        {
             "abbreviation": "behavior-videos",
             "name": "Behavior videos"
         },
         {
             "abbreviation": "ecephys",
             "name": "Extracellular electrophysiology"
-        },
-        {
-            "abbreviation": "behavior",
-            "name": "Behavior"
         }
     ],
     "modification_date": "2024-04-01",
     "mouse_platform": {
         "additional_settings": {},
         "date_surface_replaced": null,
         "decoder": null,
```

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/neuropixels/base_rig.json` & `aind_metadata_mapper-0.6.3/tests/resources/neuropixels/open-ephys-inferred_rig.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9909802043422732%*

 * *Differences: {"'ephys_assemblies'": "{0: {'manipulator': {'serial_number': 'SN45356'}, 'probes': {0: "*

 * *                       "{'serial_number': '18005114152', 'model': 'Neuropixels 1.0'}}}, 1: "*

 * *                       "{'manipulator': {'serial_number': 'SN45484'}, 'probes': {0: "*

 * *                       "{'serial_number': '18005114151', 'model': 'Neuropixels 1.0'}}}, 2: "*

 * *                       "{'manipulator': {'serial_number': 'SN45485'}, 'probes': {0: "*

 * *                       "{'serial_number': '18005102491', 'model' […]*

```diff
@@ -622,15 +622,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly A Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": null
+                "serial_number": "SN45356"
             },
             "name": "Ephys Assembly A",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -640,21 +640,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": null,
+                    "model": "Neuropixels 1.0",
                     "name": "ProbeA",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": null
+                    "serial_number": "18005114152"
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -665,15 +665,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly B Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": null
+                "serial_number": "SN45484"
             },
             "name": "Ephys Assembly B",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -683,21 +683,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": null,
+                    "model": "Neuropixels 1.0",
                     "name": "ProbeB",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": null
+                    "serial_number": "18005114151"
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -708,15 +708,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly C Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": null
+                "serial_number": "SN45485"
             },
             "name": "Ephys Assembly C",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -726,21 +726,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": null,
+                    "model": "Neuropixels 1.0",
                     "name": "ProbeC",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": null
+                    "serial_number": "18005102491"
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -751,15 +751,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly D Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": null
+                "serial_number": "SN45359"
             },
             "name": "Ephys Assembly D",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -769,21 +769,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": null,
+                    "model": "Neuropixels 1.0",
                     "name": "ProbeD",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": null
+                    "serial_number": "19192719021"
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -794,15 +794,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly E Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": null
+                "serial_number": "SN45482"
             },
             "name": "Ephys Assembly E",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -812,21 +812,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": null,
+                    "model": "Neuropixels 1.0",
                     "name": "ProbeE",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": null
+                    "serial_number": "18005114452"
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -837,15 +837,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly F Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": null
+                "serial_number": "SN45361"
             },
             "name": "Ephys Assembly F",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -855,21 +855,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": null,
+                    "model": "Neuropixels 1.0",
                     "name": "ProbeF",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": null
+                    "serial_number": "19192719061"
                 }
             ]
         }
     ],
     "fiber_assemblies": [],
     "filters": [],
     "laser_assemblies": [],
@@ -979,24 +979,24 @@
             "serial_number": null,
             "wavelength": 633,
             "wavelength_unit": "nanometer"
         }
     ],
     "modalities": [
         {
+            "abbreviation": "behavior",
+            "name": "Behavior"
+        },
+        {
             "abbreviation": "behavior-videos",
             "name": "Behavior videos"
         },
         {
             "abbreviation": "ecephys",
             "name": "Extracellular electrophysiology"
-        },
-        {
-            "abbreviation": "behavior",
-            "name": "Behavior"
         }
     ],
     "modification_date": "2024-04-01",
     "mouse_platform": {
         "additional_settings": {},
         "date_surface_replaced": null,
         "decoder": null,
```

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/neuropixels/mvr.ini` & `aind_metadata_mapper-0.6.3/tests/resources/neuropixels/mvr.ini`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/neuropixels/mvr_rig.json` & `aind_metadata_mapper-0.6.3/tests/resources/neuropixels/open-ephys_rig.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995586357148223%*

 * *Differences: {"'cameras'": "{0: {'camera': {'serial_number': None, 'recording_software': None}}, 1: {'camera': "*

 * *              "{'serial_number': None, 'recording_software': None}}, 2: {'camera': "*

 * *              "{'serial_number': None, 'recording_software': None}}}",*

 * * "'ephys_assemblies'": "{0: {'manipulator': {'serial_number': 'SN45356'}, 'probes': {0: "*

 * *                       "{'serial_number': '19192719051', 'model': 'Neuropixels 1.0'}}}, 1: "*

 * *                       "{'manipulator': {'serial_number': 'SN45484'}, 'pr […]*

```diff
@@ -71,25 +71,20 @@
                 },
                 "max_frame_rate": "102",
                 "model": "G-032",
                 "name": "Forward camera",
                 "notes": "Max frame rate is at maximum resolution.",
                 "path_to_cad": null,
                 "port_index": null,
-                "recording_software": {
-                    "name": "MVR",
-                    "parameters": {},
-                    "url": null,
-                    "version": "Not detected/provided."
-                },
+                "recording_software": null,
                 "sensor_format": null,
                 "sensor_format_unit": null,
                 "sensor_height": 7400,
                 "sensor_width": 7400,
-                "serial_number": "50-0536905703",
+                "serial_number": null,
                 "size_unit": "nanometer"
             },
             "camera_target": "Face forward",
             "filter": {
                 "additional_settings": {},
                 "center_wavelength": null,
                 "cut_off_wavelength": null,
@@ -218,25 +213,20 @@
                 },
                 "max_frame_rate": "102",
                 "model": "G-032",
                 "name": "Side camera",
                 "notes": "Max frame rate is at maximum resolution.",
                 "path_to_cad": null,
                 "port_index": null,
-                "recording_software": {
-                    "name": "MVR",
-                    "parameters": {},
-                    "url": null,
-                    "version": "Not detected/provided."
-                },
+                "recording_software": null,
                 "sensor_format": null,
                 "sensor_format_unit": null,
                 "sensor_height": 7400,
                 "sensor_width": 7400,
-                "serial_number": "50-0536876074",
+                "serial_number": null,
                 "size_unit": "nanometer"
             },
             "camera_target": "Body",
             "filter": {
                 "additional_settings": {},
                 "center_wavelength": null,
                 "cut_off_wavelength": null,
@@ -362,25 +352,20 @@
                 },
                 "max_frame_rate": "102",
                 "model": "G-032",
                 "name": "Eye camera",
                 "notes": "Max frame rate is at maximum resolution.",
                 "path_to_cad": null,
                 "port_index": null,
-                "recording_software": {
-                    "name": "MVR",
-                    "parameters": {},
-                    "url": null,
-                    "version": "Not detected/provided."
-                },
+                "recording_software": null,
                 "sensor_format": null,
                 "sensor_format_unit": null,
                 "sensor_height": 7400,
                 "sensor_width": 7400,
-                "serial_number": "50-0536905703",
+                "serial_number": null,
                 "size_unit": "nanometer"
             },
             "camera_target": "Eye",
             "filter": {
                 "additional_settings": {},
                 "center_wavelength": null,
                 "cut_off_wavelength": null,
@@ -637,15 +622,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly A Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": null
+                "serial_number": "SN45356"
             },
             "name": "Ephys Assembly A",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -655,21 +640,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": null,
+                    "model": "Neuropixels 1.0",
                     "name": "ProbeA",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": null
+                    "serial_number": "19192719051"
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -680,15 +665,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly B Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": null
+                "serial_number": "SN45484"
             },
             "name": "Ephys Assembly B",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -698,21 +683,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": null,
+                    "model": "Neuropixels 1.0",
                     "name": "ProbeB",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": null
+                    "serial_number": "19192719091"
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -723,15 +708,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly C Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": null
+                "serial_number": "SN45485"
             },
             "name": "Ephys Assembly C",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -741,21 +726,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": null,
+                    "model": "Neuropixels 1.0",
                     "name": "ProbeC",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": null
+                    "serial_number": "19192719721"
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -766,15 +751,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly D Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": null
+                "serial_number": "SN45359"
             },
             "name": "Ephys Assembly D",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -784,21 +769,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": null,
+                    "model": "Neuropixels 1.0",
                     "name": "ProbeD",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": null
+                    "serial_number": "18005117641"
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -809,15 +794,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly E Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": null
+                "serial_number": "SN45482"
             },
             "name": "Ephys Assembly E",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -827,21 +812,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": null,
+                    "model": "Neuropixels 1.0",
                     "name": "ProbeE",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": null
+                    "serial_number": "18005107542"
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -852,15 +837,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly F Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": null
+                "serial_number": "SN45361"
             },
             "name": "Ephys Assembly F",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -870,21 +855,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": null,
+                    "model": "Neuropixels 1.0",
                     "name": "ProbeF",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": null
+                    "serial_number": "19192719101"
                 }
             ]
         }
     ],
     "fiber_assemblies": [],
     "filters": [],
     "laser_assemblies": [],
```

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/neuropixels/open-ephys-inferred_rig.json` & `aind_metadata_mapper-0.6.3/tests/resources/neuropixels/sync_rig.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994469531107462%*

 * *Differences: {"'daqs'": "{0: {'channels': [OrderedDict([('channel_name', 'barcode_ephys'), ('device_name', "*

 * *           "'Sync'), ('channel_type', 'Digital Input'), ('port', None), ('channel_index', 0), "*

 * *           "('sample_rate', '100000.0'), ('sample_rate_unit', 'hertz'), ('event_based_sampling', "*

 * *           "False)]), OrderedDict([('channel_name', 'vsync_stim'), ('device_name', 'Sync'), "*

 * *           "('channel_type', 'Digital Input'), ('port', None), ('channel_index', 2), "*

 * *           "('sample_rate', '100000.0'), […]*

```diff
@@ -462,15 +462,176 @@
             }
         }
     ],
     "ccf_coordinate_transform": null,
     "daqs": [
         {
             "additional_settings": {},
-            "channels": [],
+            "channels": [
+                {
+                    "channel_index": 0,
+                    "channel_name": "barcode_ephys",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 2,
+                    "channel_name": "vsync_stim",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 4,
+                    "channel_name": "stim_photodiode",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 5,
+                    "channel_name": "stim_running",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 8,
+                    "channel_name": "beh_frame_received",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 9,
+                    "channel_name": "eye_frame_received",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 10,
+                    "channel_name": "face_frame_received",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 17,
+                    "channel_name": "stim_running_opto",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 18,
+                    "channel_name": "stim_trial_opto",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 21,
+                    "channel_name": "beh_cam_frame_readout",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 22,
+                    "channel_name": "face_cam_frame_readout",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 25,
+                    "channel_name": "eye_cam_frame_readout",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 27,
+                    "channel_name": "beh_cam_exposing",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 28,
+                    "channel_name": "face_cam_exposing",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 29,
+                    "channel_name": "eye_cam_exposing",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                },
+                {
+                    "channel_index": 31,
+                    "channel_name": "lick_sensor",
+                    "channel_type": "Digital Input",
+                    "device_name": "Sync",
+                    "event_based_sampling": false,
+                    "port": null,
+                    "sample_rate": "100000.0",
+                    "sample_rate_unit": "hertz"
+                }
+            ],
             "computer_name": "127.0.0.1",
             "data_interface": "PCIe",
             "device_type": "DAQ Device",
             "firmware_version": null,
             "hardware_version": null,
             "manufacturer": {
                 "abbreviation": null,
@@ -622,15 +783,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly A Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": "SN45356"
+                "serial_number": null
             },
             "name": "Ephys Assembly A",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -640,21 +801,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": "Neuropixels 1.0",
+                    "model": null,
                     "name": "ProbeA",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": "18005114152"
+                    "serial_number": null
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -665,15 +826,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly B Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": "SN45484"
+                "serial_number": null
             },
             "name": "Ephys Assembly B",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -683,21 +844,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": "Neuropixels 1.0",
+                    "model": null,
                     "name": "ProbeB",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": "18005114151"
+                    "serial_number": null
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -708,15 +869,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly C Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": "SN45485"
+                "serial_number": null
             },
             "name": "Ephys Assembly C",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -726,21 +887,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": "Neuropixels 1.0",
+                    "model": null,
                     "name": "ProbeC",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": "18005102491"
+                    "serial_number": null
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -751,15 +912,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly D Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": "SN45359"
+                "serial_number": null
             },
             "name": "Ephys Assembly D",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -769,21 +930,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": "Neuropixels 1.0",
+                    "model": null,
                     "name": "ProbeD",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": "19192719021"
+                    "serial_number": null
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -794,15 +955,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly E Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": "SN45482"
+                "serial_number": null
             },
             "name": "Ephys Assembly E",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -812,21 +973,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": "Neuropixels 1.0",
+                    "model": null,
                     "name": "ProbeE",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": "18005114452"
+                    "serial_number": null
                 }
             ]
         },
         {
             "manipulator": {
                 "additional_settings": {},
                 "device_type": "Manipulator",
@@ -837,15 +998,15 @@
                     "registry_identifier": null
                 },
                 "model": "06591-M-0004",
                 "name": "Ephys Assembly F Manipulator",
                 "notes": null,
                 "path_to_cad": null,
                 "port_index": null,
-                "serial_number": "SN45361"
+                "serial_number": null
             },
             "name": "Ephys Assembly F",
             "probes": [
                 {
                     "additional_settings": {},
                     "device_type": "Ephys probe",
                     "headstage": null,
@@ -855,21 +1016,21 @@
                         "name": "Interuniversity Microelectronics Center",
                         "registry": {
                             "abbreviation": "ROR",
                             "name": "Research Organization Registry"
                         },
                         "registry_identifier": "02kcbn207"
                     },
-                    "model": "Neuropixels 1.0",
+                    "model": null,
                     "name": "ProbeF",
                     "notes": null,
                     "path_to_cad": null,
                     "port_index": null,
                     "probe_model": "Neuropixels 1.0",
-                    "serial_number": "19192719061"
+                    "serial_number": null
                 }
             ]
         }
     ],
     "fiber_assemblies": [],
     "filters": [],
     "laser_assemblies": [],
```

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/neuropixels/settings.mislabeled-probes-0.xml` & `aind_metadata_mapper-0.6.3/tests/resources/neuropixels/settings.mislabeled-probes-0.xml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/neuropixels/settings.mislabeled-probes-1.xml` & `aind_metadata_mapper-0.6.3/tests/resources/neuropixels/settings.mislabeled-probes-1.xml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/neuropixels/settings.xml` & `aind_metadata_mapper-0.6.3/tests/resources/neuropixels/settings.xml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/resources/neuropixels/sync.yml` & `aind_metadata_mapper-0.6.3/tests/resources/neuropixels/sync.yml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/test_bergamo.py` & `aind_metadata_mapper-0.6.3/tests/test_bergamo.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/test_ephys.py` & `aind_metadata_mapper-0.6.3/tests/test_ephys.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     RESOURCES_DIR / "settings_main.xml",
     RESOURCES_DIR / "settings_surface_finding.xml",
 ]
 
 EXPECTED_SESSION = RESOURCES_DIR / "ephys_session.json"
 
 
-class TestSchemaWriter(unittest.TestCase):
-    """Test methods in SchemaWriter class."""
+class TestEphysSession(unittest.TestCase):
+    """Test methods in ephys session module."""
 
     maxDiff = None  # show full diff without truncation
 
     @classmethod
     def setUpClass(cls):
         """Load record object and user settings before running tests."""
         # TODO: Add visual stimulus
```

### Comparing `aind-metadata-mapper-0.6.2/tests/test_fib.py` & `aind_metadata_mapper-0.6.3/tests/test_fib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Tests parsing of session information from fib rig."""
 
-import zoneinfo
 import json
 import os
 import unittest
+import zoneinfo
 from datetime import datetime
 from pathlib import Path
 
 from aind_data_schema.core.session import Session
 
 from aind_metadata_mapper.fib.session import FIBEtl, JobSettings
 
@@ -119,9 +119,8 @@
         job = etl_job1.run_job()
         self.assertEqual(
             self.expected_session, Session(**json.loads(job.data))
         )
 
 
 if __name__ == "__main__":
-
     unittest.main()
```

### Comparing `aind-metadata-mapper-0.6.2/tests/test_legacy_core.py` & `aind_metadata_mapper-0.6.3/tests/test_legacy_core.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.2/tests/test_mesoscope.py` & `aind_metadata_mapper-0.6.3/tests/test_mesoscope.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,23 +172,23 @@
         # mock vasculature image
         mock_image = Image.new("RGB", (100, 100))
         mock_image.tag = {306: ("2024:02:12 11:02:22",)}
         mock_open.return_value = mock_image
 
         # mock scanimage metadata
         mock_meta = [{}]
-        mock_meta[0]["SI.hRoiManager.linesPerFrame"] = (
-            self.example_scanimage_meta["lines_per_frame"]
-        )
-        mock_meta[0]["SI.hRoiManager.pixelsPerLine"] = (
-            self.example_scanimage_meta["pixels_per_line"]
-        )
-        mock_meta[0]["SI.hRoiManager.scanZoomFactor"] = (
-            self.example_scanimage_meta["fov_scale_factor"]
-        )
+        mock_meta[0][
+            "SI.hRoiManager.linesPerFrame"
+        ] = self.example_scanimage_meta["lines_per_frame"]
+        mock_meta[0][
+            "SI.hRoiManager.pixelsPerLine"
+        ] = self.example_scanimage_meta["pixels_per_line"]
+        mock_meta[0][
+            "SI.hRoiManager.scanZoomFactor"
+        ] = self.example_scanimage_meta["fov_scale_factor"]
         mock_scanimage.return_value = mock_meta
 
         extract = etl._extract()
         transformed_session = etl._transform(extract)
         for stream in transformed_session.data_streams:
             stream.stream_start_time = stream.stream_start_time.replace(
                 tzinfo=zoneinfo.ZoneInfo("UTC")
```

### Comparing `aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_mvr_rig.py` & `aind_metadata_mapper-0.6.3/tests/test_neuropixels/test_mvr_rig.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,16 @@
                 "Camera 1": test_utils.SIDE_CAMERA_ASSEMBLY_NAME,
                 "Camera 2": test_utils.EYE_CAMERA_ASSEMBLY_NAME,
                 "Camera 3": test_utils.FORWARD_CAMERA_ASSEMBLY_NAME,
             },
         )
         etl.run_job()
         mock_write_standard_file.assert_called_once_with(
-            output_directory=self.output_dir)
+            output_directory=self.output_dir
+        )
 
     @patch("aind_data_schema.base.AindCoreModel.write_standard_file")
     def test_run_job_bad_mapping(self, mock_write_standard_file: MagicMock):
         """Test MVR etl workflow with bad mapping."""
         etl = MvrRigEtl(
             self.input_source,
             self.output_dir,
@@ -63,15 +64,16 @@
                 "Camera 1": test_utils.SIDE_CAMERA_ASSEMBLY_NAME,
                 "Camera 2": test_utils.EYE_CAMERA_ASSEMBLY_NAME,
                 "Not a camera name": test_utils.FORWARD_CAMERA_ASSEMBLY_NAME,
             },
         )
         etl.run_job()
         mock_write_standard_file.assert_called_once_with(
-            output_directory=self.output_dir)
+            output_directory=self.output_dir
+        )
 
     def setUp(self):
         """Sets up test resources."""
         (
             self.input_source,
             self.output_dir,
             self.expected,
```

### Comparing `aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_neuropixels_rig.py` & `aind_metadata_mapper-0.6.3/tests/test_neuropixels/test_neuropixels_rig.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Tests for the neuropixels open ephys rig ETL with inferred probe mapping."""
 
 import os
 import unittest
-from pathlib import Path
 from datetime import date
+from pathlib import Path
 
 from aind_metadata_mapper.neuropixels.neuropixels_rig import (  # type: ignore
-    NeuropixelsRigEtl
+    NeuropixelsRigEtl,
 )
 
 RESOURCES_DIR = (
     Path(os.path.dirname(os.path.realpath(__file__)))
     / ".."
     / "resources"
     / "neuropixels"
```

### Comparing `aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_open_ephys_rig.py` & `aind_metadata_mapper-0.6.3/tests/test_neuropixels/test_open_ephys_rig.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 import unittest
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 from aind_metadata_mapper.neuropixels.open_ephys_rig import (  # type: ignore
-    OpenEphysRigEtl
+    OpenEphysRigEtl,
 )
 from tests.test_neuropixels import utils as test_utils
 
 RESOURCES_DIR = (
     Path(os.path.dirname(os.path.realpath(__file__)))
     / ".."
     / "resources"
@@ -96,15 +96,16 @@
                     "SN45361",
                 ),
             ],
             modification_date=self.expected.modification_date,
         )
         etl.run_job()
         mock_write_standard_file.assert_called_once_with(
-            output_directory=self.output_dir)
+            output_directory=self.output_dir
+        )
 
     def setUp(self):
         """Sets up test resources."""
         (
             self.input_source,
             self.output_dir,
             self.expected,
```

### Comparing `aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_open_ephys_rig_inferrred.py` & `aind_metadata_mapper-0.6.3/tests/test_neuropixels/test_open_ephys_rig_inferrred.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import unittest
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 from aind_metadata_mapper.neuropixels import open_ephys_rig  # type: ignore
 from aind_metadata_mapper.neuropixels.open_ephys_rig import (  # type: ignore
-    OpenEphysRigEtl
+    OpenEphysRigEtl,
 )
 from tests.test_neuropixels import utils as test_utils
 
 RESOURCES_DIR = (
     Path(os.path.dirname(os.path.realpath(__file__)))
     / ".."
     / "resources"
@@ -99,20 +99,20 @@
                     "SN45361",
                 ),
             ],
             modification_date=self.expected.modification_date,
         )
         etl.run_job()
         mock_write_standard_file.assert_called_once_with(
-            output_directory=self.output_dir)
+            output_directory=self.output_dir
+        )
 
     @patch("aind_data_schema.base.AindCoreModel.write_standard_file")
     def test_etl_mismatched_probe_count(
-        self,
-        mock_write_standard_file: MagicMock
+        self, mock_write_standard_file: MagicMock
     ):
         """Test ETL workflow with mismatched probe count."""
         etl = open_ephys_rig.OpenEphysRigEtl(
             RESOURCES_DIR / "base-missing-probe_rig.json",
             self.output_dir,
             open_ephys_settings_sources=[
                 RESOURCES_DIR / "settings.mislabeled-probes-0.xml",
@@ -144,15 +144,16 @@
                     "SN45361",
                 ),
             ],
             modification_date=self.expected.modification_date,
         )
         etl.run_job()
         mock_write_standard_file.assert_called_once_with(
-            output_directory=self.output_dir)
+            output_directory=self.output_dir
+        )
 
     def setUp(self):
         """Sets up test resources."""
         (
             self.input_source,
             self.output_dir,
             self.expected,
```

### Comparing `aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_sync_rig.py` & `aind_metadata_mapper-0.6.3/tests/test_neuropixels/test_sync_rig.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         etl = SyncRigEtl(
             self.input_source,
             self.output_dir,
             RESOURCES_DIR / "sync.yml",
         )
         etl.run_job()
         mock_write_standard_file.assert_called_once_with(
-            output_directory=self.output_dir)
+            output_directory=self.output_dir
+        )
 
     def setUp(self):
         """Sets up test resources."""
         (
             self.input_source,
             self.output_dir,
             self.expected,
```

### Comparing `aind-metadata-mapper-0.6.2/tests/test_neuropixels/utils.py` & `aind_metadata_mapper-0.6.3/tests/test_neuropixels/utils.py`

 * *Files identical despite different names*

