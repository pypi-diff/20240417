# Comparing `tmp/m9s_position_numbers-7.0.0.tar.gz` & `tmp/m9s_position_numbers-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_position_numbers-7.0.0.tar", last modified: Tue Feb 13 16:44:22 2024, max compression
+gzip compressed data, was "m9s_position_numbers-7.0.1.tar", last modified: Wed Apr 17 17:41:53 2024, max compression
```

## Comparing `m9s_position_numbers-7.0.0.tar` & `m9s_position_numbers-7.0.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-13 16:44:22.632539 m9s_position_numbers-7.0.0/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       86 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1892 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/.isort.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-13 16:44:22.632539 m9s_position_numbers-7.0.0/.woodpecker/
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      680 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3441 2024-02-13 16:44:22.632539 m9s_position_numbers-7.0.0/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1259 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       48 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      799 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1003 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/common.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-13 16:44:22.632539 m9s_position_numbers-7.0.0/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-13 16:44:22.632539 m9s_position_numbers-7.0.0/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       47 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       48 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/doc/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      907 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/invoice.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1079 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/invoice.xml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-13 16:44:22.628539 m9s_position_numbers-7.0.0/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1001 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/locale/de.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-13 16:44:22.632539 m9s_position_numbers-7.0.0/m9s_position_numbers.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3441 2024-02-13 16:44:22.000000 m9s_position_numbers-7.0.0/m9s_position_numbers.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1593 2024-02-13 16:44:22.000000 m9s_position_numbers-7.0.0/m9s_position_numbers.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-02-13 16:44:22.000000 m9s_position_numbers-7.0.0/m9s_position_numbers.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       70 2024-02-13 16:44:22.000000 m9s_position_numbers-7.0.0/m9s_position_numbers.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-02-13 16:44:22.000000 m9s_position_numbers-7.0.0/m9s_position_numbers.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       98 2024-02-13 16:44:22.000000 m9s_position_numbers-7.0.0/m9s_position_numbers.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-02-13 16:44:22.000000 m9s_position_numbers-7.0.0/m9s_position_numbers.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1069 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/purchase.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1039 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/purchase.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      261 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/sale.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      725 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/sale.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-02-13 16:44:22.632539 m9s_position_numbers-7.0.0/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4541 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-13 16:44:22.632539 m9s_position_numbers-7.0.0/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6080 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/tests/scenario_position_numbers.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      305 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/tests/test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      798 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/tests/test_position_numbers.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      266 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/tests/test_scenario.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      147 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/tryton.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-13 16:44:22.632539 m9s_position_numbers-7.0.0/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      317 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/view/invoice_line_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      264 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/view/invoice_line_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      264 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/view/invoice_line_tree_sequence.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      317 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/view/purchase_line_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      264 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/view/purchase_line_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      264 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/view/purchase_line_tree_sequence.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      264 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/view/sale_line_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      264 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.0/view/sale_line_tree_sequence.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-17 17:41:53.750010 m9s_position_numbers-7.0.1/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       86 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1892 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/.isort.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-17 17:41:53.746010 m9s_position_numbers-7.0.1/.woodpecker/
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      680 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3441 2024-04-17 17:41:53.750010 m9s_position_numbers-7.0.1/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1259 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       48 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      799 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1026 2024-02-14 09:53:36.000000 m9s_position_numbers-7.0.1/common.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-17 17:41:53.746010 m9s_position_numbers-7.0.1/doc/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-17 17:41:53.746010 m9s_position_numbers-7.0.1/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       47 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       48 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/doc/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      907 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/invoice.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1079 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/invoice.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-17 17:41:53.746010 m9s_position_numbers-7.0.1/locale/
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     1005 2024-04-17 15:04:45.000000 m9s_position_numbers-7.0.1/locale/de.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-17 17:41:53.750010 m9s_position_numbers-7.0.1/m9s_position_numbers.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3441 2024-04-17 17:41:53.000000 m9s_position_numbers-7.0.1/m9s_position_numbers.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1587 2024-04-17 17:41:53.000000 m9s_position_numbers-7.0.1/m9s_position_numbers.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-04-17 17:41:53.000000 m9s_position_numbers-7.0.1/m9s_position_numbers.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       70 2024-04-17 17:41:53.000000 m9s_position_numbers-7.0.1/m9s_position_numbers.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-02-13 16:44:22.000000 m9s_position_numbers-7.0.1/m9s_position_numbers.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      132 2024-04-17 17:41:53.000000 m9s_position_numbers-7.0.1/m9s_position_numbers.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-04-17 17:41:53.000000 m9s_position_numbers-7.0.1/m9s_position_numbers.egg-info/top_level.txt
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     1079 2024-04-17 15:04:45.000000 m9s_position_numbers-7.0.1/purchase.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1039 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/purchase.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      261 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/sale.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      725 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/sale.xml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-04-17 17:41:53.750010 m9s_position_numbers-7.0.1/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4593 2024-02-13 18:01:14.000000 m9s_position_numbers-7.0.1/setup.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-17 17:41:53.746010 m9s_position_numbers-7.0.1/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/tests/__init__.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     7141 2024-04-17 16:31:28.000000 m9s_position_numbers-7.0.1/tests/scenario_position_numbers.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    19230 2024-04-17 15:36:22.000000 m9s_position_numbers-7.0.1/tests/scenario_purchase.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      358 2024-02-13 18:00:28.000000 m9s_position_numbers-7.0.1/tests/test_module.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      266 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/tests/test_scenario.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/tox.ini
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      147 2024-02-13 16:44:28.000000 m9s_position_numbers-7.0.1/tryton.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-17 17:41:53.746010 m9s_position_numbers-7.0.1/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      317 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/view/invoice_line_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      264 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/view/invoice_line_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      264 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/view/invoice_line_tree_sequence.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      317 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/view/purchase_line_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      264 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/view/purchase_line_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      264 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/view/purchase_line_tree_sequence.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      264 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/view/sale_line_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      264 2024-02-13 16:28:08.000000 m9s_position_numbers-7.0.1/view/sale_line_tree_sequence.xml
```

### Comparing `m9s_position_numbers-7.0.0/.gitlab-ci.yml` & `m9s_position_numbers-7.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `m9s_position_numbers-7.0.0/.woodpecker/mail_curl.sh` & `m9s_position_numbers-7.0.1/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_position_numbers-7.0.0/.woodpecker/report.yml` & `m9s_position_numbers-7.0.1/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_position_numbers-7.0.0/.woodpecker/test.yml` & `m9s_position_numbers-7.0.1/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_position_numbers-7.0.0/COPYRIGHT` & `m9s_position_numbers-7.0.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_position_numbers-7.0.0/INSTALL` & `m9s_position_numbers-7.0.1/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_position_numbers-7.0.0/LICENSE` & `m9s_position_numbers-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_position_numbers-7.0.0/PKG-INFO` & `m9s_position_numbers-7.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_position_numbers
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton Position Numbers Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/position_numbers.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_position_numbers-7.0.0/README.md` & `m9s_position_numbers-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `m9s_position_numbers-7.0.0/__init__.py` & `m9s_position_numbers-7.0.1/__init__.py`

 * *Files identical despite different names*

### Comparing `m9s_position_numbers-7.0.0/common.py` & `m9s_position_numbers-7.0.1/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # The COPYRIGHT file at the top level of this repository contains
 # the full copyright notices and license terms.
 from trytond.model import ModelStorage, ModelView, fields
 
 
 def line_mixin(prefix):
     class LineMixin(ModelStorage, ModelView):
+        __slots__ = ()
 
         _numbered_types = ('line')
 
         item_number = fields.Function(fields.Char('Item number'),
             'get_item_number')
 
         @classmethod
```

### Comparing `m9s_position_numbers-7.0.0/invoice.py` & `m9s_position_numbers-7.0.1/invoice.py`

 * *Files identical despite different names*

### Comparing `m9s_position_numbers-7.0.0/invoice.xml` & `m9s_position_numbers-7.0.1/invoice.xml`

 * *Files identical despite different names*

### Comparing `m9s_position_numbers-7.0.0/locale/de.po` & `m9s_position_numbers-7.0.1/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.invoice.line,custom_item_number:"
 msgid "Custom item number"
-msgstr "Spezifische Position"
+msgstr "Eigene Positionsnummer"
 
 msgctxt "field:account.invoice.line,item_number:"
 msgid "Item number"
 msgstr "Position"
 
 msgctxt "field:purchase.line,custom_item_number:"
 msgid "Custom item number"
-msgstr "Spezifische Position"
+msgstr "Eigene Positionsnummer"
 
 msgctxt "field:purchase.line,item_number:"
 msgid "Item number"
 msgstr "Position"
 
 msgctxt "field:sale.line,item_number:"
 msgid "Item number"
```

### Comparing `m9s_position_numbers-7.0.0/m9s_position_numbers.egg-info/PKG-INFO` & `m9s_position_numbers-7.0.1/m9s_position_numbers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-position-numbers
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton Position Numbers Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/position_numbers.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_position_numbers-7.0.0/m9s_position_numbers.egg-info/SOURCES.txt` & `m9s_position_numbers-7.0.1/m9s_position_numbers.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 ./purchase.xml
 ./sale.py
 ./sale.xml
 ./tryton.cfg
 ./locale/de.po
 ./tests/__init__.py
 ./tests/scenario_position_numbers.rst
+./tests/scenario_purchase.rst
 ./tests/test_module.py
-./tests/test_position_numbers.py
 ./tests/test_scenario.py
 ./view/invoice_line_form.xml
 ./view/invoice_line_tree.xml
 ./view/invoice_line_tree_sequence.xml
 ./view/purchase_line_form.xml
 ./view/purchase_line_tree.xml
 ./view/purchase_line_tree_sequence.xml
@@ -56,16 +56,16 @@
 m9s_position_numbers.egg-info/dependency_links.txt
 m9s_position_numbers.egg-info/entry_points.txt
 m9s_position_numbers.egg-info/not-zip-safe
 m9s_position_numbers.egg-info/requires.txt
 m9s_position_numbers.egg-info/top_level.txt
 tests/__init__.py
 tests/scenario_position_numbers.rst
+tests/scenario_purchase.rst
 tests/test_module.py
-tests/test_position_numbers.py
 tests/test_scenario.py
 view/invoice_line_form.xml
 view/invoice_line_tree.xml
 view/invoice_line_tree_sequence.xml
 view/purchase_line_form.xml
 view/purchase_line_tree.xml
 view/purchase_line_tree_sequence.xml
```

### Comparing `m9s_position_numbers-7.0.0/purchase.py` & `m9s_position_numbers-7.0.1/purchase.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,11 +23,12 @@
 
         for line in lines:
             if line.custom_item_number:
                 numbers[line.id] = '%s *' % line.custom_item_number
         return numbers
 
     def get_invoice_line(self):
-        invoice_line, = super().get_invoice_line()
-        if self.custom_item_number:
-            invoice_line.custom_item_number = self.custom_item_number
-        return [invoice_line]
+        lines = super().get_invoice_line()
+        for line in lines:
+            if self.custom_item_number:
+                line.custom_item_number = self.custom_item_number
+        return lines
```

### Comparing `m9s_position_numbers-7.0.0/purchase.xml` & `m9s_position_numbers-7.0.1/purchase.xml`

 * *Files identical despite different names*

### Comparing `m9s_position_numbers-7.0.0/sale.xml` & `m9s_position_numbers-7.0.1/sale.xml`

 * *Files identical despite different names*

### Comparing `m9s_position_numbers-7.0.0/setup.py` & `m9s_position_numbers-7.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     if not re.match(r'(ir|res)(\W|$)', dep):
         prefix = MODULE2PREFIX.get(dep, 'trytond')
         requires.append(get_require_version('%s_%s' % (prefix, dep)))
 requires.append(get_require_version('m9s-trytond'))
 
 tests_require = [
     get_require_version('proteus'),
+    get_require_version('trytond_account_invoice'),
     get_require_version('trytond_sale'),
     get_require_version('trytond_purchase'),
     ]
 
 setup(name=name,
     version=version,
     description='Tryton Position Numbers Module',
```

### Comparing `m9s_position_numbers-7.0.0/tests/scenario_position_numbers.rst` & `m9s_position_numbers-7.0.1/tests/scenario_position_numbers.rst`

 * *Files 14% similar despite different names*

```diff
@@ -142,29 +142,33 @@
     >>> Purchase = Model.get('purchase.purchase')
     >>> purchase = Purchase()
     >>> purchase.party = party
     >>> purchase.payment_term = payment_term
     >>> purchase_line1 = purchase.lines.new()
     >>> purchase_line1.product = product
     >>> purchase_line1.quantity = 1.0
+    >>> purchase_line1.unit_price = Decimal('5.0000')
     >>> purchase_title = purchase.lines.new()
     >>> purchase_title.type = 'title'
     >>> purchase_line2 = purchase.lines.new()
     >>> purchase_line2.product = product
     >>> purchase_line2.quantity = 1.0
+    >>> purchase_line2.unit_price = Decimal('5.0000')
     >>> purchase_comment = purchase.lines.new()
     >>> purchase_comment.type = 'comment'
     >>> purchase_subtotal = purchase.lines.new()
     >>> purchase_subtotal.type = 'subtotal'
     >>> purchase_line3 = purchase.lines.new()
     >>> purchase_line3.product = product
     >>> purchase_line3.quantity = 1.0
+    >>> purchase_line3.unit_price = Decimal('15.0000')
     >>> purchase_line4 = purchase.lines.new()
     >>> purchase_line4.product = product
     >>> purchase_line4.quantity = 1.0
+    >>> purchase_line4.unit_price = Decimal('25.0000')
     >>> purchase_line4.custom_item_number = '100'
     >>> purchase.save()
     >>> purchase.reload()
     >>> purchase.lines[0].item_number
     '1'
     >>> purchase.lines[1].item_number
     >>> purchase.lines[2].item_number
@@ -172,25 +176,50 @@
     >>> purchase.lines[3].item_number
     >>> purchase.lines[4].item_number
     >>> purchase.lines[5].item_number
     '3'
     >>> purchase.lines[6].item_number
     '100 *'
 
-Check if the invoice has the same item numbers::
+Check if the invoice has the correct item numbers (only type 'line' is copied to invoice)::
 
     >>> purchase.click('quote')
     >>> purchase.click('confirm')
     >>> purchase.reload()
     >>> invoice, = purchase.invoices
     >>> invoice.lines[0].item_number
     '1'
     >>> invoice.lines[1].item_number
+    '2'
+    >>> invoice.lines[2].item_number
+    '3'
+    >>> invoice.lines[3].item_number
+    '100 *'
+    
+Check for the correct behavior with non-line types::
+    
+    >>> invoice.lines[0].sequence = 1
+    >>> invoice.lines[1].sequence = 10
+    >>> invoice.lines[2].sequence = 20
+    >>> invoice.lines[3].sequence = 30
+    >>> invoice_line4 = invoice.lines.new()
+    >>> invoice_line4.type = 'subtotal'
+    >>> invoice_line4.sequence = 5
+    >>> invoice_line5 = invoice.lines.new()
+    >>> invoice_line5.type = 'title'
+    >>> invoice_line5.sequence = 15
+    >>> invoice_line6 = invoice.lines.new()
+    >>> invoice_line6.type = 'comment'
+    >>> invoice_line6.sequence = 25
+    >>> invoice.save()
+    >>> invoice.reload()
+    >>> invoice.lines[0].item_number
+    '1'
+    >>> invoice.lines[1].item_number
     >>> invoice.lines[2].item_number
     '2'
     >>> invoice.lines[3].item_number
     >>> invoice.lines[4].item_number
-    >>> invoice.lines[5].item_number
     '3'
+    >>> invoice.lines[5].item_number
     >>> invoice.lines[6].item_number
     '100 *'
-
```

### Comparing `m9s_position_numbers-7.0.0/tox.ini` & `m9s_position_numbers-7.0.1/tox.ini`

 * *Files identical despite different names*

