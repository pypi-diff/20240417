# Comparing `tmp/dbis-relational-model-0.0.9.tar.gz` & `tmp/dbis_relational_model-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-relational-model-0.0.9.tar", last modified: Wed May 11 09:14:38 2022, max compression
+gzip compressed data, was "dbis_relational_model-1.0.1.tar", last modified: Wed Apr 17 08:19:29 2024, max compression
```

## Comparing `dbis-relational-model-0.0.9.tar` & `dbis_relational_model-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 philipph  (1000) philipph  (1000)        0 2022-05-11 09:14:38.844212 dbis-relational-model-0.0.9/
--rw-r--r--   0 philipph  (1000) philipph  (1000)    11357 2022-04-25 13:46:59.000000 dbis-relational-model-0.0.9/LICENSE
--rw-r--r--   0 philipph  (1000) philipph  (1000)      753 2022-05-11 09:14:38.844212 dbis-relational-model-0.0.9/PKG-INFO
--rw-r--r--   0 philipph  (1000) philipph  (1000)      161 2022-04-25 14:25:35.000000 dbis-relational-model-0.0.9/README.md
-drwxr-xr-x   0 philipph  (1000) philipph  (1000)        0 2022-05-11 09:14:38.844212 dbis-relational-model-0.0.9/dbis_relational_model.egg-info/
--rw-r--r--   0 philipph  (1000) philipph  (1000)      753 2022-05-11 09:14:38.000000 dbis-relational-model-0.0.9/dbis_relational_model.egg-info/PKG-INFO
--rw-r--r--   0 philipph  (1000) philipph  (1000)      272 2022-05-11 09:14:38.000000 dbis-relational-model-0.0.9/dbis_relational_model.egg-info/SOURCES.txt
--rw-r--r--   0 philipph  (1000) philipph  (1000)        1 2022-05-11 09:14:38.000000 dbis-relational-model-0.0.9/dbis_relational_model.egg-info/dependency_links.txt
--rw-r--r--   0 philipph  (1000) philipph  (1000)       17 2022-05-11 09:14:38.000000 dbis-relational-model-0.0.9/dbis_relational_model.egg-info/top_level.txt
-drwxr-xr-x   0 philipph  (1000) philipph  (1000)        0 2022-05-11 09:14:38.844212 dbis-relational-model-0.0.9/relational_model/
--rw-r--r--   0 philipph  (1000) philipph  (1000)        0 2022-04-25 13:46:59.000000 dbis-relational-model-0.0.9/relational_model/__init__.py
--rw-r--r--   0 philipph  (1000) philipph  (1000)    10831 2022-05-11 09:12:29.000000 dbis-relational-model-0.0.9/relational_model/relational_model.py
--rw-r--r--   0 philipph  (1000) philipph  (1000)       38 2022-05-11 09:14:38.844212 dbis-relational-model-0.0.9/setup.cfg
--rw-r--r--   0 philipph  (1000) philipph  (1000)     1086 2022-05-11 09:12:54.000000 dbis-relational-model-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:19:29.418484 dbis_relational_model-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-02-06 11:28:22.000000 dbis_relational_model-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      903 2024-04-17 08:19:29.418484 dbis_relational_model-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-02-06 11:28:22.000000 dbis_relational_model-1.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-04-17 08:00:00.000000 dbis_relational_model-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 08:19:29.418484 dbis_relational_model-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:19:29.414484 dbis_relational_model-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:19:29.414484 dbis_relational_model-1.0.1/src/dbis_relational_model/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-17 08:00:00.000000 dbis_relational_model-1.0.1/src/dbis_relational_model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18225 2024-04-17 08:02:44.000000 dbis_relational_model-1.0.1/src/dbis_relational_model/relational_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:19:29.418484 dbis_relational_model-1.0.1/src/dbis_relational_model.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      903 2024-04-17 08:19:29.000000 dbis_relational_model-1.0.1/src/dbis_relational_model.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      379 2024-04-17 08:19:29.000000 dbis_relational_model-1.0.1/src/dbis_relational_model.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 08:19:29.000000 dbis_relational_model-1.0.1/src/dbis_relational_model.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-17 08:19:29.000000 dbis_relational_model-1.0.1/src/dbis_relational_model.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-17 08:19:29.000000 dbis_relational_model-1.0.1/src/dbis_relational_model.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:19:29.418484 dbis_relational_model-1.0.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4352 2024-04-17 08:02:44.000000 dbis_relational_model-1.0.1/tests/test_Task.py
```

### Comparing `dbis-relational-model-0.0.9/LICENSE` & `dbis_relational_model-1.0.1/LICENSE`

 * *Files identical despite different names*

