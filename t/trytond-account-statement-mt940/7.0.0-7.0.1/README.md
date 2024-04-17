# Comparing `tmp/trytond_account_statement_mt940-7.0.0.tar.gz` & `tmp/trytond_account_statement_mt940-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement_mt940-7.0.0.tar", last modified: Mon Oct 30 17:24:32 2023, max compression
+gzip compressed data, was "trytond_account_statement_mt940-7.0.1.tar", last modified: Wed Apr 17 10:41:15 2024, max compression
```

## Comparing `trytond_account_statement_mt940-7.0.0.tar` & `trytond_account_statement_mt940-7.0.1.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:32.643918 trytond_account_statement_mt940-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-22 17:22:55.000000 trytond_account_statement_mt940-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:03:23.000000 trytond_account_statement_mt940-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:03:23.000000 trytond_account_statement_mt940-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2804 2023-10-30 17:24:32.643918 trytond_account_statement_mt940-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      541 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5419 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1365 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:32.643918 trytond_account_statement_mt940-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2824 2023-10-22 17:22:55.000000 trytond_account_statement_mt940-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:55.000000 trytond_account_statement_mt940-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:32.643918 trytond_account_statement_mt940-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/icons/LICENSE
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:32.640584 trytond_account_statement_mt940-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      972 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      967 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      973 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      980 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      967 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-28 12:11:20.000000 trytond_account_statement_mt940-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:24:32.643918 trytond_account_statement_mt940-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4758 2023-10-27 17:38:49.000000 trytond_account_statement_mt940-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:32.640584 trytond_account_statement_mt940-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      162 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/tests/MT940.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3486 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/tests/scenario_account_statement_mt940.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_statement_mt940-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       91 2023-10-30 17:03:19.000000 trytond_account_statement_mt940-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:32.643918 trytond_account_statement_mt940-7.0.0/trytond_account_statement_mt940.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2804 2023-10-30 17:24:32.000000 trytond_account_statement_mt940-7.0.0/trytond_account_statement_mt940.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1667 2023-10-30 17:24:32.000000 trytond_account_statement_mt940-7.0.0/trytond_account_statement_mt940.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:24:32.000000 trytond_account_statement_mt940-7.0.0/trytond_account_statement_mt940.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-10-30 17:24:32.000000 trytond_account_statement_mt940-7.0.0/trytond_account_statement_mt940.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:55:54.000000 trytond_account_statement_mt940-7.0.0/trytond_account_statement_mt940.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      109 2023-10-30 17:24:32.000000 trytond_account_statement_mt940-7.0.0/trytond_account_statement_mt940.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:24:32.000000 trytond_account_statement_mt940-7.0.0/trytond_account_statement_mt940.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:32.640584 trytond_account_statement_mt940-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-08-13 15:26:13.000000 trytond_account_statement_mt940-7.0.0/view/statement_import_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.107930 trytond_account_statement_mt940-7.0.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-17 10:41:12.000000 trytond_account_statement_mt940-7.0.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-17 10:41:12.000000 trytond_account_statement_mt940-7.0.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2795 2024-04-17 10:41:15.107930 trytond_account_statement_mt940-7.0.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      541 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5441 2024-04-12 22:34:01.000000 trytond_account_statement_mt940-7.0.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1365 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.104597 trytond_account_statement_mt940-7.0.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2802 2024-03-03 16:24:20.000000 trytond_account_statement_mt940-7.0.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.104597 trytond_account_statement_mt940-7.0.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/icons/LICENSE
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.104597 trytond_account_statement_mt940-7.0.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      972 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      967 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      973 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      980 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      967 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:41:15.107930 trytond_account_statement_mt940-7.0.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4749 2024-03-03 16:24:03.000000 trytond_account_statement_mt940-7.0.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.107930 trytond_account_statement_mt940-7.0.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      162 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/tests/MT940.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3486 2024-02-05 16:24:27.000000 trytond_account_statement_mt940-7.0.1/tests/scenario_account_statement_mt940.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       91 2024-02-05 16:24:27.000000 trytond_account_statement_mt940-7.0.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.107930 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2795 2024-04-17 10:41:14.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1649 2024-04-17 10:41:15.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:41:14.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-17 10:41:14.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:38.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      109 2024-04-17 10:41:14.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:41:14.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.107930 trytond_account_statement_mt940-7.0.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/view/statement_import_start_form.xml
```

### Comparing `trytond_account_statement_mt940-7.0.0/COPYRIGHT` & `trytond_account_statement_mt940-7.0.1/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2022-2023 B2CK
-Copyright (C) 2022-2023 Cédric Krier
+Copyright (C) 2022-2024 B2CK
+Copyright (C) 2022-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_statement_mt940-7.0.0/LICENSE` & `trytond_account_statement_mt940-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/PKG-INFO` & `trytond_account_statement_mt940-7.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement_mt940
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton module to import MT940 statements
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: bugs@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-statement-mt940
+Project-URL: Documentation, https://docs.tryton.org/modules-account-statement-mt940
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account statement mt940
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_account_statement_mt940-7.0.0/__init__.py` & `trytond_account_statement_mt940-7.0.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/account.py` & `trytond_account_statement_mt940-7.0.1/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         Origin = pool.get('account.statement.origin')
 
         origin = Origin()
         origin.number = transaction.id
         origin.date = transaction.date
         origin.amount = transaction.amount
         origin.party = self.mt940_party(mt940_statement, transaction)
-        origin.description = transaction.description
+        origin.description = ''.join(transaction.description.splitlines())
         origin.information = self.mt940_information(
             mt940_statement, transaction)
         return [origin]
 
     def mt940_party(self, mt940_statement, transaction):
         pool = Pool()
         AccountNumber = pool.get('bank.account.number')
```

### Comparing `trytond_account_statement_mt940-7.0.0/account.xml` & `trytond_account_statement_mt940-7.0.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/doc/conf.py` & `trytond_account_statement_mt940-7.0.1/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 base_url = os.environ.get('DOC_BASE_URL')
 if base_url:
     modules_url = base_url + '/modules-{module}/'
     trytond_url = base_url + '/server/'
 else:
     modules_url = (
-        'https://docs.tryton.org/projects/modules-{module}/en/{series}/')
-    trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
+        'https://docs.tryton.org/${series}/modules-{module}/')
+    trytond_url = 'https://docs.tryton.org/${series}/server/'
 
 
 def get_info():
     import configparser
     import subprocess
     import sys
```

### Comparing `trytond_account_statement_mt940-7.0.0/icons/LICENSE` & `trytond_account_statement_mt940-7.0.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/bg.po` & `trytond_account_statement_mt940-7.0.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/ca.po` & `trytond_account_statement_mt940-7.0.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/cs.po` & `trytond_account_statement_mt940-7.0.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/de.po` & `trytond_account_statement_mt940-7.0.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/es.po` & `trytond_account_statement_mt940-7.0.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/es_419.po` & `trytond_account_statement_mt940-7.0.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/et.po` & `trytond_account_statement_mt940-7.0.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/fa.po` & `trytond_account_statement_mt940-7.0.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/fi.po` & `trytond_account_statement_mt940-7.0.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/fr.po` & `trytond_account_statement_mt940-7.0.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/hu.po` & `trytond_account_statement_mt940-7.0.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/id.po` & `trytond_account_statement_mt940-7.0.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/it.po` & `trytond_account_statement_mt940-7.0.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/lo.po` & `trytond_account_statement_mt940-7.0.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/lt.po` & `trytond_account_statement_mt940-7.0.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/nl.po` & `trytond_account_statement_mt940-7.0.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/pl.po` & `trytond_account_statement_mt940-7.0.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/pt.po` & `trytond_account_statement_mt940-7.0.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/ro.po` & `trytond_account_statement_mt940-7.0.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/ru.po` & `trytond_account_statement_mt940-7.0.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/sl.po` & `trytond_account_statement_mt940-7.0.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/tr.po` & `trytond_account_statement_mt940-7.0.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/uk.po` & `trytond_account_statement_mt940-7.0.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/locale/zh_CN.po` & `trytond_account_statement_mt940-7.0.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/setup.py` & `trytond_account_statement_mt940-7.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author='Tryton',
     author_email='bugs@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/'
+            'https://docs.tryton.org/'
             'modules-account-statement-mt940'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account statement mt940',
     package_dir={'trytond.modules.account_statement_mt940': '.'},
     packages=(
```

### Comparing `trytond_account_statement_mt940-7.0.0/tests/scenario_account_statement_mt940.rst` & `trytond_account_statement_mt940-7.0.1/tests/scenario_account_statement_mt940.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/tox.ini` & `trytond_account_statement_mt940-7.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.0/trytond_account_statement_mt940.egg-info/PKG-INFO` & `trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-statement-mt940
-Version: 7.0.0
+Name: trytond_account_statement_mt940
+Version: 7.0.1
 Summary: Tryton module to import MT940 statements
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: bugs@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-statement-mt940
+Project-URL: Documentation, https://docs.tryton.org/modules-account-statement-mt940
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account statement mt940
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_account_statement_mt940-7.0.0/trytond_account_statement_mt940.egg-info/SOURCES.txt` & `trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 account.py
```

