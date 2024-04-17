# Comparing `tmp/trytond_sale_extra-7.0.0.tar.gz` & `tmp/trytond_sale_extra-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_extra-7.0.0.tar", last modified: Mon Oct 30 17:37:46 2023, max compression
+gzip compressed data, was "trytond_sale_extra-7.0.1.tar", last modified: Wed Apr 17 10:36:47 2024, max compression
```

## Comparing `trytond_sale_extra-7.0.0.tar` & `trytond_sale_extra-7.0.1.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:46.024368 trytond_sale_extra-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-22 17:23:17.000000 trytond_sale_extra-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1726 2023-10-30 17:11:56.000000 trytond_sale_extra-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:11:56.000000 trytond_sale_extra-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_extra-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_extra-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3757 2023-10-30 17:37:46.024368 trytond_sale_extra-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1100 2023-01-16 14:00:21.000000 trytond_sale_extra-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-04-15 07:12:15.000000 trytond_sale_extra-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:46.021035 trytond_sale_extra-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2811 2023-10-22 17:23:17.000000 trytond_sale_extra-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1100 2023-01-16 14:00:21.000000 trytond_sale_extra-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:17.000000 trytond_sale_extra-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:46.017702 trytond_sale_extra-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2189 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1976 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1806 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1970 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1985 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1765 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2008 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2151 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2000 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1840 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1954 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2217 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1921 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1970 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1979 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2028 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1972 2023-10-30 16:47:45.000000 trytond_sale_extra-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1720 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1808 2023-10-28 12:11:25.000000 trytond_sale_extra-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7854 2023-08-13 15:26:13.000000 trytond_sale_extra-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4683 2023-04-15 07:12:15.000000 trytond_sale_extra-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:37:46.024368 trytond_sale_extra-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4397 2023-10-27 17:38:49.000000 trytond_sale_extra-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:46.021035 trytond_sale_extra-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_extra-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4733 2023-10-07 15:40:36.000000 trytond_sale_extra-7.0.0/tests/scenario_sale_extra.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_sale_extra-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_extra-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_extra-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-10-30 17:11:52.000000 trytond_sale_extra-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:46.024368 trytond_sale_extra-7.0.0/trytond_sale_extra.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3757 2023-10-30 17:37:45.000000 trytond_sale_extra-7.0.0/trytond_sale_extra.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1655 2023-10-30 17:37:45.000000 trytond_sale_extra-7.0.0/trytond_sale_extra.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:37:45.000000 trytond_sale_extra-7.0.0/trytond_sale_extra.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-10-30 17:37:45.000000 trytond_sale_extra-7.0.0/trytond_sale_extra.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_sale_extra-7.0.0/trytond_sale_extra.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:37:45.000000 trytond_sale_extra-7.0.0/trytond_sale_extra.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:37:45.000000 trytond_sale_extra-7.0.0/trytond_sale_extra.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:46.021035 trytond_sale_extra-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      732 2023-01-16 14:00:21.000000 trytond_sale_extra-7.0.0/view/extra_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-01-16 14:00:21.000000 trytond_sale_extra-7.0.0/view/extra_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_extra-7.0.0/view/extra_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_sale_extra-7.0.0/view/extra_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-04-15 07:12:15.000000 trytond_sale_extra-7.0.0/view/extra_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:36:47.254936 trytond_sale_extra-7.0.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1827 2024-04-17 10:36:44.000000 trytond_sale_extra-7.0.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-17 10:36:44.000000 trytond_sale_extra-7.0.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3757 2024-04-17 10:36:47.254936 trytond_sale_extra-7.0.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1100 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:36:47.251603 trytond_sale_extra-7.0.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2789 2024-03-03 16:24:20.000000 trytond_sale_extra-7.0.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1100 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:36:47.251603 trytond_sale_extra-7.0.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2189 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1976 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1806 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1970 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1985 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1765 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2008 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2151 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2000 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1840 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1954 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2217 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1921 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1970 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1979 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2028 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2199 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1972 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1720 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1808 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7969 2024-04-12 22:42:09.000000 trytond_sale_extra-7.0.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4683 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:36:47.254936 trytond_sale_extra-7.0.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4397 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:36:47.251603 trytond_sale_extra-7.0.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4733 2024-02-05 16:24:27.000000 trytond_sale_extra-7.0.1/tests/scenario_sale_extra.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2024-02-05 16:24:27.000000 trytond_sale_extra-7.0.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:36:47.254936 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3757 2024-04-17 10:36:46.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1637 2024-04-17 10:36:47.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:36:46.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-17 10:36:46.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:06.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-17 10:36:46.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:36:46.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:36:47.254936 trytond_sale_extra-7.0.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      732 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/view/extra_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/view/extra_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/view/extra_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/view/extra_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/view/extra_list.xml
```

### Comparing `trytond_sale_extra-7.0.0/CHANGELOG` & `trytond_sale_extra-7.0.1/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.0.1 - 2024-04-17
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 
 Version 6.8.0 - 2023-05-01
 --------------------------
```

### Comparing `trytond_sale_extra-7.0.0/LICENSE` & `trytond_sale_extra-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/PKG-INFO` & `trytond_sale_extra-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_extra
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton module for sale extra
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_extra-7.0.0/README.rst` & `trytond_sale_extra-7.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/doc/conf.py` & `trytond_sale_extra-7.0.1/doc/conf.py`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_sale_extra-7.0.0/doc/index.rst` & `trytond_sale_extra-7.0.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/bg.po` & `trytond_sale_extra-7.0.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/ca.po` & `trytond_sale_extra-7.0.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/cs.po` & `trytond_sale_extra-7.0.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/de.po` & `trytond_sale_extra-7.0.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/es.po` & `trytond_sale_extra-7.0.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/es_419.po` & `trytond_sale_extra-7.0.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/et.po` & `trytond_sale_extra-7.0.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/fa.po` & `trytond_sale_extra-7.0.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/fi.po` & `trytond_sale_extra-7.0.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/fr.po` & `trytond_sale_extra-7.0.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/hu.po` & `trytond_sale_extra-7.0.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/id.po` & `trytond_sale_extra-7.0.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/it.po` & `trytond_sale_extra-7.0.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/lo.po` & `trytond_sale_extra-7.0.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/lt.po` & `trytond_sale_extra-7.0.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/nl.po` & `trytond_sale_extra-7.0.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/pl.po` & `trytond_sale_extra-7.0.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/pt.po` & `trytond_sale_extra-7.0.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/ro.po` & `trytond_sale_extra-7.0.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/ru.po` & `trytond_sale_extra-7.0.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/sl.po` & `trytond_sale_extra-7.0.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/tr.po` & `trytond_sale_extra-7.0.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/uk.po` & `trytond_sale_extra-7.0.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/locale/zh_CN.po` & `trytond_sale_extra-7.0.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/sale.py` & `trytond_sale_extra-7.0.1/sale.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,16 @@
         # because extra must be set after to have correct amount
         cls.write(sales, {'state': 'draft'})
         removed = []
         for sale in sales:
             removed.extend(sale.set_extra())
         Line.delete(removed)
         cls.save(sales)
+        # Reset to quotation state to avoid duplicate log entries
+        cls.write(sales, {'state': 'quotation'})
 
     def set_extra(self):
         'Set extra lines and fill lines_to_delete'
         pool = Pool()
         Extra = pool.get('sale.extra')
         removed = []
         extra_lines = Extra.get_lines(self)
```

### Comparing `trytond_sale_extra-7.0.0/sale.xml` & `trytond_sale_extra-7.0.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/setup.py` & `trytond_sale_extra-7.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/tests/scenario_sale_extra.rst` & `trytond_sale_extra-7.0.1/tests/scenario_sale_extra.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/tox.ini` & `trytond_sale_extra-7.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/trytond_sale_extra.egg-info/PKG-INFO` & `trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: trytond-sale-extra
-Version: 7.0.0
+Name: trytond_sale_extra
+Version: 7.0.1
 Summary: Tryton module for sale extra
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_extra-7.0.0/trytond_sale_extra.egg-info/SOURCES.txt` & `trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 sale.py
```

### Comparing `trytond_sale_extra-7.0.0/view/extra_form.xml` & `trytond_sale_extra-7.0.1/view/extra_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.0/view/extra_line_form.xml` & `trytond_sale_extra-7.0.1/view/extra_line_form.xml`

 * *Files identical despite different names*

