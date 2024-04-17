# Comparing `tmp/trytond_account_payment_stripe-7.0.2.tar.gz` & `tmp/trytond_account_payment_stripe-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_stripe-7.0.2.tar", last modified: Sun Mar  3 12:25:47 2024, max compression
+gzip compressed data, was "trytond_account_payment_stripe-7.0.3.tar", last modified: Wed Apr 17 10:42:05 2024, max compression
```

## Comparing `trytond_account_payment_stripe-7.0.2.tar` & `trytond_account_payment_stripe-7.0.3.tar`

### file list

```diff
@@ -1,80 +1,79 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:25:47.497309 trytond_account_payment_stripe-7.0.2/
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2235 2024-03-03 12:25:44.000000 trytond_account_payment_stripe-7.0.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-03-03 12:25:44.000000 trytond_account_payment_stripe-7.0.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-03-03 12:25:47.497309 trytond_account_payment_stripe-7.0.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2533 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      953 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5183 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/checkout.html
--rw-r--r--   0 ced       (1000) ced       (1000)     5064 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:25:47.490643 trytond_account_payment_stripe-7.0.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2823 2024-02-05 16:24:27.000000 trytond_account_payment_stripe-7.0.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2533 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1274 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/email_checkout.html
--rw-r--r--   0 ced       (1000) ced       (1000)     1091 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:25:47.493976 trytond_account_payment_stripe-7.0.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17701 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17557 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17713 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14745 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14708 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17994 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17665 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14826 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16182 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16208 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17330 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16207 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16909 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14655 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16624 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14625 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      780 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2285 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    70751 2024-02-29 11:46:26.000000 trytond_account_payment_stripe-7.0.2/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17754 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2861 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-03-03 12:25:47.497309 trytond_account_payment_stripe-7.0.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4553 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:25:47.493976 trytond_account_payment_stripe-7.0.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10828 2024-02-29 11:47:00.000000 trytond_account_payment_stripe-7.0.2/tests/scenario_account_payment_stripe.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8962 2024-02-29 11:47:00.000000 trytond_account_payment_stripe-7.0.2/tests/scenario_account_payment_stripe_dispute.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3211 2024-02-05 16:24:27.000000 trytond_account_payment_stripe-7.0.2/tests/scenario_account_payment_stripe_identical.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5579 2024-02-29 11:47:00.000000 trytond_account_payment_stripe-7.0.2/tests/scenario_account_payment_stripe_intent.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      132 2024-02-05 16:24:27.000000 trytond_account_payment_stripe-7.0.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:25:47.497309 trytond_account_payment_stripe-7.0.2/trytond_account_payment_stripe.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-03-03 12:25:47.000000 trytond_account_payment_stripe-7.0.2/trytond_account_payment_stripe.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2024-03-03 12:25:47.000000 trytond_account_payment_stripe-7.0.2/trytond_account_payment_stripe.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-03-03 12:25:47.000000 trytond_account_payment_stripe-7.0.2/trytond_account_payment_stripe.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-03-03 12:25:47.000000 trytond_account_payment_stripe-7.0.2/trytond_account_payment_stripe.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:36.000000 trytond_account_payment_stripe-7.0.2/trytond_account_payment_stripe.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      143 2024-03-03 12:25:47.000000 trytond_account_payment_stripe-7.0.2/trytond_account_payment_stripe.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-03-03 12:25:47.000000 trytond_account_payment_stripe-7.0.2/trytond_account_payment_stripe.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:25:47.497309 trytond_account_payment_stripe-7.0.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/view/customer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/view/customer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/view/customer_source_detach_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/view/party_reception_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2519 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      439 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      955 2024-02-05 16:24:27.000000 trytond_account_payment_stripe-7.0.2/view/refund_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.2/view/refund_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:42:05.739939 trytond_account_payment_stripe-7.0.3/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2336 2024-04-17 10:42:02.000000 trytond_account_payment_stripe-7.0.3/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-17 10:42:02.000000 trytond_account_payment_stripe-7.0.3/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-04-17 10:42:05.739939 trytond_account_payment_stripe-7.0.3/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2533 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      953 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5183 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/checkout.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     5064 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:42:05.733273 trytond_account_payment_stripe-7.0.3/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2801 2024-03-03 16:24:20.000000 trytond_account_payment_stripe-7.0.3/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2533 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1274 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/email_checkout.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     1091 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:42:05.736606 trytond_account_payment_stripe-7.0.3/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17701 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17557 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17713 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14745 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14708 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17994 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17665 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14826 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16182 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16208 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17330 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16207 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16909 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14655 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16624 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14625 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      780 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2285 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    70748 2024-04-12 20:15:59.000000 trytond_account_payment_stripe-7.0.3/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17754 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2861 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:42:05.739939 trytond_account_payment_stripe-7.0.3/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4553 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:42:05.736606 trytond_account_payment_stripe-7.0.3/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10828 2024-02-29 11:47:00.000000 trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8962 2024-02-29 11:47:00.000000 trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe_dispute.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3211 2024-02-05 16:24:27.000000 trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe_identical.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5579 2024-02-29 11:47:00.000000 trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe_intent.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      132 2024-03-03 12:25:53.000000 trytond_account_payment_stripe-7.0.3/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:42:05.739939 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-04-17 10:42:05.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2607 2024-04-17 10:42:05.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:42:05.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-17 10:42:05.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:36.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      143 2024-04-17 10:42:05.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:42:05.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:42:05.739939 trytond_account_payment_stripe-7.0.3/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/customer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/customer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/customer_source_detach_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/party_reception_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2519 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      439 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      955 2024-02-05 16:24:27.000000 trytond_account_payment_stripe-7.0.3/view/refund_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/refund_list.xml
```

### Comparing `trytond_account_payment_stripe-7.0.2/CHANGELOG` & `trytond_account_payment_stripe-7.0.3/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.0.3 - 2024-04-17
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.2 - 2024-03-03
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.1 - 2024-02-03
 --------------------------
```

### Comparing `trytond_account_payment_stripe-7.0.2/COPYRIGHT` & `trytond_account_payment_stripe-7.0.3/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/LICENSE` & `trytond_account_payment_stripe-7.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/PKG-INFO` & `trytond_account_payment_stripe-7.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_stripe
-Version: 7.0.2
+Version: 7.0.3
 Summary: Tryton module for Stripe payment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_payment_stripe-7.0.2/README.rst` & `trytond_account_payment_stripe-7.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/__init__.py` & `trytond_account_payment_stripe-7.0.3/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/checkout.html` & `trytond_account_payment_stripe-7.0.3/checkout.html`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/common.py` & `trytond_account_payment_stripe-7.0.3/common.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/doc/conf.py` & `trytond_account_payment_stripe-7.0.3/doc/conf.py`

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

### Comparing `trytond_account_payment_stripe-7.0.2/doc/index.rst` & `trytond_account_payment_stripe-7.0.3/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/email_checkout.html` & `trytond_account_payment_stripe-7.0.3/email_checkout.html`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/ir.py` & `trytond_account_payment_stripe-7.0.3/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/bg.po` & `trytond_account_payment_stripe-7.0.3/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/ca.po` & `trytond_account_payment_stripe-7.0.3/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/cs.po` & `trytond_account_payment_stripe-7.0.3/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/de.po` & `trytond_account_payment_stripe-7.0.3/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/es.po` & `trytond_account_payment_stripe-7.0.3/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/es_419.po` & `trytond_account_payment_stripe-7.0.3/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/et.po` & `trytond_account_payment_stripe-7.0.3/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/fa.po` & `trytond_account_payment_stripe-7.0.3/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/fi.po` & `trytond_account_payment_stripe-7.0.3/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/fr.po` & `trytond_account_payment_stripe-7.0.3/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/hu.po` & `trytond_account_payment_stripe-7.0.3/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/id.po` & `trytond_account_payment_stripe-7.0.3/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/it.po` & `trytond_account_payment_stripe-7.0.3/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/lo.po` & `trytond_account_payment_stripe-7.0.3/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/lt.po` & `trytond_account_payment_stripe-7.0.3/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/nl.po` & `trytond_account_payment_stripe-7.0.3/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/pl.po` & `trytond_account_payment_stripe-7.0.3/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/pt.po` & `trytond_account_payment_stripe-7.0.3/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/ro.po` & `trytond_account_payment_stripe-7.0.3/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/ru.po` & `trytond_account_payment_stripe-7.0.3/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/sl.po` & `trytond_account_payment_stripe-7.0.3/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/tr.po` & `trytond_account_payment_stripe-7.0.3/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/uk.po` & `trytond_account_payment_stripe-7.0.3/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/locale/zh_CN.po` & `trytond_account_payment_stripe-7.0.3/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/message.xml` & `trytond_account_payment_stripe-7.0.3/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/party.py` & `trytond_account_payment_stripe-7.0.3/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/party.xml` & `trytond_account_payment_stripe-7.0.3/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/payment.py` & `trytond_account_payment_stripe-7.0.3/payment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1074,15 +1074,15 @@
         refunds = Refund.search([
                 ('stripe_refund_id', '=', rf['id']),
                 ])
         if not refunds:
             logger.error("charge.refund.updated: No refund '%s'", rf['id'])
         for refund in refunds:
             if rf['status'] == 'pending':
-                Refund.processing([refund])
+                Refund.process([refund])
             elif rf['status'] == 'succeeded':
                 Refund.succeed([refund])
             elif rf['status'] in {'failed', 'canceled'}:
                 refund.stripe_error_code = rf['failure_reason']
                 Refund.fail([refund])
             refund.save()
         return bool(refunds)
```

### Comparing `trytond_account_payment_stripe-7.0.2/payment.xml` & `trytond_account_payment_stripe-7.0.3/payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/routes.py` & `trytond_account_payment_stripe-7.0.3/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/setup.py` & `trytond_account_payment_stripe-7.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/tests/scenario_account_payment_stripe.rst` & `trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/tests/scenario_account_payment_stripe_dispute.rst` & `trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe_dispute.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/tests/scenario_account_payment_stripe_identical.rst` & `trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe_identical.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/tests/scenario_account_payment_stripe_intent.rst` & `trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe_intent.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/tox.ini` & `trytond_account_payment_stripe-7.0.3/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/trytond_account_payment_stripe.egg-info/PKG-INFO` & `trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_stripe
-Version: 7.0.2
+Version: 7.0.3
 Summary: Tryton module for Stripe payment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_payment_stripe-7.0.2/trytond_account_payment_stripe.egg-info/SOURCES.txt` & `trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/SOURCES.txt`

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
 checkout.html
```

### Comparing `trytond_account_payment_stripe-7.0.2/view/account_form.xml` & `trytond_account_payment_stripe-7.0.3/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/view/customer_form.xml` & `trytond_account_payment_stripe-7.0.3/view/customer_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/view/party_reception_direct_debit_form.xml` & `trytond_account_payment_stripe-7.0.3/view/party_reception_direct_debit_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/view/payment_form.xml` & `trytond_account_payment_stripe-7.0.3/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.2/view/refund_form.xml` & `trytond_account_payment_stripe-7.0.3/view/refund_form.xml`

 * *Files identical despite different names*

