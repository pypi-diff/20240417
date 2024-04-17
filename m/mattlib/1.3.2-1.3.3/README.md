# Comparing `tmp/mattlib-1.3.2.tar.gz` & `tmp/mattlib-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mattlib-1.3.2.tar", last modified: Thu Feb  8 13:33:09 2024, max compression
+gzip compressed data, was "mattlib-1.3.3.tar", last modified: Tue Apr 16 18:39:42 2024, max compression
```

## Comparing `mattlib-1.3.2.tar` & `mattlib-1.3.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.973608 mattlib-1.3.2/
--rw-r--r--   0 livia     (1000) livia     (1000)    35149 2023-10-23 23:40:32.000000 mattlib-1.3.2/COPYING
--rw-r--r--   0 livia     (1000) livia     (1000)      840 2024-02-08 13:33:09.973608 mattlib-1.3.2/PKG-INFO
--rw-r--r--   0 livia     (1000) livia     (1000)      147 2023-10-23 23:40:32.000000 mattlib-1.3.2/README.md
--rw-r--r--   0 livia     (1000) livia     (1000)      104 2023-10-23 23:40:32.000000 mattlib-1.3.2/pyproject.toml
--rw-r--r--   0 livia     (1000) livia     (1000)      839 2024-02-08 13:33:09.973608 mattlib-1.3.2/setup.cfg
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.833608 mattlib-1.3.2/src/
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.873608 mattlib-1.3.2/src/mattlib/
--rw-r--r--   0 livia     (1000) livia     (1000)      951 2024-02-08 13:31:56.000000 mattlib-1.3.2/src/mattlib/API_factory.py
--rw-r--r--   0 livia     (1000) livia     (1000)     3413 2024-02-08 13:28:02.000000 mattlib-1.3.2/src/mattlib/BaseAPI.py
--rw-r--r--   0 livia     (1000) livia     (1000)      235 2023-11-22 10:34:26.000000 mattlib-1.3.2/src/mattlib/__init__.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.893608 mattlib-1.3.2/src/mattlib/adobe/
--rw-r--r--   0 livia     (1000) livia     (1000)     3332 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/adobe/AdobeAPI.py
--rw-r--r--   0 livia     (1000) livia     (1000)       30 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/adobe/__init__.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.903608 mattlib-1.3.2/src/mattlib/apis/
--rw-r--r--   0 livia     (1000) livia     (1000)    10010 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/apis/AzureAPI.py
--rw-r--r--   0 livia     (1000) livia     (1000)     1917 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/apis/GraphAPI.py
--rw-r--r--   0 livia     (1000) livia     (1000)     4355 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/apis/SalesForceAPI.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.913608 mattlib-1.3.2/src/mattlib/clockify/
--rw-r--r--   0 livia     (1000) livia     (1000)      751 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/clockify/ClockifyAPI.py
--rw-r--r--   0 livia     (1000) livia     (1000)       26 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/clockify/__init__.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.913608 mattlib-1.3.2/src/mattlib/docusign/
--rw-r--r--   0 livia     (1000) livia     (1000)     1832 2023-10-24 04:38:34.000000 mattlib-1.3.2/src/mattlib/docusign/DocusignAPI.py
--rw-r--r--   0 livia     (1000) livia     (1000)       37 2023-10-24 01:02:05.000000 mattlib-1.3.2/src/mattlib/docusign/__init__.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.923608 mattlib-1.3.2/src/mattlib/fourmatters/
--rw-r--r--   0 livia     (1000) livia     (1000)     8016 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/fourmatters/virtual_machine.py
--rw-r--r--   0 livia     (1000) livia     (1000)     2964 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/fourmatters/virtual_network.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.923608 mattlib-1.3.2/src/mattlib/gcp/
--rw-r--r--   0 livia     (1000) livia     (1000)      484 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/gcp/PubSub.py
--rw-r--r--   0 livia     (1000) livia     (1000)       21 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/gcp/__init__.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.933608 mattlib-1.3.2/src/mattlib/google/
--rw-r--r--   0 livia     (1000) livia     (1000)     1116 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/google/BaseGoogleAPI.py
--rw-r--r--   0 livia     (1000) livia     (1000)     1061 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/google/GCPAPI.py
--rw-r--r--   0 livia     (1000) livia     (1000)     1175 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/google/GoogleWorkspaceAPI.py
--rw-r--r--   0 livia     (1000) livia     (1000)      484 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/google/PubSub.py
--rw-r--r--   0 livia     (1000) livia     (1000)     1483 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/google/SQL.py
--rw-r--r--   0 livia     (1000) livia     (1000)      750 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/google/Storage.py
--rw-r--r--   0 livia     (1000) livia     (1000)      139 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/google/__init__.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.933608 mattlib-1.3.2/src/mattlib/http/
--rw-r--r--   0 livia     (1000) livia     (1000)     1302 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/http/HttpListener.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.933608 mattlib-1.3.2/src/mattlib/logger/
--rw-r--r--   0 livia     (1000) livia     (1000)     1370 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/logger/Logger.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.943608 mattlib-1.3.2/src/mattlib/microsoft/
--rw-r--r--   0 livia     (1000) livia     (1000)    18681 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/microsoft/AzureAPI.py
--rw-r--r--   0 livia     (1000) livia     (1000)     1950 2024-02-08 13:30:11.000000 mattlib-1.3.2/src/mattlib/microsoft/BaseMicrosoftAPI.py
--rw-r--r--   0 livia     (1000) livia     (1000)    15597 2024-02-08 13:29:27.000000 mattlib-1.3.2/src/mattlib/microsoft/GraphAPI.py
--rw-r--r--   0 livia     (1000) livia     (1000)       61 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/microsoft/__init__.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.953608 mattlib-1.3.2/src/mattlib/network/
--rw-r--r--   0 livia     (1000) livia     (1000)     1373 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/network/HttpListener.py
--rw-r--r--   0 livia     (1000) livia     (1000)       39 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/network/__init__.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.953608 mattlib-1.3.2/src/mattlib/salesforce/
--rw-r--r--   0 livia     (1000) livia     (1000)     6525 2024-02-08 12:57:03.000000 mattlib-1.3.2/src/mattlib/salesforce/SalesForceAPI.py
--rw-r--r--   0 livia     (1000) livia     (1000)       41 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/salesforce/__init__.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.963608 mattlib-1.3.2/src/mattlib/snow/
--rw-r--r--   0 livia     (1000) livia     (1000)       28 2023-11-22 10:34:26.000000 mattlib-1.3.2/src/mattlib/snow/__init__.py
--rw-r--r--   0 livia     (1000) livia     (1000)     4018 2024-02-08 13:31:09.000000 mattlib-1.3.2/src/mattlib/snow/snowAPI.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.963608 mattlib-1.3.2/src/mattlib/system/
--rw-r--r--   0 livia     (1000) livia     (1000)     1370 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/system/Logger.py
--rw-r--r--   0 livia     (1000) livia     (1000)       27 2023-10-23 23:40:32.000000 mattlib-1.3.2/src/mattlib/system/__init__.py
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.973608 mattlib-1.3.2/src/mattlib.egg-info/
--rw-r--r--   0 livia     (1000) livia     (1000)      840 2024-02-08 13:33:09.000000 mattlib-1.3.2/src/mattlib.egg-info/PKG-INFO
--rw-r--r--   0 livia     (1000) livia     (1000)     1453 2024-02-08 13:33:09.000000 mattlib-1.3.2/src/mattlib.egg-info/SOURCES.txt
--rw-r--r--   0 livia     (1000) livia     (1000)        1 2024-02-08 13:33:09.000000 mattlib-1.3.2/src/mattlib.egg-info/dependency_links.txt
--rw-r--r--   0 livia     (1000) livia     (1000)       91 2024-02-08 13:33:09.000000 mattlib-1.3.2/src/mattlib.egg-info/requires.txt
--rw-r--r--   0 livia     (1000) livia     (1000)        8 2024-02-08 13:33:09.000000 mattlib-1.3.2/src/mattlib.egg-info/top_level.txt
-drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-02-08 13:33:09.963608 mattlib-1.3.2/test/
--rw-r--r--   0 livia     (1000) livia     (1000)      628 2023-10-23 23:40:32.000000 mattlib-1.3.2/test/test_salesforce.py
--rw-r--r--   0 livia     (1000) livia     (1000)      766 2023-10-23 23:40:32.000000 mattlib-1.3.2/test/test_vm_size.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.855570 mattlib-1.3.3/
+-rw-r--r--   0 livia     (1000) livia     (1000)    35149 2024-02-27 23:45:51.000000 mattlib-1.3.3/COPYING
+-rw-r--r--   0 livia     (1000) livia     (1000)      840 2024-04-16 18:39:42.855570 mattlib-1.3.3/PKG-INFO
+-rw-r--r--   0 livia     (1000) livia     (1000)      147 2024-02-27 23:45:51.000000 mattlib-1.3.3/README.md
+-rw-r--r--   0 livia     (1000) livia     (1000)      104 2024-02-27 23:45:51.000000 mattlib-1.3.3/pyproject.toml
+-rw-r--r--   0 livia     (1000) livia     (1000)      839 2024-04-16 18:39:42.855570 mattlib-1.3.3/setup.cfg
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.835570 mattlib-1.3.3/src/
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.845570 mattlib-1.3.3/src/mattlib/
+-rw-r--r--   0 livia     (1000) livia     (1000)      951 2024-02-27 23:45:51.000000 mattlib-1.3.3/src/mattlib/API_factory.py
+-rw-r--r--   0 livia     (1000) livia     (1000)     3413 2024-02-27 23:45:51.000000 mattlib-1.3.3/src/mattlib/BaseAPI.py
+-rw-r--r--   0 livia     (1000) livia     (1000)      235 2024-02-27 23:45:51.000000 mattlib-1.3.3/src/mattlib/__init__.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.845570 mattlib-1.3.3/src/mattlib/adobe/
+-rw-r--r--   0 livia     (1000) livia     (1000)     3332 2024-02-27 23:45:51.000000 mattlib-1.3.3/src/mattlib/adobe/AdobeAPI.py
+-rw-r--r--   0 livia     (1000) livia     (1000)       30 2024-02-27 23:45:51.000000 mattlib-1.3.3/src/mattlib/adobe/__init__.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.845570 mattlib-1.3.3/src/mattlib/apis/
+-rw-r--r--   0 livia     (1000) livia     (1000)    10010 2024-02-27 23:45:51.000000 mattlib-1.3.3/src/mattlib/apis/AzureAPI.py
+-rw-r--r--   0 livia     (1000) livia     (1000)     1917 2024-02-27 23:45:51.000000 mattlib-1.3.3/src/mattlib/apis/GraphAPI.py
+-rw-r--r--   0 livia     (1000) livia     (1000)     4355 2024-02-27 23:45:51.000000 mattlib-1.3.3/src/mattlib/apis/SalesForceAPI.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.845570 mattlib-1.3.3/src/mattlib/clockify/
+-rw-r--r--   0 livia     (1000) livia     (1000)      751 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/clockify/ClockifyAPI.py
+-rw-r--r--   0 livia     (1000) livia     (1000)       26 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/clockify/__init__.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.845570 mattlib-1.3.3/src/mattlib/docusign/
+-rw-r--r--   0 livia     (1000) livia     (1000)     1832 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/docusign/DocusignAPI.py
+-rw-r--r--   0 livia     (1000) livia     (1000)       37 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/docusign/__init__.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.845570 mattlib-1.3.3/src/mattlib/fourmatters/
+-rw-r--r--   0 livia     (1000) livia     (1000)     8016 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/fourmatters/virtual_machine.py
+-rw-r--r--   0 livia     (1000) livia     (1000)     2964 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/fourmatters/virtual_network.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.845570 mattlib-1.3.3/src/mattlib/gcp/
+-rw-r--r--   0 livia     (1000) livia     (1000)      484 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/gcp/PubSub.py
+-rw-r--r--   0 livia     (1000) livia     (1000)       21 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/gcp/__init__.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.855570 mattlib-1.3.3/src/mattlib/google/
+-rw-r--r--   0 livia     (1000) livia     (1000)     1116 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/google/BaseGoogleAPI.py
+-rw-r--r--   0 livia     (1000) livia     (1000)     1061 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/google/GCPAPI.py
+-rw-r--r--   0 livia     (1000) livia     (1000)     1175 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/google/GoogleWorkspaceAPI.py
+-rw-r--r--   0 livia     (1000) livia     (1000)      484 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/google/PubSub.py
+-rw-r--r--   0 livia     (1000) livia     (1000)     1483 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/google/SQL.py
+-rw-r--r--   0 livia     (1000) livia     (1000)      750 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/google/Storage.py
+-rw-r--r--   0 livia     (1000) livia     (1000)      139 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/google/__init__.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.855570 mattlib-1.3.3/src/mattlib/http/
+-rw-r--r--   0 livia     (1000) livia     (1000)     1302 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/http/HttpListener.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.855570 mattlib-1.3.3/src/mattlib/logger/
+-rw-r--r--   0 livia     (1000) livia     (1000)     1370 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/logger/Logger.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.855570 mattlib-1.3.3/src/mattlib/microsoft/
+-rw-r--r--   0 livia     (1000) livia     (1000)    18681 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/microsoft/AzureAPI.py
+-rw-r--r--   0 livia     (1000) livia     (1000)     1950 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/microsoft/BaseMicrosoftAPI.py
+-rw-r--r--   0 livia     (1000) livia     (1000)    15597 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/microsoft/GraphAPI.py
+-rw-r--r--   0 livia     (1000) livia     (1000)       61 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/microsoft/__init__.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.855570 mattlib-1.3.3/src/mattlib/network/
+-rw-r--r--   0 livia     (1000) livia     (1000)     1373 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/network/HttpListener.py
+-rw-r--r--   0 livia     (1000) livia     (1000)       39 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/network/__init__.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.855570 mattlib-1.3.3/src/mattlib/salesforce/
+-rw-r--r--   0 livia     (1000) livia     (1000)     6479 2024-04-16 18:24:44.000000 mattlib-1.3.3/src/mattlib/salesforce/SalesForceAPI.py
+-rw-r--r--   0 livia     (1000) livia     (1000)       41 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/salesforce/__init__.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.855570 mattlib-1.3.3/src/mattlib/snow/
+-rw-r--r--   0 livia     (1000) livia     (1000)       28 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/snow/__init__.py
+-rw-r--r--   0 livia     (1000) livia     (1000)     4018 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/snow/snowAPI.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.855570 mattlib-1.3.3/src/mattlib/system/
+-rw-r--r--   0 livia     (1000) livia     (1000)     1370 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/system/Logger.py
+-rw-r--r--   0 livia     (1000) livia     (1000)       27 2024-02-27 23:45:52.000000 mattlib-1.3.3/src/mattlib/system/__init__.py
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.855570 mattlib-1.3.3/src/mattlib.egg-info/
+-rw-r--r--   0 livia     (1000) livia     (1000)      840 2024-04-16 18:39:42.000000 mattlib-1.3.3/src/mattlib.egg-info/PKG-INFO
+-rw-r--r--   0 livia     (1000) livia     (1000)     1453 2024-04-16 18:39:42.000000 mattlib-1.3.3/src/mattlib.egg-info/SOURCES.txt
+-rw-r--r--   0 livia     (1000) livia     (1000)        1 2024-04-16 18:39:42.000000 mattlib-1.3.3/src/mattlib.egg-info/dependency_links.txt
+-rw-r--r--   0 livia     (1000) livia     (1000)       91 2024-04-16 18:39:42.000000 mattlib-1.3.3/src/mattlib.egg-info/requires.txt
+-rw-r--r--   0 livia     (1000) livia     (1000)        8 2024-04-16 18:39:42.000000 mattlib-1.3.3/src/mattlib.egg-info/top_level.txt
+drwxr-xr-x   0 livia     (1000) livia     (1000)        0 2024-04-16 18:39:42.855570 mattlib-1.3.3/test/
+-rw-r--r--   0 livia     (1000) livia     (1000)      628 2024-02-27 23:45:52.000000 mattlib-1.3.3/test/test_salesforce.py
+-rw-r--r--   0 livia     (1000) livia     (1000)      766 2024-02-27 23:45:52.000000 mattlib-1.3.3/test/test_vm_size.py
```

### Comparing `mattlib-1.3.2/COPYING` & `mattlib-1.3.3/COPYING`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/PKG-INFO` & `mattlib-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattlib
-Version: 1.3.2
+Version: 1.3.3
 Summary: API data extraction and formatting utilities.
 Home-page: https://source.cloud.google.com/mtz-repos-global/mattlib
 Author: 4matt
 Author-email: mattzero@4matt.com.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `mattlib-1.3.2/setup.cfg` & `mattlib-1.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mattlib
-version = 1.3.2
+version = 1.3.3
 author = 4matt
 author_email = mattzero@4matt.com.br
 description = API data extraction and formatting utilities.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://source.cloud.google.com/mtz-repos-global/mattlib
 classifiers =
```

### Comparing `mattlib-1.3.2/src/mattlib/API_factory.py` & `mattlib-1.3.3/src/mattlib/API_factory.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/BaseAPI.py` & `mattlib-1.3.3/src/mattlib/BaseAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/adobe/AdobeAPI.py` & `mattlib-1.3.3/src/mattlib/adobe/AdobeAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/apis/AzureAPI.py` & `mattlib-1.3.3/src/mattlib/apis/AzureAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/apis/GraphAPI.py` & `mattlib-1.3.3/src/mattlib/apis/GraphAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/apis/SalesForceAPI.py` & `mattlib-1.3.3/src/mattlib/apis/SalesForceAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/clockify/ClockifyAPI.py` & `mattlib-1.3.3/src/mattlib/clockify/ClockifyAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/docusign/DocusignAPI.py` & `mattlib-1.3.3/src/mattlib/docusign/DocusignAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/fourmatters/virtual_machine.py` & `mattlib-1.3.3/src/mattlib/fourmatters/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/fourmatters/virtual_network.py` & `mattlib-1.3.3/src/mattlib/fourmatters/virtual_network.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/google/BaseGoogleAPI.py` & `mattlib-1.3.3/src/mattlib/google/BaseGoogleAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/google/GCPAPI.py` & `mattlib-1.3.3/src/mattlib/google/GCPAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/google/GoogleWorkspaceAPI.py` & `mattlib-1.3.3/src/mattlib/google/GoogleWorkspaceAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/google/SQL.py` & `mattlib-1.3.3/src/mattlib/google/SQL.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/google/Storage.py` & `mattlib-1.3.3/src/mattlib/google/Storage.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/http/HttpListener.py` & `mattlib-1.3.3/src/mattlib/http/HttpListener.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/logger/Logger.py` & `mattlib-1.3.3/src/mattlib/logger/Logger.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/microsoft/AzureAPI.py` & `mattlib-1.3.3/src/mattlib/microsoft/AzureAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/microsoft/BaseMicrosoftAPI.py` & `mattlib-1.3.3/src/mattlib/microsoft/BaseMicrosoftAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/microsoft/GraphAPI.py` & `mattlib-1.3.3/src/mattlib/microsoft/GraphAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/network/HttpListener.py` & `mattlib-1.3.3/src/mattlib/network/HttpListener.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/salesforce/SalesForceAPI.py` & `mattlib-1.3.3/src/mattlib/salesforce/SalesForceAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,14 @@
     def call_api(self, url):
         values = []
         i = 0
         while url != None:
             try:
                 response = requests.get(url, headers=self.headers)
                 response = json.loads(response.text)
-                values += response['records']
             except:
                 raise Exception(f"SalesForceAPI failed.\n "\
                   f"Response: {response}")
 
             values += response['records']
             if 'nextRecordsUrl' in response.keys():
                 url_aux = response['nextRecordsUrl']
```

### Comparing `mattlib-1.3.2/src/mattlib/snow/snowAPI.py` & `mattlib-1.3.3/src/mattlib/snow/snowAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib/system/Logger.py` & `mattlib-1.3.3/src/mattlib/system/Logger.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/src/mattlib.egg-info/PKG-INFO` & `mattlib-1.3.3/src/mattlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattlib
-Version: 1.3.2
+Version: 1.3.3
 Summary: API data extraction and formatting utilities.
 Home-page: https://source.cloud.google.com/mtz-repos-global/mattlib
 Author: 4matt
 Author-email: mattzero@4matt.com.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `mattlib-1.3.2/src/mattlib.egg-info/SOURCES.txt` & `mattlib-1.3.3/src/mattlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/test/test_salesforce.py` & `mattlib-1.3.3/test/test_salesforce.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.3.2/test/test_vm_size.py` & `mattlib-1.3.3/test/test_vm_size.py`

 * *Files identical despite different names*

