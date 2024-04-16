# Comparing `tmp/qbraid-core-0.1.2.dev3.tar.gz` & `tmp/qbraid_core-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-core-0.1.2.dev3.tar", last modified: Fri Apr 12 00:48:18 2024, max compression
+gzip compressed data, was "qbraid_core-0.1.3.tar", last modified: Tue Apr 16 22:36:44 2024, max compression
```

## Comparing `qbraid-core-0.1.2.dev3.tar` & `qbraid_core-0.1.3.tar`

### file list

```diff
@@ -1,99 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.469962 qbraid-core-0.1.2.dev3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.449962 qbraid-core-0.1.2.dev3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.449962 qbraid-core-0.1.2.dev3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.449962 qbraid-core-0.1.2.dev3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-12 00:48:18.469962 qbraid-core-0.1.2.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.453961 qbraid-core-0.1.2.dev3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.453961 qbraid-core-0.1.2.dev3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.453961 qbraid-core-0.1.2.dev3/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.453961 qbraid-core-0.1.2.dev3/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/_static/css/s4defs-roles.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.453961 qbraid-core-0.1.2.dev3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/api/qbraid_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/api/qbraid_core.services.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/api/qbraid_core.system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.457961 qbraid-core-0.1.2.dev3/qbraid_core/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-12 00:48:18.000000 qbraid-core-0.1.2.dev3/qbraid_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.461962 qbraid-core-0.1.2.dev3/qbraid_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.461962 qbraid-core-0.1.2.dev3/qbraid_core/services/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/services/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/services/environments/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/services/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/services/environments/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/services/environments/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/services/environments/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/services/environments/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.461962 qbraid-core-0.1.2.dev3/qbraid_core/services/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/services/quantum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/services/quantum/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/services/quantum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/services/quantum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/services/quantum/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.465962 qbraid-core-0.1.2.dev3/qbraid_core/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/system/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/system/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/system/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/qbraid_core/system/threader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.465962 qbraid-core-0.1.2.dev3/qbraid_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-12 00:48:18.000000 qbraid-core-0.1.2.dev3/qbraid_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-12 00:48:18.000000 qbraid-core-0.1.2.dev3/qbraid_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 00:48:18.000000 qbraid-core-0.1.2.dev3/qbraid_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 00:48:18.000000 qbraid-core-0.1.2.dev3/qbraid_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 00:48:18.000000 qbraid-core-0.1.2.dev3/qbraid_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 00:48:18.469962 qbraid-core-0.1.2.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.465962 qbraid-core-0.1.2.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.465962 qbraid-core-0.1.2.dev3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/fixtures/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/test_create_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/test_create_local_venv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/test_delete_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/test_installed_envs_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/test_replace_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/test_system_executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/test_system_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tests/test_update_install_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:48:18.465962 qbraid-core-0.1.2.dev3/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-12 00:48:14.000000 qbraid-core-0.1.2.dev3/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.353411 qbraid_core-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.333411 qbraid_core-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.337411 qbraid_core-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.337411 qbraid_core-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-16 22:36:44.353411 qbraid_core-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.337411 qbraid_core-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.337411 qbraid_core-0.1.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.337411 qbraid_core-0.1.3/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.337411 qbraid_core-0.1.3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/css/s4defs-roles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.341411 qbraid_core-0.1.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/api/qbraid_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/api/qbraid_core.services.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/api/qbraid_core.system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.341411 qbraid_core-0.1.3/qbraid_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-16 22:36:44.000000 qbraid_core-0.1.3/qbraid_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.345411 qbraid_core-0.1.3/qbraid_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.345411 qbraid_core-0.1.3/qbraid_core/services/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.345411 qbraid_core-0.1.3/qbraid_core/services/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/quantum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/quantum/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/quantum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/quantum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/quantum/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/quantum/proxy_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/qbraid_core/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/system/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/system/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/system/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/system/threader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/qbraid_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-16 22:36:44.000000 qbraid_core-0.1.3/qbraid_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-16 22:36:44.000000 qbraid_core-0.1.3/qbraid_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:36:44.000000 qbraid_core-0.1.3/qbraid_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 22:36:44.000000 qbraid_core-0.1.3/qbraid_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 22:36:44.000000 qbraid_core-0.1.3/qbraid_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:36:44.353411 qbraid_core-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tests/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tests/environments/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/fixtures/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tests/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/quantum/test_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tests/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/system/test_executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/system/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/system/test_packages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tests/top_level/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/top_level/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/top_level/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/top_level/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/top_level/test_sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tools/verify_headers.py
```

### Comparing `qbraid-core-0.1.2.dev3/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid_core-0.1.3/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid_core-0.1.3/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/.github/workflows/docs.yml` & `qbraid_core-0.1.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/.github/workflows/format.yml` & `qbraid_core-0.1.3/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/.github/workflows/main.yml` & `qbraid_core-0.1.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/.github/workflows/publish.yml` & `qbraid_core-0.1.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/.github/workflows/test-publish.yml` & `qbraid_core-0.1.3/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/.gitignore` & `qbraid_core-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/LICENSE` & `qbraid_core-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/PKG-INFO` & `qbraid_core-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.2.dev3
+Version: 0.1.3
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid-core-0.1.2.dev3/README.md` & `qbraid_core-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/docs/Makefile` & `qbraid_core-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/docs/_static/cards/jupyter.png` & `qbraid_core-0.1.3/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/docs/_static/cards/python.png` & `qbraid_core-0.1.3/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/docs/_static/cards/terminal.png` & `qbraid_core-0.1.3/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/docs/_static/css/custom.css` & `qbraid_core-0.1.3/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/docs/_static/css/s4defs-roles.css` & `qbraid_core-0.1.3/docs/_static/css/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/docs/_static/favicon.ico` & `qbraid_core-0.1.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/docs/_static/logo.png` & `qbraid_core-0.1.3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/docs/conf.py` & `qbraid_core-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/docs/index.rst` & `qbraid_core-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/docs/make.bat` & `qbraid_core-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/pyproject.toml` & `qbraid_core-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-core"
-version = "0.1.2.dev3"
+version = "0.1.3"
 authors = [
     {name = "qBraid Development Team", email = "contact@qbraid.com"},
 ]
 description = "Python library with core abstractions for software development in the qBraid ecosystem."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["qbraid", "quantum", "cloud"]
```

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/__init__.py` & `qbraid_core-0.1.3/qbraid_core/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/_compat.py` & `qbraid_core-0.1.3/qbraid_core/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/client.py` & `qbraid_core-0.1.3/qbraid_core/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/config.py` & `qbraid_core-0.1.3/qbraid_core/config.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/exceptions.py` & `qbraid_core-0.1.3/qbraid_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/registry.py` & `qbraid_core-0.1.3/qbraid_core/registry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/retry.py` & `qbraid_core-0.1.3/qbraid_core/retry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/services/environments/__init__.py` & `qbraid_core-0.1.3/qbraid_core/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/services/environments/client.py` & `qbraid_core-0.1.3/qbraid_core/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/services/environments/create.py` & `qbraid_core-0.1.3/qbraid_core/services/environments/create.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/services/environments/paths.py` & `qbraid_core-0.1.3/qbraid_core/services/environments/paths.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,31 +35,39 @@
         A list of pathlib.Path objects representing the qBraid environments paths.
     """
     qbraid_envs_path = os.getenv("QBRAID_ENVS_PATH", str(DEFAULT_LOCAL_ENVS_PATH))
     return [Path(path) for path in qbraid_envs_path.split(os.pathsep)]
 
 
 def get_env_path(slug: str) -> Path:
-    """Return path to qbraid environment.
+    """
+    Return path to qbraid environment.
 
     Args:
         slug (str): The environment directory to search for.
 
     Returns:
         pathlib.Path: The path to the environment directory.
 
     Raises:
         FileNotFoundError: If the environment directory does not exist.
     """
     qbraid_env_paths = get_default_envs_paths()
-    for path in qbraid_env_paths:
-        if path.is_dir() and path.name == slug:
-            return path / slug
+    searched_paths = []  # Keep track of paths that were searched
 
-    raise FileNotFoundError(f"Environment '{slug}' not found in any qBraid environment path.")
+    for env_path in qbraid_env_paths:
+        target_path = env_path / slug  # Directly create the path to the target
+        if target_path.is_dir():
+            return target_path
+        searched_paths.append(target_path)
+
+    # Improving error message by showing all searched paths
+    raise FileNotFoundError(
+        f"Environment '{slug}' not found. Searched in: {', '.join(str(p) for p in searched_paths)}"
+    )
 
 
 def get_tmp_dir_names(envs_path: Union[str, Path]) -> List[str]:
     """Return list of tmp directories paths in envs_path"""
     pattern = re.compile(r"^tmp\d{1,2}$")  # Regex for tmp directories
 
     envs_dir = Path(envs_path)
```

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/services/environments/state.py` & `qbraid_core-0.1.3/qbraid_core/services/environments/state.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/services/environments/validate.py` & `qbraid_core-0.1.3/qbraid_core/services/environments/validate.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/services/quantum/__init__.py` & `qbraid_core-0.1.3/qbraid_core/services/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/services/quantum/adapter.py` & `qbraid_core-0.1.3/qbraid_core/services/quantum/adapter.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/services/quantum/client.py` & `qbraid_core-0.1.3/qbraid_core/services/quantum/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 import sys
 from typing import Any, Dict, List, Optional
 
 from qbraid_core.client import QbraidClient
 from qbraid_core.exceptions import RequestsApiError
 from qbraid_core.registry import register_client
-from qbraid_core.system import get_active_python_path
+from qbraid_core.system import get_active_python_path, python_paths_equivalent
 
 from .exceptions import QuantumServiceRequestError
 from .proxy import SUPPORTED_QJOB_LIBS, quantum_lib_proxy_state
 
 
 @register_client()
 class QuantumClient(QbraidClient):
@@ -143,15 +143,19 @@
         Returns:
             Dict[str, Any]: A dictionary containing the system's executable path and the states
                             of libraries relevant to qBraid Quantum Jobs. The libraries' states
                             include whether they are supported and enabled.
         """
         python_exe = get_active_python_path()
         environment_state = {"exe": str(python_exe)}
+        is_default_python = python_paths_equivalent(sys.executable, str(python_exe))
 
-        check_libs = [device_lib] if device_lib else SUPPORTED_QJOB_LIBS
+        check_libs = [device_lib] if device_lib else list(SUPPORTED_QJOB_LIBS.keys())
 
-        libs_state = {lib: quantum_lib_proxy_state(lib) for lib in check_libs}
+        libs_state = {
+            lib: quantum_lib_proxy_state(lib, is_default_python=is_default_python)
+            for lib in check_libs
+        }
 
         environment_state["libs"] = libs_state
 
         return environment_state
```

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/services/quantum/proxy.py` & `qbraid_core-0.1.3/qbraid_core/services/quantum/proxy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,27 @@
 # Copyright (c) 2024, qBraid Development Team
 # All rights reserved.
 
 """
 Module for checking state of qBraid Quantum Jobs proxies.
 
 """
-
 import logging
-from importlib.metadata import PackageNotFoundError, distribution
 from pathlib import Path
 from typing import Dict, Optional, Tuple, Union
 
 from qbraid_core.system import get_active_site_packages_path, get_venv_site_packages_path
 
 from .exceptions import QbraidException
+from .proxy_braket import _check_proxy_braket
 
 logger = logging.getLogger(__name__)
 
-SUPPORTED_QJOB_LIBS = ["braket"]
-
-
-def _check_proxy_braket() -> Tuple[bool, bool]:
-    """
-    Determine the braket proxy state by checking that amazon-braket-sdk,
-    boto3, and botocore are installed and that botocore is the qBraid fork.
-
-    Returns:
-        Tuple[bool, bool]: A tuple of two booleans indicating whether qBraid
-                           Quantum Jobs are supported and enabled, respectively.
-
-    """
-    packages = ["amazon-braket-sdk", "boto3", "botocore"]
-
-    supported = True
-    enabled = False
-
-    botocore_data = None
-    for package in packages:
-        try:
-            dist = distribution(package)
-            if package == "botocore":
-                botocore_data = dist.metadata
-        except PackageNotFoundError:
-            return False, False
-
-    if botocore_data:
-        homepage = botocore_data.get("Home-page", "")
-        if "github.com/qBraid/botocore" in homepage:
-            enabled = True
-
-    return supported, enabled
+SUPPORTED_QJOB_LIBS = {"braket": ("botocore", "httpsession.py")}
+# SUPPORTED_QJOB_LIBS = {"braket": ("amazon-braket-sdk", ("botocore", "httpsession.py"))}
 
 
 def _check_proxy(
     proxy_spec: Tuple[str, ...], slug_path: Optional[Path] = None
 ) -> Tuple[bool, bool, Path]:
     """
     Checks if the specified proxy file exists and contains the string 'qbraid'.
@@ -93,44 +61,50 @@
         return True, False, site_packages_path
     except Exception as err:  # pylint: disable=broad-exception-caught
         logger.debug("Unexpected error checking qBraid proxy: %s", err)
 
     return True, False, site_packages_path
 
 
-def quantum_lib_proxy_state(device_lib: str, **kwargs) -> Dict[str, Union[str, bool]]:
+def quantum_lib_proxy_state(
+    device_lib: str, is_default_python: bool = True, **kwargs
+) -> Dict[str, Union[str, bool]]:
     """Checks if qBraid Quantum Jobs are supported and if so, checks whether they are enabled.
     Returns dictionary providing information about the state of qBraid Quantum Jobs support
     and configuration for the given quantum device library.
 
     Args:
         device_lib (str): The name of the quantum device library, e.g., "braket".
+        is_default_python (bool): Indicates whether the Python environment is known to
+                                  be the default system Python. Default assumption is True.
 
     Returns:
         dict: A dictionary containing the following keys:
-            - 'proxy_lib' (str): The name of the python library that would be modified by the
-                                 quantum jobs proxy.
             - 'supported' (bool): Indicates whether the necessary proxy file exists for the
                                   specified quantum device library.
             - 'enabled' (bool): True if the library is configured to support qBraid Quantum Jobs,
                                 False otherwise.
     """
-    state = {
-        "supported": False,
-        "enabled": False,
-    }
-
     if device_lib not in SUPPORTED_QJOB_LIBS:
-        raise ValueError(f"Unsupported quantum job library. Expected one of {SUPPORTED_QJOB_LIBS}")
+        raise ValueError(
+            f"Unsupported quantum job library. Expected one of {list(SUPPORTED_QJOB_LIBS.keys())}"
+        )
+
+    supported = False
+    enabled = False
+
+    proxy_spec = SUPPORTED_QJOB_LIBS[device_lib]
 
     if device_lib == "braket":
-        supported, enabled = _check_proxy_braket()
-        if supported and not enabled:
-            proxy_lib = "botocore"
-            proxy_spec = (proxy_lib, "httpsession.py")
+        if is_default_python:
+            supported, enabled = _check_proxy_braket()
+            if supported and not enabled:
+                supported, enabled, _ = _check_proxy(proxy_spec, **kwargs)
+        else:
             supported, enabled, _ = _check_proxy(proxy_spec, **kwargs)
 
     # add more device libraries here as needed
 
-    state["supported"] = supported
-    state["enabled"] = enabled
-    return state
+    return {
+        "supported": supported,
+        "enabled": enabled,
+    }
```

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/sessions.py` & `qbraid_core-0.1.3/qbraid_core/sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/system/__init__.py` & `qbraid_core-0.1.3/qbraid_core/system/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
    get_python_version_from_exe
    get_venv_site_packages_path
    get_active_site_packages_path
    get_active_python_path
    get_local_package_path
    get_local_package_version
    get_latest_package_version
+   python_paths_equivalent
    replace_str
    echo_log
 
 Exceptions
 ------------
 
 .. autosummary::
@@ -46,14 +47,15 @@
 from .exceptions import QbraidSystemError, UnknownFileSystemObjectError
 from .executables import (
     get_active_python_path,
     get_python_version_from_cfg,
     get_python_version_from_exe,
     is_exe,
     is_valid_python,
+    python_paths_equivalent,
 )
 from .generic import echo_log, replace_str
 from .packages import (
     get_active_site_packages_path,
     get_latest_package_version,
     get_local_package_path,
     get_local_package_version,
```

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/system/executables.py` & `qbraid_core-0.1.3/qbraid_core/system/executables.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,72 @@
 
 """
 Module for serving information about system executables.
 
 """
 import logging
 import os
+import re
 import shutil
 import stat
 import subprocess
 import sys
 from pathlib import Path
 from typing import Optional, Union
 
 logger = logging.getLogger(__name__)
 
 
+def _extract_python_version(python_exe: str) -> Union[int, None]:
+    """
+    Extracts the major version number from a Python version string.
+
+    Args:
+        s (str): The string from which to extract the major version number.
+
+    Returns:
+        int or None: The major version number if present, otherwise None.
+    """
+    match = re.search(r"python\s*-?(\d+)(?:\.\d*)?$", python_exe)
+    return int(match.group(1)) if match else None
+
+
+def python_paths_equivalent(path1: Union[str, Path], path2: Union[str, Path]) -> bool:
+    """
+    Determines if two Python path strings refer to the same version of Python,
+    ignoring any minor version numbers and only considering major version equivalency.
+
+    Args:
+        path1 (Union[str, Path]): First Python path.
+        path2 (Union[str, Path]): Second Python path.
+
+    Returns:
+        bool: True if paths are considered equivalent, otherwise False.
+    """
+
+    if sys.platform == "win32":
+        return str(path1) == str(path2)
+
+    def normalize_python_path(path: Union[str, Path]) -> tuple:
+        path = str(path)  # Convert Path to string if needed
+        version = _extract_python_version(path)
+        normalized_path = re.sub(r"python-?\d+(\.\d+)?$", "python", path)
+        return version, normalized_path
+
+    # Normalize both paths
+    version1, normalized_path1 = normalize_python_path(path1)
+    version2, normalized_path2 = normalize_python_path(path2)
+
+    # Check if paths are equivalent
+    paths_equal = normalized_path1 == normalized_path2
+    versions_equal = version1 == version2 if version1 and version2 else True
+
+    return paths_equal and versions_equal
+
+
 def get_active_python_path(verify: bool = False) -> Path:
     """Retrieves the path of the currently active Python interpreter."""
     current_python_path = Path(sys.executable)
     shell_python_path = None
 
     # Choose command based on operating system
     cmd = ["where", "python"] if sys.platform == "win32" else ["which", "python"]
```

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/system/generic.py` & `qbraid_core-0.1.3/qbraid_core/system/generic.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/system/packages.py` & `qbraid_core-0.1.3/qbraid_core/system/packages.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 import ast
 import logging
 import site
 import subprocess
 import sys
 from importlib.metadata import PackageNotFoundError, version
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Union
 
 import requests
 
 from .exceptions import QbraidSystemError
 from .executables import (
     get_active_python_path,
     get_python_version_from_cfg,
     get_python_version_from_exe,
+    python_paths_equivalent,
 )
 
 logger = logging.getLogger(__name__)
 
 
 def get_venv_site_packages_path(venv_path: Path) -> Path:
     """
@@ -69,29 +70,31 @@
     respecting active virtual environments, as well.
 
     """
 
     current_python_path = Path(sys.executable)
     shell_python_path = python_path or get_active_python_path()
 
-    if shell_python_path == current_python_path:
+    if python_paths_equivalent(shell_python_path, current_python_path):
         site_packages_paths = [Path(path) for path in site.getsitepackages()]
 
     else:
         try:
             result = subprocess.run(
                 [shell_python_path, "-c", "import site; print(site.getsitepackages())"],
                 capture_output=True,
                 text=True,
                 check=True,
             )
         except subprocess.CalledProcessError as err:
             raise QbraidSystemError(
-                "Failed to get user site-packages directory from the shell's Python interpreter."
+                f"Failed to get user site-packages directory from {shell_python_path}."
             ) from err
+        except FileNotFoundError as err:
+            raise QbraidSystemError(f"Python executable not found at {shell_python_path}.") from err
 
         paths = ast.literal_eval(result.stdout.strip())
         site_packages_paths = [Path(path) for path in paths]
 
     # Common logic for finding the correct site-packages path
     if len(site_packages_paths) == 1:
         return site_packages_paths[0]
@@ -115,23 +118,41 @@
 
 def get_local_package_path(package: str) -> Path:
     """Retrieves the local path of a package."""
     try:
         site_packages_path = get_active_site_packages_path()
         return site_packages_path / package
     except (PackageNotFoundError, ModuleNotFoundError) as err:
-        raise QbraidSystemError(f"{package} is not installed in the current environment.") from err
+        raise QbraidSystemError(f"{package} not found in the current environment.") from err
 
 
-def get_local_package_version(package: str) -> str:
+def get_local_package_version(package: str, python_path: Optional[Union[str, Path]] = None) -> str:
     """Retrieves the local version of a package."""
+    if python_path:
+        try:
+            result = subprocess.run(
+                [
+                    str(python_path),
+                    "-c",
+                    f"import importlib.metadata; print(importlib.metadata.version('{package}'))",
+                ],
+                capture_output=True,
+                text=True,
+                check=True,
+            )
+            return result.stdout.strip()
+        except subprocess.CalledProcessError as err:
+            raise QbraidSystemError(f"{package} not found in the current environment.") from err
+        except FileNotFoundError as err:
+            raise QbraidSystemError(f"Python executable not found at {python_path}.") from err
+
     try:
         return version(package)
     except PackageNotFoundError as err:
-        raise QbraidSystemError(f"{package} is not installed in the current environment.") from err
+        raise QbraidSystemError(f"{package} not found in the current environment.") from err
 
 
 def get_latest_package_version(package: str) -> str:
     """Retrieves the latest version of package from PyPI."""
     url = f"https://pypi.org/pypi/{package}/json"
     try:
         response = requests.get(url, timeout=5)
```

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core/system/threader.py` & `qbraid_core-0.1.3/qbraid_core/system/threader.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core.egg-info/PKG-INFO` & `qbraid_core-0.1.3/qbraid_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.2.dev3
+Version: 0.1.3
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid-core-0.1.2.dev3/qbraid_core.egg-info/SOURCES.txt` & `qbraid_core-0.1.3/qbraid_core.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -49,31 +49,33 @@
 qbraid_core/services/environments/state.py
 qbraid_core/services/environments/validate.py
 qbraid_core/services/quantum/__init__.py
 qbraid_core/services/quantum/adapter.py
 qbraid_core/services/quantum/client.py
 qbraid_core/services/quantum/exceptions.py
 qbraid_core/services/quantum/proxy.py
+qbraid_core/services/quantum/proxy_braket.py
 qbraid_core/system/__init__.py
 qbraid_core/system/exceptions.py
 qbraid_core/system/executables.py
 qbraid_core/system/generic.py
 qbraid_core/system/packages.py
 qbraid_core/system/threader.py
 tests/__init__.py
-tests/conftest.py
-tests/test_client.py
-tests/test_compat.py
-tests/test_config.py
-tests/test_create_environment.py
-tests/test_create_local_venv.py
-tests/test_delete_environment.py
-tests/test_environments.py
-tests/test_installed_envs_data.py
-tests/test_replace_str.py
-tests/test_session.py
-tests/test_system_executables.py
-tests/test_system_packages.py
-tests/test_update_install_status.py
-tests/fixtures/__init__.py
-tests/fixtures/environments.py
+tests/environments/__init__.py
+tests/environments/conftest.py
+tests/environments/test_client.py
+tests/environments/test_create.py
+tests/environments/test_paths.py
+tests/environments/test_state.py
+tests/environments/test_validate.py
+tests/environments/fixtures/__init__.py
+tests/environments/fixtures/environments.py
+tests/quantum/test_proxy.py
+tests/system/test_executables.py
+tests/system/test_generic.py
+tests/system/test_packages.py
+tests/top_level/test_client.py
+tests/top_level/test_compat.py
+tests/top_level/test_config.py
+tests/top_level/test_sessions.py
 tools/verify_headers.py
```

### Comparing `qbraid-core-0.1.2.dev3/tests/fixtures/environments.py` & `qbraid_core-0.1.3/tests/environments/fixtures/environments.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/tests/test_client.py` & `qbraid_core-0.1.3/tests/top_level/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/tests/test_compat.py` & `qbraid_core-0.1.3/tests/top_level/test_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/tests/test_config.py` & `qbraid_core-0.1.3/tests/top_level/test_config.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/tests/test_create_local_venv.py` & `qbraid_core-0.1.3/tests/environments/test_create.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/tests/test_installed_envs_data.py` & `qbraid_core-0.1.3/tests/environments/test_paths.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,49 @@
 # Copyright (c) 2024, qBraid Development Team
 # All rights reserved.
 
 """
-Unit tests for the `installed_envs_data` function in the `qbraid_cli.envs.data_handling` module.
+Unit tests for functions that get environment path(s) data.
 
 """
-
 import json
+import os
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
-from qbraid_core.services.environments.paths import installed_envs_data
+from qbraid_core.services.environments.paths import get_default_envs_paths, installed_envs_data
+
+skip_remote_tests: bool = os.getenv("QBRAID_RUN_REMOTE_TESTS", "False").lower() != "true"
+REASON = "QBRAID_RUN_REMOTE_TESTS not set (requires configuration of qBraid storage)"
+
+
+def test_get_default_envs_paths_with_env_var_set(monkeypatch):
+    """Test the get_qbraid_envs_paths function when QBRAID_ENVS_PATH is set."""
+    # Mocking QBRAID_ENVS_PATH with two paths for the test
+    mock_path_1, mock_path_2 = "/path/to/envs1", "/path/to/envs2"
+    mock_envs_path = mock_path_1 + os.pathsep + mock_path_2
+    monkeypatch.setenv("QBRAID_ENVS_PATH", mock_envs_path)
+
+    expected_paths = [Path(mock_path_1), Path(mock_path_2)]
+    default_paths = get_default_envs_paths()
+    assert (
+        default_paths == expected_paths
+    ), "Should return paths from QBRAID_ENVS_PATH environment variable"
+
+
+def test_get_qbraid_envs_paths_with_no_env_var_set(monkeypatch):
+    """Test the get_qbraid_envs_paths function when QBRAID_ENVS_PATH is not set."""
+    # Removing QBRAID_ENVS_PATH to simulate it not being set
+    monkeypatch.delenv("QBRAID_ENVS_PATH", raising=False)
+
+    expected_paths = [str(Path.home() / ".qbraid" / "environments")]
+    default_paths = [str(path) for path in get_default_envs_paths()]
+    assert (
+        default_paths == expected_paths
+    ), "Should return the default path when QBRAID_ENVS_PATH is not set"
 
 
 def mock_path_iterdir(paths):
     """Helper to create a mock for Path.iterdir, returning mock Path objects for a list of paths."""
     return [MagicMock(spec=Path, name=path, is_dir=MagicMock(return_value=True)) for path in paths]
```

### Comparing `qbraid-core-0.1.2.dev3/tests/test_replace_str.py` & `qbraid_core-0.1.3/tests/system/test_generic.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/tests/test_session.py` & `qbraid_core-0.1.3/tests/top_level/test_sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev3/tests/test_system_packages.py` & `qbraid_core-0.1.3/tests/system/test_packages.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) 2024, qBraid Development Team
 # All rights reserved.
 
 """
 Unit tests for qBraid core helper functions related to system site-packages.
 
 """
+import sys
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 import pytest
 
 from qbraid_core.exceptions import QbraidException
 from qbraid_core.system.exceptions import QbraidSystemError
@@ -119,11 +120,33 @@
 
 def test_get_latest_version_raises():
     """Test the _get_latest_version function when an error occurs."""
     with pytest.raises(QbraidException):
         get_latest_package_version("nonexistent_package")
 
 
-def test_get_local_version_raises():
+@pytest.mark.parametrize(
+    "package,python_path", [("not_a_package", None), ("not_a_package", sys.executable)]
+)
+def test_get_local_version_raises_for_bad_package(package, python_path):
     """Test the _get_local_version function when an error occurs."""
-    with pytest.raises(QbraidException):
-        get_local_package_version("nonexistent_package")
+    with pytest.raises(QbraidException) as exc_info:
+        get_local_package_version(package, python_path=python_path)
+    assert f"{package} not found in the current environment." in str(exc_info)
+
+
+def test_get_local_version_raises_for_():
+    """Test the _get_local_version function when an error occurs."""
+    package = "pytest"  # valid package guaranteed to be installed
+    python_path = "/bad/python/path"  # invalid python path
+    with pytest.raises(QbraidException) as exc_info:
+        get_local_package_version(package, python_path=python_path)
+    assert f"Python executable not found at {python_path}." in str(exc_info)
+
+
+@pytest.mark.parametrize("python_path", [None, Path(sys.executable), sys.executable])
+def test_get_local_package_version_alt_python(python_path):
+    """Test the get_latest_package_version function with an alternative Python path."""
+    python_path = Path(sys.executable)
+    with patch("subprocess.run") as mock_run:
+        mock_run.return_value = MagicMock(stdout="2.31.0\n")
+        assert get_local_package_version("requests", python_path=python_path) == "2.31.0"
```

### Comparing `qbraid-core-0.1.2.dev3/tests/test_update_install_status.py` & `qbraid_core-0.1.3/tests/environments/test_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (c) 2024, qBraid Development Team
 # All rights reserved.
 
 """
-Unit tests for the update_install_status function in the envs app.
+Unit tests for getting and update environment state files
+including state.json and install_status.txt.
 
 """
 
 import json
 
-from qbraid_core.services.environments import update_install_status
+from qbraid_core.services.environments.state import update_install_status
 
 
 def test_update_install_status_creates_file_if_not_exists(tmp_path):
     """Test that the function creates a state.json file if it does not exist."""
     slug_path = tmp_path
     state_json_path = slug_path / "state.json"
     install_complete = 1
```

### Comparing `qbraid-core-0.1.2.dev3/tools/verify_headers.py` & `qbraid_core-0.1.3/tools/verify_headers.py`

 * *Files identical despite different names*

