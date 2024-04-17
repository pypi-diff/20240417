# Comparing `tmp/chexus-24.4.0.tar.gz` & `tmp/chexus-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chexus-24.4.0.tar", last modified: Fri Apr  5 11:49:16 2024, max compression
+gzip compressed data, was "chexus-24.4.1.tar", last modified: Wed Apr 17 09:22:48 2024, max compression
```

## Comparing `chexus-24.4.0.tar` & `chexus-24.4.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.843132 chexus-24.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-05 11:48:56.000000 chexus-24.4.0/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.831132 chexus-24.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/nightly_at_main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/nightly_at_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/python-version-ci
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/unpinned.yml
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-05 11:48:56.000000 chexus-24.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-05 11:48:56.000000 chexus-24.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-05 11:48:56.000000 chexus-24.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-05 11:48:56.000000 chexus-24.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-05 11:48:56.000000 chexus-24.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 11:48:56.000000 chexus-24.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-05 11:49:16.843132 chexus-24.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-05 11:48:56.000000 chexus-24.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-05 11:48:56.000000 chexus-24.4.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/_static/anaconda-icon.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/_templates/class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/_templates/doc_version.html
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/_templates/module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/_typehints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/about/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/docs/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/developer/coding-conventions.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/developer/dependency-management.md
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/developer/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/developer/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-05 11:48:56.000000 chexus-24.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.839132 chexus-24.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/basetest.in
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/basetest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/make_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/mypy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/nightly.in
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/nightly.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/wheels.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 11:49:16.847132 chexus-24.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.831132 chexus-24.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.843132 chexus-24.4.0/src/chexus/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/json.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.843132 chexus-24.4.0/src/chexus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-05 11:49:16.000000 chexus-24.4.0/src/chexus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-05 11:49:16.000000 chexus-24.4.0/src/chexus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:49:16.000000 chexus-24.4.0/src/chexus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 11:49:16.000000 chexus-24.4.0/src/chexus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 11:49:16.000000 chexus-24.4.0/src/chexus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 11:49:16.000000 chexus-24.4.0/src/chexus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.843132 chexus-24.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-05 11:48:56.000000 chexus-24.4.0/tests/package_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-05 11:48:56.000000 chexus-24.4.0/tests/validate_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-04-05 11:48:56.000000 chexus-24.4.0/tests/validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-05 11:48:56.000000 chexus-24.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.549421 chexus-24.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-17 09:22:37.000000 chexus-24.4.1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.537421 chexus-24.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-17 09:22:37.000000 chexus-24.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.541421 chexus-24.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-17 09:22:37.000000 chexus-24.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-17 09:22:37.000000 chexus-24.4.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-17 09:22:37.000000 chexus-24.4.1/.github/workflows/nightly_at_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-17 09:22:37.000000 chexus-24.4.1/.github/workflows/nightly_at_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 09:22:37.000000 chexus-24.4.1/.github/workflows/python-version-ci
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-17 09:22:37.000000 chexus-24.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-17 09:22:37.000000 chexus-24.4.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-17 09:22:37.000000 chexus-24.4.1/.github/workflows/unpinned.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-17 09:22:37.000000 chexus-24.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-17 09:22:37.000000 chexus-24.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-17 09:22:37.000000 chexus-24.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-17 09:22:37.000000 chexus-24.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-17 09:22:37.000000 chexus-24.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 09:22:37.000000 chexus-24.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-17 09:22:48.549421 chexus-24.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-17 09:22:37.000000 chexus-24.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.541421 chexus-24.4.1/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-17 09:22:37.000000 chexus-24.4.1/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.541421 chexus-24.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.541421 chexus-24.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-17 09:22:37.000000 chexus-24.4.1/docs/_static/anaconda-icon.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.541421 chexus-24.4.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-17 09:22:37.000000 chexus-24.4.1/docs/_templates/class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 09:22:37.000000 chexus-24.4.1/docs/_templates/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-17 09:22:37.000000 chexus-24.4.1/docs/_templates/module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-17 09:22:37.000000 chexus-24.4.1/docs/_typehints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.541421 chexus-24.4.1/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-17 09:22:37.000000 chexus-24.4.1/docs/about/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.541421 chexus-24.4.1/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-17 09:22:37.000000 chexus-24.4.1/docs/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-17 09:22:37.000000 chexus-24.4.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.541421 chexus-24.4.1/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-17 09:22:37.000000 chexus-24.4.1/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 09:22:37.000000 chexus-24.4.1/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-17 09:22:37.000000 chexus-24.4.1/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-17 09:22:37.000000 chexus-24.4.1/docs/developer/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-17 09:22:37.000000 chexus-24.4.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-17 09:22:37.000000 chexus-24.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.545421 chexus-24.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/basetest.in
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/basetest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/make_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/nightly.in
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/nightly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-17 09:22:37.000000 chexus-24.4.1/requirements/wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-17 09:22:48.549421 chexus-24.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.537421 chexus-24.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.549421 chexus-24.4.1/src/chexus/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-17 09:22:37.000000 chexus-24.4.1/src/chexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-17 09:22:37.000000 chexus-24.4.1/src/chexus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-17 09:22:37.000000 chexus-24.4.1/src/chexus/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-17 09:22:37.000000 chexus-24.4.1/src/chexus/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-17 09:22:37.000000 chexus-24.4.1/src/chexus/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:37.000000 chexus-24.4.1/src/chexus/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-17 09:22:37.000000 chexus-24.4.1/src/chexus/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-17 09:22:37.000000 chexus-24.4.1/src/chexus/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-17 09:22:37.000000 chexus-24.4.1/src/chexus/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.549421 chexus-24.4.1/src/chexus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-17 09:22:48.000000 chexus-24.4.1/src/chexus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-17 09:22:48.000000 chexus-24.4.1/src/chexus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:22:48.000000 chexus-24.4.1/src/chexus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 09:22:48.000000 chexus-24.4.1/src/chexus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 09:22:48.000000 chexus-24.4.1/src/chexus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 09:22:48.000000 chexus-24.4.1/src/chexus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:48.549421 chexus-24.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-17 09:22:37.000000 chexus-24.4.1/tests/package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-17 09:22:37.000000 chexus-24.4.1/tests/validate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-04-17 09:22:37.000000 chexus-24.4.1/tests/validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-17 09:22:37.000000 chexus-24.4.1/tox.ini
```

### Comparing `chexus-24.4.0/.github/workflows/ci.yml` & `chexus-24.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/.github/workflows/docs.yml` & `chexus-24.4.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/.github/workflows/nightly_at_main.yml` & `chexus-24.4.1/.github/workflows/nightly_at_main.yml`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/.github/workflows/nightly_at_release.yml` & `chexus-24.4.1/.github/workflows/nightly_at_release.yml`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/.github/workflows/release.yml` & `chexus-24.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/.github/workflows/test.yml` & `chexus-24.4.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/.github/workflows/unpinned.yml` & `chexus-24.4.1/.github/workflows/unpinned.yml`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/.pre-commit-config.yaml` & `chexus-24.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/CODE_OF_CONDUCT.md` & `chexus-24.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/CONTRIBUTING.md` & `chexus-24.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/LICENSE` & `chexus-24.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/PKG-INFO` & `chexus-24.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chexus
-Version: 24.4.0
+Version: 24.4.1
 Summary: Validate and check NeXus files
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
```

### Comparing `chexus-24.4.0/README.md` & `chexus-24.4.1/README.md`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/conda/meta.yaml` & `chexus-24.4.1/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/docs/_static/anaconda-icon.js` & `chexus-24.4.1/docs/_static/anaconda-icon.js`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/docs/_templates/class-template.rst` & `chexus-24.4.1/docs/_templates/class-template.rst`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/docs/_templates/module-template.rst` & `chexus-24.4.1/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/docs/_typehints.py` & `chexus-24.4.1/docs/_typehints.py`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/docs/about/index.md` & `chexus-24.4.1/docs/about/index.md`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/docs/conf.py` & `chexus-24.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/docs/developer/coding-conventions.md` & `chexus-24.4.1/docs/developer/coding-conventions.md`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/docs/developer/dependency-management.md` & `chexus-24.4.1/docs/developer/dependency-management.md`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/docs/developer/getting-started.md` & `chexus-24.4.1/docs/developer/getting-started.md`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/pyproject.toml` & `chexus-24.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/requirements/ci.txt` & `chexus-24.4.1/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/requirements/dev.txt` & `chexus-24.4.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/requirements/docs.txt` & `chexus-24.4.1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/requirements/make_base.py` & `chexus-24.4.1/requirements/make_base.py`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/requirements/static.txt` & `chexus-24.4.1/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/src/chexus/__init__.py` & `chexus-24.4.1/src/chexus/__init__.py`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/src/chexus/__main__.py` & `chexus-24.4.1/src/chexus/__main__.py`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/src/chexus/hdf5.py` & `chexus-24.4.1/src/chexus/hdf5.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import Any
 
 import h5py
 
 from .tree import Dataset, Group
 
 
-def read_hdf5(path: str) -> Group:
+def read_hdf5(path: str, **kwargs) -> Group:
     """Read HDF5 file and return tree of datasets and groups"""
-    with h5py.File(path, "r") as f:
+    with h5py.File(path, "r", **kwargs) as f:
         return _read_group(f)
 
 
 def _read_attrs(node: h5py.Dataset | h5py.Group) -> dict[str, Any]:
     """Read HDF5 attributes"""
     attrs = dict(node.attrs)
     # Convert bytes to strings
```

### Comparing `chexus-24.4.0/src/chexus/io.py` & `chexus-24.4.1/src/chexus/io.py`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/src/chexus/json.py` & `chexus-24.4.1/src/chexus/json.py`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/src/chexus/tree.py` & `chexus-24.4.1/src/chexus/tree.py`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/src/chexus/validate.py` & `chexus-24.4.1/src/chexus/validate.py`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/src/chexus/validators.py` & `chexus-24.4.1/src/chexus/validators.py`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/src/chexus.egg-info/PKG-INFO` & `chexus-24.4.1/src/chexus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chexus
-Version: 24.4.0
+Version: 24.4.1
 Summary: Validate and check NeXus files
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
```

### Comparing `chexus-24.4.0/src/chexus.egg-info/SOURCES.txt` & `chexus-24.4.1/src/chexus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/tests/validate_test.py` & `chexus-24.4.1/tests/validate_test.py`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/tests/validators_test.py` & `chexus-24.4.1/tests/validators_test.py`

 * *Files identical despite different names*

### Comparing `chexus-24.4.0/tox.ini` & `chexus-24.4.1/tox.ini`

 * *Files identical despite different names*

