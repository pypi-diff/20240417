# Comparing `tmp/depthcharge-ms-0.3.1.tar.gz` & `tmp/depthcharge_ms-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depthcharge-ms-0.3.1.tar", last modified: Sat Aug 19 04:03:22 2023, max compression
+gzip compressed data, was "depthcharge_ms-0.4.0.tar", last modified: Wed Apr 17 20:34:40 2024, max compression
```

## Comparing `depthcharge-ms-0.3.1.tar` & `depthcharge_ms-0.4.0.tar`

### file list

```diff
@@ -1,89 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.695894 depthcharge-ms-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.679893 depthcharge-ms-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.683894 depthcharge-ms-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-19 04:03:22.695894 depthcharge-ms-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.683894 depthcharge-ms-0.3.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/data/TMT10-Trial-8.mgf
--rw-r--r--   0 runner    (1001) docker     (123)   333865 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/data/TMT10-Trial-8.mzML
--rw-r--r--   0 runner    (1001) docker     (123)    67798 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/data/TMT10-Trial-8.mzXML
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.683894 depthcharge-ms-0.3.1/depthcharge/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.687893 depthcharge-ms-0.3.1/depthcharge/data/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/data/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/data/peptide_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/data/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23991 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/data/spectrum_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.687893 depthcharge-ms-0.3.1/depthcharge/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/encoders/sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/feedforward.py
--rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.687893 depthcharge-ms-0.3.1/depthcharge/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/tokenizers/peptides.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/tokenizers/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.687893 depthcharge-ms-0.3.1/depthcharge/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/transformers/peptides.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/transformers/spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/depthcharge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.687893 depthcharge-ms-0.3.1/depthcharge_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-19 04:03:22.000000 depthcharge-ms-0.3.1/depthcharge_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-19 04:03:22.000000 depthcharge-ms-0.3.1/depthcharge_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-19 04:03:22.000000 depthcharge-ms-0.3.1/depthcharge_ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-19 04:03:22.000000 depthcharge-ms-0.3.1/depthcharge_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-19 04:03:22.000000 depthcharge-ms-0.3.1/depthcharge_ms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.687893 depthcharge-ms-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/docs/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.691893 depthcharge-ms-0.3.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/docs/api/datasets.md
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/docs/api/encoders.md
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/docs/api/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/docs/api/primitives.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/docs/api/tokenizers.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/docs/api/transformers.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.691893 depthcharge-ms-0.3.1/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.691893 depthcharge-ms-0.3.1/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-19 04:03:22.695894 depthcharge-ms-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.691893 depthcharge-ms-0.3.1/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    50058 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    46385 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/static/logo-light.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.691893 depthcharge-ms-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.691893 depthcharge-ms-0.3.1/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.691893 depthcharge-ms-0.3.1/tests/unit_tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/tests/unit_tests/test_data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/tests/unit_tests/test_data/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/tests/unit_tests/test_data/test_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.691893 depthcharge-ms-0.3.1/tests/unit_tests/test_encoders/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/tests/unit_tests/test_encoders/test_sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/tests/unit_tests/test_feedforward.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/tests/unit_tests/test_primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.691893 depthcharge-ms-0.3.1/tests/unit_tests/test_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/tests/unit_tests/test_tokenizers/test_peptides.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 04:03:22.691893 depthcharge-ms-0.3.1/tests/unit_tests/test_transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/tests/unit_tests/test_transformers/test_peptide_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/tests/unit_tests/test_transformers/test_spectrum_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-19 04:02:59.000000 depthcharge-ms-0.3.1/tests/unit_tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.511023 depthcharge_ms-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.515023 depthcharge_ms-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.515023 depthcharge_ms-0.4.0/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/data/TMT10-Trial-8.mgf
+-rw-r--r--   0 runner    (1001) docker     (127)   333839 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/data/TMT10-Trial-8.mzML
+-rw-r--r--   0 runner    (1001) docker     (127)    67798 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/data/TMT10-Trial-8.mzXML
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.519024 depthcharge_ms-0.4.0/depthcharge/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.519024 depthcharge_ms-0.4.0/depthcharge/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/analyte_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11974 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18908 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18318 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/spectrum_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.519024 depthcharge_ms-0.4.0/depthcharge/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/encoders/sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.519024 depthcharge_ms-0.4.0/depthcharge/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/tokenizers/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/tokenizers/peptides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/tokenizers/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.519024 depthcharge_ms-0.4.0/depthcharge/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/transformers/analytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/transformers/spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/depthcharge_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-17 20:34:40.000000 depthcharge_ms-0.4.0/depthcharge_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-17 20:34:40.000000 depthcharge_ms-0.4.0/depthcharge_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:34:40.000000 depthcharge_ms-0.4.0/depthcharge_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-17 20:34:40.000000 depthcharge_ms-0.4.0/depthcharge_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 20:34:40.000000 depthcharge_ms-0.4.0/depthcharge_ms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.523023 depthcharge_ms-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.523023 depthcharge_ms-0.4.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/api/datasets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/api/encoders.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/api/primitives.md
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/api/tokenizers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/api/transformers.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.523023 depthcharge_ms-0.4.0/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.523023 depthcharge_ms-0.4.0/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.523023 depthcharge_ms-0.4.0/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    50058 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46385 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/static/logo-light.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.523023 depthcharge_ms-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/tests/unit_tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_data/test_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_data/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_data/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/tests/unit_tests/test_encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_encoders/test_sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/tests/unit_tests/test_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_tokenizers/test_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_tokenizers/test_peptides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/tests/unit_tests/test_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_transformers/test_analyte_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_transformers/test_spectrum_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_version.py
```

### Comparing `depthcharge-ms-0.3.1/.github/workflows/lint.yml` & `depthcharge_ms-0.4.0/.github/workflows/tests.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-name: Lint
+name: tests
 
 on:
   push:
     branches: [ main ]
   pull_request:
     branches: [ main ]
 
 jobs:
-  lint:
-    runs-on: ubuntu-latest
+  build:
+    runs-on: ${{ matrix.os }}
+    strategy:
+      matrix:
+        os: [ubuntu-latest, windows-latest, macos-latest]
+
     steps:
-      - uses: actions/checkout@v3
-      - name: Setup Python 3.10
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.10"
-
-      - name: Install Ruff
-        run: |
-          python -m pip install --upgrade pip
-          pip install ruff
-
-      - name: Run black
-        uses: psf/black@stable
-
-      - name: Lint with Ruff
-        run: |
-          ruff check . --format=github
-
-      - name: Check for debugging print statements
-        run: |
-          if grep -rq "print(" depthcharge; then
-              echo "Found the following print statements:"
-              grep -r "print(" deptchcharge
-              exit 1
-          fi
+    - uses: actions/checkout@v3
+    - name: Set up Python 3.10
+      uses: actions/setup-python@v4
+      with:
+        python-version: "3.10"
+
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        pip install pytest pytest-cov wheel
+        pip install -e .
+
+    - name: Run unit and system tests
+      run: |
+        pytest --cov=depthcharge --verbose tests/
+
+    - name: Upload coverage to codecov
+      uses: codecov/codecov-action@v3
+      with:
+        token: ${{ secrets.CODECOV_TOKEN }}
+        fail_ci_if_error: true
```

### Comparing `depthcharge-ms-0.3.1/.github/workflows/publish.yml` & `depthcharge_ms-0.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/CHANGELOG.md` & `depthcharge_ms-0.4.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,41 @@
-# Changelog for depthcharge
+# Changelog for Depthcharge
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v0.4.0]
+
+We have completely reworked of the data module.
+Depthcharge now uses Apache Arrow-based formats instead of HDF5; spectra are converted either Parquet or streamed with PyArrow, optionally into Lance datasets.
+
+We now also have full support for small molecules, with the `MoleculeTokenizer`,
+`AnalyteTransformerEncoder`, and `AnalyteTransformerDecoder` classes.
+
+### Breaking Changes
+- `PeptideTransformer*` are now `AnalyteTransformer*`, providing full support for small molecule analytes. Additionally the interface has been completely reworked.
+- Mass spectrometry data parsers now function as iterators, yielding batches of spectra as `pyarrow.RecordBatch` objects.
+- Parsers can now be told to read arbitrary fields from their respective file formats with the `custom_fields` parameter.
+- The parsing functionality of `SpctrumDataset` and its subclasses have been moved to the `spectra_to_*` functions in the data module.
+- `SpectrumDataset` and its subclasses now return dictionaries of data rather than a tuple of data. This allows us to incorporate arbitrary additional data
+- `SpectrumDataset` and its subclasses are now `lance.torch.data.LanceDataset` subclasses, providing native PyTorch integration.
+- All dataset classes now do not have a `loader()` method.
+
+### Added
+- Support for small molecules.
+- Added the `StreamingSpectrumDataset` for fast inference.
+- Added `spectra_to_df`, `spectra_to_df`, `spectra_to_stream` to the `depthcharge.data` module.
+
+### Changed
+- Determining the mass spectrometry data file format is now less fragile.
+  It now looks for known line contents, rather than relying on the extension.
+
 ## [v0.3.1] - 2023-08-18
 ### Added
 - Support for fine-tuning the wavelengths used for encoding floating point numbers like m/z and intensity to the `FloatEncoder` and `PeakEncoder`.
 
 ### Fixed
 - The `tgt_mask` in the `PeptideTransformerDecoder` was the incorrect type.
   Now it is `bool` as it should be.
@@ -25,14 +51,17 @@
 - Tight integration with `spectrum_utils` 💪
 
 ### Changed
 - Moving preprocessing onto parsing instead of data loading (similar to @bittremieux's proposal in #31)
 - Combining the SpectrumIndex and SpectrumDataset classes into one.
 - Changing peak encodings. Instead of encoding the intensity using a linear projection and summing with the sinusoidal m/z encodings, now the intensity is also sinusoidally encoded and is combined with the sinusoidal m/z encodings using a linear layer.
 
+## [v0.2.3] - 2023-08-18
+### Fixed
+- Applied hotfix from v0.3.1
 
 ## [v0.2.2] - 2023-05-15
 ### Fixed
 - Fixed retrieving version information.
 
 ## [v0.2.1] - 2023-05-13
 ### Changed
```

### Comparing `depthcharge-ms-0.3.1/CODE_OF_CONDUCT.md` & `depthcharge_ms-0.4.0/CODE_OF_CONDUCT.md`

 * *Files 0% similar despite different names*

```diff
@@ -116,8 +116,7 @@
 
 This Code of Conduct is adapted from the [Contributor Covenant][homepage],
 version 2.0, available at
 [https://www.contributor-covenant.org/version/2/0/code_of_conduct.html][v2.0].
 
 [homepage]: https://www.contributor-covenant.org
 [v2.0]: https://www.contributor-covenant.org/version/2/0/code_of_conduct.html
-
```

### Comparing `depthcharge-ms-0.3.1/CONTRIBUTING.md` & `depthcharge_ms-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/LICENSE` & `depthcharge_ms-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/README.md` & `depthcharge_ms-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/data/TMT10-Trial-8.mgf` & `depthcharge_ms-0.4.0/data/TMT10-Trial-8.mgf`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/data/TMT10-Trial-8.mzML` & `depthcharge_ms-0.4.0/data/TMT10-Trial-8.mzML`

 * *Files 0% similar despite different names*

#### Comparing `depthcharge-ms-0.3.1/data/TMT10-Trial-8.mzML` & `depthcharge_ms-0.4.0/data/TMT10-Trial-8.mzML`

```diff
@@ -79,15 +79,15 @@
         <processingMethod order="0" softwareRef="pwiz_3.0.9987">
           <cvParam cvRef="MS" accession="MS:1000544" name="Conversion to mzML" value=""/>
         </processingMethod>
       </dataProcessing>
     </dataProcessingList>
     <run id="TMT10-Trial-8" defaultInstrumentConfigurationRef="IC1" startTimeStamp="2018-01-26T22:53:26.1262695Z" defaultSourceFileRef="RAW1">
       <spectrumList count="11" defaultDataProcessingRef="pwiz_Reader_conversion">
-        <spectrum index="0" id="controllerType=0 controllerNumber=1 scan=500" defaultArrayLength="483">
+        <spectrum index="0" id="index=500" defaultArrayLength="483">
           <cvParam cvRef="MS" accession="MS:1000511" name="ms level" value="1"/>
           <cvParam cvRef="MS" accession="MS:1000579" name="MS1 spectrum" value=""/>
           <cvParam cvRef="MS" accession="MS:1000130" name="positive scan" value=""/>
           <cvParam cvRef="MS" accession="MS:1000285" name="total ion current" value="9104850"/>
           <cvParam cvRef="MS" accession="MS:1000127" name="centroid spectrum" value=""/>
           <cvParam cvRef="MS" accession="MS:1000504" name="base peak m/z" value="624.24169921875" unitCvRef="MS" unitAccession="MS:1000040" unitName="m/z"/>
           <cvParam cvRef="MS" accession="MS:1000505" name="base peak intensity" value="908558.6875" unitCvRef="MS" unitAccession="MS:1000131" unitName="number of detector counts"/>
@@ -153,15 +153,15 @@
                 <cvParam cvRef="MS" accession="MS:1000827" name="isolation window target m/z" value="804.774963378906" unitCvRef="MS" unitAccession="MS:1000040" unitName="m/z"/>
                 <cvParam cvRef="MS" accession="MS:1000828" name="isolation window lower offset" value="0.35" unitCvRef="MS" unitAccession="MS:1000040" unitName="m/z"/>
                 <cvParam cvRef="MS" accession="MS:1000829" name="isolation window upper offset" value="0.35" unitCvRef="MS" unitAccession="MS:1000040" unitName="m/z"/>
               </isolationWindow>
               <selectedIonList count="1">
                 <selectedIon>
                   <cvParam cvRef="MS" accession="MS:1000744" name="selected ion m/z" value="804.774963378906" unitCvRef="MS" unitAccession="MS:1000040" unitName="m/z"/>
-                  <cvParam cvRef="MS" accession="MS:1000041" name="charge state" value="3"/>
+                  <cvParam cvRef="MS" accession="MS:1000633" name="possible charge state" value="3"/>
                   <cvParam cvRef="MS" accession="MS:1000042" name="peak intensity" value="11531.6333007813" unitCvRef="MS" unitAccession="MS:1000131" unitName="number of detector counts"/>
                 </selectedIon>
               </selectedIonList>
               <activation>
                 <cvParam cvRef="MS" accession="MS:1000045" name="collision energy" value="35" unitCvRef="UO" unitAccession="UO:0000266" unitName="electronvolt"/>
                 <cvParam cvRef="MS" accession="MS:1000133" name="collision-induced dissociation" value=""/>
               </activation>
```

### Comparing `depthcharge-ms-0.3.1/data/TMT10-Trial-8.mzXML` & `depthcharge_ms-0.4.0/data/TMT10-Trial-8.mzXML`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/depthcharge/data/preprocessing.py` & `depthcharge_ms-0.4.0/depthcharge/data/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 SpectrumDataset(
     ...,
     preprocessing_fn=my_func,
 )
 ```
 
 """
+
 from collections.abc import Callable
 from functools import wraps
 
 import numpy as np
 
 from ..primitives import MassSpectrum
 
@@ -75,14 +76,15 @@
         **kwargs : dict
             Keyword arguments that are passed to the MsmsSpectrum method.
 
         Returns
         -------
         Callable
             A valid deptcharge preprocessing function.
+
         """
 
         @wraps(wrapper)
         def preprocess(spec: MassSpectrum) -> MassSpectrum:
             """The wrapped preprocessing function.
 
             Parameters
@@ -90,14 +92,15 @@
             spec : MassSpectrum
                 The mass spectrum to preprocess
 
             Returns
             -------
             MassSpectrum
                 The processed mass spectrum.
+
             """
             # Call the spectrum_utils method:
             getattr(spec, func)(*args, **kwargs)
             return spec
 
         return preprocess
```

### Comparing `depthcharge-ms-0.3.1/depthcharge/encoders/sinusoidal.py` & `depthcharge_ms-0.4.0/depthcharge/encoders/sinusoidal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Simple encoders for input into Transformers and the like."""
+
 import math
 
 import einops
 import numpy as np
 import torch
 
 
@@ -16,14 +17,15 @@
     min_wavelength : float, optional
         The minimum wavelength to use.
     max_wavelength : float, optional
         The maximum wavelength to use.
     learnable_wavelengths : bool, optional
         Allow the selected wavelengths to be fine-tuned
         by the model.
+
     """
 
     def __init__(
         self,
         d_model: int,
         min_wavelength: float = 0.001,
         max_wavelength: float = 10000,
@@ -67,14 +69,15 @@
         X : torch.Tensor of shape (batch_size, n_float)
             The masses to embed.
 
         Returns
         -------
         torch.Tensor of shape (batch_size, n_float, d_model)
             The encoded features for the floating point numbers.
+
         """
         sin_mz = torch.sin(X[:, :, None] / self.sin_term)
         cos_mz = torch.cos(X[:, :, None] / self.cos_term)
         return torch.cat([sin_mz, cos_mz], axis=-1)
 
 
 class PeakEncoder(torch.nn.Module):
@@ -93,14 +96,15 @@
         intensities between [0, 1].
     max_intensity_wavelength : float, optional
         The maximum wavelength to use for intensity. The default assumes
         intensities between [0, 1].
     learnable_wavelengths : bool, optional
         Allow the selected wavelengths to be fine-tuned
         by the model.
+
     """
 
     def __init__(
         self,
         d_model: int,
         min_mz_wavelength: float = 0.001,
         max_mz_wavelength: float = 10000,
@@ -142,14 +146,15 @@
             should be zero-padded, such that all of the spectra in the batch
             are the same length.
 
         Returns
         -------
         torch.Tensor of shape (n_spectra, n_peaks, d_model)
             The encoded features for the mass spectra.
+
         """
         encoded = torch.cat(
             [
                 self.mz_encoder(X[:, :, 0]),
                 self.int_encoder(X[:, :, 1]),
             ],
             dim=2,
@@ -165,14 +170,15 @@
     ----------
     d_model : int
         The number of features to output.
     min_wavelength : float, optional
         The shortest wavelength in the geometric progression.
     max_wavelength : float, optional
         The longest wavelength in the geometric progression.
+
     """
 
     def __init__(
         self,
         d_model: int,
         min_wavelength: float = 1.0,
         max_wavelength: float = 1e5,
@@ -194,14 +200,15 @@
             peptide) and the second dimension should be the sequence (i.e.
             each should be an amino acid representation).
 
         Returns
         -------
         torch.Tensor of shape (batch_size, n_sequence, n_features)
             The encoded features for the mass spectra.
+
         """
         pos = torch.arange(X.shape[1]).type_as(self.sin_term)
         pos = einops.repeat(pos, "n -> b n", b=X.shape[0])
         sin_in = einops.repeat(pos, "b n -> b n f", f=len(self.sin_term))
         cos_in = einops.repeat(pos, "b n -> b n f", f=len(self.cos_term))
 
         sin_pos = torch.sin(sin_in / self.sin_term)
```

### Comparing `depthcharge-ms-0.3.1/depthcharge/feedforward.py` & `depthcharge_ms-0.4.0/depthcharge/feedforward.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A flexible feed-forward neural network."""
+
 from collections.abc import Iterable
 
 import numpy as np
 import torch
 
 
 class FeedForward(torch.nn.Module):
@@ -21,14 +22,15 @@
     dropout : float, optionalf
         If greater than zero, add dropout layers with the specified
         probability.
     activation: torch.nn.Module, optional
         The activation function to place between layers.
     append : torch.nn.Module or None, optional
         A final layer to append, such as a sigmoid or tanh.
+
     """
 
     def __init__(
         self,
         in_features: int,
         out_features: int,
         layers: int | Iterable[int],
@@ -69,9 +71,10 @@
         X : torch.Tensor of shape (..., in_features)
             The input tensor.
 
         Returns
         -------
         torch.Tensor of shape (..., out_features)
             The output tensor.
+
         """
         return self.layers(X)
```

### Comparing `depthcharge-ms-0.3.1/depthcharge/primitives.py` & `depthcharge_ms-0.4.0/depthcharge/primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Fundamental dataclasses for depthcharge."""
+
 from __future__ import annotations
 
 import re
 from collections.abc import Sequence
 from dataclasses import dataclass
 
 import numpy as np
@@ -42,14 +43,15 @@
         The modification at each amino acid. This should be the length of
         ``sequence`` + 2, where index 0 and -1 are used for N- and C-terminal
         modification respectively. Use ``None`` in the iterable to specify
         unmodified positions. When ``modifications`` is ``None``, it is assumed
         that no modifications are present.
     charge : int, optional
         The charge of the peptide.
+
     """
 
     sequence: str
     modifications: Sequence[str | float | None] | None = None
     charge: int | None = None
 
     def __post_init__(self) -> None:
@@ -135,14 +137,15 @@
         sequence : str
             A ProForma 2.0-compliant string.
 
         Returns
         -------
         Peptide
             The parsed ProForma peptide.
+
         """
         pep, meta = proforma.parse(sequence)
         try:
             charge = meta["charge_state"].charge
         except AttributeError:
             charge = None
 
@@ -187,14 +190,15 @@
             The charge state of the peptide.
 
         Returns
         -------
         Peptide
             The parsed MassIVE peptide after conversion to a ProForma
             format.
+
         """
         sequence = cls.massivekb_to_proforma(sequence, charge)
         return cls.from_proforma(sequence)
 
     @classmethod
     def massivekb_to_proforma(
         cls, sequence: str, charge: int | None = None
@@ -213,14 +217,15 @@
             The charge state of the peptide.
 
         Returns
         -------
         str
             The parsed MassIVE peptide after conversion to a ProForma
             format.
+
         """
         sequence = "".join(
             [
                 MSKB_TO_UNIMOD.get(aa, aa)
                 for aa in re.split(r"(?<=.)(?=[A-Z])", sequence)
             ]
         )
@@ -238,14 +243,15 @@
     ----------
     tokens : list[str]
         The string tokens that comprise the peptide sequence.
     precursor : float
         The monoisotopic m/z of the precursor ion.
     fragments : torch.Tensor[float]
         The generated fragment ions originated from the peptide.
+
     """
 
     tokens: list[str]
     precursor: float
     fragments: torch.Tensor[float]
 
     @property
@@ -270,14 +276,15 @@
 
     Parameters
     ----------
     smiles : str
         A SMILES string defining the molecule.
     charge : int, optional
         The charge of the molecule.
+
     """
 
     smiles: str
     charge: int | None = None
 
     def __post_init__(self) -> None:
         """Validate parameters."""
@@ -291,14 +298,15 @@
     def show(self, **kwargs: dict) -> PngImageFile:
         """Show the molecule in 2D.
 
         Parameters
         ----------
         **kwargs : dict
             Keyword arguments passed to ``rdkit.Chem.Draw.MolToImage``
+
         """
         return Draw.MolToImage(self._mol, **kwargs)
 
     def to_selfies(self) -> str:
         """Convert SMILES to a SELFIES representaion."""
         return sf.encoder(self.smiles)
 
@@ -317,14 +325,15 @@
         charge : int, optional
             The charge of the molecule.
 
         Returns
         -------
         Molecule
             The parsed Molecule.
+
         """
         return cls(sf.decoder(selfies), charge)
 
 
 class MassSpectrum(MsmsSpectrum):
     """A mass spectrum.
 
@@ -346,31 +355,34 @@
         The precursor ion m/z, if applicable.
     precursor_charge: int, optional
         The precursor charge, if applicable.
     label: str, optional
         A label for the mass spectrum. This is typically an
         annotation, such as the generating peptide sequence,
         but is distinct from spectrum_utils' annotation.
+
     """
 
     def __init__(
         self,
         filename: str,
         scan_id: str,
         mz: ArrayLike,
         intensity: ArrayLike,
+        ms_level: int = None,
         retention_time: float | None = None,
         ion_mobility: float | None = None,
         precursor_mz: float | None = None,
         precursor_charge: int | None = None,
         label: str | None = None,
     ) -> None:
         """Initialize a MassSpectrum."""
         self.filename = filename
         self.scan_id = scan_id
+        self.ms_level = ms_level
         self.label = label
 
         # Not currently supported by spectrum_utils:
         self.ion_mobility = ion_mobility
 
         # spectrum_utils requires a precursor. Will remove after
         # I make a PR:
@@ -415,9 +427,10 @@
     def to_tensor(self) -> torch.tensor:
         """Combine the m/z and intensity arrays into a single tensor.
 
         Returns
         -------
         torch.tensor of shape (n_peaks, 2)
             The mass spectrum information.
+
         """
         return torch.tensor(np.vstack([self.mz, self.intensity]).T)
```

### Comparing `depthcharge-ms-0.3.1/depthcharge/tokenizers/peptides.py` & `depthcharge_ms-0.4.0/depthcharge/tokenizers/peptides.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,302 +1,280 @@
 """Tokenizers for peptides."""
+
 from __future__ import annotations
 
 import re
 from collections.abc import Iterable
 
-import numba as nb
-import numpy as np
 import torch
 from pyteomics.proforma import GenericModification, MassModification
 
 from .. import utils
 from ..constants import H2O, PROTON
-from ..primitives import MSKB_TO_UNIMOD, Peptide, PeptideIons
+from ..primitives import MSKB_TO_UNIMOD, Peptide
 from .tokenizer import Tokenizer
 
 
 class PeptideTokenizer(Tokenizer):
     """A tokenizer for ProForma peptide sequences.
 
-    Parse and tokenize ProForma-compliant peptide sequences. Additionally,
-    use this class to calculate fragment and precursor ion masses.
+    Parse and tokenize ProForma-compliant peptide sequences.
 
     Parameters
     ----------
     residues : dict[str, float], optional
-        Residues and modifications to add to the vocabulary beyond the
-        standard 20 amino acids.
-    replace_isoleucine_with_leucine : bool
-        Replace I with L residues, because they are isobaric and often
+        Residues and modifications to add to the vocabulary beyond
+        the standard 20 amino acids.
+    replace_isoleucine_with_leucine : bool, optional
+        Replace I with L residues, because they are isomeric and often
         indistinguishable by mass spectrometry.
-    reverse : bool
+    reverse : bool, optional
         Reverse the sequence for tokenization, C-terminus to N-terminus.
+    start_token : str, optional
+        The start token to use.
+    stop_token : str, optional
+        The stop token to use.
 
     Attributes
     ----------
-    residues : numba.typed.Dict[str, float]
+    residues : SortedDict[str, float]
         The residues and modifications and their associated masses.
         terminal modifcations are indicated by `-`.
     index : SortedDict{str, int}
         The mapping of residues and modifications to integer representations.
     reverse_index : list[None | str]
         The ordered residues and modifications where the list index is the
         integer representation for a token.
+    start_token : str
+        The start token
     stop_token : str
         The stop token.
+    start_int : int
+        The integer representation of the start token
+    stop_int : int
+        The integer representation of the stop token.
+    padding_int : int
+        The integer used to represent padding.
+
     """
 
-    residues = nb.typed.Dict.empty(
-        nb.types.unicode_type,
-        nb.types.float64,
-    )
-    residues.update(
-        G=57.021463735,
-        A=71.037113805,
-        S=87.032028435,
-        P=97.052763875,
-        V=99.068413945,
-        T=101.047678505,
-        C=103.009184505,
-        L=113.084064015,
-        I=113.084064015,
-        N=114.042927470,
-        D=115.026943065,
-        Q=128.058577540,
-        K=128.094963050,
-        E=129.042593135,
-        M=131.040484645,
-        H=137.058911875,
-        F=147.068413945,
-        R=156.101111050,
-        Y=163.063328575,
-        W=186.079312980,
-    )
+    residues = {
+        "G": 57.021463735,
+        "A": 71.037113805,
+        "S": 87.032028435,
+        "P": 97.052763875,
+        "V": 99.068413945,
+        "T": 101.047678505,
+        "C": 103.009184505,
+        "L": 113.084064015,
+        "I": 113.084064015,
+        "N": 114.042927470,
+        "D": 115.026943065,
+        "Q": 128.058577540,
+        "K": 128.094963050,
+        "E": 129.042593135,
+        "M": 131.040484645,
+        "H": 137.058911875,
+        "F": 147.068413945,
+        "R": 156.101111050,
+        "Y": 163.063328575,
+        "W": 186.079312980,
+    }
 
     # The peptide parsing function:
     _parse_peptide = Peptide.from_proforma
 
     def __init__(
         self,
-        residues: dict[str, float] | None = None,
+        residues: Iterable[str] | None = None,
         replace_isoleucine_with_leucine: bool = False,
         reverse: bool = False,
+        start_token: str | None = None,
+        stop_token: str | None = "$",
     ) -> None:
         """Initialize a PeptideTokenizer."""
         self.replace_isoleucine_with_leucine = replace_isoleucine_with_leucine
         self.reverse = reverse
+
+        # Note that these also secretly work on dicts too ;)
         self.residues = self.residues.copy()
         if residues is not None:
             self.residues.update(residues)
 
         if self.replace_isoleucine_with_leucine:
-            del self.residues["I"]
+            if "I" in self.residues:
+                del self.residues["I"]
+
+        super().__init__(self.residues, start_token, stop_token)
+        self.masses = torch.tensor(
+            [self.residues.get(a, 0.0) for a in self.reverse_index]
+        )
+
+    def calculate_precursor_ions(
+        self,
+        tokens: torch.Tensor | Iterable[str],
+        charges: torch.Tensor,
+    ) -> torch.Tensor:
+        """Calculate the m/z for precursor ions.
+
+        Parameters
+        ----------
+        tokens : torch.Tensor of shape (n_sequences, len_seq)
+            The tokens corresponding to the peptide sequence.
+        charges : torch.Tensor of shape (n_sequences,)
+            The charge state for each peptide.
+
+        Returns
+        -------
+        torch.Tensor
+            The monoisotopic m/z for each charged peptide.
+
+        """
+        if isinstance(tokens[0], str):
+            tokens = self.tokenize(utils.listify(tokens))
+
+        if not isinstance(charges, torch.Tensor):
+            charges = torch.tensor(charges)
+            if not charges.shape:
+                charges = charges[None]
 
-        super().__init__(list(self.residues.keys()))
+        masses = self.masses[tokens].sum(dim=1) + H2O
+        return (masses / charges) + PROTON
 
     def split(self, sequence: str) -> list[str]:
         """Split a ProForma peptide sequence.
 
         Parameters
         ----------
         sequence : str
             The peptide sequence.
 
         Returns
         -------
         list[str]
-            The tokens that compprise the peptide sequence.
+            The tokens that comprise the peptide sequence.
+
         """
         pep = self._parse_peptide(sequence)
         if self.replace_isoleucine_with_leucine:
             pep.sequence = pep.sequence.replace("I", "L")
 
         pep = pep.split()
         if self.reverse:
             pep.reverse()
 
         return pep
 
-    def ions(  # noqa: C901
-        self,
-        sequences: Iterable[str],
-        precursor_charges: Iterable[int] | str,
-        max_fragment_charge: int | None = None,
-    ) -> tuple[torch.Tensor[float], list[torch.Tensor[float]]]:
-        """Calculate the m/z for the precursor and fragment ions.
-
-        Currently depthcharge only support b and y ions.
-
-        Parameters
-        ----------
-        sequences : Iterable[str],
-            The peptide sequences.
-        precursor_charges : Iterable[int] or None, optional
-            The charge of each precursor ion. If ``None``, the charge state
-            is expected to be found in the peptide strings.
-        max_fragment_charge : int or None, optional
-            The maximum charge for fragment ions. The default is to consider
-            up to the ``max(precursor_charge - 1, 1)``.
-
-        Returns
-        -------
-        list of PeptideIons
-            The precursor and fragment ions generated by the peptide.
-        """
-        sequences = utils.listify(sequences)
-        if max_fragment_charge is None:
-            max_fragment_charge = np.inf
-
-        if precursor_charges is None:
-            precursor_charges = [None] * len(sequences)
-        else:
-            precursor_charges = utils.listify(precursor_charges)
-
-        if len(sequences) != len(precursor_charges):
-            raise ValueError(
-                "The number of sequences and precursor charges did not match."
-            )
-
-        out = []
-        for seq, charge in zip(sequences, precursor_charges):
-            if isinstance(seq, str):
-                if self.replace_isoleucine_with_leucine:
-                    seq = seq.replace("I", "L")
-
-                try:
-                    pep = Peptide.from_proforma(seq)
-                except ValueError:
-                    pep = Peptide.from_massivekb(seq)
-
-                tokens = pep.split()
-                if charge is None:
-                    charge = max(pep.charge - 1, 1)
-            else:
-                tokens = seq
-
-            if charge is None:
-                raise ValueError(
-                    f"No charge was provided for {seq}",
-                )
-
-            try:
-                prec = _calc_precursor_mass(
-                    nb.typed.List(tokens),
-                    charge,
-                    self.residues,
-                )
-            except KeyError as err:
-                raise ValueError(
-                    f"Unrecognized token(s) in {''.join(tokens)}"
-                ) from err
-
-            frags = _calc_fragment_masses(
-                nb.typed.List(tokens),
-                min(charge, max_fragment_charge),
-                self.residues,
-            )
-
-            ions = PeptideIons(
-                tokens=tokens,
-                precursor=prec,
-                fragments=torch.tensor(frags),
-            )
-
-            out.append(ions)
-
-        return out
-
     @classmethod
     def from_proforma(
         cls,
         sequences: Iterable[str],
-        replace_isoleucine_with_leucine: bool = True,
+        replace_isoleucine_with_leucine: bool = False,
         reverse: bool = True,
+        start_token: str | None = None,
+        stop_token: str | None = "$",
     ) -> PeptideTokenizer:
         """Create a tokenizer with the observed peptide modications.
 
         Modifications are parsed from ProForma 2.0-compliant peptide strings
         and added to the vocabulary.
 
         Parameters
         ----------
         sequences : Iterable[str]
             The peptides from which to parse modifications.
-        replace_isoleucine_with_leucine : bool
+        replace_isoleucine_with_leucine : bool, optional
             Replace I with L residues, because they are isobaric and often
             indistinguishable by mass spectrometry.
-        reverse : bool
+        reverse : bool, optional
             Reverse the sequence for tokenization, C-terminus to N-terminus.
+        start_token : str, optional
+            The start token to use.
+        stop_token : str, optional
+            The stop token to use.
 
         Returns
         -------
         PeptideTokenizer
             A tokenizer for peptides with the observed modifications.
+
         """
         if isinstance(sequences, str):
             sequences = [sequences]
 
         # Parse modifications:
-        new_res = cls.residues.copy()
+        new_res = {}
         for peptide in sequences:
             parsed = Peptide.from_proforma(peptide).split()
             for token in parsed:
-                if token in new_res.keys():
-                    continue
-
-                if token == "-":
+                if token in cls.residues:
                     continue
 
-                match = re.search(r"(.*)\[(.*)\]", token)
                 try:
-                    res, mod = match.groups()
-                    if res and res != "-":
-                        res_mass = new_res[res]
-                    else:
-                        res_mass = 0
-                except (AttributeError, KeyError) as err:
-                    raise ValueError("Unrecognized token {token}.") from err
+                    res, mod = re.search(r"(.*)\[(.*)\]", token).groups()
+                    try:
+                        mod_mass = MassModification(mod).mass
+                    except ValueError:
+                        mod_mass = GenericModification(mod).mass
+                except AttributeError as err:
+                    raise KeyError(f"Unknown residue {token}") from err
 
                 try:
-                    mod = MassModification(mod)
-                except ValueError:
-                    mod = GenericModification(mod)
+                    res_mass = cls.residues.get(res, 0)
+                except KeyError as err:
+                    raise ValueError(f"Unrecognized token {token}.") from err
+                except AttributeError:
+                    res_mass = 0.0  # In case we don't care about ions.
 
-                new_res[token] = res_mass + mod.mass
+                new_res[token] = res_mass + mod_mass
 
-        return cls(new_res, replace_isoleucine_with_leucine, reverse)
+        return cls(
+            new_res,
+            replace_isoleucine_with_leucine,
+            reverse,
+            start_token,
+            stop_token,
+        )
 
     @staticmethod
     def from_massivekb(
-        replace_isoleucine_with_leucine: bool = True,
+        replace_isoleucine_with_leucine: bool = False,
         reverse: bool = True,
+        start_token: str | None = None,
+        stop_token: str | None = "$",
     ) -> MskbPeptideTokenizer:
         """Create a tokenizer with the observed peptide modications.
 
         Modifications are parsed from MassIVE-KB peptide strings
         and added to the vocabulary.
 
         Parameters
         ----------
-        replace_isoleucine_with_leucine : bool
+        replace_isoleucine_with_leucine : bool, optional
             Replace I with L residues, because they are isobaric and often
             indistinguishable by mass spectrometry.
-        reverse : bool
+        reverse : bool, optional
             Reverse the sequence for tokenization, C-terminus to N-terminus.
+        start_token : str, optional
+            The start token to use.
+        stop_token : str, optional
+            The stop token to use.
 
         Returns
         -------
         MskbPeptideTokenizer
             A tokenizer for peptides with the observed modifications.
+
         """
         return MskbPeptideTokenizer.from_proforma(
             [f"{mod}A" for mod in MSKB_TO_UNIMOD.values()],
             replace_isoleucine_with_leucine,
             reverse,
+            start_token,
+            stop_token,
         )
 
 
 class MskbPeptideTokenizer(PeptideTokenizer):
     """A tokenizer for MassIVE-KB peptide sequences.
 
     MassIVE-KB includes N-term carbamylation, NH3-loss, acetylation, as well as
@@ -306,132 +284,32 @@
     Parameters
     ----------
     replace_isoleucine_with_leucine : bool
         Replace I with L residues, because they are isobaric and often
         indistinguishable by mass spectrometry.
     reverse : bool
         Reverse the sequence for tokenization, C-terminus to N-terminus.
+    start_token : str, optional
+        The start token to use.
+    stop_token : str, optional
+        The stop token to use.
 
     Attributes
     ----------
     residues : SortedDict[str, float]
         The residues and modifications and their associated masses.
         terminal modifcations are indicated by `-`.
     index : SortedDicte{str, int}
         The mapping of residues and modifications to integer representations.
     reverse_index : list[None | str]
         The ordered residues and modifications where the list index is the
         integer representation for a token.
-    stop_token : str
-        The stop token.
+    start_int : int
+        The integer representation of the start token
+    stop_int : int
+        The integer representation of the stop token.
+    padding_int : int
+        The integer used to represent padding.
 
     """
 
     _parse_peptide = Peptide.from_massivekb
-
-
-@nb.njit
-def _calc_precursor_mass(
-    tokens: list[str],
-    charge: int,
-    masses: nb.typed.Dict,
-) -> float:
-    """Calculate the precursor mass of a peptide sequence.
-
-    Parameters
-    ----------
-    tokens : list of str
-        The tokenized peptide sequence.
-    charge : int
-        The charge state to consider. Use 'None' to get the neutral mass.
-    masses : nb.typed.Dict
-        The mass dictionary to use.
-
-    Returns
-    -------
-    float
-        The precurosr monoisotopic m/z.
-    """
-    mass = sum([masses[t] for t in tokens]) + H2O
-    if charge is not None:
-        mass = _mass2mz(mass, charge)
-
-    return mass
-
-
-@nb.njit
-def _calc_fragment_masses(
-    tokens: list[str],
-    charge: int,
-    masses: nb.typed.Dict,
-) -> np.ndarray[float]:
-    """Calculate the b and y ions for a peptide sequence.
-
-    Parameters
-    ----------
-    tokens : list of str
-        The tokenized peptide sequence.
-    charge : int
-        The charge state to consider. Use 'None' to get the neutral mass.
-    masses : nb.typed.Dict
-        The mass dictionary to use.
-
-    Returns
-    -------
-    np.ndarray of shape (2, len(seq) - 1, charge)
-        The m/z of the predicted b and y ions.
-    """
-    # Handle terminal mods:
-    seq = np.empty(len(tokens))
-    n_mod = False
-    c_mod = False
-    for idx, token in enumerate(tokens):
-        if not idx and token.endswith("-"):
-            n_mod = True
-
-        if idx == (len(tokens) - 1) and token.startswith("-"):
-            c_mod = True
-
-        seq[idx] = masses[token]
-
-    if n_mod:
-        seq[1] += seq[0]
-        seq = seq[1:]
-
-    if c_mod:
-        seq[-2] += seq[-1]
-        seq = seq[:-1]
-
-    # Calculate fragments:
-    max_charge = min(charge, 2)
-    n_ions = len(seq) - 1
-    ions = np.empty((2, n_ions, max_charge))
-    b_mass = 0
-    y_mass = H2O
-    for idx in range(n_ions):
-        b_mass += seq[idx]
-        y_mass += seq[-(idx + 1)]
-        for cur_charge in range(1, max_charge + 1):
-            z_idx = cur_charge - 1
-            ions[0, idx, z_idx] = _mass2mz(b_mass, cur_charge)
-            ions[1, idx, z_idx] = _mass2mz(y_mass, cur_charge)
-
-    return ions
-
-
-@nb.njit
-def _mass2mz(mass: float, charge: int) -> float:
-    """Calculate the m/z.
-
-    Parameters
-    ----------
-    mass : float
-        The neutral mass.
-    charge : int
-        The charge.
-
-    Returns
-    -------
-    float
-       The m/z
-    """
-    return (mass / charge) + PROTON
```

### Comparing `depthcharge-ms-0.3.1/depthcharge/tokenizers/tokenizer.py` & `depthcharge_ms-0.4.0/depthcharge/tokenizers/tokenizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A base Tokenizer class."""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections.abc import Iterable, Sequence
 
 import torch
 from sortedcontainers import SortedDict, SortedSet
@@ -14,119 +15,146 @@
 class Tokenizer(ABC):
     """An abstract base class for Depthcharge tokenizers.
 
     Parameters
     ----------
     tokens : Sequence[str]
         The tokens to consider.
+    start_token : str, optional
+        The start token to use.
     stop_token : str, optional
         The stop token to use.
+
     """
 
-    def __init__(self, tokens: Sequence[str], stop_token: str = "$") -> None:
+    def __init__(
+        self,
+        tokens: Sequence[str],
+        start_token: str | None = None,
+        stop_token: str | None = "$",
+    ) -> None:
         """Initialize a tokenizer."""
+        self.start_token = start_token
         self.stop_token = stop_token
 
         tokens = SortedSet(tokens)
         if self.stop_token in tokens:
             raise ValueError(
                 f"Stop token {stop_token} already exists in tokens.",
             )
 
-        tokens.add(self.stop_token)
+        if start_token is not None:
+            tokens.add(self.start_token)
+        if stop_token is not None:
+            tokens.add(self.stop_token)
+
         self.index = SortedDict({k: i + 1 for i, k in enumerate(tokens)})
-        self.reverse_index = [None] + list(tokens)
-        self.stop_int = self.index[self.stop_token]
+        self.reverse_index = [None] + list(tokens)  # 0 is padding.
+        self.start_int = self.index.get(self.start_token, None)
+        self.stop_int = self.index.get(self.stop_token, None)
+        self.padding_int = 0
 
     def __len__(self) -> int:
         """The number of tokens."""
         return len(self.index)
 
     @abstractmethod
     def split(self, sequence: str) -> list[str]:
         """Split a sequence into the constituent string tokens."""
 
     def tokenize(
         self,
-        sequences: Iterable[str],
-        to_strings: bool = False,
+        sequences: Iterable[str] | str,
+        add_start: bool = False,
         add_stop: bool = False,
-    ) -> torch.Tensor | list[list[str]]:
+        to_strings: bool = False,
+    ) -> torch.tensor | list[list[str]]:
         """Tokenize the input sequences.
 
         Parameters
         ----------
-        sequences : Iterable[str]
+        sequences : Iterable[str] or str
             The sequences to tokenize.
+        add_start : bool, optional
+            Prepend the start token to the beginning of the sequence.
+        add_stop : bool, optional
+            Append the stop token to the end of the sequence.
         to_strings : bool, optional
             Return each as a list of token strings rather than a
             tensor. This is useful for debugging.
-        add_stop : bool, optional
-            Append the stop token tothe end of the sequence.
 
         Returns
         -------
-        torch.Tensor of shape (n_sequences, max_length) or list[list[str]]
+        torch.tensor of shape (n_sequences, max_length) or list[list[str]]
             Either a tensor containing the integer values for each
             token, padded with 0's, or the list of tokens comprising
             each sequence.
+
         """
+        add_start = add_start and self.start_token is not None
+        add_stop = add_stop and self.stop_token is not None
         try:
             out = []
             for seq in utils.listify(sequences):
                 tokens = self.split(seq)
+                if add_start and tokens[0] != self.start_token:
+                    tokens.insert(0, self.start_token)
+
                 if add_stop and tokens[-1] != self.stop_token:
                     tokens.append(self.stop_token)
 
                 if to_strings:
                     out.append(tokens)
                     continue
 
                 out.append(torch.tensor([self.index[t] for t in tokens]))
 
             if to_strings:
                 return out
 
-            if isinstance(sequences, str):
-                return out[0]
-
             return nn.utils.rnn.pad_sequence(out, batch_first=True)
         except KeyError as err:
             raise ValueError("Unrecognized token") from err
 
     def detokenize(
         self,
         tokens: torch.Tensor,
         join: bool = True,
+        trim_start_token: bool = True,
         trim_stop_token: bool = True,
     ) -> list[str] | list[list[str]]:
         """Retreive sequences from tokens.
 
         Parameters
         ----------
         tokens : torch.Tensor of shape (n_sequences, max_length)
             The zero-padded tensor of integerized tokens to decode.
         join : bool, optional
             Join tokens into strings?
+        trim_start_token : bool, optional
+            Remove the start token from the beginning of a sequence.
         trim_stop_token : bool, optional
             Remove the stop token from the end of a sequence.
 
         Returns
         -------
         list[str] or list[list[str]]
             The decoded sequences each as a string or list or strings.
+
         """
         decoded = []
         for row in tokens:
             seq = [
                 self.reverse_index[i]
                 for i in row
                 if self.reverse_index[i] is not None
             ]
 
+            if trim_start_token and seq[0] == self.start_token:
+                seq.pop(0)
             if trim_stop_token and seq[-1] == self.stop_token:
                 seq.pop(-1)
 
             if join:
                 seq = "".join(seq)
 
             decoded.append(seq)
```

### Comparing `depthcharge-ms-0.3.1/depthcharge_ms.egg-info/SOURCES.txt` & `depthcharge_ms-0.4.0/depthcharge_ms.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,35 +7,41 @@
 codecov.yml
 mkdocs.yml
 pyproject.toml
 .github/workflows/docs.yml
 .github/workflows/lint.yml
 .github/workflows/publish.yml
 .github/workflows/tests.yml
+data/README.md
 data/TMT10-Trial-8.mgf
 data/TMT10-Trial-8.mzML
 data/TMT10-Trial-8.mzXML
 depthcharge/__init__.py
 depthcharge/constants.py
 depthcharge/feedforward.py
+depthcharge/mixins.py
 depthcharge/primitives.py
+depthcharge/testing.py
 depthcharge/utils.py
 depthcharge/version.py
 depthcharge/data/__init__.py
+depthcharge/data/analyte_datasets.py
+depthcharge/data/arrow.py
+depthcharge/data/fields.py
 depthcharge/data/parsers.py
-depthcharge/data/peptide_datasets.py
 depthcharge/data/preprocessing.py
 depthcharge/data/spectrum_datasets.py
 depthcharge/encoders/__init__.py
 depthcharge/encoders/sinusoidal.py
 depthcharge/tokenizers/__init__.py
+depthcharge/tokenizers/molecules.py
 depthcharge/tokenizers/peptides.py
 depthcharge/tokenizers/tokenizer.py
 depthcharge/transformers/__init__.py
-depthcharge/transformers/peptides.py
+depthcharge/transformers/analytes.py
 depthcharge/transformers/spectra.py
 depthcharge_ms.egg-info/PKG-INFO
 depthcharge_ms.egg-info/SOURCES.txt
 depthcharge_ms.egg-info/dependency_links.txt
 depthcharge_ms.egg-info/requires.txt
 depthcharge_ms.egg-info/top_level.txt
 docs/CHANGELOG.md
@@ -53,15 +59,18 @@
 docs/stylesheets/extra.css
 static/icon.svg
 static/logo-dark.png
 static/logo-light.png
 tests/conftest.py
 tests/unit_tests/test_feedforward.py
 tests/unit_tests/test_primitives.py
+tests/unit_tests/test_testing.py
 tests/unit_tests/test_version.py
+tests/unit_tests/test_data/test_arrow.py
 tests/unit_tests/test_data/test_datasets.py
 tests/unit_tests/test_data/test_loaders.py
 tests/unit_tests/test_data/test_parsers.py
 tests/unit_tests/test_encoders/test_sinusoidal.py
+tests/unit_tests/test_tokenizers/test_molecules.py
 tests/unit_tests/test_tokenizers/test_peptides.py
-tests/unit_tests/test_transformers/test_peptide_transformers.py
+tests/unit_tests/test_transformers/test_analyte_transformers.py
 tests/unit_tests/test_transformers/test_spectrum_transformers.py
```

### Comparing `depthcharge-ms-0.3.1/docs/CHANGELOG.md` & `depthcharge_ms-0.4.0/docs/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,41 @@
-# Changelog for depthcharge
+# Changelog for Depthcharge
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v0.4.0]
+
+We have completely reworked of the data module.
+Depthcharge now uses Apache Arrow-based formats instead of HDF5; spectra are converted either Parquet or streamed with PyArrow, optionally into Lance datasets.
+
+We now also have full support for small molecules, with the `MoleculeTokenizer`,
+`AnalyteTransformerEncoder`, and `AnalyteTransformerDecoder` classes.
+
+### Breaking Changes
+- `PeptideTransformer*` are now `AnalyteTransformer*`, providing full support for small molecule analytes. Additionally the interface has been completely reworked.
+- Mass spectrometry data parsers now function as iterators, yielding batches of spectra as `pyarrow.RecordBatch` objects.
+- Parsers can now be told to read arbitrary fields from their respective file formats with the `custom_fields` parameter.
+- The parsing functionality of `SpctrumDataset` and its subclasses have been moved to the `spectra_to_*` functions in the data module.
+- `SpectrumDataset` and its subclasses now return dictionaries of data rather than a tuple of data. This allows us to incorporate arbitrary additional data
+- `SpectrumDataset` and its subclasses are now `lance.torch.data.LanceDataset` subclasses, providing native PyTorch integration.
+- All dataset classes now do not have a `loader()` method.
+
+### Added
+- Support for small molecules.
+- Added the `StreamingSpectrumDataset` for fast inference.
+- Added `spectra_to_df`, `spectra_to_df`, `spectra_to_stream` to the `depthcharge.data` module.
+
+### Changed
+- Determining the mass spectrometry data file format is now less fragile.
+  It now looks for known line contents, rather than relying on the extension.
+
 ## [v0.3.1] - 2023-08-18
 ### Added
 - Support for fine-tuning the wavelengths used for encoding floating point numbers like m/z and intensity to the `FloatEncoder` and `PeakEncoder`.
 
 ### Fixed
 - The `tgt_mask` in the `PeptideTransformerDecoder` was the incorrect type.
   Now it is `bool` as it should be.
@@ -25,14 +51,17 @@
 - Tight integration with `spectrum_utils` 💪
 
 ### Changed
 - Moving preprocessing onto parsing instead of data loading (similar to @bittremieux's proposal in #31)
 - Combining the SpectrumIndex and SpectrumDataset classes into one.
 - Changing peak encodings. Instead of encoding the intensity using a linear projection and summing with the sinusoidal m/z encodings, now the intensity is also sinusoidally encoded and is combined with the sinusoidal m/z encodings using a linear layer.
 
+## [v0.2.3] - 2023-08-18
+### Fixed
+- Applied hotfix from v0.3.1
 
 ## [v0.2.2] - 2023-05-15
 ### Fixed
 - Fixed retrieving version information.
 
 ## [v0.2.1] - 2023-05-13
 ### Changed
```

### Comparing `depthcharge-ms-0.3.1/docs/CODE_OF_CONDUCT.md` & `depthcharge_ms-0.4.0/docs/CODE_OF_CONDUCT.md`

 * *Files 0% similar despite different names*

```diff
@@ -116,8 +116,7 @@
 
 This Code of Conduct is adapted from the [Contributor Covenant][homepage],
 version 2.0, available at
 [https://www.contributor-covenant.org/version/2/0/code_of_conduct.html][v2.0].
 
 [homepage]: https://www.contributor-covenant.org
 [v2.0]: https://www.contributor-covenant.org/version/2/0/code_of_conduct.html
-
```

### Comparing `depthcharge-ms-0.3.1/docs/CONTRIBUTING.md` & `depthcharge_ms-0.4.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/docs/api/index.md` & `depthcharge_ms-0.4.0/docs/api/index.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/docs/getting-started/installation.md` & `depthcharge_ms-0.4.0/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/docs/index.md` & `depthcharge_ms-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/docs/stylesheets/extra.css` & `depthcharge_ms-0.4.0/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/mkdocs.yml` & `depthcharge_ms-0.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/pyproject.toml` & `depthcharge_ms-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -11,20 +11,22 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 requires-python = ">=3.10"
 dependencies = [
-    "torch>=1.11.0",
+    "torch>=2.0.0",
+    "polars>=0.19.0",
+    "pyarrow>=12.0.1",
+    "pylance>=0.7.5",
     "pyteomics>=4.4.2",
     "numpy>=1.18.1",
     "numba>=0.48.0",
     "lxml>=4.9.1",
-    "h5py>=3.7.0",
     "einops>=0.4.1",
     "tqdm>=4.65.0",
     "lark>=1.1.4",
     "selfies>=2.1.1",
     "sortedcontainers>=2.4.0",
     "dill>=0.3.6",
     "rdkit>=2023.03.1",
@@ -56,47 +58,26 @@
 
 [tool.setuptools.packages]
 find = {namespaces = false}
 
 [tool.setuptools_scm]
 
 [tool.ruff]
-select = ["E", "F", "W", "C", "I", "D", "UP", "N", "ANN", "T20"]
+line-length = 79
+target-version = "py310"
+
+[tool.ruff.lint]
+select = ["E", "F", "W", "C", "I", "D", "UP", "N", "T20"]
 
 # ANN101 Missing type annotation for `self` in method
 # D213 Multi-line docstring summary should start at the second lin
 # D203 1 blank line required before class docstring
 # D100 Missing docstring in public module
 # ANN102 Missing type annotation for `cls` in classmethod
 # D401 First line of docstring should be in imperative mood
 ignore = ["D213", "ANN101", "D203", "D100", "ANN102", "D401"]
-fix = true
 
-[tool.ruff.per-file-ignores]
-"*tests/*.py" = ["ANN", "N806"]
+[tool.ruff.lint.per-file-ignores]
+"*tests/*.py" = ["ANN", "N806", "C408"]
 "__init__.py" = ["F401", "D104"]
 "depthcharge/encoders/sinusoidal.py" = ["N803"]
 "depthcharge/feedforward.py" = ["N803"]
-
-[tool.black]
-line-length = 79
-target-version = ['py310']
-include = '\.pyi?$'
-exclude = '''
-
-(
-  /(
-      \.eggs         # exclude a few common directories in the
-    | \.git          # root of the project
-    | \.hg
-    | \.mypy_cache
-    | \.tox
-    | \.venv
-    | _build
-    | buck-out
-    | build
-    | dist
-  )/
-  | foo.py           # also separately exclude a file named foo.py in
-                     # the root of the project
-)
-'''
```

### Comparing `depthcharge-ms-0.3.1/static/icon.svg` & `depthcharge_ms-0.4.0/static/icon.svg`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/static/logo-dark.png` & `depthcharge_ms-0.4.0/static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/static/logo-light.png` & `depthcharge_ms-0.4.0/static/logo-light.png`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.3.1/tests/conftest.py` & `depthcharge_ms-0.4.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Pytest fixtures."""
+
 from pathlib import Path
 
 import numpy as np
 import pytest
 from pyteomics.mass import calculate_mass
 
 DATA_DIR = Path(__file__).parent / ".." / "data"
@@ -37,29 +38,29 @@
 def mgf_small(tmp_path):
     """An MGF file with 2 annotated spectra."""
     peptides = ["LESLIEK", "EDITHR"]
     mgf_file = tmp_path / "small.mgf"
     return _create_mgf(peptides, mgf_file)
 
 
-# Utility functions -----------------------------------------------------------
 def _create_mgf_entry(peptide, charge=2):
     """Create a MassIVE-KB style MGF entry for a single PSM.
 
     Parameters
     ----------
     peptide : str
         A peptide sequence.
     charge : int, optional
         The peptide charge state.
 
     Returns
     -------
     str
         The PSM entry in an MGF file format.
+
     """
     missing = not charge
     charge = 2 if not charge else charge
     mz = calculate_mass(peptide, charge=int(charge))
     frags = []
     for idx in range(len(peptide)):
         for zstate in range(1, charge):
@@ -105,14 +106,15 @@
         The random seed. The charge states are chosen to be
         2 or 3 randomly.
 
     Returns
     -------
     PathLike
         The MGF file.
+
     """
     rng = np.random.default_rng(random_state)
     peptides = list(peptides)
     entries = [_create_mgf_entry(p, rng.choice([2, 3])) for p in peptides]
 
     if add_problems:
         entries[-2] = _create_mgf_entry(peptides[-2], 0)
@@ -143,12 +145,13 @@
     random_state : int or numpy.random.Generator
         The random seed or state.
 
     Yields
     ------
     str
         A peptide sequence
+
     """
     rng = np.random.default_rng(random_state)
     residues = "ACDEFGHIKLMNPQRSTUVWY"
     for i in range(n_peptides):
         yield "".join(rng.choice(list(residues), rng.integers(6, 50)))
```

### Comparing `depthcharge-ms-0.3.1/tests/unit_tests/test_encoders/test_sinusoidal.py` & `depthcharge_ms-0.4.0/tests/unit_tests/test_encoders/test_sinusoidal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the encoders."""
+
 import numpy as np
 import pytest
 import torch
 
 from depthcharge.encoders import (
     FloatEncoder,
     PeakEncoder,
```

### Comparing `depthcharge-ms-0.3.1/tests/unit_tests/test_feedforward.py` & `depthcharge_ms-0.4.0/tests/unit_tests/test_feedforward.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the feedforward model."""
+
 import torch
 
 from depthcharge.feedforward import FeedForward
 
 
 def test_init():
     """Test initialization."""
```

### Comparing `depthcharge-ms-0.3.1/tests/unit_tests/test_primitives.py` & `depthcharge_ms-0.4.0/tests/unit_tests/test_primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test that our fundamental dataclasses work."""
+
 import numpy as np
 import pytest
 import torch
 from pyteomics.proforma import ProFormaError
 
 from depthcharge.primitives import (
     MassSpectrum,
```

### Comparing `depthcharge-ms-0.3.1/tests/unit_tests/test_version.py` & `depthcharge_ms-0.4.0/tests/unit_tests/test_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test getting the version."""
+
 from importlib.metadata import PackageNotFoundError
 
 import depthcharge
 
 
 def test_version():
     """Just make sure its something."""
```

