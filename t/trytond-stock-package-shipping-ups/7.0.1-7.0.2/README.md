# Comparing `tmp/trytond_stock_package_shipping_ups-7.0.1.tar.gz` & `tmp/trytond_stock_package_shipping_ups-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package_shipping_ups-7.0.1.tar", last modified: Sun Mar  3 12:15:27 2024, max compression
+gzip compressed data, was "trytond_stock_package_shipping_ups-7.0.2.tar", last modified: Wed Apr 17 10:32:51 2024, max compression
```

## Comparing `trytond_stock_package_shipping_ups-7.0.1.tar` & `trytond_stock_package_shipping_ups-7.0.2.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:15:27.804325 trytond_stock_package_shipping_ups-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1934 2024-03-03 12:15:25.000000 trytond_stock_package_shipping_ups-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2024-03-03 12:15:24.000000 trytond_stock_package_shipping_ups-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3114 2024-03-03 12:15:27.804325 trytond_stock_package_shipping_ups-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      610 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5822 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2827 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:15:27.797655 trytond_stock_package_shipping_ups-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2827 2024-02-05 16:24:27.000000 trytond_stock_package_shipping_ups-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      459 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1316 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:15:27.800990 trytond_stock_package_shipping_ups-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3397 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4132 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3298 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4247 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4176 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3212 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3349 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4293 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3298 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4279 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3335 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3243 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3330 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3392 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3310 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4165 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3374 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3590 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3435 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3377 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3544 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3298 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3212 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3298 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1284 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-03-03 12:15:27.804325 trytond_stock_package_shipping_ups-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4795 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15586 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      737 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:15:27.800990 trytond_stock_package_shipping_ups-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7906 2024-02-05 16:24:27.000000 trytond_stock_package_shipping_ups-7.0.1/tests/scenario_shipping_ups.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-02-29 11:49:06.000000 trytond_stock_package_shipping_ups-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2024-02-05 16:24:27.000000 trytond_stock_package_shipping_ups-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:15:27.804325 trytond_stock_package_shipping_ups-7.0.1/trytond_stock_package_shipping_ups.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3114 2024-03-03 12:15:27.000000 trytond_stock_package_shipping_ups-7.0.1/trytond_stock_package_shipping_ups.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1913 2024-03-03 12:15:27.000000 trytond_stock_package_shipping_ups-7.0.1/trytond_stock_package_shipping_ups.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-03-03 12:15:27.000000 trytond_stock_package_shipping_ups-7.0.1/trytond_stock_package_shipping_ups.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-03-03 12:15:27.000000 trytond_stock_package_shipping_ups-7.0.1/trytond_stock_package_shipping_ups.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:16.000000 trytond_stock_package_shipping_ups-7.0.1/trytond_stock_package_shipping_ups.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-03-03 12:15:27.000000 trytond_stock_package_shipping_ups-7.0.1/trytond_stock_package_shipping_ups.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-03-03 12:15:27.000000 trytond_stock_package_shipping_ups-7.0.1/trytond_stock_package_shipping_ups.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:15:27.804325 trytond_stock_package_shipping_ups-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/view/package_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/view/ups_credential_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.1/view/ups_credential_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2035 2024-04-17 10:32:49.000000 trytond_stock_package_shipping_ups-7.0.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      684 2024-04-17 10:32:48.000000 trytond_stock_package_shipping_ups-7.0.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3105 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      610 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5822 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2827 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:32:51.841093 trytond_stock_package_shipping_ups-7.0.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2805 2024-03-03 16:24:20.000000 trytond_stock_package_shipping_ups-7.0.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      459 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1316 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3397 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4132 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3298 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4247 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4176 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3212 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3349 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4293 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3298 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4279 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3335 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3243 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3330 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3392 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3310 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4165 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3374 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3590 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3435 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3377 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3544 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3298 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3212 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3298 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1284 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4786 2024-03-03 16:24:03.000000 trytond_stock_package_shipping_ups-7.0.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15604 2024-04-12 20:13:29.000000 trytond_stock_package_shipping_ups-7.0.2/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      737 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7906 2024-02-05 16:24:27.000000 trytond_stock_package_shipping_ups-7.0.2/tests/scenario_shipping_ups.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-02-29 11:49:06.000000 trytond_stock_package_shipping_ups-7.0.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      219 2024-03-03 12:15:34.000000 trytond_stock_package_shipping_ups-7.0.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3105 2024-04-17 10:32:51.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1895 2024-04-17 10:32:51.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:32:51.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-17 10:32:51.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:16.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-17 10:32:51.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:32:51.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/view/package_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/view/ups_credential_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/view/ups_credential_list.xml
```

### Comparing `trytond_stock_package_shipping_ups-7.0.1/CHANGELOG` & `trytond_stock_package_shipping_ups-7.0.2/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.0.2 - 2024-04-17
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.1 - 2024-03-03
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
```

### Comparing `trytond_stock_package_shipping_ups-7.0.1/COPYRIGHT` & `trytond_stock_package_shipping_ups-7.0.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/LICENSE` & `trytond_stock_package_shipping_ups-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/PKG-INFO` & `trytond_stock_package_shipping_ups-7.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package_shipping_ups
-Version: 7.0.1
+Version: 7.0.2
 Summary: UPS connector for the Tryton application platform
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-package-shipping-ups
+Project-URL: Documentation, https://docs.tryton.org/modules-stock-package-shipping-ups
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping ups
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_stock_package_shipping_ups-7.0.1/__init__.py` & `trytond_stock_package_shipping_ups-7.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/carrier.py` & `trytond_stock_package_shipping_ups-7.0.2/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/carrier.xml` & `trytond_stock_package_shipping_ups-7.0.2/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/doc/conf.py` & `trytond_stock_package_shipping_ups-7.0.2/doc/conf.py`

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

### Comparing `trytond_stock_package_shipping_ups-7.0.1/doc/design.rst` & `trytond_stock_package_shipping_ups-7.0.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/doc/usage.rst` & `trytond_stock_package_shipping_ups-7.0.2/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/bg.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/ca.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/cs.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/de.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/es.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/es_419.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/et.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/fa.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/fi.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/fr.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/hu.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/id.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/it.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/lo.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/lt.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/nl.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/pl.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/pt.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/ro.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/ru.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/sl.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/tr.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/uk.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/locale/zh_CN.po` & `trytond_stock_package_shipping_ups-7.0.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/message.xml` & `trytond_stock_package_shipping_ups-7.0.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/setup.py` & `trytond_stock_package_shipping_ups-7.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/'
+            'https://docs.tryton.org/'
             'modules-stock-package-shipping-ups'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock package shipping ups',
     package_dir={'trytond.modules.stock_package_shipping_ups': '.'},
     packages=(
```

### Comparing `trytond_stock_package_shipping_ups-7.0.1/stock.py` & `trytond_stock_package_shipping_ups-7.0.2/stock.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,16 +209,16 @@
                 gettext('stock_package_shipping_ups.msg_ups_webservice_error',
                     message=response_status['Description']))
 
         shipment_results = shipment_response['ShipmentResults']
         shipment.shipping_reference = (
             shipment_results['ShipmentIdentificationNumber'])
         ups_packages = shipment_results['PackageResults']
-        if len(packages) == 1:
-            # In case only one package is requested UPS returns a dictionnary
+        if not isinstance(ups_packages, list):
+            # In case only one package is requested UPS may return a dictionary
             # instead of a list of one package
             ups_packages = [ups_packages]
 
         for tryton_pkg, ups_pkg in zip_longest(packages, ups_packages):
             label = fields.Binary.cast(base64.b64decode(
                     ups_pkg['ShippingLabel']['GraphicImage']))
             tryton_pkg.shipping_reference = ups_pkg['TrackingNumber']
```

### Comparing `trytond_stock_package_shipping_ups-7.0.1/stock.xml` & `trytond_stock_package_shipping_ups-7.0.2/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/tests/scenario_shipping_ups.rst` & `trytond_stock_package_shipping_ups-7.0.2/tests/scenario_shipping_ups.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/tox.ini` & `trytond_stock_package_shipping_ups-7.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/trytond_stock_package_shipping_ups.egg-info/PKG-INFO` & `trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package_shipping_ups
-Version: 7.0.1
+Version: 7.0.2
 Summary: UPS connector for the Tryton application platform
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-package-shipping-ups
+Project-URL: Documentation, https://docs.tryton.org/modules-stock-package-shipping-ups
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping ups
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_stock_package_shipping_ups-7.0.1/trytond_stock_package_shipping_ups.egg-info/SOURCES.txt` & `trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/SOURCES.txt`

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
 carrier.py
```

### Comparing `trytond_stock_package_shipping_ups-7.0.1/view/carrier_form.xml` & `trytond_stock_package_shipping_ups-7.0.2/view/carrier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.1/view/ups_credential_form.xml` & `trytond_stock_package_shipping_ups-7.0.2/view/ups_credential_form.xml`

 * *Files identical despite different names*

