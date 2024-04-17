# Comparing `tmp/trytond_purchase-7.0.2.tar.gz` & `tmp/trytond_purchase-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase-7.0.2.tar", last modified: Thu Apr  4 07:50:34 2024, max compression
+gzip compressed data, was "trytond_purchase-7.0.3.tar", last modified: Wed Apr 17 10:40:49 2024, max compression
```

## Comparing `trytond_purchase-7.0.2.tar` & `trytond_purchase-7.0.3.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:50:34.118419 trytond_purchase-7.0.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     7190 2024-04-04 07:50:31.000000 trytond_purchase-7.0.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-04 07:50:31.000000 trytond_purchase-7.0.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-04 07:50:34.118419 trytond_purchase-7.0.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1909 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3581 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2554 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:50:34.108419 trytond_purchase-7.0.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2787 2024-03-03 16:24:20.000000 trytond_purchase-7.0.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7482 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:50:34.108419 trytond_purchase-7.0.2/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      208 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2000 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/doc/usage/prepurchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4855 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2027 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/doc/usage/returns.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:50:34.111752 trytond_purchase-7.0.2/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/icons/tryton-purchase.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5622 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1761 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:50:34.111752 trytond_purchase-7.0.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    37669 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37866 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32868 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38333 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38062 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32388 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34581 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39805 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32855 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38221 2024-01-26 17:57:52.000000 trytond_purchase-7.0.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36910 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33506 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36150 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37669 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35653 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38239 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34203 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35891 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32093 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38224 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37603 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32846 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31183 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36322 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4337 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3677 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    21315 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    77930 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/purchase.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    83831 2024-04-04 07:37:13.000000 trytond_purchase-7.0.2/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    30912 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11639 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/purchase_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24226 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/purchase_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-04 07:50:34.118419 trytond_purchase-7.0.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4577 2024-03-03 16:24:03.000000 trytond_purchase-7.0.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8582 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4823 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:50:34.115086 trytond_purchase-7.0.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19200 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/tests/scenario_purchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1676 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/tests/scenario_purchase_copy_product_suppliers.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1564 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/tests/scenario_purchase_default_taxes.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1332 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/tests/scenario_purchase_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2463 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/tests/scenario_purchase_manual_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3064 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/tests/scenario_purchase_modify_header.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5191 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/tests/scenario_purchase_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2999 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/tests/scenario_purchase_return_wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5595 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2024-02-05 16:24:27.000000 trytond_purchase-7.0.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:50:34.118419 trytond_purchase-7.0.2/trytond_purchase.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-04 07:50:33.000000 trytond_purchase-7.0.2/trytond_purchase.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4959 2024-04-04 07:50:34.000000 trytond_purchase-7.0.2/trytond_purchase.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-04 07:50:33.000000 trytond_purchase-7.0.2/trytond_purchase.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-04-04 07:50:33.000000 trytond_purchase-7.0.2/trytond_purchase.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:00.000000 trytond_purchase-7.0.2/trytond_purchase.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-04 07:50:33.000000 trytond_purchase-7.0.2/trytond_purchase.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-04 07:50:33.000000 trytond_purchase-7.0.2/trytond_purchase.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:50:34.118419 trytond_purchase-7.0.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/handle_invoice_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/handle_shipment_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/modify_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      482 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/move_list_shipment_in.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/product_list_purchase_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/product_supplier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/product_supplier_price_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/product_supplier_price_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/product_supplier_price_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/product_supplier_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/product_supplier_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3543 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1818 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      741 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      544 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_reporting_main_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_reporting_main_time_series_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_reporting_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_reporting_supplier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/purchase_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/return_purchase_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-10-30 17:06:38.000000 trytond_purchase-7.0.2/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.381936 trytond_purchase-7.0.3/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7291 2024-04-17 10:40:46.000000 trytond_purchase-7.0.3/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-17 10:40:46.000000 trytond_purchase-7.0.3/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-17 10:40:49.381936 trytond_purchase-7.0.3/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1909 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3581 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2554 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.371937 trytond_purchase-7.0.3/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2787 2024-03-03 16:24:20.000000 trytond_purchase-7.0.3/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7482 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.375270 trytond_purchase-7.0.3/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      208 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2000 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/doc/usage/prepurchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4855 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/doc/usage/process.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2027 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/doc/usage/returns.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.375270 trytond_purchase-7.0.3/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/icons/tryton-purchase.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5622 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1761 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.375270 trytond_purchase-7.0.3/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    37669 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37866 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32868 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38333 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38062 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32388 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34581 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39805 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32855 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38221 2024-01-26 17:57:52.000000 trytond_purchase-7.0.3/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36910 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33506 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36150 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37669 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35653 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38239 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34203 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35891 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32093 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38224 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37603 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32846 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31183 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36322 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4337 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3677 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    21315 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    77930 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/purchase.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    83768 2024-04-12 17:44:57.000000 trytond_purchase-7.0.3/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    30912 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11639 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/purchase_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24226 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/purchase_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:40:49.381936 trytond_purchase-7.0.3/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4577 2024-03-03 16:24:03.000000 trytond_purchase-7.0.3/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8582 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4823 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.378603 trytond_purchase-7.0.3/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19200 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1676 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_copy_product_suppliers.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1564 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_default_taxes.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1332 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2463 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_manual_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3064 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_modify_header.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5191 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2999 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_return_wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5595 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2024-04-04 07:50:42.000000 trytond_purchase-7.0.3/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.381936 trytond_purchase-7.0.3/trytond_purchase.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-17 10:40:48.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4959 2024-04-17 10:40:49.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:40:48.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-04-17 10:40:48.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:00.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-17 10:40:48.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:40:48.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.381936 trytond_purchase-7.0.3/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/handle_invoice_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/handle_shipment_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/modify_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      482 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/move_list_shipment_in.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_list_purchase_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_supplier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_supplier_price_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_supplier_price_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_supplier_price_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_supplier_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_supplier_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3543 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1818 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      741 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      544 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_main_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_main_time_series_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_supplier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/return_purchase_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/template_tree.xml
```

### Comparing `trytond_purchase-7.0.2/CHANGELOG` & `trytond_purchase-7.0.3/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.0.3 - 2024-04-17
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.2 - 2024-04-04
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.1 - 2024-02-03
 --------------------------
```

### Comparing `trytond_purchase-7.0.2/COPYRIGHT` & `trytond_purchase-7.0.3/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/LICENSE` & `trytond_purchase-7.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/PKG-INFO` & `trytond_purchase-7.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase
-Version: 7.0.2
+Version: 7.0.3
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase-7.0.2/__init__.py` & `trytond_purchase-7.0.3/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/configuration.py` & `trytond_purchase-7.0.3/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/configuration.xml` & `trytond_purchase-7.0.3/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/doc/conf.py` & `trytond_purchase-7.0.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/doc/design.rst` & `trytond_purchase-7.0.3/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/doc/usage/prepurchase.rst` & `trytond_purchase-7.0.3/doc/usage/prepurchase.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/doc/usage/process.rst` & `trytond_purchase-7.0.3/doc/usage/process.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/doc/usage/returns.rst` & `trytond_purchase-7.0.3/doc/usage/returns.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/icons/LICENSE` & `trytond_purchase-7.0.3/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/invoice.py` & `trytond_purchase-7.0.3/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/invoice.xml` & `trytond_purchase-7.0.3/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/bg.po` & `trytond_purchase-7.0.3/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/ca.po` & `trytond_purchase-7.0.3/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/cs.po` & `trytond_purchase-7.0.3/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/de.po` & `trytond_purchase-7.0.3/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/es.po` & `trytond_purchase-7.0.3/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/es_419.po` & `trytond_purchase-7.0.3/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/et.po` & `trytond_purchase-7.0.3/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/fa.po` & `trytond_purchase-7.0.3/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/fi.po` & `trytond_purchase-7.0.3/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/fr.po` & `trytond_purchase-7.0.3/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/hu.po` & `trytond_purchase-7.0.3/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/id.po` & `trytond_purchase-7.0.3/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/it.po` & `trytond_purchase-7.0.3/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/lo.po` & `trytond_purchase-7.0.3/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/lt.po` & `trytond_purchase-7.0.3/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/nl.po` & `trytond_purchase-7.0.3/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/pl.po` & `trytond_purchase-7.0.3/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/pt.po` & `trytond_purchase-7.0.3/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/ro.po` & `trytond_purchase-7.0.3/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/ru.po` & `trytond_purchase-7.0.3/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/sl.po` & `trytond_purchase-7.0.3/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/tr.po` & `trytond_purchase-7.0.3/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/uk.po` & `trytond_purchase-7.0.3/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/locale/zh_CN.po` & `trytond_purchase-7.0.3/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/message.xml` & `trytond_purchase-7.0.3/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/party.py` & `trytond_purchase-7.0.3/party.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/party.xml` & `trytond_purchase-7.0.3/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/product.py` & `trytond_purchase-7.0.3/product.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/product.xml` & `trytond_purchase-7.0.3/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/purchase.fodt` & `trytond_purchase-7.0.3/purchase.fodt`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/purchase.py` & `trytond_purchase-7.0.3/purchase.py`

 * *Files 0% similar despite different names*

```diff
@@ -832,20 +832,19 @@
         return_shipment = self._get_return_shipment()
         return_shipment.moves = return_moves
         return return_shipment
 
     def is_done(self):
         return ((self.invoice_state == 'paid'
                 or (self.invoice_state == 'none'
-                    and all(not l.quantity
-                        for l in self.lines if l.type == 'line')))
+                    and self.invoice_method != 'manual'))
             and (self.shipment_state == 'received'
-                or (self.shipment_state == 'none'
-                    and all(l.product.type == 'service'
-                        for l in self.lines if l.product))))
+                or self.shipment_state == 'none'
+                or all(l.product.type == 'service'
+                    for l in self.lines if l.product)))
 
     @classmethod
     def delete(cls, purchases):
         # Cancel before delete
         cls.cancel(purchases)
         for purchase in purchases:
             if purchase.state != 'cancelled':
```

### Comparing `trytond_purchase-7.0.2/purchase.xml` & `trytond_purchase-7.0.3/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/purchase_reporting.py` & `trytond_purchase-7.0.3/purchase_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/purchase_reporting.xml` & `trytond_purchase-7.0.3/purchase_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/setup.py` & `trytond_purchase-7.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/stock.py` & `trytond_purchase-7.0.3/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/stock.xml` & `trytond_purchase-7.0.3/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/tests/scenario_purchase.rst` & `trytond_purchase-7.0.3/tests/scenario_purchase.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/tests/scenario_purchase_copy_product_suppliers.rst` & `trytond_purchase-7.0.3/tests/scenario_purchase_copy_product_suppliers.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/tests/scenario_purchase_default_taxes.rst` & `trytond_purchase-7.0.3/tests/scenario_purchase_default_taxes.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/tests/scenario_purchase_empty.rst` & `trytond_purchase-7.0.3/tests/scenario_purchase_empty.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/tests/scenario_purchase_manual_invoice.rst` & `trytond_purchase-7.0.3/tests/scenario_purchase_manual_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/tests/scenario_purchase_modify_header.rst` & `trytond_purchase-7.0.3/tests/scenario_purchase_modify_header.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/tests/scenario_purchase_reporting.rst` & `trytond_purchase-7.0.3/tests/scenario_purchase_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/tests/scenario_purchase_return_wizard.rst` & `trytond_purchase-7.0.3/tests/scenario_purchase_return_wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/tests/test_module.py` & `trytond_purchase-7.0.3/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/tox.ini` & `trytond_purchase-7.0.3/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/trytond_purchase.egg-info/PKG-INFO` & `trytond_purchase-7.0.3/trytond_purchase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase
-Version: 7.0.2
+Version: 7.0.3
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase-7.0.2/trytond_purchase.egg-info/SOURCES.txt` & `trytond_purchase-7.0.3/trytond_purchase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/view/party_form.xml` & `trytond_purchase-7.0.3/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/view/product_supplier_form.xml` & `trytond_purchase-7.0.3/view/product_supplier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/view/purchase_form.xml` & `trytond_purchase-7.0.3/view/purchase_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/view/purchase_line_form.xml` & `trytond_purchase-7.0.3/view/purchase_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/view/purchase_line_tree.xml` & `trytond_purchase-7.0.3/view/purchase_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/view/purchase_line_tree_sequence.xml` & `trytond_purchase-7.0.3/view/purchase_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/view/purchase_reporting_context_form.xml` & `trytond_purchase-7.0.3/view/purchase_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/view/purchase_tree.xml` & `trytond_purchase-7.0.3/view/purchase_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.2/view/template_form.xml` & `trytond_purchase-7.0.3/view/template_form.xml`

 * *Files identical despite different names*

