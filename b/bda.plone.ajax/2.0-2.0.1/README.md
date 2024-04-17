# Comparing `tmp/bda.plone.ajax-2.0.tar.gz` & `tmp/bda.plone.ajax-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bda.plone.ajax-2.0.tar", last modified: Sun Mar 10 22:06:57 2019, max compression
+gzip compressed data, was "bda.plone.ajax-2.0.1.tar", last modified: Wed Apr 17 14:17:00 2024, max compression
```

## Comparing `bda.plone.ajax-2.0.tar` & `bda.plone.ajax-2.0.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       38 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/setup.cfg
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    21497 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/PKG-INFO
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1700 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/setup.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      954 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/buildout.cfg
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    12083 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/README.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       87 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/MANIFEST.in
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1504 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/LICENSE.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2064 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/CHANGES.rst
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda.plone.ajax.egg-info/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        4 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda.plone.ajax.egg-info/top_level.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       47 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda.plone.ajax.egg-info/requires.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda.plone.ajax.egg-info/not-zip-safe
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       14 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda.plone.ajax.egg-info/namespace_packages.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       53 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda.plone.ajax.egg-info/entry_points.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda.plone.ajax.egg-info/dependency_links.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1838 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda.plone.ajax.egg-info/SOURCES.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    21497 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda.plone.ajax.egg-info/PKG-INFO
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       56 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/__init__.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       56 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/__init__.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      213 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/utils.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      343 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/setuphandlers.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      875 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/profile.zcml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      143 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/interfaces.py
--rwxrwxr-x   0 jensens   (1000) jensens   (1000)     2200 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/i18n.sh
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      607 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/form.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1283 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/configure.zcml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       49 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/bda.ajax.pt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     4315 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/batch.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     4648 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/batch.pt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2422 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/action.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     8940 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/__init__.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/resources/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    10364 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/resources/jquerytools-custom.js
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/profile/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/profile/uninstall/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      435 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/profile/uninstall/registry.xml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      150 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/profile/uninstall/browserlayer.xml
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/profile/default/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      972 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/profile/default/registry.xml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      102 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/profile/default/metadata.xml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      132 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/profile/default/browserlayer.xml
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/locales/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      855 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/locales/bda.plone.ajax.pot
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/locales/en/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/locales/en/LC_MESSAGES/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      756 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/locales/en/LC_MESSAGES/bda.plone.ajax.po
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/locales/de/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/locales/de/LC_MESSAGES/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      762 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/locales/de/LC_MESSAGES/bda.plone.ajax.po
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      580 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/tile_b.pt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      432 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/tile_a.pt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1005 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/provider.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      545 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/ploneview.pt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1380 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/examplebatch.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1986 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/configure.zcml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      553 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/batchview.pt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      676 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/batchedresult.pt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      730 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/ajaxoverlayformview.pt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      543 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/ajaxformview.pt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1376 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/ajaxform.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      581 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/ajaxform.pt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2019-03-10 22:06:57.000000 bda.plone.ajax-2.0/src/bda/plone/ajax/examples/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.444669 bda.plone.ajax-2.0.1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2285 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1504 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       87 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    16785 2024-04-17 14:17:00.444669 bda.plone.ajax-2.0.1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11957 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      954 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/buildout.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2024-04-17 14:17:00.444669 bda.plone.ajax-2.0.1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1702 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.440669 bda.plone.ajax-2.0.1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.440669 bda.plone.ajax-2.0.1/src/bda/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.440669 bda.plone.ajax-2.0.1/src/bda/plone/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.440669 bda.plone.ajax-2.0.1/src/bda/plone/ajax/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8940 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2422 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/action.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4725 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/batch.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4315 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/batch.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       49 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/bda.ajax.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1283 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/configure.zcml
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.444669 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      581 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/ajaxform.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1376 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/ajaxform.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      543 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/ajaxformview.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      730 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/ajaxoverlayformview.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      676 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/batchedresult.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      553 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/batchview.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1986 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/configure.zcml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1380 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/examplebatch.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      545 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/ploneview.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1005 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/provider.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      432 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/tile_a.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      580 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/tile_b.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      607 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/form.py
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)     2201 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/i18n.sh
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      143 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/interfaces.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.444669 bda.plone.ajax-2.0.1/src/bda/plone/ajax/locales/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      855 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/locales/bda.plone.ajax.pot
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.440669 bda.plone.ajax-2.0.1/src/bda/plone/ajax/locales/de/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.444669 bda.plone.ajax-2.0.1/src/bda/plone/ajax/locales/de/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      762 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/locales/de/LC_MESSAGES/bda.plone.ajax.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.440669 bda.plone.ajax-2.0.1/src/bda/plone/ajax/locales/en/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.444669 bda.plone.ajax-2.0.1/src/bda/plone/ajax/locales/en/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      756 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/locales/en/LC_MESSAGES/bda.plone.ajax.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.440669 bda.plone.ajax-2.0.1/src/bda/plone/ajax/profile/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.444669 bda.plone.ajax-2.0.1/src/bda/plone/ajax/profile/default/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      132 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/profile/default/browserlayer.xml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      106 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/profile/default/metadata.xml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      976 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/profile/default/registry.xml
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.444669 bda.plone.ajax-2.0.1/src/bda/plone/ajax/profile/uninstall/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      150 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/profile/uninstall/browserlayer.xml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      435 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/profile/uninstall/registry.xml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1120 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/profile.zcml
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.444669 bda.plone.ajax-2.0.1/src/bda/plone/ajax/resources/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10364 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/resources/jquerytools-custom.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      343 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/setuphandlers.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      213 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda/plone/ajax/utils.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-04-17 14:17:00.444669 bda.plone.ajax-2.0.1/src/bda.plone.ajax.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    16785 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda.plone.ajax.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1848 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda.plone.ajax.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda.plone.ajax.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       40 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda.plone.ajax.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       14 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda.plone.ajax.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda.plone.ajax.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       47 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda.plone.ajax.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        4 2024-04-17 14:17:00.000000 bda.plone.ajax-2.0.1/src/bda.plone.ajax.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bda.plone.ajax-2.0/setup.py` & `bda.plone.ajax-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 import os
 
 
-version = '2.0'
+version = '2.0.1'
 shortdesc = "bdajax integration for Plone."
 longdesc = open(os.path.join(os.path.dirname(__file__), 'README.rst')).read()
 longdesc += open(os.path.join(os.path.dirname(__file__), 'CHANGES.rst')).read()
 longdesc += open(os.path.join(os.path.dirname(__file__), 'LICENSE.rst')).read()
 
 
 setup(
```

### Comparing `bda.plone.ajax-2.0/buildout.cfg` & `bda.plone.ajax-2.0.1/buildout.cfg`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/README.rst` & `bda.plone.ajax-2.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 Integration package
 ===================
 
 This is the plone integration package for
-`bdajax <http://github.com/bluedynamics/bdajax/>`_.
+`bdajax <https://github.com/bluedynamics/bdajax/>`_.
 
 
 Installation
 ============
 
 - Make egg available in your instance.
 - Apply extension profile.
 
 
-Usage
-=====
-
-For detailed documentation about ``bdajax`` please refer to
-`bdajax <http://github.com/bluedynamics/bdajax/>`_.
-
-
 Implement ajax action as browser view
 -------------------------------------
 
 An ajax action can be implemented as simple browser view. The easiest way is to
 render a template only. Create template ``tile_a.pt``:
 
 .. code-block:: xml
@@ -434,17 +427,17 @@
 
 
 Source Code
 ===========
 
 If you want to help with the development (improvement, update, bug-fixing, ...) of ``bda.plone.ajax`` this is a great idea!
 
-The code is located in the `github collective <http://github.com/collective/bda.plone.ajax>`_.
+The code is located in the `github collective <https://github.com/collective/bda.plone.ajax>`_.
 
-You can clone it or `get access to the github-collective <http://collective.github.com/>`_ and work directly on the project.
+You can clone it or `get access to the github-collective <https://collective.github.io>`_ and work directly on the project.
 
 Maintainers are Robert Niederreiter and the BlueDynamics Alliance developer team.
 We appreciate any contribution and if a release is needed to be done on pypi, please just contact one of us:
 `dev@bluedynamics dot com <mailto:dev@bluedynamics.com>`_
 
 
 Contributors
```

### Comparing `bda.plone.ajax-2.0/LICENSE.rst` & `bda.plone.ajax-2.0.1/LICENSE.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 License
 =======
 
-Copyright (c) 2010-2019, BlueDynamics Alliance, Austria
+Copyright (c) 2010-2024, BlueDynamics Alliance, Austria
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `bda.plone.ajax-2.0/CHANGES.rst` & `bda.plone.ajax-2.0.1/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 Changes
 =======
 
+2.0.1 (2024-04-17)
+------------------
+
+- Use Python expressions instead of TALES in ``batch.pt``.
+  [jensens]
+
+- Update ``condition`` for jQuery overlay resources and adjust ``depends`` for
+  bdajax resources.
+  [petschki]
+
+
 2.0 (2019-03-10)
 ----------------
 
-- Drop Plone 4 support (Needs 5.1+). 
+- Drop Plone 4 support (Needs 5.1+).
   [agitator]
-  
+
 - Add Python 3 support.
   [agitator]
-  
+
 - Minimal custom jquerytools with overlay added, no more dependency on ``plone.app.jquerytools``.
   [agitator]
 
 
 1.8 (2019-02-08)
 ----------------
 
@@ -122,7 +133,8 @@
 
 
 1.0
 ---
 
 - make it work.
   [rnix]
+
```

### Comparing `bda.plone.ajax-2.0/src/bda.plone.ajax.egg-info/SOURCES.txt` & `bda.plone.ajax-2.0.1/src/bda.plone.ajax.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CHANGES.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
 buildout.cfg
+setup.cfg
 setup.py
 src/bda/__init__.py
 src/bda.plone.ajax.egg-info/PKG-INFO
 src/bda.plone.ajax.egg-info/SOURCES.txt
 src/bda.plone.ajax.egg-info/dependency_links.txt
 src/bda.plone.ajax.egg-info/entry_points.txt
 src/bda.plone.ajax.egg-info/namespace_packages.txt
```

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/profile.zcml` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/profile.zcml`

 * *Files 10% similar despite different names*

```diff
@@ -18,8 +18,18 @@
     directory="profiles/uninstall"
     description="Uninstalls the bda.plone.ajax."
     provides="Products.GenericSetup.interfaces.EXTENSION" />
 
   <!-- Hide profiles/products from Quick Installer -->
   <utility factory=".setuphandlers.HiddenProfiles" name="bda.plone.ajax" />
 
+  <!-- upgradeSteps -->
+  <genericsetup:upgradeDepends
+      title="Reload Resourceregistry"
+      description=""
+      profile="bda.plone.ajax:default"
+      source="*"
+      destination="3001"
+      import_steps="plone.app.registry"
+      />
+
 </configure>
```

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/i18n.sh` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/i18n.sh`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 # Assume i18ndude is installed with buildout
 # and this script is run under src/ folder with two nested namespaces in the package name (like collective.bla)
 I18NDUDE=../../../../../../bin/i18ndude
 
 if test ! -e $I18NDUDE; then
         echo "You must install i18ndude with buildout"
-        echo "See http://svn.plone.org/svn/collective/collective.developermanual/trunk/source/i18n/localization.txt"
+        echo "See https://svn.plone.org/svn/collective/collective.developermanual/trunk/source/i18n/localization.txt"
         exit
 fi
 
 #
 # Do we need to merge manual PO entries from a file called manual.pot.
 # this option is later passed to i18ndude
 #
```

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/form.py` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/form.py`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/configure.zcml` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/configure.zcml`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/batch.py` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/batch.py`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/batch.pt` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/batch.pt`

 * *Files 5% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 <div xmlns:tal="http://xml.zope.org/namespaces/tal"
      xmlns:ajax="http://namesspaces.bluedynamics.eu/ajax"
      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
      i18n:domain="bda.plone.ajax"
      tal:omit-tag="">
 
-  <div tal:condition="view/display"
+  <div tal:condition="python:view.display"
        class="batch">
 
     <tal:fistpage
-        define="firstpage view/firstpage;
+        define="firstpage python:view.firstpage;
                 invisible python:not firstpage['visible'] or firstpage['current'];
                 css string:page;
                 css python:invisible and css + ' invisible' or css"
         condition="firstpage">
 
       <a href="#"
          ajax:bind="click"
          ajax:target=""
          ajax:event=""
          tal:condition="not:invisible"
          tal:attributes="href firstpage/url;
                          class css;
                          ajax:target firstpage/url;
-                         ajax:event string:batchclicked:.${view/batchname}sensitiv;"
+                         ajax:event string:batchclicked:.${python:view.batchname}sensitiv;"
          i18n:translate="first">First</a>
 
       <a href="javascript:void(0)"
          tal:condition="invisible"
          tal:attributes="class css"
          i18n:translate="first">First</a>
 
     </tal:fistpage>
 
     <tal:prevpage
-        define="prevpage view/prevpage;
+        define="prevpage python:view.prevpage;
                 invisible python:not prevpage['visible'] or prevpage['current'];
                 css string:page;
                 css python:invisible and css + ' invisible' or css"
         condition="prevpage">
 
       <a href="#"
          ajax:bind="click"
          ajax:target=""
          ajax:event=""
          tal:condition="not:invisible"
          tal:attributes="href prevpage/url;
                          class css;
                          ajax:target prevpage/url;
-                         ajax:event string:batchclicked:.${view/batchname}sensitiv"
+                         ajax:event string:batchclicked:.${python:view.batchname}sensitiv"
          i18n:translate="previous">Previous</a>
 
       <a href="javascript:void(0)"
          tal:condition="invisible"
          tal:attributes="class css"
          i18n:translate="previous">Previous</a>
 
     </tal:prevpage>
 
     <span>
 
-      <tal:pages repeat="page view/pages">
+      <tal:pages repeat="page python:view.pages">
         <tal:page
             define="invisible not:page/visible;
                     current page/current;
                     css string:page;
                     css python:invisible and css + ' invisible' or css;
                     css python:current and css + ' current' or css">
 
@@ -71,68 +71,68 @@
              ajax:bind="click"
              ajax:target=""
              ajax:event=""
              tal:condition="python:not invisible and not current"
              tal:attributes="href page/url;
                              class css;
                              ajax:target page/url;
-                             ajax:event string:batchclicked:.${view/batchname}sensitiv"
+                             ajax:event string:batchclicked:.${python:view.batchname}sensitiv"
              tal:content="page/page">X</a>
 
            <a href="javascript:void(0)"
               tal:condition="python:invisible or current"
               tal:attributes="class css"
               tal:content="page/page">X</a>
 
         </tal:page>
       </tal:pages>
 
     </span>
 
     <tal:nextpage
-        define="nextpage view/nextpage;
+        define="nextpage python:view.nextpage;
                 invisible python:not nextpage['visible'] or nextpage['current'];
                 css string:page;
                 css python:invisible and css + ' invisible' or css"
         condition="nextpage">
 
       <a href="#"
          ajax:bind="click"
          ajax:target=""
          ajax:event=""
          tal:condition="not:invisible"
          tal:attributes="href nextpage/url;
                          class css;
                          ajax:target nextpage/url;
-                         ajax:event string:batchclicked:.${view/batchname}sensitiv"
+                         ajax:event string:batchclicked:.${python:view.batchname}sensitiv"
          i18n:translate="next">Next</a>
 
       <a href="javascript:void(0)"
          tal:condition="invisible"
          tal:attributes="class css"
          i18n:translate="next">Next</a>
 
     </tal:nextpage>
 
     <tal:lastpage
-        define="lastpage view/lastpage;
+        define="lastpage python:view.lastpage;
                 invisible python:not lastpage['visible'] or lastpage['current'];
                 css string:page;
                 css python:invisible and css + ' invisible' or css"
         condition="lastpage">
 
       <a href="#"
          ajax:bind="click"
          ajax:target=""
          ajax:event=""
          tal:condition="not:invisible"
          tal:attributes="href lastpage/url;
                          class css;
                          ajax:target lastpage/url;
-                         ajax:event string:batchclicked:.${view/batchname}sensitiv"
+                         ajax:event string:batchclicked:.${python:view.batchname}sensitiv"
          i18n:translate="last">Last</a>
 
       <a href="javascript:void(0)"
          tal:condition="invisible"
          tal:attributes="class css"
          i18n:translate="last">Last</a>
```

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/action.py` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/action.py`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/__init__.py` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/__init__.py`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/resources/jquerytools-custom.js` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/resources/jquerytools-custom.js`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/profile/default/registry.xml` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/profile/default/registry.xml`

 * *Files 4% similar despite different names*

#### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/profile/default/registry.xml` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/profile/default/registry.xml`

```diff
@@ -2,17 +2,17 @@
 <registry xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="bda.plone.ajax">
   <!-- minimal custom jquerytools with overlay -->
   <records prefix="plone.bundles/plonebdajax-jquerytools-overlay" interface="Products.CMFPlone.interfaces.IBundleRegistry">
     <value key="enabled">True</value>
     <value key="jscompilation">++resource++plonebdajax/jquerytools-custom.js</value>
     <value key="compile">False</value>
     <value key="depends">plone</value>
-    <value key="expression">python: member is None</value>
+    <value key="expression"/>
   </records>
   <records prefix="plone.bundles/bdajax" interface="Products.CMFPlone.interfaces.IBundleRegistry">
     <value key="enabled">True</value>
     <value key="jscompilation">++resource++bdajax/bdajax.js</value>
     <value key="csscompilation">++resource++bdajax/bdajax.css</value>
     <value key="compile">False</value>
-    <value key="depends">plone</value>
+    <value key="depends">plonebdajax-jquerytools-overlay</value>
   </records>
 </registry>
```

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/locales/bda.plone.ajax.pot` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/locales/bda.plone.ajax.pot`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/locales/en/LC_MESSAGES/bda.plone.ajax.po` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/locales/en/LC_MESSAGES/bda.plone.ajax.po`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/locales/de/LC_MESSAGES/bda.plone.ajax.po` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/locales/de/LC_MESSAGES/bda.plone.ajax.po`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/examples/tile_b.pt` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/tile_b.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/examples/provider.py` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/provider.py`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/examples/ploneview.pt` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/ploneview.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/examples/examplebatch.py` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/examplebatch.py`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/examples/configure.zcml` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/configure.zcml`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/examples/batchview.pt` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/batchview.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/examples/batchedresult.pt` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/batchedresult.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/examples/ajaxoverlayformview.pt` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/ajaxoverlayformview.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/examples/ajaxformview.pt` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/ajaxformview.pt`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/examples/ajaxform.py` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/ajaxform.py`

 * *Files identical despite different names*

### Comparing `bda.plone.ajax-2.0/src/bda/plone/ajax/examples/ajaxform.pt` & `bda.plone.ajax-2.0.1/src/bda/plone/ajax/examples/ajaxform.pt`

 * *Files identical despite different names*

