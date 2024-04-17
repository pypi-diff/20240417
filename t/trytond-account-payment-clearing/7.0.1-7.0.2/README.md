# Comparing `tmp/trytond_account_payment_clearing-7.0.1.tar.gz` & `tmp/trytond_account_payment_clearing-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_clearing-7.0.1.tar", last modified: Mon Jan 15 23:22:07 2024, max compression
+gzip compressed data, was "trytond_account_payment_clearing-7.0.2.tar", last modified: Wed Apr 17 10:45:14 2024, max compression
```

## Comparing `trytond_account_payment_clearing-7.0.1.tar` & `trytond_account_payment_clearing-7.0.2.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:22:07.239788 trytond_account_payment_clearing-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2904 2024-01-15 23:22:04.000000 trytond_account_payment_clearing-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-01-15 23:22:04.000000 trytond_account_payment_clearing-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-01-15 23:22:07.239788 trytond_account_payment_clearing-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1794 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:22:07.233121 trytond_account_payment_clearing-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2825 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1331 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:22:07.236455 trytond_account_payment_clearing-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2638 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2669 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2636 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2248 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2424 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2557 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2654 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2049 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2248 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2456 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2161 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2564 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2140 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2297 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2033 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16598 2024-01-13 00:37:09.000000 trytond_account_payment_clearing-7.0.1/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2402 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-01-15 23:22:07.239788 trytond_account_payment_clearing-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4898 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8612 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/statement.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:22:07.236455 trytond_account_payment_clearing-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3317 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/tests/scenario_account_negative_payment_clearing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14076 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/tests/scenario_account_payment_clearing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5337 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/tests/scenario_account_payment_clearing_invoice_amount_to_pay.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-10-30 17:55:12.000000 trytond_account_payment_clearing-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:22:07.239788 trytond_account_payment_clearing-7.0.1/trytond_account_payment_clearing.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-01-15 23:22:06.000000 trytond_account_payment_clearing-7.0.1/trytond_account_payment_clearing.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2145 2024-01-15 23:22:07.000000 trytond_account_payment_clearing-7.0.1/trytond_account_payment_clearing.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-01-15 23:22:06.000000 trytond_account_payment_clearing-7.0.1/trytond_account_payment_clearing.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       86 2024-01-15 23:22:06.000000 trytond_account_payment_clearing-7.0.1/trytond_account_payment_clearing.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:36.000000 trytond_account_payment_clearing-7.0.1/trytond_account_payment_clearing.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2024-01-15 23:22:06.000000 trytond_account_payment_clearing-7.0.1/trytond_account_payment_clearing.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-01-15 23:22:06.000000 trytond_account_payment_clearing-7.0.1/trytond_account_payment_clearing.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:22:07.239788 trytond_account_payment_clearing-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/view/payment_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.1/view/succeed_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:14.984990 trytond_account_payment_clearing-7.0.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3005 2024-04-17 10:45:12.000000 trytond_account_payment_clearing-7.0.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-17 10:45:11.000000 trytond_account_payment_clearing-7.0.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3049 2024-04-17 10:45:14.984990 trytond_account_payment_clearing-7.0.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1794 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:14.981656 trytond_account_payment_clearing-7.0.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2803 2024-03-03 16:24:20.000000 trytond_account_payment_clearing-7.0.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1331 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:14.981656 trytond_account_payment_clearing-7.0.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2638 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2669 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2636 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2248 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2424 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2557 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2654 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2049 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2248 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2456 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2161 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2564 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2140 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2297 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2033 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16668 2024-04-12 22:39:25.000000 trytond_account_payment_clearing-7.0.2/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2402 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:45:14.984990 trytond_account_payment_clearing-7.0.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4889 2024-03-03 16:24:03.000000 trytond_account_payment_clearing-7.0.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8612 2024-02-05 16:24:27.000000 trytond_account_payment_clearing-7.0.2/statement.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:14.981656 trytond_account_payment_clearing-7.0.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3317 2024-02-05 16:24:27.000000 trytond_account_payment_clearing-7.0.2/tests/scenario_account_negative_payment_clearing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14076 2024-02-05 16:24:27.000000 trytond_account_payment_clearing-7.0.2/tests/scenario_account_payment_clearing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5337 2024-02-05 16:24:27.000000 trytond_account_payment_clearing-7.0.2/tests/scenario_account_payment_clearing_invoice_amount_to_pay.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-02-05 16:24:27.000000 trytond_account_payment_clearing-7.0.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:14.984990 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3049 2024-04-17 10:45:14.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2127 2024-04-17 10:45:14.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:45:14.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       86 2024-04-17 10:45:14.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:36.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      215 2024-04-17 10:45:14.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:45:14.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:14.984990 trytond_account_payment_clearing-7.0.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/view/payment_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/view/succeed_start_form.xml
```

### Comparing `trytond_account_payment_clearing-7.0.1/CHANGELOG` & `trytond_account_payment_clearing-7.0.2/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.0.2 - 2024-04-17
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.1 - 2024-01-15
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
```

### Comparing `trytond_account_payment_clearing-7.0.1/COPYRIGHT` & `trytond_account_payment_clearing-7.0.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/LICENSE` & `trytond_account_payment_clearing-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/PKG-INFO` & `trytond_account_payment_clearing-7.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_clearing
-Version: 7.0.1
+Version: 7.0.2
 Summary: Tryton module for payment clearing
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-payment-clearing
+Project-URL: Documentation, https://docs.tryton.org/modules-account-payment-clearing
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment clearing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_account_payment_clearing-7.0.1/__init__.py` & `trytond_account_payment_clearing-7.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/account.py` & `trytond_account_payment_clearing-7.0.2/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/doc/conf.py` & `trytond_account_payment_clearing-7.0.2/doc/conf.py`

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

### Comparing `trytond_account_payment_clearing-7.0.1/doc/design.rst` & `trytond_account_payment_clearing-7.0.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/bg.po` & `trytond_account_payment_clearing-7.0.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/ca.po` & `trytond_account_payment_clearing-7.0.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/cs.po` & `trytond_account_payment_clearing-7.0.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/de.po` & `trytond_account_payment_clearing-7.0.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/es.po` & `trytond_account_payment_clearing-7.0.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/es_419.po` & `trytond_account_payment_clearing-7.0.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/et.po` & `trytond_account_payment_clearing-7.0.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/fa.po` & `trytond_account_payment_clearing-7.0.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/fi.po` & `trytond_account_payment_clearing-7.0.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/fr.po` & `trytond_account_payment_clearing-7.0.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/hu.po` & `trytond_account_payment_clearing-7.0.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/id.po` & `trytond_account_payment_clearing-7.0.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/it.po` & `trytond_account_payment_clearing-7.0.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/lo.po` & `trytond_account_payment_clearing-7.0.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/lt.po` & `trytond_account_payment_clearing-7.0.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/nl.po` & `trytond_account_payment_clearing-7.0.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/pl.po` & `trytond_account_payment_clearing-7.0.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/pt.po` & `trytond_account_payment_clearing-7.0.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/ro.po` & `trytond_account_payment_clearing-7.0.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/ru.po` & `trytond_account_payment_clearing-7.0.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/sl.po` & `trytond_account_payment_clearing-7.0.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/tr.po` & `trytond_account_payment_clearing-7.0.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/uk.po` & `trytond_account_payment_clearing-7.0.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/locale/zh_CN.po` & `trytond_account_payment_clearing-7.0.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/payment.py` & `trytond_account_payment_clearing-7.0.2/payment.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,18 +175,20 @@
         cls.account.domain = [
             cls.account.domain,
             cls._account_type_domain(),
             ]
 
     @classmethod
     def _account_type_domain(cls):
-        return If(Eval('kind') == 'receivable',
-            ('type.receivable', '=', True),
-            ('type.payable', '=', True),
-            )
+        return If(Eval('state') == 'draft',
+            If(Eval('kind') == 'receivable',
+                ('type.receivable', '=', True),
+                ('type.payable', '=', True),
+                ),
+            ())
 
     @fields.depends('party', 'kind', 'date')
     def on_change_party(self):
         super().on_change_party()
         if self.kind == 'receivable':
             if self.party:
                 with Transaction().set_context(date=self.date):
```

### Comparing `trytond_account_payment_clearing-7.0.1/payment.xml` & `trytond_account_payment_clearing-7.0.2/payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/setup.py` & `trytond_account_payment_clearing-7.0.2/setup.py`

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
             'modules-account-payment-clearing'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account payment clearing',
     package_dir={'trytond.modules.account_payment_clearing': '.'},
     packages=(
```

### Comparing `trytond_account_payment_clearing-7.0.1/statement.py` & `trytond_account_payment_clearing-7.0.2/statement.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/tests/scenario_account_negative_payment_clearing.rst` & `trytond_account_payment_clearing-7.0.2/tests/scenario_account_negative_payment_clearing.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/tests/scenario_account_payment_clearing.rst` & `trytond_account_payment_clearing-7.0.2/tests/scenario_account_payment_clearing.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/tests/scenario_account_payment_clearing_invoice_amount_to_pay.rst` & `trytond_account_payment_clearing-7.0.2/tests/scenario_account_payment_clearing_invoice_amount_to_pay.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/tox.ini` & `trytond_account_payment_clearing-7.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/trytond_account_payment_clearing.egg-info/PKG-INFO` & `trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-payment-clearing
-Version: 7.0.1
+Name: trytond_account_payment_clearing
+Version: 7.0.2
 Summary: Tryton module for payment clearing
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-payment-clearing
+Project-URL: Documentation, https://docs.tryton.org/modules-account-payment-clearing
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment clearing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_account_payment_clearing-7.0.1/trytond_account_payment_clearing.egg-info/SOURCES.txt` & `trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_payment_clearing-7.0.1/view/payment_form.xml` & `trytond_account_payment_clearing-7.0.2/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.1/view/payment_journal_form.xml` & `trytond_account_payment_clearing-7.0.2/view/payment_journal_form.xml`

 * *Files identical despite different names*

