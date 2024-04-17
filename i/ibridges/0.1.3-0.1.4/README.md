# Comparing `tmp/ibridges-0.1.3.tar.gz` & `tmp/ibridges-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibridges-0.1.3.tar", last modified: Tue Apr  9 11:50:44 2024, max compression
+gzip compressed data, was "ibridges-0.1.4.tar", last modified: Wed Apr 17 12:04:19 2024, max compression
```

## Comparing `ibridges-0.1.3.tar` & `ibridges-0.1.4.tar`

### file list

```diff
@@ -1,117 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.077844 ibridges-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:50:39.000000 ibridges-0.1.3/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.053844 ibridges-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.057844 ibridges-0.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.057844 ibridges-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/workflows/integration-tests-irods.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/workflows/integration-tests-yoda.yml
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/workflows/pypi_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-09 11:50:39.000000 ibridges-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-09 11:50:39.000000 ibridges-0.1.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-09 11:50:39.000000 ibridges-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-09 11:50:44.077844 ibridges-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-09 11:50:39.000000 ibridges-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.057844 ibridges-0.1.3/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.057844 ibridges-0.1.3/docker/irods_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_catalog/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_catalog/init-user-db.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.061844 ibridges-0.1.3/docker/irods_catalog_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_catalog_provider/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_catalog_provider/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_catalog_provider/setup-4.3.1.input
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.061844 ibridges-0.1.3/docker/irods_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.053844 ibridges-0.1.3/docker/irods_client/environments/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.061844 ibridges-0.1.3/docker/irods_client/environments/plain-irods/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/environments/plain-irods/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/environments/plain-irods/irods_environment.json
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/environments/plain-irods/irods_environment_testuser.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.061844 ibridges-0.1.3/docker/irods_client/environments/yoda/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/environments/yoda/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/environments/yoda/irods_environment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.061844 ibridges-0.1.3/docker/irods_client/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/testdata/beach.rtf
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/testdata/bunny.rtf
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/testdata/example.r
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.061844 ibridges-0.1.3/docker/irods_client/testdata/more_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/testdata/more_data/polarbear.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/testdata/plant.rtf
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/testdata/sun.rtf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.065844 ibridges-0.1.3/docker/irods_client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_data_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_ticket.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.065844 ibridges-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.065844 ibridges-0.1.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.069844 ibridges-0.1.3/ibridges/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 11:50:43.000000 ibridges-0.1.3/ibridges/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/data_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/export_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/icat_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13582 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/tickets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.073844 ibridges-0.1.3/ibridges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-09 11:50:44.000000 ibridges-0.1.3/ibridges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-09 11:50:44.000000 ibridges-0.1.3/ibridges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:50:44.000000 ibridges-0.1.3/ibridges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 11:50:44.000000 ibridges-0.1.3/ibridges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 11:50:44.000000 ibridges-0.1.3/ibridges.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-09 11:50:39.000000 ibridges-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:50:44.077844 ibridges-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.069844 ibridges-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-09 11:50:39.000000 ibridges-0.1.3/tests/test_irodspath.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.069844 ibridges-0.1.3/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-04-09 11:50:39.000000 ibridges-0.1.3/tests/testdata/bunny.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.069844 ibridges-0.1.3/tests/testdata/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 11:50:39.000000 ibridges-0.1.3/tests/testdata/subfolder/sun.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.069844 ibridges-0.1.3/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/01-Setup-and-connect.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12711 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/02-Working-with-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/03-iRODS-Paths.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/04-Metadata.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/05-Data-Sharing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/Data_sync.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24498 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/QuickStart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.069844 ibridges-0.1.3/tutorials/example_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/example_rules/example.r
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/iRODS_paths.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.073844 ibridges-0.1.3/tutorials/img/
--rw-r--r--   0 runner    (1001) docker     (127)   227136 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/DataObject1.png
--rw-r--r--   0 runner    (1001) docker     (127)   246217 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/DataObject2.png
--rw-r--r--   0 runner    (1001) docker     (127)   277830 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/DataObject3.png
--rw-r--r--   0 runner    (1001) docker     (127)   297047 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/DataObject4.png
--rw-r--r--   0 runner    (1001) docker     (127)   291147 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/DataObject5.png
--rw-r--r--   0 runner    (1001) docker     (127)   303681 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/DataObject6.png
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/Save_json.png
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/Yoda_environment.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.295724 ibridges-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 12:04:10.000000 ibridges-0.1.4/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.275724 ibridges-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.275724 ibridges-0.1.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-17 12:04:10.000000 ibridges-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-17 12:04:10.000000 ibridges-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-17 12:04:10.000000 ibridges-0.1.4/.github/workflows/integration-tests-irods.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-17 12:04:10.000000 ibridges-0.1.4/.github/workflows/integration-tests-yoda.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-17 12:04:10.000000 ibridges-0.1.4/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-17 12:04:10.000000 ibridges-0.1.4/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-17 12:04:10.000000 ibridges-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-17 12:04:10.000000 ibridges-0.1.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 12:04:10.000000 ibridges-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-17 12:04:19.295724 ibridges-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-17 12:04:10.000000 ibridges-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_catalog/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_catalog/init-user-db.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_catalog_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_catalog_provider/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_catalog_provider/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_catalog_provider/setup-4.3.1.input
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.275724 ibridges-0.1.4/docker/irods_client/environments/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_client/environments/plain-irods/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/environments/plain-irods/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/environments/plain-irods/irods_environment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/environments/plain-irods/irods_environment_testuser.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_client/environments/yoda/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/environments/yoda/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/environments/yoda/irods_environment.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_client/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/testdata/beach.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/testdata/bunny.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/testdata/example.r
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_client/testdata/more_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/testdata/more_data/polarbear.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/testdata/plant.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/testdata/sun.rtf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.283724 ibridges-0.1.4/docker/irods_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_data_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.283724 ibridges-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.283724 ibridges-0.1.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.287724 ibridges-0.1.4/ibridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18555 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/data_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/export_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/icat_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11123 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/tickets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.291724 ibridges-0.1.4/ibridges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-17 12:04:10.000000 ibridges-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 12:04:19.295724 ibridges-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.287724 ibridges-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-17 12:04:10.000000 ibridges-0.1.4/tests/test_irodspath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.287724 ibridges-0.1.4/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-04-17 12:04:10.000000 ibridges-0.1.4/tests/testdata/bunny.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.287724 ibridges-0.1.4/tests/testdata/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-17 12:04:10.000000 ibridges-0.1.4/tests/testdata/subfolder/sun.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.287724 ibridges-0.1.4/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/01-Setup-and-connect.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12711 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/02-Working-with-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/03-iRODS-Paths.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/04-Metadata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/05-Data-Sharing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/Data_sync.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24498 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/QuickStart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.287724 ibridges-0.1.4/tutorials/example_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/example_rules/example.r
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/iRODS_paths.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.291724 ibridges-0.1.4/tutorials/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   227136 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/DataObject1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   246217 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/DataObject2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   277830 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/DataObject3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   297047 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/DataObject4.png
+-rw-r--r--   0 runner    (1001) docker     (127)   291147 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/DataObject5.png
+-rw-r--r--   0 runner    (1001) docker     (127)   303681 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/DataObject6.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/Save_json.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/Yoda_environment.png
```

### Comparing `ibridges-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md` & `ibridges-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `ibridges-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/.github/workflows/integration-tests-irods.yml` & `ibridges-0.1.4/.github/workflows/integration-tests-irods.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/.github/workflows/integration-tests-yoda.yml` & `ibridges-0.1.4/.github/workflows/integration-tests-yoda.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/.github/workflows/main.yml` & `ibridges-0.1.4/.github/workflows/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,18 @@
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install .[test]
 
+    - name: Lint with PyLint
+      run: |
+        pylint ibridges
+
     - name: Check types with MyPy
       run: |
         mypy ibridges
 
     - name: Check if documentation builds.
       run: |
         cd docs; make html SPHINXOPTS="--keep-going"
```

### Comparing `ibridges-0.1.3/.github/workflows/pypi_release.yml` & `ibridges-0.1.4/.github/workflows/pypi_release.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/.gitignore` & `ibridges-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/.readthedocs.yaml` & `ibridges-0.1.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/LICENSE` & `ibridges-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/PKG-INFO` & `ibridges-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibridges
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package for accessing data and metadata on iRods servers.
 Author-email: Christine Staiger <c.staiger@uu.nl>
 License: MIT License
         
         Copyright (c) 2024 Utrecht University
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -33,16 +33,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: python-irodsclient==1.1.6
+Requires-Dist: python-irodsclient>=1.1.6
 Requires-Dist: tqdm
+Requires-Dist: importlib-metadata; python_version < "3.10"
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: types-tqdm; extra == "test"
@@ -120,14 +121,54 @@
 # Download data
 from ibridges import download
 
 download(session, "/irods/path", "/other/local/path")
 
 ```
 
+## Commandline interface
+To simply upload or download data you do not need to write full python program, we offer a Commandline interface
+
+- Establish a connection
+
+  ```bash
+  ibridges init
+  ```
+
+- List a colletion
+  
+  ```bash
+  # list your home collection
+  ibridges list
+  
+  # list a different collection in your home
+  ibridges list irods:~/<collection>
+  
+  # list a collection on a different path than your home
+  ibridges. list irods:<full_irods_path>
+  ```
+
+- Upload data
+
+  ```bash
+  ibridges upload my_file.json irods:~/some_collection
+  ```
+
+- Download data
+
+  ```bash
+  ibridges download irods:~/some_collection/some_object download_dir
+  ```
+
+- Synchronise data
+
+  ```bash
+      ibridges sync some_local_directory irods:~/some_collection
+  ```
+
 ## Tutorials
 ### Documentation
 - **[ReadTheDocs](https://ibridges.readthedocs.io/en/latest/)**
 
 ### Guides
 - [QuickStart](tutorials/QuickStart.ipynb)
 - [iRODS Paths](tutorials/iRODS_paths.ipynb)
```

### Comparing `ibridges-0.1.3/README.md` & `ibridges-0.1.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -65,14 +65,54 @@
 # Download data
 from ibridges import download
 
 download(session, "/irods/path", "/other/local/path")
 
 ```
 
+## Commandline interface
+To simply upload or download data you do not need to write full python program, we offer a Commandline interface
+
+- Establish a connection
+
+  ```bash
+  ibridges init
+  ```
+
+- List a colletion
+  
+  ```bash
+  # list your home collection
+  ibridges list
+  
+  # list a different collection in your home
+  ibridges list irods:~/<collection>
+  
+  # list a collection on a different path than your home
+  ibridges. list irods:<full_irods_path>
+  ```
+
+- Upload data
+
+  ```bash
+  ibridges upload my_file.json irods:~/some_collection
+  ```
+
+- Download data
+
+  ```bash
+  ibridges download irods:~/some_collection/some_object download_dir
+  ```
+
+- Synchronise data
+
+  ```bash
+      ibridges sync some_local_directory irods:~/some_collection
+  ```
+
 ## Tutorials
 ### Documentation
 - **[ReadTheDocs](https://ibridges.readthedocs.io/en/latest/)**
 
 ### Guides
 - [QuickStart](tutorials/QuickStart.ipynb)
 - [iRODS Paths](tutorials/iRODS_paths.ipynb)
```

#### html2text {}

```diff
@@ -29,24 +29,33 @@
 features, you can install the development branch: ```bash pip install
 git+https://github.com/UtrechtUniversity/iBridges.git@develop ``` ## Usage
 Below are some basic examples of the features in iBridges. ```py # Create an
 iRODS session from ibridges import Session session = Session
 (irods_env_path="~/.irods/irods_environment.json", password="mypassword") #
 Upload data from ibridges import upload upload(session, "/your/local/path", "/
 irods/path") # Download data from ibridges import download download(session, "/
-irods/path", "/other/local/path") ``` ## Tutorials ### Documentation - **
-[ReadTheDocs](https://ibridges.readthedocs.io/en/latest/)** ### Guides -
-[QuickStart](tutorials/QuickStart.ipynb) - [iRODS Paths](tutorials/
-iRODS_paths.ipynb) - [Data synchronisation](tutorials/Data_sync.ipynb) ###
-Beginners tutorials - [Setup client configuration](tutorials/01-Setup-and-
-connect.ipynb) - [Working with data](tutorials/02-Working-with-data.ipynb) -
-[iRODS and local Paths](tutorials/03-iRODS-Paths.ipynb) - [Metadata](tutorials/
-04-Metadata.ipynb) - [Sharing data](tutorials/05-Data-Sharing.ipynb) ## Authors
-**Christine Staiger (Maintainer) [ORCID](https://orcid.org/0000-0002-6754-
-7647)** - *Wageningen University & Research* 2021 - 2022 - *Utrecht University*
-2022 **Tim van Daalen**, *Wageningen University & Research* 2021 **Maarten
-Schermer (Maintainer) [ORCID](https://orcid.org/my-orcid?orcid=0000-0001-6770-
-3155)**, *Utrecht University* 2023 **Raoul Schram (Maintainer) [ORCID](https://
+irods/path", "/other/local/path") ``` ## Commandline interface To simply upload
+or download data you do not need to write full python program, we offer a
+Commandline interface - Establish a connection ```bash ibridges init ``` - List
+a colletion ```bash # list your home collection ibridges list # list a
+different collection in your home ibridges list irods:~/ # list a collection on
+a different path than your home ibridges. list irods: ``` - Upload data ```bash
+ibridges upload my_file.json irods:~/some_collection ``` - Download data
+```bash ibridges download irods:~/some_collection/some_object download_dir ```
+- Synchronise data ```bash ibridges sync some_local_directory irods:~/
+some_collection ``` ## Tutorials ### Documentation - **[ReadTheDocs](https://
+ibridges.readthedocs.io/en/latest/)** ### Guides - [QuickStart](tutorials/
+QuickStart.ipynb) - [iRODS Paths](tutorials/iRODS_paths.ipynb) - [Data
+synchronisation](tutorials/Data_sync.ipynb) ### Beginners tutorials - [Setup
+client configuration](tutorials/01-Setup-and-connect.ipynb) - [Working with
+data](tutorials/02-Working-with-data.ipynb) - [iRODS and local Paths]
+(tutorials/03-iRODS-Paths.ipynb) - [Metadata](tutorials/04-Metadata.ipynb) -
+[Sharing data](tutorials/05-Data-Sharing.ipynb) ## Authors **Christine Staiger
+(Maintainer) [ORCID](https://orcid.org/0000-0002-6754-7647)** - *Wageningen
+University & Research* 2021 - 2022 - *Utrecht University* 2022 **Tim van
+Daalen**, *Wageningen University & Research* 2021 **Maarten Schermer
+(Maintainer) [ORCID](https://orcid.org/my-orcid?orcid=0000-0001-6770-3155)**,
+*Utrecht University* 2023 **Raoul Schram (Maintainer) [ORCID](https://
 orcid.org/my-orcid?orcid=0000-0001-6616-230X)**. *Utrecht University* 2023 ##
 Contributors **J.P. Mc Farland**, *University of Groningen, Center for
 Information Technology*, 2022 ## License This project is licensed under the MIT
 license. The full license can be found in [LICENSE](LICENSE).
```

### Comparing `ibridges-0.1.3/docker/.gitattributes` & `ibridges-0.1.4/docker/.gitattributes`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/README.md` & `ibridges-0.1.4/docker/README.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_catalog_provider/Dockerfile` & `ibridges-0.1.4/docker/irods_catalog_provider/Dockerfile`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/Dockerfile` & `ibridges-0.1.4/docker/irods_client/Dockerfile`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/entrypoint.sh` & `ibridges-0.1.4/docker/irods_client/entrypoint.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /bin/bash -e
 
 echo "waiting for iRODS to be ready"
 
 irods_catalog_provider_hostname=irods-catalog-provider
 until nc -z ${irods_catalog_provider_hostname} 1247
 do
-    sleep 1
+    sleep 10
 done
 
 # After setting up iRODS, the server will respond on port 1247. However, the server process is
 # stopped after some preliminary tests are completed. The irods-catalog-provider service will
 # start the server manually again, but this will take a few seconds. Sleep here to ensure that
 # next time the server responds is not the temporary uptime provided during setup.
 sleep 3
@@ -20,20 +20,31 @@
 done
 
 echo "iRODS is ready"
 
 # pre-authenticate the user so the iCommands are ready to use
 echo 'rods' | iinit
 echo 'Authenticated as rods'
+
+# wait until second resource is created
+ilsresc | grep 'resc2' &> /dev/null
+while [ $? != 0 ];
+do
+    echo "Sleep"
+    sleep 1
+done
+
+# create second user
 iadmin mkuser testuser rodsuser
 iadmin moduser testuser password testuser
 echo 'testuser created'
 echo $(iadmin lu testuser)
 
 cd /ibridges/integration_test
 pytest .
+
 result=$?
 if [[ -z "$CI" ]]; then
-  /bin/bash
+    /bin/bash
 else
-  exit $result
-fi
+    exit $result
+fi
```

### Comparing `ibridges-0.1.3/docker/irods_client/environments/yoda/config.toml` & `ibridges-0.1.4/docker/irods_client/environments/yoda/config.toml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/environments/yoda/irods_environment.json` & `ibridges-0.1.4/docker/irods_client/environments/yoda/irods_environment.json`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/testdata/beach.rtf` & `ibridges-0.1.4/docker/irods_client/testdata/beach.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/testdata/bunny.rtf` & `ibridges-0.1.4/docker/irods_client/testdata/bunny.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/testdata/more_data/polarbear.txt` & `ibridges-0.1.4/docker/irods_client/testdata/more_data/polarbear.txt`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/testdata/plant.rtf` & `ibridges-0.1.4/docker/irods_client/testdata/plant.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/testdata/sun.rtf` & `ibridges-0.1.4/docker/irods_client/testdata/sun.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/tests/conftest.py` & `ibridges-0.1.4/docker/irods_client/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/tests/test_data_ops.py` & `ibridges-0.1.4/docker/irods_client/tests/test_data_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     upload,
 )
 from ibridges.path import IrodsPath
 
 
 def _get_digest(obj_or_file):
     with open(obj_or_file, "rb") as handle:
-        digest = hashlib.sha1(handle.read()).digest()
+        digest = hashlib.sha256(handle.read()).digest()
     return digest
 
 def _check_files_equal(*files):
     assert len(files) > 0
     digests = [_get_digest(f) for f in files]
 
     for dig in digests[1:]:
```

### Comparing `ibridges-0.1.3/docker/irods_client/tests/test_meta.py` & `ibridges-0.1.4/docker/irods_client/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/tests/test_permissions.py` & `ibridges-0.1.4/docker/irods_client/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/tests/test_session.py` & `ibridges-0.1.4/docker/irods_client/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/tests/test_sync.py` & `ibridges-0.1.4/docker/irods_client/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker/irods_client/tests/test_ticket.py` & `ibridges-0.1.4/docker/irods_client/tests/test_ticket.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docker-compose.yml` & `ibridges-0.1.4/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docs/Makefile` & `ibridges-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docs/make.bat` & `ibridges-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docs/source/api.rst` & `ibridges-0.1.4/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docs/source/conf.py` & `ibridges-0.1.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docs/source/faq.rst` & `ibridges-0.1.4/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/docs/source/index.rst` & `ibridges-0.1.4/docs/source/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 .. toctree::
    :hidden:
    :maxdepth: 2
    :caption: Contents:
 
    quickstart
+   cli
    faq
    api
 
 
 Indices and tables
 ==================
```

### Comparing `ibridges-0.1.3/docs/source/quickstart.rst` & `ibridges-0.1.4/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/ibridges/__init__.py` & `ibridges-0.1.4/ibridges/__init__.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/ibridges/data_operations.py` & `ibridges-0.1.4/ibridges/data_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,27 +162,30 @@
         options[kw.RESC_NAME_KW] = resc_name
     if overwrite or not obj_exists:
         session.irods_session.data_objects.put(local_path, str(irods_path), **options)
     else:
         raise irods.exception.OVERWRITE_WITHOUT_FORCE_FLAG
 
 def _obj_get(session: Session, irods_path: Union[str, IrodsPath], local_path: Union[str, Path],
-             overwrite: bool = False, options: Optional[dict] = None):
+             overwrite: bool = False, resc_name: Optional[str] = '',
+             options: Optional[dict] = None):
     """Download `irods_path` to `local_path` following iRODS `options`.
 
     Parameters
     ----------
     session :
         Session to get the object from.
     irods_path : str or IrodsPath
         Path of iRODS data object.
     local_path : str or Path
         Path of local file or directory/folder.
     overwrite :
         Whether to overwrite the local file if it exists.
+    resc_name:
+        Name of the resource to get the object from.
     options : dict
         iRODS transfer options.
 
     """
     irods_path = IrodsPath(session, irods_path)
     if not irods_path.dataobject_exists():
         raise ValueError("irods_path must be a data object.")
@@ -190,15 +193,16 @@
         options = {}
     options.update({
         kw.NUM_THREADS_KW: NUM_THREADS,
         kw.VERIFY_CHKSUM_KW: '',
         })
     if overwrite:
         options[kw.FORCE_FLAG_KW] = ''
-
+    if resc_name not in ['', None]:
+        options[kw.RESC_NAME_KW] = resc_name
     session.irods_session.data_objects.get(str(irods_path), local_path, **options)
 
 def _create_irods_dest(local_path: Path, irods_path: IrodsPath
                        ) -> list[tuple[Path, IrodsPath]]:
     """Assembles the irods destination paths for upload of a folder."""
     upload_path = irods_path.joinpath(local_path.name)
     paths = [(str(Path(root).relative_to(local_path)), f)
@@ -269,15 +273,15 @@
         cur_lpath = (download_path / IrodsPath(session, subcoll_path).relative_to(irods_path)
                                    / obj_name)
         source_to_dest.append((cur_ipath, cur_lpath))
     return source_to_dest
 
 
 def _download_collection(session: Session, irods_path: Union[str, IrodsPath], local_path: Path,
-                         overwrite: bool = False, ignore_err: bool = False,
+                         overwrite: bool = False, ignore_err: bool = False, resc_name: str = '',
                          options: Optional[dict] = None):
     """Download a collection to the local filesystem.
 
     Parameters
     ----------
     session :
         Session to download the collection from.
@@ -288,14 +292,16 @@
     overwrite : bool
         Overwrite existing local data
     ignore_err : bool
         If an error occurs during download, and ignore_err is set to True, any errors encountered
         will be transformed into warnings and iBridges will continue to download the remaining
         files.
         By default all errors will stop the process of uploading.
+    resc_name : str
+        Name of the resource from which data is downloaded, by default the server will decide
     options : dict
         More options for the download
 
     """
     irods_path = IrodsPath(session, irods_path)
     if not irods_path.collection_exists():
         raise ValueError("irods_path must be a collection.")
@@ -303,15 +309,15 @@
     source_to_dest = _create_local_dest(session, irods_path, local_path)
 
     for source, dest in source_to_dest:
         # ensure local folder exists
         if not dest.parent.is_dir():
             os.makedirs(dest.parent)
         try:
-            _obj_get(session, source, dest, overwrite, options)
+            _obj_get(session, source, dest, overwrite, resc_name, options)
         except irods.exception.OVERWRITE_WITHOUT_FORCE_FLAG:
             warnings.warn(f'File already exists\tSkipping {source}')
         except KeyError as e:
             if ignore_err is True:
                 warnings.warn(f'Download failed: {source}i\n'+repr(e))
             else:
                 raise ValueError(f'Download failed: {source}: '+repr(e)) from e
@@ -349,22 +355,28 @@
 
     """
     local_path = Path(local_path)
     try:
         if local_path.is_dir():
             _upload_collection(session, local_path, irods_path, overwrite, ignore_err,
                                resc_name, options)
-        else:
+        elif local_path.is_file():
             _obj_put(session, local_path, irods_path, overwrite, resc_name, options)
+        else:
+            raise FileNotFoundError(f"Cannot find local file '{local_path}', check the path.")
     except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
         raise PermissionError(
             f"During upload operation to '{irods_path}': iRODS server forbids action.") from exc
+    except irods.exception.OVERWRITE_WITHOUT_FORCE_FLAG as exc:
+        raise FileExistsError(f"Dataset or collection (in) {irods_path} already exists. "
+                              "Use overwrite=True to overwrite the existing file(s).") from exc
 
 def download(session: Session, irods_path: Union[str, IrodsPath], local_path: Union[str, Path],
-             overwrite: bool = False, ignore_err: bool = False, options: Optional[dict] = None):
+             overwrite: bool = False, ignore_err: bool = False, resc_name: str = '',
+             options: Optional[dict] = None):
     """Download a collection or data object to the local filesystem.
 
     Parameters
     ----------
     session :
         Session to download the collection from.
     irods_path : IrodsPath
@@ -374,14 +386,16 @@
     overwrite : bool
         If an error occurs during download, and ignore_err is set to True, any errors encountered
         will be transformed into warnings and iBridges will continue to download the remaining
         files.
         By default all errors will stop the process of downloading.
     ignore_err : bool
         Collections: If download of an item fails print error and continue with next item.
+    resc_name : str
+        Name of the resource from which data is downloaded, by default the server will decide.
     options : dict
         More options for the download
 
     Raises
     ------
     PermissionError:
         If the iRods server (for whatever reason) forbids downloading the file or
@@ -390,21 +404,27 @@
         If the irods_path is not pointing to either a collection or a data object.
 
     """
     irods_path = IrodsPath(session, irods_path)
     local_path = Path(local_path)
     try:
         if irods_path.collection_exists():
-            _download_collection(session, irods_path, local_path, overwrite, ignore_err, options)
+            _download_collection(session, irods_path, local_path, overwrite, ignore_err, resc_name,
+                                 options)
+        elif irods_path.dataobject_exists():
+            _obj_get(session, irods_path, local_path, overwrite, resc_name, options)
         else:
-            _obj_get(session, irods_path, local_path, overwrite, options)
+            raise ValueError(f"Data object or collection not found: '{irods_path}'")
     except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
         raise PermissionError(
             f"During download operation from '{irods_path}': iRODS server forbids action."
             ) from exc
+    except irods.exception.OVERWRITE_WITHOUT_FORCE_FLAG as exc:
+        raise FileExistsError(f"File or directory {local_path} already exists. "
+                              "Use overwrite=True to overwrite the existing file(s).") from exc
 
 def get_size(session: Session, item: Union[irods.data_object.iRODSDataObject,
                                irods.collection.iRODSCollection]) -> int:
     """Collect the sizes of a data object or a collection.
 
     Parameters
     ----------
```

### Comparing `ibridges-0.1.3/ibridges/export_metadata.py` & `ibridges-0.1.4/ibridges/export_metadata.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/ibridges/icat_columns.py` & `ibridges-0.1.4/ibridges/icat_columns.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/ibridges/interactive.py` & `ibridges-0.1.4/ibridges/interactive.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Interactive authentication with iRODS server."""
 
-import json
 import os
 from getpass import getpass
 from pathlib import Path
 from typing import Optional, Union
 
-from ibridges.session import Session
+from ibridges.session import Session, LoginError, PasswordError
 
 DEFAULT_IENV_PATH = Path(os.path.expanduser("~")).joinpath(".irods", "irods_environment.json")
 
 def interactive_auth(password: Optional[str] = None,
-                     irods_env_path: Union[str, Path] = DEFAULT_IENV_PATH) -> Session:
+                     irods_env_path: Union[None, str, Path] = None) -> Session:
     """Interactive authentication with iRODS server.
 
     Stores the password in ~/.irods/.irodsA upon success.
 
     Parameters
     ----------
     password:
@@ -31,43 +30,58 @@
         If the connection to the iRods server cannot be established.
 
     Returns
     -------
         A connected session to the server.
 
     """
+    if irods_env_path is None:
+        irods_env_path = DEFAULT_IENV_PATH
     if not os.path.exists(irods_env_path):
         print(f'File not found: {irods_env_path}')
         raise FileNotFoundError
 
-    if os.path.exists(Path(os.path.expanduser("~")).joinpath(".irods", ".irodsA")):
-        try:
-            session = Session(irods_env_path)
-            return session
-        except IndexError:
-            print('INFO: The cached password in ~/.irods/.irodsA has been corrupted')
-        except ValueError:
-            print('INFO: The cached password in ~/.irods/.irodsA is wrong.')
+    session = None
+    if os.path.exists(Path(os.path.expanduser("~")).joinpath(".irods", ".irodsA")) and \
+            password is None:
+        session = _from_pw_file(irods_env_path)
 
-    with open(irods_env_path, "r", encoding="utf-8") as f:
-        ienv = json.load(f)
     if password is not None:
+        session = _from_password(irods_env_path, password)
+
+    if session is not None:
+        return session
+
+    # If provided passwords in file or on prompt were wrong
+    n_tries = 0
+    success = False
+    while not success and n_tries < 3:
+        password = getpass("Your iRODS password: ")
         try:
-            session = Session(ienv, password=password)
+            session = Session(irods_env=irods_env_path, password=password)
             session.write_pam_password()
+            success = True
             return session
-        except ValueError:
+        except PasswordError as e:
+            print(repr(e))
             print('INFO: The provided password is wrong.')
-    else:
-        n_tries = 0
-        success = False
-        while not success and n_tries < 3:
-            password = getpass("Your iRODS password: ")
-            try:
-                session = Session(irods_env=ienv, password=password)
-                session.write_pam_password()
-                success = True
-                return session
-            except ValueError:
-                print('INFO: The provided password is wrong.')
-                n_tries+=1
-    raise ValueError("Connection to iRODS could not be established.")
+            n_tries+=1
+    raise LoginError("Connection to iRODS could not be established.")
+
+def _from_pw_file(irods_env_path):
+    try:
+        session = Session(irods_env_path)
+        return session
+    except IndexError:
+        print('INFO: The cached password in ~/.irods/.irodsA has been corrupted')
+    except PasswordError:
+        print('INFO: The cached password in ~/.irods/.irodsA is wrong.')
+    return None
+
+def _from_password(irods_env_path, password):
+    try:
+        session = Session(irods_env=irods_env_path, password=password)
+        session.write_pam_password()
+        return session
+    except PasswordError:
+        print('INFO: Wrong password.')
+    return None
```

### Comparing `ibridges-0.1.3/ibridges/meta.py` & `ibridges-0.1.4/ibridges/meta.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/ibridges/path.py` & `ibridges-0.1.4/ibridges/path.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/ibridges/permissions.py` & `ibridges-0.1.4/ibridges/permissions.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/ibridges/resources.py` & `ibridges-0.1.4/ibridges/resources.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/ibridges/rules.py` & `ibridges-0.1.4/ibridges/rules.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/ibridges/search.py` & `ibridges-0.1.4/ibridges/search.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/ibridges/sync.py` & `ibridges-0.1.4/ibridges/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     The command can be in one of the two modes: synchronization of data from the client's local file
     system to iRODS, or from iRODS to the local file system. The mode is determined by the type of
     the values for `source` and `target` (IrodsPath or str/Path).
 
     The command considers the file size and the checksum to determine whether a file should be
     synchronized.
 
-    
+
     Parameters
     ----------
     session : ibridges.Session
         An authorized iBridges session.
     source : str or Path or IrodsPath
         Existing local folder or iRODS collection. An exception will be raised if it doesn't exist.
     target : str or Path or IrodsPath
@@ -113,27 +113,28 @@
         Controls the depth up to which the file tree will be synchronized. A max level of 1
         synchronizes only the source's root, max level 2 also includes the first set of
         subfolders/subcollections and their contents, etc. Set to None, there is no limit
         (full recursive synchronization).
     dry_run : bool, default False
         List all source files and folders that need to be synchronized without actually
         performing synchronization.
-    ignore_err : If an error occurs during the transfer, and ignore_err is set to True, 
+    ignore_err : If an error occurs during the transfer, and ignore_err is set to True,
         any errors encountered will be transformed into warnings and iBridges will continue
         to transfer the remaining files.
     copy_empty_folders : bool, default False
         Controls whether folders/collections that contain no files or  subfolders/subcollections
         will be synchronized.
 
 
     Returns
     -------
         A dict object containing two keys: 'changed_folders' and 'changed_files'.
         These contain lists of changed folders and files, respectively
         (or of to-be-changed folders and files, when in dry-run mode).
+
     """
     _param_checks(source, target)
 
     if isinstance(source, IrodsPath):
         if not source.collection_exists():
             raise ValueError(f"Source collection '{source.absolute_path()}' does not exist")
         src_files, src_folders=_get_irods_tree(
```

### Comparing `ibridges-0.1.3/ibridges/tickets.py` & `ibridges-0.1.4/ibridges/tickets.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/ibridges.egg-info/PKG-INFO` & `ibridges-0.1.4/ibridges.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibridges
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package for accessing data and metadata on iRods servers.
 Author-email: Christine Staiger <c.staiger@uu.nl>
 License: MIT License
         
         Copyright (c) 2024 Utrecht University
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -33,16 +33,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: python-irodsclient==1.1.6
+Requires-Dist: python-irodsclient>=1.1.6
 Requires-Dist: tqdm
+Requires-Dist: importlib-metadata; python_version < "3.10"
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: types-tqdm; extra == "test"
@@ -120,14 +121,54 @@
 # Download data
 from ibridges import download
 
 download(session, "/irods/path", "/other/local/path")
 
 ```
 
+## Commandline interface
+To simply upload or download data you do not need to write full python program, we offer a Commandline interface
+
+- Establish a connection
+
+  ```bash
+  ibridges init
+  ```
+
+- List a colletion
+  
+  ```bash
+  # list your home collection
+  ibridges list
+  
+  # list a different collection in your home
+  ibridges list irods:~/<collection>
+  
+  # list a collection on a different path than your home
+  ibridges. list irods:<full_irods_path>
+  ```
+
+- Upload data
+
+  ```bash
+  ibridges upload my_file.json irods:~/some_collection
+  ```
+
+- Download data
+
+  ```bash
+  ibridges download irods:~/some_collection/some_object download_dir
+  ```
+
+- Synchronise data
+
+  ```bash
+      ibridges sync some_local_directory irods:~/some_collection
+  ```
+
 ## Tutorials
 ### Documentation
 - **[ReadTheDocs](https://ibridges.readthedocs.io/en/latest/)**
 
 ### Guides
 - [QuickStart](tutorials/QuickStart.ipynb)
 - [iRODS Paths](tutorials/iRODS_paths.ipynb)
```

### Comparing `ibridges-0.1.3/ibridges.egg-info/SOURCES.txt` & `ibridges-0.1.4/ibridges.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 README.md
 docker-compose.yml
 pyproject.toml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/integration-tests-irods.yml
 .github/workflows/integration-tests-yoda.yml
-.github/workflows/lint.yml
 .github/workflows/main.yml
 .github/workflows/pypi_release.yml
 docker/.gitattributes
 docker/README.md
 docker/irods_catalog/Dockerfile
 docker/irods_catalog/init-user-db.sh
 docker/irods_catalog_provider/Dockerfile
@@ -29,31 +28,34 @@
 docker/irods_client/testdata/beach.rtf
 docker/irods_client/testdata/bunny.rtf
 docker/irods_client/testdata/example.r
 docker/irods_client/testdata/plant.rtf
 docker/irods_client/testdata/sun.rtf
 docker/irods_client/testdata/more_data/polarbear.txt
 docker/irods_client/tests/conftest.py
+docker/irods_client/tests/test_cli.py
 docker/irods_client/tests/test_data_ops.py
 docker/irods_client/tests/test_meta.py
 docker/irods_client/tests/test_permissions.py
 docker/irods_client/tests/test_resources.py
 docker/irods_client/tests/test_rules.py
 docker/irods_client/tests/test_session.py
 docker/irods_client/tests/test_sync.py
 docker/irods_client/tests/test_ticket.py
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/api.rst
+docs/source/cli.rst
 docs/source/conf.py
 docs/source/faq.rst
 docs/source/index.rst
 docs/source/quickstart.rst
 ibridges/__init__.py
+ibridges/__main__.py
 ibridges/_version.py
 ibridges/data_operations.py
 ibridges/export_metadata.py
 ibridges/icat_columns.py
 ibridges/interactive.py
 ibridges/meta.py
 ibridges/path.py
@@ -63,14 +65,15 @@
 ibridges/search.py
 ibridges/session.py
 ibridges/sync.py
 ibridges/tickets.py
 ibridges.egg-info/PKG-INFO
 ibridges.egg-info/SOURCES.txt
 ibridges.egg-info/dependency_links.txt
+ibridges.egg-info/entry_points.txt
 ibridges.egg-info/requires.txt
 ibridges.egg-info/top_level.txt
 tests/test_irodspath.py
 tests/testdata/bunny.txt
 tests/testdata/subfolder/sun.csv
 tutorials/01-Setup-and-connect.ipynb
 tutorials/02-Working-with-data.ipynb
```

### Comparing `ibridges-0.1.3/pyproject.toml` & `ibridges-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -19,16 +19,17 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
 ]
 
 dependencies = [
-    "python-irodsclient==1.1.6",
+    "python-irodsclient>=1.1.6",
     "tqdm",
+    "importlib-metadata;python_version<'3.10'",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 GitHub = "https://github.com/UtrechtUniversity/iBridges"
 documentation = "https://github.com/UtrechtUniversity/iBridges"
@@ -42,14 +43,17 @@
     "mypy",
     "types-tqdm",
     "sphinx", "sphinx-rtd-theme", "sphinxcontrib-napoleon",
     "sphinx-autodoc-typehints", "sphinx_inline_tabs", "sphinx_copybutton",
 ]
 
 
+[project.scripts]
+ibridges = "ibridges.__main__:main"
+
 [tool.setuptools]
 packages = ["ibridges"]
 
 [tool.setuptools_scm]
 write_to = "ibridges/_version.py"
 
 [[tool.mypy.overrides]]
```

### Comparing `ibridges-0.1.3/tests/test_irodspath.py` & `ibridges-0.1.4/tests/test_irodspath.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tests/testdata/bunny.txt` & `ibridges-0.1.4/tests/testdata/bunny.txt`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tests/testdata/subfolder/sun.csv` & `ibridges-0.1.4/tests/testdata/subfolder/sun.csv`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/01-Setup-and-connect.ipynb` & `ibridges-0.1.4/tutorials/01-Setup-and-connect.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/02-Working-with-data.ipynb` & `ibridges-0.1.4/tutorials/02-Working-with-data.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/03-iRODS-Paths.ipynb` & `ibridges-0.1.4/tutorials/03-iRODS-Paths.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/04-Metadata.ipynb` & `ibridges-0.1.4/tutorials/04-Metadata.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/05-Data-Sharing.ipynb` & `ibridges-0.1.4/tutorials/05-Data-Sharing.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/Data_sync.ipynb` & `ibridges-0.1.4/tutorials/Data_sync.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/QuickStart.ipynb` & `ibridges-0.1.4/tutorials/QuickStart.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/iRODS_paths.ipynb` & `ibridges-0.1.4/tutorials/iRODS_paths.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/img/DataObject1.png` & `ibridges-0.1.4/tutorials/img/DataObject1.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/img/DataObject2.png` & `ibridges-0.1.4/tutorials/img/DataObject2.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/img/DataObject3.png` & `ibridges-0.1.4/tutorials/img/DataObject3.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/img/DataObject4.png` & `ibridges-0.1.4/tutorials/img/DataObject4.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/img/DataObject5.png` & `ibridges-0.1.4/tutorials/img/DataObject5.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/img/DataObject6.png` & `ibridges-0.1.4/tutorials/img/DataObject6.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/img/Save_json.png` & `ibridges-0.1.4/tutorials/img/Save_json.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.3/tutorials/img/Yoda_environment.png` & `ibridges-0.1.4/tutorials/img/Yoda_environment.png`

 * *Files identical despite different names*

