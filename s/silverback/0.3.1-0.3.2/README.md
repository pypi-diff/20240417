# Comparing `tmp/silverback-0.3.1.tar.gz` & `tmp/silverback-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverback-0.3.1.tar", last modified: Thu Mar 28 19:09:08 2024, max compression
+gzip compressed data, was "silverback-0.3.2.tar", last modified: Wed Apr 17 00:47:13 2024, max compression
```

## Comparing `silverback-0.3.1.tar` & `silverback-0.3.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:09:08.690580 silverback-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:09:08.682580 silverback-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:09:08.682580 silverback-0.3.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-28 19:08:00.000000 silverback-0.3.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-28 19:08:00.000000 silverback-0.3.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-28 19:08:00.000000 silverback-0.3.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-28 19:08:00.000000 silverback-0.3.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-28 19:08:00.000000 silverback-0.3.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:09:08.682580 silverback-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-28 19:08:00.000000 silverback-0.3.1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-28 19:08:00.000000 silverback-0.3.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-28 19:08:00.000000 silverback-0.3.1/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-28 19:08:00.000000 silverback-0.3.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-28 19:08:00.000000 silverback-0.3.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-28 19:08:00.000000 silverback-0.3.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-03-28 19:08:00.000000 silverback-0.3.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-28 19:08:00.000000 silverback-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-28 19:08:00.000000 silverback-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-28 19:08:00.000000 silverback-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-28 19:08:00.000000 silverback-0.3.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-28 19:08:00.000000 silverback-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-03-28 19:09:08.690580 silverback-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-03-28 19:08:00.000000 silverback-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-03-28 19:08:00.000000 silverback-0.3.1/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:09:08.682580 silverback-0.3.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:09:08.686580 silverback-0.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:09:08.686580 silverback-0.3.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:09:08.686580 silverback-0.3.1/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/commands/run.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:09:08.686580 silverback-0.3.1/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/methoddocs/application.md
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/methoddocs/middlewares.md
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/methoddocs/runner.md
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/methoddocs/subscriptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:09:08.686580 silverback-0.3.1/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/userguides/development.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-28 19:08:00.000000 silverback-0.3.1/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-28 19:08:00.000000 silverback-0.3.1/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-28 19:08:00.000000 silverback-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-28 19:09:08.690580 silverback-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-03-28 19:08:00.000000 silverback-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:09:08.686580 silverback-0.3.1/silverback/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-28 19:08:00.000000 silverback-0.3.1/silverback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-03-28 19:08:00.000000 silverback-0.3.1/silverback/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-03-28 19:08:00.000000 silverback-0.3.1/silverback/_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-03-28 19:08:00.000000 silverback-0.3.1/silverback/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-28 19:08:00.000000 silverback-0.3.1/silverback/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-03-28 19:08:00.000000 silverback-0.3.1/silverback/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-03-28 19:08:00.000000 silverback-0.3.1/silverback/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 19:08:00.000000 silverback-0.3.1/silverback/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-03-28 19:08:00.000000 silverback-0.3.1/silverback/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-03-28 19:08:00.000000 silverback-0.3.1/silverback/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-03-28 19:08:00.000000 silverback-0.3.1/silverback/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-28 19:08:00.000000 silverback-0.3.1/silverback/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-03-28 19:08:00.000000 silverback-0.3.1/silverback/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-28 19:09:08.000000 silverback-0.3.1/silverback/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:09:08.690580 silverback-0.3.1/silverback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-03-28 19:09:08.000000 silverback-0.3.1/silverback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-28 19:09:08.000000 silverback-0.3.1/silverback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:09:08.000000 silverback-0.3.1/silverback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-28 19:09:08.000000 silverback-0.3.1/silverback.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:09:08.000000 silverback-0.3.1/silverback.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-28 19:09:08.000000 silverback-0.3.1/silverback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-28 19:09:08.000000 silverback-0.3.1/silverback.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:09:08.690580 silverback-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 19:08:00.000000 silverback-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-28 19:08:00.000000 silverback-0.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-28 19:08:00.000000 silverback-0.3.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.643592 silverback-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-17 00:46:12.000000 silverback-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-17 00:46:12.000000 silverback-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-17 00:46:12.000000 silverback-0.3.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-17 00:46:12.000000 silverback-0.3.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-17 00:46:12.000000 silverback-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-17 00:47:13.643592 silverback-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-17 00:46:12.000000 silverback-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-17 00:46:12.000000 silverback-0.3.2/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/commands/run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/methoddocs/application.md
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/methoddocs/middlewares.md
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/methoddocs/runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/methoddocs/subscriptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.643592 silverback-0.3.2/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/userguides/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-17 00:46:12.000000 silverback-0.3.2/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-17 00:46:12.000000 silverback-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 00:47:13.643592 silverback-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-17 00:46:12.000000 silverback-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.643592 silverback-0.3.2/silverback/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.643592 silverback-0.3.2/silverback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.643592 silverback-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:46:12.000000 silverback-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-17 00:46:12.000000 silverback-0.3.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-17 00:46:12.000000 silverback-0.3.2/tests/test_cli.py
```

### Comparing `silverback-0.3.1/.github/ISSUE_TEMPLATE/bug.md` & `silverback-0.3.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/.github/ISSUE_TEMPLATE/feature.md` & `silverback-0.3.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/.github/ISSUE_TEMPLATE/work-item.md` & `silverback-0.3.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/.github/release-drafter.yml` & `silverback-0.3.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/.github/workflows/codeql.yaml` & `silverback-0.3.2/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/.github/workflows/commitlint.yaml` & `silverback-0.3.2/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/.github/workflows/docs.yaml` & `silverback-0.3.2/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/.github/workflows/prtitle.yaml` & `silverback-0.3.2/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/.github/workflows/publish.yaml` & `silverback-0.3.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/.github/workflows/test.yaml` & `silverback-0.3.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/.gitignore` & `silverback-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/.pre-commit-config.yaml` & `silverback-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/CONTRIBUTING.md` & `silverback-0.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/Dockerfile` & `silverback-0.3.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/LICENSE` & `silverback-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/PKG-INFO` & `silverback-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.3.1
+Version: 0.3.2
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.3.1/README.md` & `silverback-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/build_docs.py` & `silverback-0.3.2/build_docs.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/docs/_static/custom.css` & `silverback-0.3.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/docs/_static/custom.js` & `silverback-0.3.2/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/docs/_templates/layout.html` & `silverback-0.3.2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/docs/conf.py` & `silverback-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/docs/favicon.ico` & `silverback-0.3.2/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/docs/logo.gif` & `silverback-0.3.2/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/docs/userguides/development.md` & `silverback-0.3.2/docs/userguides/development.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/example.py` & `silverback-0.3.2/example.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/pyproject.toml` & `silverback-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/setup.py` & `silverback-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/silverback/_cli.py` & `silverback-0.3.2/silverback/_cli.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/silverback/_importer.py` & `silverback-0.3.2/silverback/_importer.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/silverback/exceptions.py` & `silverback-0.3.2/silverback/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from typing import Any
 
 from ape.exceptions import ApeException
 from ape.logging import logger
 
+from .types import TaskType
+
 
 class ImportFromStringError(Exception):
     pass
 
 
-class DuplicateHandlerError(Exception):
-    def __init__(self, handler_type: str):
-        super().__init__(f"Only one handler allowed for: {handler_type}")
-
-
 class InvalidContainerTypeError(Exception):
     def __init__(self, container: Any):
         super().__init__(f"Invalid container type: {container.__class__}")
 
 
+class ContainerTypeMismatchError(Exception):
+    def __init__(self, task_type: TaskType, container: Any):
+        super().__init__(f"Invalid container type for '{task_type}': {container.__class__}")
+
+
 class NoWebsocketAvailableError(Exception):
     def __init__(self):
         super().__init__(
             "Attempted to a use WebsocketRunner without a websocket-compatible provider."
         )
```

### Comparing `silverback-0.3.1/silverback/middlewares.py` & `silverback-0.3.2/silverback/middlewares.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,20 @@
-from typing import Any, Optional, Tuple
+from typing import Any
 
 from ape.logging import logger
 from ape.types import ContractLog
 from ape.utils import ManagerAccessMixin
 from eth_utils.conversions import to_hex
 from taskiq import TaskiqMessage, TaskiqMiddleware, TaskiqResult
 
 from silverback.persistence import HandlerResult
-from silverback.types import SilverbackID, handler_id_block, handler_id_event
+from silverback.types import SilverbackID, TaskType
 from silverback.utils import hexbytes_dict
 
 
-def resolve_task(message: TaskiqMessage) -> Tuple[str, Optional[int], Optional[int]]:
-    block_number = None
-    log_index = None
-    task_id = message.task_name
-
-    if task_id == "block":
-        block_number = message.args[0].number
-        task_id = handler_id_block(block_number)
-    elif "event" in task_id:
-        block_number = message.args[0].block_number
-        log_index = message.args[0].log_index
-        # TODO: Should standardize on event signature here instead of name in case of overloading
-        task_id = handler_id_event(message.args[0].contract_address, message.args[0].event_name)
-
-    return task_id, block_number, log_index
-
-
 class SilverbackMiddleware(TaskiqMiddleware, ManagerAccessMixin):
     def __init__(self, *args, **kwargs):
         def compute_block_time() -> int:
             genesis = self.chain_manager.blocks[0]
             head = self.chain_manager.blocks.head
 
             if not head.number or head.number == 0:
@@ -62,61 +45,71 @@
             return fixed_data
 
         message.args = [(fix_dict(arg) if isinstance(arg, dict) else arg) for arg in message.args]
 
         return message
 
     def _create_label(self, message: TaskiqMessage) -> str:
-        if message.task_name == "block":
-            args = f"[block={message.args[0].hash.hex()}]"
-
-        elif "event" in message.task_name:
-            args = f"[txn={message.args[0].transaction_hash},log_index={message.args[0].log_index}]"
+        if labels_str := ",".join(f"{k}={v}" for k, v in message.labels.items()):
+            return f"{message.task_name}[{labels_str}]"
 
         else:
-            args = ""
-
-        return f"{message.task_name}{args}"
+            return message.task_name
 
     def pre_execute(self, message: TaskiqMessage) -> TaskiqMessage:
-        if message.task_name == "block":
+        if not (task_type := message.labels.pop("task_type")):
+            return message  # Not a silverback task
+
+        try:
+            task_type = TaskType(task_type)
+        except ValueError:
+            return message  # Not a silverback task
+
+        # Add extra labels for our task to see what their source was
+        if task_type is TaskType.NEW_BLOCKS:
             # NOTE: Necessary because we don't know the exact block class
-            message.args[0] = self.provider.network.ecosystem.decode_block(
+            block = message.args[0] = self.provider.network.ecosystem.decode_block(
                 hexbytes_dict(message.args[0])
             )
+            message.labels["block_number"] = str(block.number)
+            message.labels["block_hash"] = block.hash.hex()
 
-        elif "event" in message.task_name:
+        elif task_type is TaskType.EVENT_LOG:
             # NOTE: Just in case the user doesn't specify type as `ContractLog`
-            message.args[0] = ContractLog.model_validate(message.args[0])
+            log = message.args[0] = ContractLog.model_validate(message.args[0])
+            message.labels["block_number"] = str(log.block_number)
+            message.labels["transaction_hash"] = log.transaction_hash
+            message.labels["log_index"] = str(log.log_index)
 
-        logger.info(f"{self._create_label(message)} - Started")
+        logger.debug(f"{self._create_label(message)} - Started")
         return message
 
     def post_execute(self, message: TaskiqMessage, result: TaskiqResult):
-        percentage_time = 100 * (result.execution_time / self.block_time)
-        logger.info(
-            f"{self._create_label(message)} "
-            f"- {result.execution_time:.3f}s ({percentage_time:.1f}%)"
+        if self.block_time:
+            percentage_time = 100 * (result.execution_time / self.block_time)
+            percent_display = f" ({percentage_time:.1f}%)"
+
+        else:
+            percent_display = ""
+
+        (logger.error if result.error else logger.success)(
+            f"{self._create_label(message)} " f"- {result.execution_time:.3f}s{percent_display}"
         )
 
     async def post_save(self, message: TaskiqMessage, result: TaskiqResult):
         if not self.persistence:
             return
 
-        handler_id, block_number, log_index = resolve_task(message)
-
         handler_result = HandlerResult.from_taskiq(
-            self.ident, handler_id, block_number, log_index, result
+            self.ident,
+            message.task_name,
+            message.labels.get("block_number"),
+            message.labels.get("log_index"),
+            result,
         )
 
         try:
             await self.persistence.add_result(handler_result)
         except Exception as err:
             logger.error(f"Error storing result: {err}")
 
-    async def on_error(
-        self,
-        message: TaskiqMessage,
-        result: TaskiqResult,
-        exception: BaseException,
-    ):
-        logger.error(f"{message.task_name} - {type(exception).__name__}: {exception}")
+    # NOTE: Unless stdout is ignored, error traceback appears in stdout, no need for `on_error`
```

### Comparing `silverback-0.3.1/silverback/persistence.py` & `silverback-0.3.2/silverback/persistence.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/silverback/runner.py` & `silverback-0.3.2/silverback/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from taskiq import AsyncTaskiqDecoratedTask, TaskiqResult
 
 from .application import SilverbackApp
 from .exceptions import Halt, NoWebsocketAvailableError
 from .persistence import BasePersistentStore
 from .settings import Settings
 from .subscriptions import SubscriptionType, Web3SubscriptionsManager
-from .types import SilverbackID, SilverbackStartupState
+from .types import SilverbackID, SilverbackStartupState, TaskType
 from .utils import async_wrap_iter, hexbytes_dict
 
 settings = Settings()
 
 
 class BaseRunner(ABC):
     def __init__(self, app: SilverbackApp, *args, max_exceptions: int = 3, **kwargs):
@@ -99,44 +99,43 @@
             if boot_state:
                 self.last_block_seen = boot_state.last_block_seen
                 self.last_block_processed = boot_state.last_block_processed
 
         await self.app.broker.startup()
 
         # Execute Silverback startup task before we init the rest
-        if startup_handler := self.app.get_startup_handler():
-            task = await startup_handler.kiq(
+        for startup_task in self.app.tasks[TaskType.STARTUP]:
+            task = await startup_task.handler.kiq(
                 SilverbackStartupState(
                     last_block_seen=self.last_block_seen,
                     last_block_processed=self.last_block_processed,
                 )
             )
             result = await task.wait_result()
             self._handle_result(result)
 
-        if block_handler := self.app.get_block_handler():
-            tasks = [self._block_task(block_handler)]
-        else:
-            tasks = []
+        tasks = []
+        for task in self.app.tasks[TaskType.NEW_BLOCKS]:
+            tasks.append(self._block_task(task.handler))
 
-        for contract_address in self.app.contract_events:
-            for event_name, contract_event in self.app.contract_events[contract_address].items():
-                if event_handler := self.app.get_event_handler(contract_address, event_name):
-                    tasks.append(self._event_task(contract_event, event_handler))
+        for task in self.app.tasks[TaskType.EVENT_LOG]:
+            tasks.append(self._event_task(task.container, task.handler))
 
         if len(tasks) == 0:
             raise Halt("No tasks to execute")
 
-        await asyncio.gather(*tasks)
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            logger.error(f"Fatal error detected, shutting down: '{e}'")
 
         # Execute Silverback shutdown task before shutting down the broker
-        if shutdown_handler := self.app.get_shutdown_handler():
-            task = await shutdown_handler.kiq()
-            result = await task.wait_result()
-            self._handle_result(result)
+        for shutdown_task in self.app.tasks[TaskType.SHUTDOWN]:
+            task = await shutdown_task.handler.kiq()
+            result = self._handle_result(await task.wait_result())
 
         await self.app.broker.shutdown()
 
 
 class WebsocketRunner(BaseRunner, ManagerAccessMixin):
     """
     Run a single app against a live network using a basic in-memory queue and websockets.
```

### Comparing `silverback-0.3.1/silverback/settings.py` & `silverback-0.3.2/silverback/settings.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/silverback/subscriptions.py` & `silverback-0.3.2/silverback/subscriptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import json
 from enum import Enum
 from typing import AsyncGenerator, Dict, List, Optional
 
 from ape.logging import logger
+from websockets import ConnectionClosedError
 from websockets import client as ws_client
 
 
 class SubscriptionType(Enum):
     BLOCKS = "newHeads"
     EVENTS = "logs"
 
@@ -141,10 +142,16 @@
         return success
 
     async def __aexit__(self, exc_type, exc, tb):
         try:
             # Try to gracefully unsubscribe to all events
             await asyncio.gather(*(self.unsubscribe(sub_id) for sub_id in self._subscriptions))
 
+        except ConnectionClosedError:
+            pass  # Websocket already closed (ctrl+C and patiently waiting)
+
         finally:
             # Disconnect and release websocket
-            await self.connection.close()
+            try:
+                await self.connection.close()
+            except RuntimeError:
+                pass  # No running event loop to disconnect from (multiple ctrl+C presses)
```

### Comparing `silverback-0.3.1/silverback/utils.py` & `silverback-0.3.2/silverback/utils.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/silverback.egg-info/PKG-INFO` & `silverback-0.3.2/silverback.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.3.1
+Version: 0.3.2
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.3.1/silverback.egg-info/SOURCES.txt` & `silverback-0.3.2/silverback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `silverback-0.3.1/silverback.egg-info/requires.txt` & `silverback-0.3.2/silverback.egg-info/requires.txt`

 * *Files identical despite different names*

