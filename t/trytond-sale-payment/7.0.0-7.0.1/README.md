# Comparing `tmp/trytond_sale_payment-7.0.0.tar.gz` & `tmp/trytond_sale_payment-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_payment-7.0.0.tar", last modified: Mon Oct 30 17:38:37 2023, max compression
+gzip compressed data, was "trytond_sale_payment-7.0.1.tar", last modified: Wed Apr 17 10:34:36 2024, max compression
```

## Comparing `trytond_sale_payment-7.0.0.tar` & `trytond_sale_payment-7.0.1.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:37.224613 trytond_sale_payment-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      205 2023-10-22 17:23:18.000000 trytond_sale_payment-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1251 2023-10-30 17:12:22.000000 trytond_sale_payment-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      765 2023-10-30 17:12:22.000000 trytond_sale_payment-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35146 2023-01-16 14:00:21.000000 trytond_sale_payment-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_payment-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3100 2023-10-30 17:38:37.224613 trytond_sale_payment-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-01-16 14:00:21.000000 trytond_sale_payment-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_sale_payment-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6408 2023-08-13 15:26:13.000000 trytond_sale_payment-7.0.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:37.221279 trytond_sale_payment-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2813 2023-10-22 17:23:18.000000 trytond_sale_payment-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-01-16 14:00:21.000000 trytond_sale_payment-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:18.000000 trytond_sale_payment-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:37.217946 trytond_sale_payment-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      628 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      673 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      695 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      661 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      513 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-28 12:11:25.000000 trytond_sale_payment-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      594 2023-04-15 07:12:15.000000 trytond_sale_payment-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2927 2023-04-15 07:12:15.000000 trytond_sale_payment-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1017 2023-04-15 07:12:15.000000 trytond_sale_payment-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:38:37.224613 trytond_sale_payment-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4526 2023-10-27 17:38:49.000000 trytond_sale_payment-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:37.221279 trytond_sale_payment-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_payment-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5586 2023-10-24 07:56:52.000000 trytond_sale_payment-7.0.0/tests/scenario_sale_payment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2911 2023-10-24 07:56:52.000000 trytond_sale_payment-7.0.0/tests/scenario_sale_payment_no_clearing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-04-15 07:12:15.000000 trytond_sale_payment-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_payment-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_payment-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-10-30 17:12:19.000000 trytond_sale_payment-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:37.221279 trytond_sale_payment-7.0.0/trytond_sale_payment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3100 2023-10-30 17:38:36.000000 trytond_sale_payment-7.0.0/trytond_sale_payment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1595 2023-10-30 17:38:37.000000 trytond_sale_payment-7.0.0/trytond_sale_payment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:38:36.000000 trytond_sale_payment-7.0.0/trytond_sale_payment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-30 17:38:36.000000 trytond_sale_payment-7.0.0/trytond_sale_payment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_sale_payment-7.0.0/trytond_sale_payment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-10-30 17:38:36.000000 trytond_sale_payment-7.0.0/trytond_sale_payment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:38:36.000000 trytond_sale_payment-7.0.0/trytond_sale_payment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:37.221279 trytond_sale_payment-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_sale_payment-7.0.0/view/sale_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:34:36.781681 trytond_sale_payment-7.0.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1352 2024-04-17 10:34:33.000000 trytond_sale_payment-7.0.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      765 2024-04-17 10:34:33.000000 trytond_sale_payment-7.0.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35146 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3100 2024-04-17 10:34:36.781681 trytond_sale_payment-7.0.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6422 2024-04-12 22:41:37.000000 trytond_sale_payment-7.0.1/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:34:36.778348 trytond_sale_payment-7.0.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2791 2024-03-03 16:24:20.000000 trytond_sale_payment-7.0.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:34:36.781681 trytond_sale_payment-7.0.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      628 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      673 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      695 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      661 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      513 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      594 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2927 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1017 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:34:36.781681 trytond_sale_payment-7.0.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4526 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:34:36.781681 trytond_sale_payment-7.0.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5586 2024-02-05 16:24:27.000000 trytond_sale_payment-7.0.1/tests/scenario_sale_payment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2911 2024-02-05 16:24:27.000000 trytond_sale_payment-7.0.1/tests/scenario_sale_payment_no_clearing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2024-02-05 16:24:27.000000 trytond_sale_payment-7.0.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:34:36.781681 trytond_sale_payment-7.0.1/trytond_sale_payment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3100 2024-04-17 10:34:36.000000 trytond_sale_payment-7.0.1/trytond_sale_payment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-17 10:34:36.000000 trytond_sale_payment-7.0.1/trytond_sale_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:34:36.000000 trytond_sale_payment-7.0.1/trytond_sale_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-17 10:34:36.000000 trytond_sale_payment-7.0.1/trytond_sale_payment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:08.000000 trytond_sale_payment-7.0.1/trytond_sale_payment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2024-04-17 10:34:36.000000 trytond_sale_payment-7.0.1/trytond_sale_payment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:34:36.000000 trytond_sale_payment-7.0.1/trytond_sale_payment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:34:36.781681 trytond_sale_payment-7.0.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-10-30 17:06:38.000000 trytond_sale_payment-7.0.1/view/sale_form.xml
```

### Comparing `trytond_sale_payment-7.0.0/CHANGELOG` & `trytond_sale_payment-7.0.1/CHANGELOG`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_sale_payment-7.0.0/COPYRIGHT` & `trytond_sale_payment-7.0.1/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Copyright (c) 2017 Mark S Hayden.
 Copyright (c) 2017 Coalesco Digital Systemc Inc.
-Copyright (c) 2017-2023 Cédric Krier.
-Copyright (c) 2017-2023 B2CK.
+Copyright (c) 2017-2024 Cédric Krier.
+Copyright (c) 2017-2024 B2CK.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_payment-7.0.0/LICENSE` & `trytond_sale_payment-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/PKG-INFO` & `trytond_sale_payment-7.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_payment
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton module that manage payments on sale
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_payment-7.0.0/account.py` & `trytond_sale_payment-7.0.1/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 getattr(sale, 'invoice_party', None)
                 or getattr(sale, 'party', None))
             if party:
                 self.party = party
             sale_amount = getattr(sale, 'total_amount', None)
             payment_amount = sum(
                 (p.amount for p in getattr(sale, 'payments', [])
-                    if p.state != 'failed'),
+                    if p.state != 'failed' and p != self),
                 Decimal(0))
             if sale_amount is not None:
                 self.kind = 'receivable' if sale_amount > 0 else 'payable'
                 self.amount = abs(sale_amount) - payment_amount
             currency = getattr(sale, 'currency', None)
             if currency is not None:
                 self.currency = currency
```

### Comparing `trytond_sale_payment-7.0.0/doc/conf.py` & `trytond_sale_payment-7.0.1/doc/conf.py`

 * *Files 8% similar despite different names*

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

### Comparing `trytond_sale_payment-7.0.0/locale/ca.po` & `trytond_sale_payment-7.0.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/locale/de.po` & `trytond_sale_payment-7.0.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/locale/es.po` & `trytond_sale_payment-7.0.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/locale/et.po` & `trytond_sale_payment-7.0.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/locale/fa.po` & `trytond_sale_payment-7.0.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/locale/fr.po` & `trytond_sale_payment-7.0.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/locale/id.po` & `trytond_sale_payment-7.0.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/locale/it.po` & `trytond_sale_payment-7.0.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/locale/nl.po` & `trytond_sale_payment-7.0.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/locale/pl.po` & `trytond_sale_payment-7.0.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/locale/pt.po` & `trytond_sale_payment-7.0.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/locale/ro.po` & `trytond_sale_payment-7.0.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/message.xml` & `trytond_sale_payment-7.0.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/sale.py` & `trytond_sale_payment-7.0.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/sale.xml` & `trytond_sale_payment-7.0.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/setup.py` & `trytond_sale_payment-7.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/tests/scenario_sale_payment.rst` & `trytond_sale_payment-7.0.1/tests/scenario_sale_payment.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/tests/scenario_sale_payment_no_clearing.rst` & `trytond_sale_payment-7.0.1/tests/scenario_sale_payment_no_clearing.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/tox.ini` & `trytond_sale_payment-7.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.0.0/trytond_sale_payment.egg-info/PKG-INFO` & `trytond_sale_payment-7.0.1/trytond_sale_payment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: trytond-sale-payment
-Version: 7.0.0
+Name: trytond_sale_payment
+Version: 7.0.1
 Summary: Tryton module that manage payments on sale
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_payment-7.0.0/trytond_sale_payment.egg-info/SOURCES.txt` & `trytond_sale_payment-7.0.1/trytond_sale_payment.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

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

