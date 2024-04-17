# Comparing `tmp/bda.plone.orders-2.0b1.tar.gz` & `tmp/bda.plone.orders-2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bda.plone.orders-2.0b1.tar", last modified: Wed Apr 17 13:49:56 2024, max compression
+gzip compressed data, was "bda.plone.orders-2.0b2.tar", last modified: Wed Apr 17 14:20:57 2024, max compression
```

## Comparing `bda.plone.orders-2.0b1.tar` & `bda.plone.orders-2.0b2.tar`

### file list

```diff
@@ -1,167 +1,168 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.915731 bda.plone.orders-2.0b1/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    15804 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1504 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)    18092 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/LICENSE_GPL.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       71 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)    32990 2024-04-17 13:49:56.915731 bda.plone.orders-2.0b1/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)    14259 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)      258 2024-04-17 13:49:56.915731 bda.plone.orders-2.0b1/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1956 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.903731 bda.plone.orders-2.0b1/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.903731 bda.plone.orders-2.0b1/src/bda/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.907731 bda.plone.orders-2.0b1/src/bda/plone/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.907731 bda.plone.orders-2.0b1/src/bda/plone/orders/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1319 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.907731 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       24 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    26601 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/bookings.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2748 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/common.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9860 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/configure.zcml
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5256 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/contacts.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1572 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/dropdown.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    14385 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/export.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.907731 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/forms/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1145 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/forms/mailtemplates.yaml
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1040 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/forms/notify_customers.yaml
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1527 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/forms/orders_export.yaml
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4592 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/invoice.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2465 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/mailtemplates.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5339 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/notify_customers.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    14789 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/order.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    22413 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/orders.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.911731 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      211 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/bookings.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      223 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/cross.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      274 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/delete.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      292 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/invoice.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      211 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/invoices.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)    56209 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/jquery-barcode.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      240 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/notify_customers.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      175 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/order.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)    10281 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/orders.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    12838 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/orders.css.map
--rw-r--r--   0 rnix      (1000) rnix      (1000)    16064 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/orders.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      211 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/orders.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      218 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/pencil.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      239 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/print.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)    36243 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/qrcode.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1849 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/spinner.gif
--rw-r--r--   0 rnix      (1000) rnix      (1000)      189 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/tick.png
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.911731 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      410 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/bookings.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      573 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/bookings_view.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1968 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/contacts.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1265 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/dropdown.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1068 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/export.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)    10355 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/invoice.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2265 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/mailtemplates_view.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11610 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/order.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1128 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/order_done.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      421 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/orders.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      568 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/orders_view.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      756 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/protected_view.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1169 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/table.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1659 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/browser/views.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4477 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/catalogfactories.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    10848 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/checkout.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7335 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/common.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3476 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/configure.zcml
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5043 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/contacts.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.911731 bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/
--rw-r--r--   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3947 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/base.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4030 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/booking.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1158 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/buyable.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6002 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/order.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4088 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/orders.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3082 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/payment.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1525 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/events.py
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)     2214 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/i18n.sh
--rw-r--r--   0 rnix      (1000) rnix      (1000)      493 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/indexer.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.911731 bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2069 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1427 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/events.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      602 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/mailtemplates.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      627 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/markers.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1059 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/notifications.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2268 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/orders.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      266 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/tradings.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      517 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/workflow.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.911731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    23074 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/bda.plone.orders.pot
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.903731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/de/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.911731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/de/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    27066 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/de/LC_MESSAGES/bda.plone.orders.po
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.903731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/en/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.911731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/en/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    25302 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/en/LC_MESSAGES/bda.plone.orders.po
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.903731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/fr/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.911731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/fr/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    24033 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/fr/LC_MESSAGES/bda.plone.orders.po
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.903731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/it/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.911731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/it/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    24019 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/it/LC_MESSAGES/bda.plone.orders.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1495 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/manual.pot
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.903731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/nl/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.911731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/nl/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6148 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/nl/LC_MESSAGES/.DS_Store
--rw-r--r--   0 rnix      (1000) rnix      (1000)    25611 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/nl/LC_MESSAGES/bda.plone.orders.po
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.903731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/nn/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.911731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/nn/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    24452 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/nn/LC_MESSAGES/bda.plone.orders.po
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.903731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/no/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.911731 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/no/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    24098 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/locales/no/LC_MESSAGES/bda.plone.orders.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)      675 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/localroles.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    31138 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/mailnotify.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.915731 bda.plone.orders-2.0b1/src/bda/plone/orders/mailtemplates/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      990 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/mailtemplates/booking_cancelled.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1028 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/mailtemplates/booking_reserved_to_ordered.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11052 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/mailtemplates/order_success.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      770 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/mailtemplates/stock_threshold_reached.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)    22128 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/mailtemplates.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1283 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/permissions.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      955 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/permissions.zcml
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.903731 bda.plone.orders-2.0b1/src/bda/plone/orders/profiles/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.915731 bda.plone.orders-2.0b1/src/bda/plone/orders/profiles/default/
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)      150 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/profiles/default/browserlayer.xml
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)      204 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/profiles/default/catalog.xml
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)      363 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/profiles/default/metadata.xml
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)     1859 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/profiles/default/registry.xml
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)     1719 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/profiles/default/rolemap.xml
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.915731 bda.plone.orders-2.0b1/src/bda/plone/orders/profiles/uninstall/
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)      171 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/profiles/uninstall/browserlayer.xml
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)      166 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/profiles/uninstall/catalog.xml
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)      265 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/profiles/uninstall/registry.xml
--rw-r--r--   0 rnix      (1000) rnix      (1000)      867 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/profiles.zcml
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.915731 bda.plone.orders-2.0b1/src/bda/plone/orders/restapi/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       24 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/restapi/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2707 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/restapi/booking.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1149 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/restapi/configure.zcml
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2082 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/restapi/order.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1857 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/restapi/serializer.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      454 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/setuphandlers.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      300 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/subscriber.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.915731 bda.plone.orders-2.0b1/src/bda/plone/orders/tests/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1142 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/tests/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2829 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/tests/dynamicmaillibrary.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2277 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/tests/dynamicmailtemplate.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)      668 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/tests/test_contacts.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      735 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/tests/test_doctests.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      755 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/tests/test_mailnotify.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1452 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/tests/test_orders.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2918 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/tests/test_restapi_serializer.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5568 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/transitions.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    15103 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/upgrades.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3187 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/upgrades.zcml
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4227 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda/plone/orders/vocabularies.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 13:49:56.915731 bda.plone.orders-2.0b1/src/bda.plone.orders.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    32990 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda.plone.orders.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5911 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda.plone.orders.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda.plone.orders.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       14 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda.plone.orders.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda.plone.orders.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)      292 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda.plone.orders.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        4 2024-04-17 13:49:56.000000 bda.plone.orders-2.0b1/src/bda.plone.orders.egg-info/top_level.txt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.273133 bda.plone.orders-2.0b2/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    15892 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1504 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    18092 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/LICENSE_GPL.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       71 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    33078 2024-04-17 14:20:57.273133 bda.plone.orders-2.0b2/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    14259 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      258 2024-04-17 14:20:57.273133 bda.plone.orders-2.0b2/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1956 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.257133 bda.plone.orders-2.0b2/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.261133 bda.plone.orders-2.0b2/src/bda/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.261133 bda.plone.orders-2.0b2/src/bda/plone/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.265133 bda.plone.orders-2.0b2/src/bda/plone/orders/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1319 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.265133 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       24 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    26601 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/bookings.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2748 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/common.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9860 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/configure.zcml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5256 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/contacts.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1572 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/dropdown.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    14385 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/export.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.265133 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/forms/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1145 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/forms/mailtemplates.yaml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1040 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/forms/notify_customers.yaml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1527 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/forms/orders_export.yaml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4592 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/invoice.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2465 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/mailtemplates.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5339 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/notify_customers.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    14789 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/order.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    22413 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/orders.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.265133 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      211 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/bookings.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      223 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/cross.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      274 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/delete.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      292 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/invoice.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      211 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/invoices.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    56209 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/jquery-barcode.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      240 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/notify_customers.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      175 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/order.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10152 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/orders.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2218 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/orders.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    16064 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/orders.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8027 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/orders.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      211 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/orders.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      218 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/pencil.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      239 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/print.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    36243 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/qrcode.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1849 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/spinner.gif
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      189 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/tick.png
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.265133 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      410 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/bookings.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      573 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/bookings_view.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1968 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/contacts.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1265 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/dropdown.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1068 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/export.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10355 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/invoice.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2265 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/mailtemplates_view.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11610 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/order.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1128 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/order_done.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      421 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/orders.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      568 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/orders_view.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      756 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/protected_view.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1169 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/table.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1659 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/browser/views.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4477 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/catalogfactories.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10848 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/checkout.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7335 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/common.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3476 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/configure.zcml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5043 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/contacts.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3947 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/base.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4030 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/booking.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1158 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/buyable.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6002 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/order.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4088 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/orders.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3082 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/payment.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1525 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/events.py
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)     2214 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/i18n.sh
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      493 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/indexer.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2069 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1427 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/events.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      602 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/mailtemplates.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      627 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/markers.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1059 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/notifications.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2268 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/orders.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      266 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/tradings.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      517 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/workflow.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    23074 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/bda.plone.orders.pot
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.261133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/de/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/de/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    27066 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/de/LC_MESSAGES/bda.plone.orders.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.261133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/en/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/en/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    25302 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/en/LC_MESSAGES/bda.plone.orders.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.261133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/fr/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    24033 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/fr/LC_MESSAGES/bda.plone.orders.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.261133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/it/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/it/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    24019 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/it/LC_MESSAGES/bda.plone.orders.po
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1495 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/manual.pot
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.261133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/nl/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6148 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/nl/LC_MESSAGES/.DS_Store
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    25611 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/nl/LC_MESSAGES/bda.plone.orders.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.261133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/nn/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/nn/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    24452 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/nn/LC_MESSAGES/bda.plone.orders.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.261133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/no/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/no/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    24098 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/locales/no/LC_MESSAGES/bda.plone.orders.po
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      675 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/localroles.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    31138 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/mailnotify.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/mailtemplates/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      990 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/mailtemplates/booking_cancelled.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1028 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/mailtemplates/booking_reserved_to_ordered.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11052 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/mailtemplates/order_success.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      770 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/mailtemplates/stock_threshold_reached.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    22128 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/mailtemplates.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1283 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/permissions.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      955 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/permissions.zcml
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.261133 bda.plone.orders-2.0b2/src/bda/plone/orders/profiles/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/profiles/default/
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)      150 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/profiles/default/browserlayer.xml
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)      204 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/profiles/default/catalog.xml
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)      363 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/profiles/default/metadata.xml
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)     1859 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/profiles/default/registry.xml
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)     1719 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/profiles/default/rolemap.xml
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/profiles/uninstall/
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)      171 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/profiles/uninstall/browserlayer.xml
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)      166 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/profiles/uninstall/catalog.xml
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)      265 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/profiles/uninstall/registry.xml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      867 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/profiles.zcml
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/restapi/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       24 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/restapi/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2707 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/restapi/booking.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1149 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/restapi/configure.zcml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2082 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/restapi/order.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1857 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/restapi/serializer.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      454 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/setuphandlers.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      300 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/subscriber.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda/plone/orders/tests/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1142 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/tests/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2829 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/tests/dynamicmaillibrary.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2277 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/tests/dynamicmailtemplate.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      668 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/tests/test_contacts.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      735 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/tests/test_doctests.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      755 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/tests/test_mailnotify.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1452 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/tests/test_orders.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2918 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/tests/test_restapi_serializer.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5568 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/transitions.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    15103 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/upgrades.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3187 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/upgrades.zcml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4227 2024-04-17 14:20:56.000000 bda.plone.orders-2.0b2/src/bda/plone/orders/vocabularies.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:20:57.269133 bda.plone.orders-2.0b2/src/bda.plone.orders.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    33078 2024-04-17 14:20:57.000000 bda.plone.orders-2.0b2/src/bda.plone.orders.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5965 2024-04-17 14:20:57.000000 bda.plone.orders-2.0b2/src/bda.plone.orders.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-04-17 14:20:57.000000 bda.plone.orders-2.0b2/src/bda.plone.orders.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       14 2024-04-17 14:20:57.000000 bda.plone.orders-2.0b2/src/bda.plone.orders.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-04-17 14:20:57.000000 bda.plone.orders-2.0b2/src/bda.plone.orders.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      292 2024-04-17 14:20:57.000000 bda.plone.orders-2.0b2/src/bda.plone.orders.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        4 2024-04-17 14:20:57.000000 bda.plone.orders-2.0b2/src/bda.plone.orders.egg-info/top_level.txt
```

### Comparing `bda.plone.orders-2.0b1/CHANGES.rst` & `bda.plone.orders-2.0b2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2.0b2 (2024-04-17)
+------------------
+
+- Add missing compiled resources.
+  [petschki]
+
+
 2.0b1 (2024-04-17)
 ------------------
 
 - Introduce base class to allow more flexible subclassing for export.
   [jensens]
 
 - Use csv23 for py2/3 csv export.
```

### Comparing `bda.plone.orders-2.0b1/LICENSE.rst` & `bda.plone.orders-2.0b2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/LICENSE_GPL.rst` & `bda.plone.orders-2.0b2/LICENSE_GPL.rst`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/PKG-INFO` & `bda.plone.orders-2.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bda.plone.orders
-Version: 2.0b1
+Version: 2.0b2
 Summary: Orders persistence and backoffice UI for bda.plone.shop
 Author: BlueDynamics Alliance
 Author-email: dev@bluedynamics.com
 License: GNU General Public Licence
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Addon
@@ -502,14 +502,21 @@
 
 
 Icons used are `Silk-Icons by FamFamFam <http://www.famfamfam.com/lab/icons/silk/>`_
 under CC-BY 2.5 license.
 Changelog
 =========
 
+2.0b2 (2024-04-17)
+------------------
+
+- Add missing compiled resources.
+  [petschki]
+
+
 2.0b1 (2024-04-17)
 ------------------
 
 - Introduce base class to allow more flexible subclassing for export.
   [jensens]
 
 - Use csv23 for py2/3 csv export.
```

### Comparing `bda.plone.orders-2.0b1/README.rst` & `bda.plone.orders-2.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/setup.py` & `bda.plone.orders-2.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
 import os
 
 
-version = "2.0b1"
+version = "2.0b2"
 shortdesc = "Orders persistence and backoffice UI for bda.plone.shop"
 longdesc = open(os.path.join(os.path.dirname(__file__), "README.rst")).read()
 longdesc += open(os.path.join(os.path.dirname(__file__), "CHANGES.rst")).read()
 longdesc += open(os.path.join(os.path.dirname(__file__), "LICENSE.rst")).read()
 
 
 setup(
```

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/__init__.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/bookings.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/bookings.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/common.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/common.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/configure.zcml` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/contacts.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/contacts.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/dropdown.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/dropdown.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/export.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/export.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/forms/mailtemplates.yaml` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/forms/mailtemplates.yaml`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/forms/notify_customers.yaml` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/forms/notify_customers.yaml`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/forms/orders_export.yaml` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/forms/orders_export.yaml`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/invoice.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/invoice.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/mailtemplates.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/mailtemplates.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/notify_customers.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/notify_customers.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/order.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/order.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/orders.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/orders.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/jquery-barcode.js` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/jquery-barcode.js`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/orders.css` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/orders.css`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #exposeMask {
   z-index: 0 !important;
   /* render exposeMask BEHIND the overlay */
 }
+
 /* dropdown menu */
 .dropdown {
   padding: 0;
   margin: 0;
   position: relative;
 }
+
 .dropdown_items {
   display: none;
   position: absolute;
   left: 0;
   margin-left: 0 !important;
   margin-top: 3px;
   padding: 6px 3px 3px 3px;
@@ -22,406 +24,483 @@
   border: #ccc 4px solid;
   background-color: #fff;
   border-radius: 3px;
   -moz-border-radius: 3px;
   -webkit-border-radius: 3px;
   -o-border-radius: 3px;
 }
+
 .dropdown_items li {
   margin: 0;
   padding-left: 5px;
 }
+
 .dropdown_items li a {
   text-decoration: none;
   border: none !important;
   padding-left: 3px;
   padding-bottom: 2px;
   line-height: 16px;
 }
+
 .dropdown_header {
   cursor: pointer;
 }
+
 /* orders filter and bookings filter */
 #orders_wrapper .filter,
 #bookings_wrapper .filter {
   padding: 0.3em;
 }
-#orders_wrapper .filter:before,
-#bookings_wrapper .filter:before,
-#orders_wrapper .filter:after,
-#bookings_wrapper .filter:after {
-  content: " ";
-  display: table;
-}
-#orders_wrapper .filter:after,
-#bookings_wrapper .filter:after {
-  clear: both;
-}
+
 #orders_wrapper .filter > div,
 #bookings_wrapper .filter > div {
   float: left;
   margin-right: 1em;
 }
+
 #orders_wrapper .filter label,
 #bookings_wrapper .filter label {
   margin-right: 0.5em;
   padding-top: 3px;
   display: inline-block;
 }
+
 #orders_wrapper .filter select,
 #bookings_wrapper .filter select {
   margin-right: 0.5em;
   width: unset;
   display: unset;
 }
+
 /* orders */
 #bdaploneorders_wrapper {
   margin-top: 1em;
   margin-bottom: 2.2em;
 }
+
 #bdaploneorders_length {
   margin-bottom: 0.8em;
 }
+
 #bdaploneorders_length select,
 #bdaploneorders_filter input {
   font-size: 90%;
   width: unset;
   display: unset;
 }
+
 #bdaploneorders_filter {
   margin-top: 0.25em;
 }
+
 #bdaploneorders {
   margin-bottom: 1em;
   border: #ddd 1px solid;
-  width: 100%!important;
+  width: 100% !important;
 }
+
 #bdaploneorders thead {
   background-color: #fafafa;
 }
+
 #bdaploneorders th {
   border-right: #ddd 1px solid;
   border-bottom: #ddd 1px solid;
 }
+
 #bdaploneorders th.datarow-actions {
   width: 120px;
 }
+
 #bdaploneorders td {
   padding: 1px 3px 1px 10px;
   border-right: #ddd 1px solid;
 }
+
 #bdaploneorders a.contenttype-document {
   border: none !important;
 }
+
 #bdaploneorders_paginate a:hover {
   color: #fff !important;
 }
+
 input.select_all_orders,
 input.select_order {
   position: relative;
   top: 2px;
 }
+
 a.notify_customers {
   border-bottom: none !important;
   display: inline-block;
   line-height: 16px;
   padding-left: 20px !important;
-  background: url('++resource++bda.plone.orders/notify_customers.png') 4px 0px no-repeat;
+  background: url("++resource++bda.plone.orders/notify_customers.png") 4px 0px no-repeat;
 }
+
 /* orders filter */
 #form-ordersfilter label {
   margin-right: 0.5em;
 }
+
 #form-ordersfilter select,
 #form-ordersfilter input {
   margin-right: 1em;
 }
+
 /* bookings */
 #bdaplonebookings_wrapper {
   margin-top: 1em;
   margin-bottom: 2.2em;
 }
+
 #bdaplonebookings_length {
   margin-bottom: 0.8em;
 }
+
 #bdaplonebookings_length select,
 #bdaplonebookings_filter input {
   font-size: 90%;
 }
+
 #bdaplonebookings {
   margin-bottom: 1em;
   border: #ddd 1px solid;
 }
+
 #bdaplonebookings_wrapper div.group_filter {
   margin-left: 3em;
 }
+
 #bdaplonebookings_wrapper div.group_filter,
 #bdaplonebookings_wrapper div.date_from_filter,
 #bdaplonebookings_wrapper div.date_to_filter {
   float: left;
   margin-right: 3em;
 }
+
 #bdaplonebookings thead {
   background-color: #fafafa;
 }
+
 #bdaplonebookings th {
   border-right: #ddd 1px solid;
   border-bottom: #ddd 1px solid;
 }
+
 #bdaplonebookings th.datarow-actions {
   width: 120px;
 }
+
 #bdaplonebookings tr.group_email,
 #bdaplonebookings tr.group_email:hover,
 #bdaplonebookings tr.group_buyable,
 #bdaplonebookings tr.group_buyable:hover {
   background-color: #ddd !important;
 }
+
 #bdaplonebookings tr.group_email td p,
 #bdaplonebookings tr.group_buyable td p {
   margin-bottom: 0;
   float: left;
   min-width: 18em;
   width: 18em;
 }
+
 #bdaplonebookings tr.group_email span,
 #bdaplonebookings tr.group_buyable span {
   min-width: 18em;
   width: 18em;
   float: left;
   margin-left: 7em;
 }
+
 #bdaplonebookings td {
   padding: 1px 3px 1px 10px;
   border-right: #ddd 1px solid;
 }
+
 #bdaplonebookings a.contenttype-document {
   border: none !important;
 }
+
 #bdaplonebookings_paginate a:hover {
   color: #fff !important;
 }
+
 /* end rules for new bookingstable */
 /* export form */
 #field-exportorders-from,
 #field-exportorders-to {
   margin: 0.4em;
 }
+
 /* mail templates */
 #array-notify_customers-array table {
   width: 100%;
 }
+
 /* notification form */
 #form-notify_customers {
   margin: 2em;
 }
+
 /* order state colors */
 .state-value-reserved {
   color: #00b400;
 }
+
 .state-value-new {
   color: #ffcc00;
 }
+
 .state-value-finished {
   color: #1600e5;
 }
+
 .state-value-cancelled {
   color: #e50000;
 }
+
 /* order salaried colors */
 .salaried-value-yes {
   color: #1600e5;
 }
+
 .salaried-value-no {
   color: #ffcc00;
 }
+
 .salaried-value-failed {
   color: #e50000;
 }
+
 /* protected order data */
 .protected_order_data form {
   display: table;
   border-spacing: 1em;
 }
+
 .protected_order_data form > div {
   display: table-row;
 }
+
 .protected_order_data form label {
   display: table-cell;
 }
+
 .protected_order_data form div.error,
 .protected_order_data form input {
   display: table-cell;
 }
+
 .protected_order_data form div.submit label {
   color: transparent;
 }
+
 .protected_order_data form div.submit input {
   float: right;
 }
+
 /* order */
 .order_details {
   padding: 1.2em;
 }
+
 .order_details .qr_code {
   position: absolute;
   right: 1em;
   top: 1em;
 }
+
 .order_details_row {
   display: table-row;
 }
+
 .order_details_row div {
   display: table-cell;
   width: 380px;
   padding: 0.4em;
 }
+
 .booking_comment_spinner {
   display: none;
 }
-input[type="text"].booking_comment_edit {
+
+input[type=text].booking_comment_edit {
   display: inline-block;
   width: 10em;
   height: unset;
   font-size: unset;
   padding: 0 0.5em;
 }
+
 .order_bookings {
   padding: 0 0.4em 0.4em 0.4em;
 }
+
 .order_bookings h3 {
   margin-top: 0.8em;
   margin-bottom: 0.3em;
 }
+
 .order_bookings table {
   width: 100%;
   border: #ddd 1px solid;
   border-spacing: 0;
   border-collapse: collapse;
 }
+
 .order_bookings table th {
   padding: 5px 3px 5px 1em;
   text-align: left;
   background-color: #fafafa;
   border-right: #ddd 1px solid;
   border-bottom: #ddd 1px solid;
   font-weight: bold;
 }
+
 .order_bookings table td {
   padding: 5px 3px 5px 1em;
   border-right: #ddd 1px solid;
 }
+
 .order_bookings tr.odd td {
   background-color: #fbfbfb;
 }
+
 /* invoice */
 .invoice_overlay {
-  width:60%;
-  min-width:800px;
-  min-width:1200px;
-  padding:2em;
-  margin-bottom:2em;
+  width: 60%;
+  min-width: 800px;
+  min-width: 1200px;
+  padding: 2em;
+  margin-bottom: 2em;
 }
+
 .invoice .print {
-  position:absolute;
-  top:2em;
-  right:2em;
+  position: absolute;
+  top: 2em;
+  right: 2em;
 }
+
 .invoice .invoice_title {
-  text-align:center;
+  text-align: center;
 }
+
 .invoice .invoice_sender {
-  width:30%;
-  float:right;
+  width: 30%;
+  float: right;
 }
+
 .invoice .invoice_receiver {
-  clear:both;
-  padding-top:2em;
-  padding-bottom:2em;
+  clear: both;
+  padding-top: 2em;
+  padding-bottom: 2em;
 }
+
 .invoice .invoice_number {
-  float:left;
-  margin-bottom:1em;
+  float: left;
+  margin-bottom: 1em;
 }
+
 .invoice .invoice_date {
-  float:right;
-  margin-top:1.2em;
+  float: right;
+  margin-top: 1.2em;
 }
+
 .invoice .invoice_listing {
-  clear:both;
-  display:table;
-  border-collapse:collapse;
-  width:100%;
+  clear: both;
+  display: table;
+  border-collapse: collapse;
+  width: 100%;
 }
+
 .invoice .invoice_listing_head {
-  display:table-row;
-  border-top:#333 1px solid;
-  border-bottom:#333 1px solid;
+  display: table-row;
+  border-top: #333 1px solid;
+  border-bottom: #333 1px solid;
 }
+
 .invoice .invoice_listing_item {
-  display:table-row;
-  border-bottom:#333 1px solid;
+  display: table-row;
+  border-bottom: #333 1px solid;
 }
+
 .invoice .invoice_listing_amount,
 .invoice .invoice_listing_position,
 .invoice .invoice_listing_price {
-  display:table-cell;
-  padding-top:0.3em;
-  padding-bottom:0.3em;
+  display: table-cell;
+  padding-top: 0.3em;
+  padding-bottom: 0.3em;
 }
+
 .invoice .invoice_listing_amount {
   width: 12%;
 }
+
 .invoice .invoice_listing_price {
-  text-align:right;
+  text-align: right;
   width: 24%;
 }
+
 .invoice .original_price {
-  float:left;
+  float: left;
   color: red;
   text-decoration: line-through;
 }
+
 .invoice .invoice_summary {
-  width:30%;
-  float:right;
-  margin-top:2em;
+  width: 30%;
+  float: right;
+  margin-top: 2em;
 }
+
 .invoice .invoice_summary_section {
-  display:table;
-  width:100%;
-  border-bottom:#333 1px solid;
-  padding-top:0.5em;
-  padding-bottom:0.5em;
+  display: table;
+  width: 100%;
+  border-bottom: #333 1px solid;
+  padding-top: 0.5em;
+  padding-bottom: 0.5em;
 }
+
 .invoice .invoice_summary_row {
-  display:table-row;
+  display: table-row;
 }
+
 .invoice .invoice_summary_label {
-  display:table-cell;
-  padding-top:0.1em;
-  padding-bottom:0.1em;
+  display: table-cell;
+  padding-top: 0.1em;
+  padding-bottom: 0.1em;
 }
+
 .invoice .invoice_summary_value {
-  display:table-cell;
-  padding-top:0.1em;
-  padding-bottom:0.1em;
-  text-align:right;
+  display: table-cell;
+  padding-top: 0.1em;
+  padding-bottom: 0.1em;
+  text-align: right;
 }
+
 .invoice .invoice_summary .red {
   color: red;
 }
+
 .invoice .invoice_bank_connection {
-  clear:both;
+  clear: both;
 }
+
 .invoice .invoice_footer {
-  margin-top:2em;
+  margin-top: 2em;
 }
+
 /* print styles */
 @media print {
-  /* rules for bookingstable  print preview */
+  /* rules for bookingstable - print preview */
   #bookings_wrapper .customfilter label,
   #bookings_wrapper #bdaplonebookings_filter label,
   #bookings_wrapper #bdaplonebookings_length label {
     font-weight: bold;
   }
   #bookings_wrapper .customfilter input,
   #bookings_wrapper #bdaplonebookings_filter input,
@@ -491,8 +570,9 @@
   #bdaplonebookings a.contenttype-document {
     border: none !important;
   }
   #bdaplonebookings_paginate {
     display: none;
   }
 }
-/*# sourceMappingURL=++resource++bda.plone.orders.css.map */
+
+/*# sourceMappingURL=orders.css.map */
```

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/orders.js` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/orders.js`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/qrcode.js` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/qrcode.js`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/resources/spinner.gif` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/resources/spinner.gif`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/bookings_view.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/bookings_view.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/contacts.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/contacts.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/dropdown.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/dropdown.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/export.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/export.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/invoice.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/invoice.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/mailtemplates_view.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/mailtemplates_view.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/order.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/order.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/order_done.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/order_done.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/orders_view.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/orders_view.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/protected_view.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/protected_view.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/templates/table.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/templates/table.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/browser/views.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/browser/views.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/catalogfactories.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/catalogfactories.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/checkout.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/checkout.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/common.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/common.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/configure.zcml` & `bda.plone.orders-2.0b2/src/bda/plone/orders/configure.zcml`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/contacts.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/contacts.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/base.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/base.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/booking.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/booking.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/buyable.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/buyable.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/order.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/order.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/orders.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/orders.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/datamanagers/payment.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/datamanagers/payment.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/events.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/events.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/i18n.sh` & `bda.plone.orders-2.0b2/src/bda/plone/orders/i18n.sh`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/__init__.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/events.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/events.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/mailtemplates.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/mailtemplates.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/markers.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/markers.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/notifications.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/notifications.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/orders.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/orders.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/interfaces/workflow.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/interfaces/workflow.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/locales/bda.plone.orders.pot` & `bda.plone.orders-2.0b2/src/bda/plone/orders/locales/bda.plone.orders.pot`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/locales/de/LC_MESSAGES/bda.plone.orders.po` & `bda.plone.orders-2.0b2/src/bda/plone/orders/locales/de/LC_MESSAGES/bda.plone.orders.po`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/locales/en/LC_MESSAGES/bda.plone.orders.po` & `bda.plone.orders-2.0b2/src/bda/plone/orders/locales/en/LC_MESSAGES/bda.plone.orders.po`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/locales/fr/LC_MESSAGES/bda.plone.orders.po` & `bda.plone.orders-2.0b2/src/bda/plone/orders/locales/fr/LC_MESSAGES/bda.plone.orders.po`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/locales/it/LC_MESSAGES/bda.plone.orders.po` & `bda.plone.orders-2.0b2/src/bda/plone/orders/locales/it/LC_MESSAGES/bda.plone.orders.po`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/locales/manual.pot` & `bda.plone.orders-2.0b2/src/bda/plone/orders/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/locales/nl/LC_MESSAGES/.DS_Store` & `bda.plone.orders-2.0b2/src/bda/plone/orders/locales/nl/LC_MESSAGES/.DS_Store`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/locales/nl/LC_MESSAGES/bda.plone.orders.po` & `bda.plone.orders-2.0b2/src/bda/plone/orders/locales/nl/LC_MESSAGES/bda.plone.orders.po`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/locales/nn/LC_MESSAGES/bda.plone.orders.po` & `bda.plone.orders-2.0b2/src/bda/plone/orders/locales/nn/LC_MESSAGES/bda.plone.orders.po`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/locales/no/LC_MESSAGES/bda.plone.orders.po` & `bda.plone.orders-2.0b2/src/bda/plone/orders/locales/no/LC_MESSAGES/bda.plone.orders.po`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/localroles.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/localroles.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/mailnotify.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/mailnotify.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/mailtemplates/booking_cancelled.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/mailtemplates/booking_cancelled.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/mailtemplates/booking_reserved_to_ordered.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/mailtemplates/booking_reserved_to_ordered.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/mailtemplates/order_success.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/mailtemplates/order_success.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/mailtemplates/stock_threshold_reached.pt` & `bda.plone.orders-2.0b2/src/bda/plone/orders/mailtemplates/stock_threshold_reached.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/mailtemplates.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/mailtemplates.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/permissions.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/permissions.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/permissions.zcml` & `bda.plone.orders-2.0b2/src/bda/plone/orders/permissions.zcml`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/profiles/default/registry.xml` & `bda.plone.orders-2.0b2/src/bda/plone/orders/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/profiles/default/rolemap.xml` & `bda.plone.orders-2.0b2/src/bda/plone/orders/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/profiles.zcml` & `bda.plone.orders-2.0b2/src/bda/plone/orders/profiles.zcml`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/restapi/booking.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/restapi/booking.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/restapi/configure.zcml` & `bda.plone.orders-2.0b2/src/bda/plone/orders/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/restapi/order.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/restapi/order.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/restapi/serializer.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/restapi/serializer.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/tests/__init__.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/tests/dynamicmaillibrary.rst` & `bda.plone.orders-2.0b2/src/bda/plone/orders/tests/dynamicmaillibrary.rst`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/tests/dynamicmailtemplate.rst` & `bda.plone.orders-2.0b2/src/bda/plone/orders/tests/dynamicmailtemplate.rst`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/tests/test_contacts.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/tests/test_contacts.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/tests/test_doctests.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/tests/test_mailnotify.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/tests/test_mailnotify.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/tests/test_orders.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/tests/test_orders.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/tests/test_restapi_serializer.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/tests/test_restapi_serializer.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/transitions.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/transitions.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/upgrades.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/upgrades.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/upgrades.zcml` & `bda.plone.orders-2.0b2/src/bda/plone/orders/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda/plone/orders/vocabularies.py` & `bda.plone.orders-2.0b2/src/bda/plone/orders/vocabularies.py`

 * *Files identical despite different names*

### Comparing `bda.plone.orders-2.0b1/src/bda.plone.orders.egg-info/PKG-INFO` & `bda.plone.orders-2.0b2/src/bda.plone.orders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bda.plone.orders
-Version: 2.0b1
+Version: 2.0b2
 Summary: Orders persistence and backoffice UI for bda.plone.shop
 Author: BlueDynamics Alliance
 Author-email: dev@bluedynamics.com
 License: GNU General Public Licence
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Addon
@@ -502,14 +502,21 @@
 
 
 Icons used are `Silk-Icons by FamFamFam <http://www.famfamfam.com/lab/icons/silk/>`_
 under CC-BY 2.5 license.
 Changelog
 =========
 
+2.0b2 (2024-04-17)
+------------------
+
+- Add missing compiled resources.
+  [petschki]
+
+
 2.0b1 (2024-04-17)
 ------------------
 
 - Introduce base class to allow more flexible subclassing for export.
   [jensens]
 
 - Use csv23 for py2/3 csv export.
```

### Comparing `bda.plone.orders-2.0b1/src/bda.plone.orders.egg-info/SOURCES.txt` & `bda.plone.orders-2.0b2/src/bda.plone.orders.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 src/bda/plone/orders/browser/resources/invoices.png
 src/bda/plone/orders/browser/resources/jquery-barcode.js
 src/bda/plone/orders/browser/resources/notify_customers.png
 src/bda/plone/orders/browser/resources/order.png
 src/bda/plone/orders/browser/resources/orders.css
 src/bda/plone/orders/browser/resources/orders.css.map
 src/bda/plone/orders/browser/resources/orders.js
+src/bda/plone/orders/browser/resources/orders.min.css
 src/bda/plone/orders/browser/resources/orders.png
 src/bda/plone/orders/browser/resources/pencil.png
 src/bda/plone/orders/browser/resources/print.png
 src/bda/plone/orders/browser/resources/qrcode.js
 src/bda/plone/orders/browser/resources/spinner.gif
 src/bda/plone/orders/browser/resources/tick.png
 src/bda/plone/orders/browser/templates/bookings.pt
```

