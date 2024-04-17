# Comparing `tmp/trytond_sale_advance_payment-7.0.1.tar.gz` & `tmp/trytond_sale_advance_payment-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_advance_payment-7.0.1.tar", last modified: Sat Feb  3 11:21:28 2024, max compression
+gzip compressed data, was "trytond_sale_advance_payment-7.0.2.tar", last modified: Wed Apr 17 10:37:38 2024, max compression
```

## Comparing `trytond_sale_advance_payment-7.0.1.tar` & `trytond_sale_advance_payment-7.0.2.tar`

### file list

```diff
@@ -1,84 +1,83 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:21:28.443130 trytond_sale_advance_payment-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-02-03 11:21:20.000000 trytond_sale_advance_payment-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-02-03 11:21:20.000000 trytond_sale_advance_payment-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4361 2024-02-03 11:21:28.443130 trytond_sale_advance_payment-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1718 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      754 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3040 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      787 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:21:28.426464 trytond_sale_advance_payment-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2821 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1718 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:21:28.433130 trytond_sale_advance_payment-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6416 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6304 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6360 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4871 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5335 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6830 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6343 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4957 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5144 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5349 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6356 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5212 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6073 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4993 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5750 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4871 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2242 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1238 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1213 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1212 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1205 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1212 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1209 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1210 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1214 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1211 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    17135 2024-01-26 18:00:26.000000 trytond_sale_advance_payment-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5721 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-03 11:21:28.443130 trytond_sale_advance_payment-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4621 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1036 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:21:28.433130 trytond_sale_advance_payment-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12088 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/tests/scenario_advance_payment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4581 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/tests/scenario_sale_advance_payment_on_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1290 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-10-30 17:55:12.000000 trytond_sale_advance_payment-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:21:28.439797 trytond_sale_advance_payment-7.0.1/trytond_sale_advance_payment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4361 2024-02-03 11:21:27.000000 trytond_sale_advance_payment-7.0.1/trytond_sale_advance_payment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2767 2024-02-03 11:21:28.000000 trytond_sale_advance_payment-7.0.1/trytond_sale_advance_payment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-03 11:21:27.000000 trytond_sale_advance_payment-7.0.1/trytond_sale_advance_payment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-02-03 11:21:27.000000 trytond_sale_advance_payment-7.0.1/trytond_sale_advance_payment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:04.000000 trytond_sale_advance_payment-7.0.1/trytond_sale_advance_payment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      168 2024-02-03 11:21:27.000000 trytond_sale_advance_payment-7.0.1/trytond_sale_advance_payment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-03 11:21:27.000000 trytond_sale_advance_payment-7.0.1/trytond_sale_advance_payment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:21:28.439797 trytond_sale_advance_payment-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      735 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/view/advance_payment_condition_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/view/advance_payment_condition_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/view/advance_payment_term_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/view/advance_payment_term_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/view/advance_payment_term_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/view/advance_payment_term_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.1/view/sale_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:37:38.483596 trytond_sale_advance_payment-7.0.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1633 2024-04-17 10:37:35.000000 trytond_sale_advance_payment-7.0.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-17 10:37:35.000000 trytond_sale_advance_payment-7.0.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4361 2024-04-17 10:37:38.483596 trytond_sale_advance_payment-7.0.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1718 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      754 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3343 2024-04-12 20:29:30.000000 trytond_sale_advance_payment-7.0.2/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      787 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:37:38.476929 trytond_sale_advance_payment-7.0.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2799 2024-03-03 16:24:20.000000 trytond_sale_advance_payment-7.0.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1718 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:37:38.480263 trytond_sale_advance_payment-7.0.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6416 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6304 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6360 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4871 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5335 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6830 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6343 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4957 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5144 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5349 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6356 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5212 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6073 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4993 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5750 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4871 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2242 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1238 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1213 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1212 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1205 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1212 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1209 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1210 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1214 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1211 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    17135 2024-02-05 16:24:27.000000 trytond_sale_advance_payment-7.0.2/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5721 2024-02-05 16:24:27.000000 trytond_sale_advance_payment-7.0.2/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:37:38.483596 trytond_sale_advance_payment-7.0.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4621 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1036 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:37:38.480263 trytond_sale_advance_payment-7.0.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12088 2024-02-05 16:24:27.000000 trytond_sale_advance_payment-7.0.2/tests/scenario_advance_payment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4581 2024-02-05 16:24:27.000000 trytond_sale_advance_payment-7.0.2/tests/scenario_sale_advance_payment_on_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-02-05 16:24:27.000000 trytond_sale_advance_payment-7.0.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1290 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2024-02-05 16:24:27.000000 trytond_sale_advance_payment-7.0.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:37:38.480263 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4361 2024-04-17 10:37:38.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2749 2024-04-17 10:37:38.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:37:38.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-17 10:37:38.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:04.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      168 2024-04-17 10:37:38.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:37:38.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:37:38.480263 trytond_sale_advance_payment-7.0.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      735 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/advance_payment_condition_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/advance_payment_condition_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/advance_payment_term_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/advance_payment_term_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/advance_payment_term_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/advance_payment_term_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/sale_form.xml
```

### Comparing `trytond_sale_advance_payment-7.0.1/CHANGELOG` & `trytond_sale_advance_payment-7.0.2/CHANGELOG`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.0.2 - 2024-04-17
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.1 - 2024-02-03
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
```

### Comparing `trytond_sale_advance_payment-7.0.1/COPYRIGHT` & `trytond_sale_advance_payment-7.0.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/LICENSE` & `trytond_sale_advance_payment-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/PKG-INFO` & `trytond_sale_advance_payment-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_advance_payment
-Version: 7.0.1
+Version: 7.0.2
 Summary: Tryton module for sale advance payment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_advance_payment-7.0.1/README.rst` & `trytond_sale_advance_payment-7.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/__init__.py` & `trytond_sale_advance_payment-7.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/account.py` & `trytond_sale_advance_payment-7.0.2/account.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,23 @@
 
         sales = set(super(Invoice, self).get_sales(name))
         for line in self.lines:
             if isinstance(line.origin, AdvancePaymentCondition):
                 sales.add(line.origin.sale.id)
         return list(sales)
 
+    @classmethod
+    def search_sales(cls, name, clause):
+        domain = super().search_sales(name, clause)
+        return ['OR',
+            domain,
+            ('lines.origin.sale' + clause[0][len(name):],
+                *clause[1:3], 'sale.advance_payment.condition', *clause[3:]),
+            ]
+
 
 class InvoiceLine(metaclass=PoolMeta):
     __name__ = 'account.invoice.line'
 
     advance_payment_recalled_lines = fields.One2Many(
         'account.invoice.line', 'origin', "Advance Payment Recalled Lines",
         readonly=True)
```

### Comparing `trytond_sale_advance_payment-7.0.1/account.xml` & `trytond_sale_advance_payment-7.0.2/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/doc/conf.py` & `trytond_sale_advance_payment-7.0.2/doc/conf.py`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_sale_advance_payment-7.0.1/doc/index.rst` & `trytond_sale_advance_payment-7.0.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/bg.po` & `trytond_sale_advance_payment-7.0.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/ca.po` & `trytond_sale_advance_payment-7.0.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/cs.po` & `trytond_sale_advance_payment-7.0.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/de.po` & `trytond_sale_advance_payment-7.0.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/es.po` & `trytond_sale_advance_payment-7.0.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/es_419.po` & `trytond_sale_advance_payment-7.0.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/et.po` & `trytond_sale_advance_payment-7.0.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/fa.po` & `trytond_sale_advance_payment-7.0.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/fi.po` & `trytond_sale_advance_payment-7.0.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/fr.po` & `trytond_sale_advance_payment-7.0.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/hu.po` & `trytond_sale_advance_payment-7.0.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/id.po` & `trytond_sale_advance_payment-7.0.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/it.po` & `trytond_sale_advance_payment-7.0.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/lo.po` & `trytond_sale_advance_payment-7.0.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/lt.po` & `trytond_sale_advance_payment-7.0.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/nl.po` & `trytond_sale_advance_payment-7.0.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/pl.po` & `trytond_sale_advance_payment-7.0.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/pt.po` & `trytond_sale_advance_payment-7.0.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/ro.po` & `trytond_sale_advance_payment-7.0.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/ru.po` & `trytond_sale_advance_payment-7.0.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/sl.po` & `trytond_sale_advance_payment-7.0.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/tr.po` & `trytond_sale_advance_payment-7.0.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/uk.po` & `trytond_sale_advance_payment-7.0.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/locale/zh_CN.po` & `trytond_sale_advance_payment-7.0.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/message.xml` & `trytond_sale_advance_payment-7.0.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/minimal_chart.xml` & `trytond_sale_advance_payment-7.0.2/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/minimal_chart_bg.xml` & `trytond_sale_advance_payment-7.0.2/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/minimal_chart_ca.xml` & `trytond_sale_advance_payment-7.0.2/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/minimal_chart_de.xml` & `trytond_sale_advance_payment-7.0.2/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/minimal_chart_en.xml` & `trytond_sale_advance_payment-7.0.2/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/minimal_chart_es.xml` & `trytond_sale_advance_payment-7.0.2/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/minimal_chart_fr.xml` & `trytond_sale_advance_payment-7.0.2/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/minimal_chart_nl.xml` & `trytond_sale_advance_payment-7.0.2/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/minimal_chart_pt.xml` & `trytond_sale_advance_payment-7.0.2/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/minimal_chart_ru.xml` & `trytond_sale_advance_payment-7.0.2/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/minimal_chart_sl.xml` & `trytond_sale_advance_payment-7.0.2/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/sale.py` & `trytond_sale_advance_payment-7.0.2/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/sale.xml` & `trytond_sale_advance_payment-7.0.2/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/setup.py` & `trytond_sale_advance_payment-7.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/stock.py` & `trytond_sale_advance_payment-7.0.2/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/tests/scenario_advance_payment.rst` & `trytond_sale_advance_payment-7.0.2/tests/scenario_advance_payment.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/tests/scenario_sale_advance_payment_on_shipment.rst` & `trytond_sale_advance_payment-7.0.2/tests/scenario_sale_advance_payment_on_shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/tests/tools.py` & `trytond_sale_advance_payment-7.0.2/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/tox.ini` & `trytond_sale_advance_payment-7.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/trytond_sale_advance_payment.egg-info/PKG-INFO` & `trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_advance_payment
-Version: 7.0.1
+Version: 7.0.2
 Summary: Tryton module for sale advance payment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_advance_payment-7.0.1/trytond_sale_advance_payment.egg-info/SOURCES.txt` & `trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/SOURCES.txt`

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

### Comparing `trytond_sale_advance_payment-7.0.1/view/advance_payment_condition_form.xml` & `trytond_sale_advance_payment-7.0.2/view/advance_payment_condition_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/view/advance_payment_term_line_form.xml` & `trytond_sale_advance_payment-7.0.2/view/advance_payment_term_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.1/view/sale_form.xml` & `trytond_sale_advance_payment-7.0.2/view/sale_form.xml`

 * *Files identical despite different names*

