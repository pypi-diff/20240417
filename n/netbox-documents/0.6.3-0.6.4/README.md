# Comparing `tmp/netbox-documents-0.6.3.tar.gz` & `tmp/netbox_documents-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-documents-0.6.3.tar", last modified: Tue Nov 21 08:11:35 2023, max compression
+gzip compressed data, was "netbox_documents-0.6.4.tar", last modified: Wed Apr 17 18:58:58 2024, max compression
```

## Comparing `netbox-documents-0.6.3.tar` & `netbox_documents-0.6.4.tar`

### file list

```diff
@@ -1,57 +1,66 @@
-drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-11-21 08:11:35.809696 netbox-documents-0.6.3/
--rw-r--r--   0 jasonyates   (502) staff       (20)    11357 2023-04-28 11:45:21.000000 netbox-documents-0.6.3/LICENSE
--rw-r--r--   0 jasonyates   (502) staff       (20)       80 2023-04-28 11:45:21.000000 netbox-documents-0.6.3/MANIFEST.in
--rw-r--r--   0 jasonyates   (502) staff       (20)     5992 2023-11-21 08:11:35.809287 netbox-documents-0.6.3/PKG-INFO
--rw-r--r--   0 jasonyates   (502) staff       (20)     5596 2023-11-21 07:51:21.000000 netbox-documents-0.6.3/README.md
-drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-11-21 08:11:35.795306 netbox-documents-0.6.3/netbox_documents/
--rw-r--r--   0 jasonyates   (502) staff       (20)      925 2023-11-21 07:52:19.000000 netbox-documents-0.6.3/netbox_documents/__init__.py
-drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-11-21 08:11:35.799093 netbox-documents-0.6.3/netbox_documents/api/
--rw-r--r--   0 jasonyates   (502) staff       (20)        0 2023-04-28 11:45:21.000000 netbox-documents-0.6.3/netbox_documents/api/__init__.py
--rw-r--r--   0 jasonyates   (502) staff       (20)      208 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/api/fields.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     4906 2023-11-20 08:42:32.000000 netbox-documents-0.6.3/netbox_documents/api/serializers.py
--rw-r--r--   0 jasonyates   (502) staff       (20)      482 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/api/urls.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     1390 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/api/views.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     2147 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/filtersets.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     4629 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/forms.py
-drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-11-21 08:11:35.801659 netbox-documents-0.6.3/netbox_documents/migrations/
--rw-r--r--   0 jasonyates   (502) staff       (20)     3867 2023-04-28 11:45:21.000000 netbox-documents-0.6.3/netbox_documents/migrations/0001_initial.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     1611 2023-04-28 11:45:21.000000 netbox-documents-0.6.3/netbox_documents/migrations/0002_AddDeviceType.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     4032 2023-04-28 11:45:21.000000 netbox-documents-0.6.3/netbox_documents/migrations/0003_alter_circuitdocument_options_and_more.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     1949 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/migrations/0004_locationdocument.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     1140 2023-11-20 08:33:46.000000 netbox-documents-0.6.3/netbox_documents/migrations/0005_alter_circuitdocument_external_url_and_more.py
--rw-r--r--   0 jasonyates   (502) staff       (20)        0 2023-04-28 11:45:21.000000 netbox-documents-0.6.3/netbox_documents/migrations/__init__.py
--rw-r--r--   0 jasonyates   (502) staff       (20)    17782 2023-11-20 08:33:38.000000 netbox-documents-0.6.3/netbox_documents/models.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     3600 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/navigation.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     1386 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/search.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     5584 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/tables.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     4823 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/template_content.py
-drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-11-21 08:11:35.789827 netbox-documents-0.6.3/netbox_documents/templates/
-drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-11-21 08:11:35.807907 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/
--rw-r--r--   0 jasonyates   (502) staff       (20)     1879 2023-11-20 08:48:12.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/circuitdocument.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     1933 2023-11-20 08:15:19.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/circuitdocument_edit.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     2275 2023-11-20 08:15:19.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/circuitdocument_include.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     1870 2023-11-20 08:48:56.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/devicedocument.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     1932 2023-11-20 08:15:19.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/devicedocument_edit.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     2253 2023-11-20 08:15:19.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/devicedocument_include.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     1895 2023-11-20 08:49:29.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/devicetypedocument.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     1937 2023-11-20 08:15:19.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/devicetypedocument_edit.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     2297 2023-11-20 08:15:19.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/devicetypedocument_include.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     1959 2023-11-20 08:15:19.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/document_edit.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     2049 2023-11-20 08:47:36.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/locationdocument.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     1971 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/locationdocument_edit.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     2290 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/locationdocument_include.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     1860 2023-11-20 08:50:20.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/sitedocument.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     1930 2023-11-20 08:15:19.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/sitedocument_edit.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     2250 2023-11-20 08:15:19.000000 netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/sitedocument_include.html
--rw-r--r--   0 jasonyates   (502) staff       (20)     3826 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/urls.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     1038 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/utils.py
--rw-r--r--   0 jasonyates   (502) staff       (20)     3564 2023-11-20 08:15:21.000000 netbox-documents-0.6.3/netbox_documents/views.py
-drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-11-21 08:11:35.808360 netbox-documents-0.6.3/netbox_documents.egg-info/
--rw-r--r--   0 jasonyates   (502) staff       (20)     5992 2023-11-21 08:11:35.000000 netbox-documents-0.6.3/netbox_documents.egg-info/PKG-INFO
--rw-r--r--   0 jasonyates   (502) staff       (20)     2192 2023-11-21 08:11:35.000000 netbox-documents-0.6.3/netbox_documents.egg-info/SOURCES.txt
--rw-r--r--   0 jasonyates   (502) staff       (20)        1 2023-11-21 08:11:35.000000 netbox-documents-0.6.3/netbox_documents.egg-info/dependency_links.txt
--rw-r--r--   0 jasonyates   (502) staff       (20)        1 2023-11-21 08:03:08.000000 netbox-documents-0.6.3/netbox_documents.egg-info/not-zip-safe
--rw-r--r--   0 jasonyates   (502) staff       (20)       24 2023-11-21 08:11:35.000000 netbox-documents-0.6.3/netbox_documents.egg-info/requires.txt
--rw-r--r--   0 jasonyates   (502) staff       (20)       17 2023-11-21 08:11:35.000000 netbox-documents-0.6.3/netbox_documents.egg-info/top_level.txt
--rw-r--r--   0 jasonyates   (502) staff       (20)       38 2023-11-21 08:11:35.809760 netbox-documents-0.6.3/setup.cfg
--rw-r--r--   0 jasonyates   (502) staff       (20)      793 2023-11-21 08:11:29.000000 netbox-documents-0.6.3/setup.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2024-04-17 18:58:58.013561 netbox_documents-0.6.4/
+-rw-r--r--   0 jasonyates   (502) staff       (20)    11357 2023-04-28 11:45:21.000000 netbox_documents-0.6.4/LICENSE
+-rw-r--r--   0 jasonyates   (502) staff       (20)      105 2024-04-17 18:58:50.000000 netbox_documents-0.6.4/MANIFEST.in
+-rw-r--r--   0 jasonyates   (502) staff       (20)     6037 2024-04-17 18:58:58.012973 netbox_documents-0.6.4/PKG-INFO
+-rw-r--r--   0 jasonyates   (502) staff       (20)     5641 2024-04-17 18:52:06.000000 netbox_documents-0.6.4/README.md
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2024-04-17 18:58:57.988681 netbox_documents-0.6.4/netbox_documents/
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1109 2024-04-17 18:49:50.000000 netbox_documents-0.6.4/netbox_documents/__init__.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2024-04-17 18:58:57.994959 netbox_documents-0.6.4/netbox_documents/api/
+-rw-r--r--   0 jasonyates   (502) staff       (20)        0 2023-04-28 11:45:21.000000 netbox_documents-0.6.4/netbox_documents/api/__init__.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)      208 2023-11-20 08:15:21.000000 netbox_documents-0.6.4/netbox_documents/api/fields.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     6978 2024-04-17 18:46:20.000000 netbox_documents-0.6.4/netbox_documents/api/serializers.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)      622 2024-04-17 18:45:30.000000 netbox_documents-0.6.4/netbox_documents/api/urls.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1916 2024-04-17 18:45:22.000000 netbox_documents-0.6.4/netbox_documents/api/views.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2968 2024-04-17 18:44:58.000000 netbox_documents-0.6.4/netbox_documents/filtersets.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     6321 2024-04-17 18:44:39.000000 netbox_documents-0.6.4/netbox_documents/forms.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2024-04-17 18:58:57.999354 netbox_documents-0.6.4/netbox_documents/migrations/
+-rw-r--r--   0 jasonyates   (502) staff       (20)     3867 2023-04-28 11:45:21.000000 netbox_documents-0.6.4/netbox_documents/migrations/0001_initial.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1611 2023-04-28 11:45:21.000000 netbox_documents-0.6.4/netbox_documents/migrations/0002_AddDeviceType.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     4032 2023-04-28 11:45:21.000000 netbox_documents-0.6.4/netbox_documents/migrations/0003_alter_circuitdocument_options_and_more.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1949 2023-11-20 08:15:21.000000 netbox_documents-0.6.4/netbox_documents/migrations/0004_locationdocument.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1140 2023-11-20 08:33:46.000000 netbox_documents-0.6.4/netbox_documents/migrations/0005_alter_circuitdocument_external_url_and_more.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1802 2024-04-17 18:28:09.000000 netbox_documents-0.6.4/netbox_documents/migrations/0006_vmdocument.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1812 2024-04-17 18:46:51.000000 netbox_documents-0.6.4/netbox_documents/migrations/0007_circuitproviderdocument.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)        0 2023-04-28 11:45:21.000000 netbox_documents-0.6.4/netbox_documents/migrations/__init__.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)    24651 2024-04-17 18:39:56.000000 netbox_documents-0.6.4/netbox_documents/models.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     4787 2024-04-17 18:39:06.000000 netbox_documents-0.6.4/netbox_documents/navigation.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1869 2024-04-17 18:38:47.000000 netbox_documents-0.6.4/netbox_documents/search.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     7696 2024-04-17 18:38:17.000000 netbox_documents-0.6.4/netbox_documents/tables.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     6727 2024-04-17 18:37:50.000000 netbox_documents-0.6.4/netbox_documents/template_content.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2024-04-17 18:58:57.977532 netbox_documents-0.6.4/netbox_documents/templates/
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2024-04-17 18:58:58.011358 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1879 2023-11-20 08:48:12.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/circuitdocument.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1933 2023-11-20 08:15:19.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/circuitdocument_edit.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2275 2023-11-20 08:15:19.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/circuitdocument_include.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1891 2024-04-17 18:37:15.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/circuitproviderdocument.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1933 2024-04-17 18:36:57.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/circuitproviderdocument_edit.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2328 2024-04-17 18:48:30.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/circuitproviderdocument_include.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1870 2023-11-20 08:48:56.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/devicedocument.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1932 2023-11-20 08:15:19.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/devicedocument_edit.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2253 2023-11-20 08:15:19.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/devicedocument_include.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1895 2023-11-20 08:49:29.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/devicetypedocument.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1937 2023-11-20 08:15:19.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/devicetypedocument_edit.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2297 2023-11-20 08:15:19.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/devicetypedocument_include.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1959 2023-11-20 08:15:19.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/document_edit.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2049 2023-11-20 08:47:36.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/locationdocument.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1971 2023-11-20 08:15:21.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/locationdocument_edit.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2290 2023-11-20 08:15:21.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/locationdocument_include.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1860 2023-11-20 08:50:20.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/sitedocument.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1930 2023-11-20 08:15:19.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/sitedocument_edit.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2250 2023-11-20 08:15:19.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/sitedocument_include.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1872 2024-04-17 18:28:09.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/vmdocument.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1928 2024-04-17 18:28:09.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/vmdocument_edit.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2279 2024-04-17 18:28:09.000000 netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/vmdocument_include.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     5360 2024-04-17 18:33:55.000000 netbox_documents-0.6.4/netbox_documents/urls.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1190 2024-04-17 18:34:33.000000 netbox_documents-0.6.4/netbox_documents/utils.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     4999 2024-04-17 18:35:04.000000 netbox_documents-0.6.4/netbox_documents/views.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2024-04-17 18:58:58.011870 netbox_documents-0.6.4/netbox_documents.egg-info/
+-rw-r--r--   0 jasonyates   (502) staff       (20)     6037 2024-04-17 18:58:57.000000 netbox_documents-0.6.4/netbox_documents.egg-info/PKG-INFO
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2741 2024-04-17 18:58:57.000000 netbox_documents-0.6.4/netbox_documents.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonyates   (502) staff       (20)        1 2024-04-17 18:58:57.000000 netbox_documents-0.6.4/netbox_documents.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonyates   (502) staff       (20)        1 2023-11-21 08:03:08.000000 netbox_documents-0.6.4/netbox_documents.egg-info/not-zip-safe
+-rw-r--r--   0 jasonyates   (502) staff       (20)       24 2024-04-17 18:58:57.000000 netbox_documents-0.6.4/netbox_documents.egg-info/requires.txt
+-rw-r--r--   0 jasonyates   (502) staff       (20)       17 2024-04-17 18:58:57.000000 netbox_documents-0.6.4/netbox_documents.egg-info/top_level.txt
+-rw-r--r--   0 jasonyates   (502) staff       (20)       23 2023-11-20 08:15:21.000000 netbox_documents-0.6.4/requirements.txt
+-rw-r--r--   0 jasonyates   (502) staff       (20)       38 2024-04-17 18:58:58.013666 netbox_documents-0.6.4/setup.cfg
+-rw-r--r--   0 jasonyates   (502) staff       (20)      885 2024-04-17 18:50:02.000000 netbox_documents-0.6.4/setup.py
```

### Comparing `netbox-documents-0.6.3/LICENSE` & `netbox_documents-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/PKG-INFO` & `netbox_documents-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-documents
-Version: 0.6.3
+Version: 0.6.4
 Summary: Manage site, location, circuit and device diagrams and documents in Netbox
 Home-page: https://github.com/jasonyates/netbox-documents
 Author: Jason Yates
 Author-email: me@jasonyates.co.uk
 Keywords: netbox,netbox-plugin,plugin
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,25 +18,27 @@
 
 * Store documents against the following NetBox models:
    - Circuits
    - Devices
    - Device Types
    - Sites
    - Locations
+   - Virtual Machines
+   - Circuit Providers
 
 * Upload documents to your NetBox media/ folder or other Django supported storage method e.g. S3
 * Supports a wide array of common file types (bmp, gif, jpeg, jpg, png, pdf, txt, doc, docx, xls, xlsx, xlsm)
 * Store links to external URL's to save duplication of remote documents
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.6+       |      0.6.3     |
+|     3.6+       |      0.6.4     |
 |     3.5.x      |      0.6.0     |
 | 3.3.x - 3.4.x  |      0.5.1     |
 
 
 ## Installation
 
 A working installation of Netbox 3.3+ is required. 3.6+ is recommended. **NOTE: Netbox 3.5 introduced breaking changes for plugins, please use the correct plugin version for your netbox install.**
```

### Comparing `netbox-documents-0.6.3/README.md` & `netbox_documents-0.6.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 
 * Store documents against the following NetBox models:
    - Circuits
    - Devices
    - Device Types
    - Sites
    - Locations
+   - Virtual Machines
+   - Circuit Providers
 
 * Upload documents to your NetBox media/ folder or other Django supported storage method e.g. S3
 * Supports a wide array of common file types (bmp, gif, jpeg, jpg, png, pdf, txt, doc, docx, xls, xlsx, xlsm)
 * Store links to external URL's to save duplication of remote documents
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.6+       |      0.6.3     |
+|     3.6+       |      0.6.4     |
 |     3.5.x      |      0.6.0     |
 | 3.3.x - 3.4.x  |      0.5.1     |
 
 
 ## Installation
 
 A working installation of Netbox 3.3+ is required. 3.6+ is recommended. **NOTE: Netbox 3.5 introduced breaking changes for plugins, please use the correct plugin version for your netbox install.**
```

### Comparing `netbox-documents-0.6.3/netbox_documents/__init__.py` & `netbox_documents-0.6.4/netbox_documents/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from extras.plugins import PluginConfig
 
 class NetboxDocuments(PluginConfig):
     name = 'netbox_documents'
     verbose_name = 'Document Storage'
     description = 'Manage site, location, circuit and device diagrams and documents in Netbox'
-    version = '0.6.3'
+    version = '0.6.4'
     author = 'Jason Yates'
     author_email = 'me@jasonyates.co.uk'
     min_version = '3.5.0'
     base_url = 'documents'
     default_settings = {
         "enable_site_documents": True,
         "enable_location_documents": True,
         "enable_circuit_documents": True,
         "enable_device_documents": True,
         "enable_device_type_documents": True, 
+        "enable_vm_documents": True,
+        "enable_circuit_provider_documents": True,
         "enable_navigation_menu": True,
         "site_documents_location": "left",
         "location_documents_location": "left",
         "circuit_documents_location": "left",
         "device_documents_location": "left",
         "device_type_documents_location": "left", 
+        "vm_documents_location": "left",
+        "circuit_provider_documents_location": "left",
     }
 
 config = NetboxDocuments
```

### Comparing `netbox-documents-0.6.3/netbox_documents/api/serializers.py` & `netbox_documents-0.6.4/netbox_documents/api/serializers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from rest_framework import serializers
 
 from netbox.api.serializers import NetBoxModelSerializer, WritableNestedSerializer
-from ..models import SiteDocument, LocationDocument, DeviceDocument, DeviceTypeDocument, CircuitDocument 
+from ..models import SiteDocument, LocationDocument, DeviceDocument, DeviceTypeDocument, CircuitDocument, VMDocument, CircuitProviderDocument
 from dcim.api.nested_serializers import NestedSiteSerializer, NestedLocationSerializer, NestedDeviceSerializer, NestedDeviceTypeSerializer 
-from circuits.api.nested_serializers import NestedCircuitSerializer
+from circuits.api.nested_serializers import NestedCircuitSerializer, NestedProviderSerializer
+from virtualization.api.nested_serializers import NestedVirtualMachineSerializer
 from .fields import UploadableBase64FileField
 
 # Site Document Serializer
 class SiteDocumentSerializer(NetBoxModelSerializer):
 
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_documents-api:sitedocument-detail'
@@ -137,7 +138,65 @@
     )
 
     class Meta:
         model = CircuitDocument
         fields = (
             'id', 'url', 'display', 'name', 'document', 'external_url', 'document_type', 'filename',
         )
+
+# VM Document Serializer
+class VMDocumentSerializer(NetBoxModelSerializer):
+
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:netbox_documents-api:vmdocument-detail'
+    )
+
+    vm = NestedVirtualMachineSerializer()
+    document = UploadableBase64FileField(required=False)
+
+    class Meta:
+        model = VMDocument
+        fields = (
+            'id', 'url', 'display', 'name', 'document', 'external_url', 'document_type', 'filename', 'vm', 'comments', 'tags', 'custom_fields', 'created',
+            'last_updated',
+        )
+
+class NestedVMDocumentSerializer(WritableNestedSerializer):
+
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:netbox_documents-api:vmdocument-detail'
+    )
+
+    class Meta:
+        model = VMDocument
+        fields = (
+            'id', 'url', 'display', 'name', 'document', 'external_url', 'document_type', 'filename',
+        )
+
+# Circuit Provider Document Serializer
+class CircuitProviderDocumentSerializer(NetBoxModelSerializer):
+
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:netbox_documents-api:circuitproviderdocument-detail'
+    )
+
+    provider = NestedProviderSerializer()
+    document = UploadableBase64FileField(required=False)
+
+    class Meta:
+        model = CircuitProviderDocument
+        fields = (
+            'id', 'url', 'display', 'name', 'document', 'external_url', 'document_type', 'filename', 'provider', 'comments', 'tags', 'custom_fields', 'created',
+            'last_updated',
+        )
+
+class NestedCircuitProviderDocumentSerializer(WritableNestedSerializer):
+
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:netbox_documents-api:circuitdocument-detail'
+    )
+
+    class Meta:
+        model = CircuitProviderDocument
+        fields = (
+            'id', 'url', 'display', 'name', 'document', 'external_url', 'document_type', 'filename',
+        )
```

### Comparing `netbox-documents-0.6.3/netbox_documents/api/views.py` & `netbox_documents-0.6.4/netbox_documents/api/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from netbox.api.viewsets import NetBoxModelViewSet
 
 from .. import models, filtersets
-from .serializers import SiteDocumentSerializer, LocationDocumentSerializer, DeviceDocumentSerializer, DeviceTypeDocumentSerializer, CircuitDocumentSerializer 
+from .serializers import SiteDocumentSerializer, LocationDocumentSerializer, DeviceDocumentSerializer, DeviceTypeDocumentSerializer, CircuitDocumentSerializer, VMDocumentSerializer, CircuitProviderDocumentSerializer
 
 class SiteDocumentViewSet(NetBoxModelViewSet):
     queryset = models.SiteDocument.objects.prefetch_related('tags')
     serializer_class = SiteDocumentSerializer
     filterset_class = filtersets.SiteDocumentFilterSet
 
 class LocationDocumentViewSet(NetBoxModelViewSet):
@@ -22,8 +22,18 @@
     queryset = models.DeviceTypeDocument.objects.prefetch_related('tags')
     serializer_class = DeviceTypeDocumentSerializer
     filterset_class = filtersets.DeviceTypeDocumentFilterSet
 
 class CircuitDocumentViewSet(NetBoxModelViewSet):
     queryset = models.CircuitDocument.objects.prefetch_related('tags')
     serializer_class = CircuitDocumentSerializer
-    filterset_class = filtersets.CircuitDocumentFilterSet
+    filterset_class = filtersets.CircuitDocumentFilterSet
+
+class VMDocumentViewSet(NetBoxModelViewSet):
+    queryset = models.VMDocument.objects.prefetch_related('tags')
+    serializer_class = VMDocumentSerializer
+    filterset_class = filtersets.VMDocumentFilterSet
+
+class CircuitProviderDocumentViewSet(NetBoxModelViewSet):
+    queryset = models.CircuitProviderDocument.objects.prefetch_related('tags')
+    serializer_class = CircuitProviderDocumentSerializer
+    filterset_class = filtersets.CircuitProviderDocumentFilterSet
```

### Comparing `netbox-documents-0.6.3/netbox_documents/filtersets.py` & `netbox_documents-0.6.4/netbox_documents/filtersets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from netbox.filtersets import NetBoxModelFilterSet
-from .models import SiteDocument, LocationDocument, DeviceDocument, DeviceTypeDocument, CircuitDocument 
+from .models import SiteDocument, LocationDocument, DeviceDocument, DeviceTypeDocument, CircuitDocument, VMDocument, CircuitProviderDocument
 from django.db.models import Q
 
 class SiteDocumentFilterSet(NetBoxModelFilterSet):
 
     class Meta:
         model = SiteDocument
         fields = ('id', 'name', 'document_type', 'site')
@@ -68,7 +68,35 @@
     def search(self, queryset, name, value):
         if not value.strip():
             return queryset
         return queryset.filter(
             Q(name__icontains=value) |
             Q(document__icontains=value)
         )
+
+class VMDocumentFilterSet(NetBoxModelFilterSet):
+
+    class Meta:
+        model = VMDocument
+        fields = ('id', 'name', 'document_type', 'vm')
+
+    def search(self, queryset, name, value):
+        if not value.strip():
+            return queryset
+        return queryset.filter(
+            Q(name__icontains=value) |
+            Q(document__icontains=value)
+        )
+    
+class CircuitProviderDocumentFilterSet(NetBoxModelFilterSet):
+
+    class Meta:
+        model = CircuitProviderDocument
+        fields = ('id', 'name', 'document_type', 'provider')
+
+    def search(self, queryset, name, value):
+        if not value.strip():
+            return queryset
+        return queryset.filter(
+            Q(name__icontains=value) |
+            Q(document__icontains=value)
+        )
```

### Comparing `netbox-documents-0.6.3/netbox_documents/forms.py` & `netbox_documents-0.6.4/netbox_documents/forms.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django import forms
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm
-from dcim.models import Site, Location, Device, DeviceType 
-from circuits.models import Circuit
+from dcim.models import Site, Location, Device, DeviceType
+from virtualization.models import VirtualMachine
+from circuits.models import Circuit, Provider
 from utilities.forms.fields import TagFilterField, CommentField, DynamicModelChoiceField
-from .models import SiteDocument, LocationDocument, DeviceDocument, DeviceTypeDocument, CircuitDocument, CircuitDocTypeChoices, SiteDocTypeChoices, LocationDocTypeChoices, DeviceDocTypeChoices, DeviceTypeDocTypeChoices 
+from .models import SiteDocument, LocationDocument, DeviceDocument, DeviceTypeDocument, CircuitDocument, CircuitDocTypeChoices, SiteDocTypeChoices, LocationDocTypeChoices, DeviceDocTypeChoices, DeviceTypeDocTypeChoices, VMDocument, VMDocTypeChoices, CircuitProviderDocument, CircuitProviderDocTypeChoices 
 
 
 #### Site Document Form & Filter Form
 class SiteDocumentForm(NetBoxModelForm):
     comments = CommentField()
 
     site = DynamicModelChoiceField(
@@ -175,7 +176,69 @@
 
     document_type = forms.MultipleChoiceField(
         choices=CircuitDocTypeChoices,
         required=False
     )
 
     tag = TagFilterField(model)
+
+#### VM Document Form & Filter Form
+class VMDocumentForm(NetBoxModelForm):
+    comments = CommentField()
+
+    vm = DynamicModelChoiceField(
+        queryset=VirtualMachine.objects.all()
+    )
+
+    class Meta:
+        model = VMDocument
+        fields = ('name', 'document', 'external_url', 'document_type', 'vm', 'comments', 'tags')
+
+class VMDocumentFilterForm(NetBoxModelFilterSetForm):
+    model = VMDocument
+
+    name = forms.CharField(
+        required=False
+    )
+
+    vm = forms.ModelMultipleChoiceField(
+        queryset=VirtualMachine.objects.all(),
+        required=False
+    )
+
+    document_type = forms.MultipleChoiceField(
+        choices=VMDocTypeChoices,
+        required=False
+    )
+
+    tag = TagFilterField(model)
+
+#### Circuit Provider Document Form & Filter Form
+class CircuitProviderDocumentForm(NetBoxModelForm):
+    comments = CommentField()
+
+    provider = DynamicModelChoiceField(
+        queryset=Provider.objects.all()
+    )
+
+    class Meta:
+        model = CircuitProviderDocument
+        fields = ('name', 'document', 'external_url', 'document_type', 'provider', 'comments', 'tags')
+
+class CircuitProviderDocumentFilterForm(NetBoxModelFilterSetForm):
+    model = CircuitProviderDocument
+
+    name = forms.CharField(
+        required=False
+    )
+
+    provider = forms.ModelMultipleChoiceField(
+        queryset=Provider.objects.all(),
+        required=False
+    )
+
+    document_type = forms.MultipleChoiceField(
+        choices=CircuitProviderDocTypeChoices,
+        required=False
+    )
+
+    tag = TagFilterField(model)
```

### Comparing `netbox-documents-0.6.3/netbox_documents/migrations/0001_initial.py` & `netbox_documents-0.6.4/netbox_documents/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/migrations/0002_AddDeviceType.py` & `netbox_documents-0.6.4/netbox_documents/migrations/0002_AddDeviceType.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/migrations/0003_alter_circuitdocument_options_and_more.py` & `netbox_documents-0.6.4/netbox_documents/migrations/0003_alter_circuitdocument_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/migrations/0004_locationdocument.py` & `netbox_documents-0.6.4/netbox_documents/migrations/0004_locationdocument.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/migrations/0005_alter_circuitdocument_external_url_and_more.py` & `netbox_documents-0.6.4/netbox_documents/migrations/0005_alter_circuitdocument_external_url_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/models.py` & `netbox_documents-0.6.4/netbox_documents/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,14 +64,41 @@
     key = 'DocTypeChoices.circuit'
 
     CHOICES = [
         ('circuitcontract', 'Circuit Contract', 'red'),
         ('diagram', 'Network Diagram', 'green'),
         ('purchaseorder', 'Purchase Order', 'orange'),
         ('quote', 'Quote', 'indigo'),
+        ('kmz', 'KMZ', 'blue'),
+        ('other', 'Other', 'gray'),
+    ]
+
+class CircuitProviderDocTypeChoices(ChoiceSet):
+    
+    key = 'DocTypeChoices.circuitprovider'
+
+    CHOICES = [
+        ('contract', 'Contract', 'red'),
+        ('msa', 'MSA', 'green'),
+        ('purchaseorder', 'Purchase Order', 'orange'),
+        ('quote', 'Quote', 'indigo'),
+        ('other', 'Other', 'gray'),
+    ]
+
+
+class VMDocTypeChoices(ChoiceSet):
+
+    key = 'DocTypeChoices.virtualmachine'
+
+    CHOICES = [
+        ('diagram', 'Network Diagram', 'green'),
+        ('manual', 'Manual', 'pink'),
+        ('purchaseorder', 'Purchase Order', 'orange'),
+        ('quote', 'Quote', 'indigo'),
+        ('supportcontract', 'Support Contract', 'blue'),
         ('other', 'Other', 'gray'),
     ]
 
 class SiteDocument(NetBoxModel):
     name = models.CharField(
         max_length=100,
         blank=True,
@@ -614,7 +641,218 @@
             self.document.delete(save=False)
 
             # Restore the name of the document as it's re-used in the notifications later
             self.document.name = _name
         else:
             # Straight delete of external URL
             super().delete(*args, **kwargs)
+
+
+class VMDocument(NetBoxModel):
+    name = models.CharField(
+        max_length=100,
+        blank=True,
+        help_text='(Optional) Specify a name to display for this document. If no name is specified, the filename will be used.'
+    )
+
+    document = models.FileField(
+        upload_to=file_upload,
+        blank=True
+    )
+
+    external_url = models.URLField(
+        blank=True,
+        max_length=255
+    )
+
+    document_type = models.CharField(
+        max_length=30,
+        choices=VMDocTypeChoices
+    )
+
+    vm = models.ForeignKey(
+        to='virtualization.VirtualMachine',
+        on_delete=models.CASCADE,
+        related_name='documents'
+    )
+
+    comments = models.TextField(
+        blank=True
+    )
+
+    class Meta:
+        ordering = ('name',)
+        verbose_name_plural = "Virtual Machine Documents"
+        verbose_name = "Virtual Machine Document"
+
+    def get_document_type_color(self):
+        return VMDocTypeChoices.colors.get(self.document_type)
+
+    @property
+    def size(self):
+        """
+        Wrapper around `document.size` to suppress an OSError in case the file is inaccessible. Also opportunistically
+        catch other exceptions that we know other storage back-ends to throw.
+        """
+        expected_exceptions = [OSError]
+
+        try:
+            from botocore.exceptions import ClientError
+            expected_exceptions.append(ClientError)
+        except ImportError:
+            pass
+
+        try:
+            return self.document.size
+        except:
+            return None
+
+    @property
+    def filename(self):
+        if self.external_url:
+            return self.external_url
+        filename = self.document.name.rsplit('/', 1)[-1]
+        return filename.split('_', 1)[1]
+
+    def __str__(self):
+        if self.name:
+            return self.name
+
+        if self.external_url:
+            return self.external_url
+
+        filename = self.document.name.rsplit('/', 1)[-1]
+        return filename.split('_', 1)[1]
+
+    def get_absolute_url(self):
+        return reverse('plugins:netbox_documents:vmdocument', args=[self.pk])
+
+    def clean(self):
+        super().clean()
+
+        # Must have an uploaded document or an external URL. cannot have both
+        if not self.document and self.external_url == '':
+            raise ValidationError("A document must contain an uploaded file or an external URL.")
+        if self.document and self.external_url:
+            raise ValidationError("A document cannot contain both an uploaded file and an external URL.")
+
+    def delete(self, *args, **kwargs):
+
+        # Check if its a document or a URL
+        if self.external_url == '':
+
+            _name = self.document.name
+
+            # Delete file from disk
+            super().delete(*args, **kwargs)
+            self.document.delete(save=False)
+
+            # Restore the name of the document as it's re-used in the notifications later
+            self.document.name = _name
+        else:
+            # Straight delete of external URL
+            super().delete(*args, **kwargs)
+
+class CircuitProviderDocument(NetBoxModel):
+    name = models.CharField(
+        max_length=100,
+        blank=True,
+        help_text='(Optional) Specify a name to display for this document. If no name is specified, the filename will be used.'
+    )
+
+    document = models.FileField(
+        upload_to=file_upload,
+        blank=True
+    )
+
+    external_url = models.URLField(
+        blank=True,
+        max_length=255
+    )
+
+    document_type = models.CharField(
+        max_length=30,
+        choices=CircuitProviderDocTypeChoices
+    )
+
+    provider = models.ForeignKey(
+        to='circuits.Provider',
+        on_delete=models.CASCADE,
+        related_name='documents'
+    )
+
+    comments = models.TextField(
+        blank=True
+    )
+
+    def get_document_type_color(self):
+        return CircuitProviderDocTypeChoices.colors.get(self.document_type)
+
+    class Meta:
+        ordering = ('name',)
+        verbose_name_plural = "Circuit Provider Documents"
+        verbose_name = "Circuit Provider Document"
+
+    @property
+    def size(self):
+        """
+        Wrapper around `document.size` to suppress an OSError in case the file is inaccessible. Also opportunistically
+        catch other exceptions that we know other storage back-ends to throw.
+        """
+        expected_exceptions = [OSError]
+
+        try:
+            from botocore.exceptions import ClientError
+            expected_exceptions.append(ClientError)
+        except ImportError:
+            pass
+
+        try:
+            return self.document.size
+        except:
+            return None
+
+    @property
+    def filename(self):
+        if self.external_url:
+            return self.external_url
+        filename = self.document.name.rsplit('/', 1)[-1]
+        return filename.split('_', 1)[1]
+
+    def __str__(self):
+        if self.name:
+            return self.name
+
+        if self.external_url:
+            return self.external_url
+
+        filename = self.document.name.rsplit('/', 1)[-1]
+        return filename.split('_', 1)[1]
+
+    def get_absolute_url(self):
+        return reverse('plugins:netbox_documents:circuitproviderdocument', args=[self.pk])
+
+    def clean(self):
+        super().clean()
+
+        # Must have an uploaded document or an external URL. cannot have both
+        if not self.document and self.external_url == '':
+            raise ValidationError("A document must contain an uploaded file or an external URL.")
+        if self.document and self.external_url:
+            raise ValidationError("A document cannot contain both an uploaded file and an external URL.")
+
+    def delete(self, *args, **kwargs):
+
+        # Check if its a document or a URL
+        if self.external_url == '':
+
+            _name = self.document.name
+
+            # Delete file from disk
+            super().delete(*args, **kwargs)
+            self.document.delete(save=False)
+
+            # Restore the name of the document as it's re-used in the notifications later
+            self.document.name = _name
+        else:
+            # Straight delete of external URL
+            super().delete(*args, **kwargs)
```

### Comparing `netbox-documents-0.6.3/netbox_documents/navigation.py` & `netbox_documents-0.6.4/netbox_documents/navigation.py`

 * *Files 11% similar despite different names*

```diff
@@ -90,11 +90,41 @@
             label='Documents',
             groups=(
                 ('Document Storage', menuitem),
             ),
             icon_class='mdi mdi-file-document-multiple'
         )
 
+    # Add a menu item for VM Documents if enabled
+    if plugin_settings.get('enable_vm_documents'):
+        menuitem.append(
+            PluginMenuItem(
+                link='plugins:netbox_documents:vmdocument_list',
+                link_text='Virtual Machine Documents',
+                buttons=[PluginMenuButton(
+                    link='plugins:netbox_documents:vmdocument_add',
+                    title='Add',
+                    icon_class='mdi mdi-plus-thick',
+                    color=ButtonColorChoices.GREEN
+                )]
+            )
+        )
+
+    # Add a menu item for Circuit Provider Documents if enabled
+    if plugin_settings.get('enable_circuit_provider_documents'):
+        menuitem.append(
+            PluginMenuItem(
+                link='plugins:netbox_documents:circuitproviderdocument_list',
+                link_text='Circuit Provider Documents',
+                buttons=[PluginMenuButton(
+                    link='plugins:netbox_documents:circuitproviderdocument_add',
+                    title='Add',
+                    icon_class='mdi mdi-plus-thick',
+                    color=ButtonColorChoices.GREEN
+                )]
+            )
+        )
+
     else:
 
         # Fall back to pre 3.4 navigation option
         menu_items = menuitem
```

### Comparing `netbox-documents-0.6.3/netbox_documents/search.py` & `netbox_documents-0.6.4/netbox_documents/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from netbox.search import SearchIndex
-from .models import SiteDocument, LocationDocument, DeviceDocument, DeviceTypeDocument, CircuitDocument 
+from .models import SiteDocument, LocationDocument, DeviceDocument, DeviceTypeDocument, CircuitDocument, VMDocument, CircuitProviderDocument
 from django.conf import settings
 
 # If we run NB 3.4+ register search indexes 
 if settings.VERSION >= '3.4.0':
     class SiteDocumentIndex(SearchIndex):
         model = SiteDocument
         fields = (
@@ -40,9 +40,25 @@
         model = DeviceDocument
         fields = (
             ("name", 100),
             ("document", 500),
             ("comments", 5000),
         )
 
+    class VMDocumentIndex(SearchIndex):
+        model = VMDocument
+        fields = (
+            ("name", 100),
+            ("document", 500),
+            ("comments", 5000),
+        )
+
+    class CircuitProviderDocumentIndex(SearchIndex):
+        model = CircuitProviderDocument
+        fields = (
+            ("name", 100),
+            ("document", 500),
+            ("comments", 5000),
+        )
+
     # Register indexes
-    indexes = [SiteDocumentIndex, LocationDocumentIndex, CircuitDocumentIndex, DeviceTypeDocumentIndex, DeviceDocumentIndex]
+    indexes = [SiteDocumentIndex, LocationDocumentIndex, CircuitDocumentIndex, DeviceTypeDocumentIndex, DeviceDocumentIndex, VMDocumentIndex, CircuitProviderDocumentIndex]
```

### Comparing `netbox-documents-0.6.3/netbox_documents/tables.py` & `netbox_documents-0.6.4/netbox_documents/tables.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import django_tables2 as tables
 
 from netbox.tables import NetBoxTable, columns
-from .models import SiteDocument, LocationDocument, DeviceDocument, DeviceTypeDocument, CircuitDocument 
+from .models import SiteDocument, LocationDocument, DeviceDocument, DeviceTypeDocument, CircuitDocument, VMDocument
 
 SITE_DOCUMENT_LINK = """
 {% if record.size %}
     <a href="{% url 'plugins:netbox_documents:sitedocument' pk=record.pk %}">{% firstof record.name record.filename %}</a> (<a href="{{record.document.url}}" target="_blank">View Document</a>)
 {% else %}
     <a href="{% url 'plugins:netbox_documents:sitedocument' pk=record.pk %}">{% firstof record.name record.filename %}</a> (<a href="{{ record.external_url }}" target="_blank">View External Document</a>)
 {% endif %}
@@ -39,14 +39,30 @@
 {% if record.size %}
     <a href="{% url 'plugins:netbox_documents:devicetypedocument' pk=record.pk %}">{% firstof record.name record.filename %}</a> (<a href="{{record.document.url}}" target="_blank">View Document</a>)
 {% else %}
     <a href="{% url 'plugins:netbox_documents:devicetypedocument' pk=record.pk %}">{% firstof record.name record.filename %}</a> (<a href="{{ record.external_url }}" target="_blank">View External Document</a>)
 {% endif %}
 """
 
+VM_DOCUMENT_LINK = """
+{% if record.size %}
+    <a href="{% url 'plugins:netbox_documents:vmdocument' pk=record.pk %}">{% firstof record.name record.filename %}</a> (<a href="{{record.document.url}}" target="_blank">View Document</a>)
+{% else %}
+    <a href="{% url 'plugins:netbox_documents:vmdocument' pk=record.pk %}">{% firstof record.name record.filename %}</a> (<a href="{{ record.external_url }}" target="_blank">View External Document</a>)
+{% endif %}
+"""
+
+CIRCUIT_PROVIDER_DOCUMENT_LINK = """
+{% if record.size %}
+    <a href="{% url 'plugins:netbox_documents:circuitproviderdocument' pk=record.pk %}">{% firstof record.name record.filename %}</a> (<a href="{{record.document.url}}" target="_blank">View Document</a>)
+{% else %}
+    <a href="{% url 'plugins:netbox_documents:circuitproviderdocument' pk=record.pk %}">{% firstof record.name record.filename %}</a> (<a href="{{ record.external_url }}" target="_blank">View External Document</a>)
+{% endif %}
+"""
+
 class SiteDocumentTable(NetBoxTable):
     name = tables.TemplateColumn(template_code=SITE_DOCUMENT_LINK)
     document_type = columns.ChoiceFieldColumn()
     site = tables.Column(
         linkify=True
     )
 
@@ -121,8 +137,40 @@
     tags = columns.TagColumn(
         url_name='dcim:sitegroup_list'
     )
 
     class Meta(NetBoxTable.Meta):
         model = CircuitDocument
         fields = ('pk', 'id', 'name', 'document_type',  'size', 'filename', 'circuit', 'comments', 'actions', 'created', 'last_updated', 'tags')
-        default_columns = ('name', 'document_type', 'circuit', 'tags')
+        default_columns = ('name', 'document_type', 'circuit', 'tags')
+
+class VMDocumentTable(NetBoxTable):
+    name = tables.TemplateColumn(template_code=VM_DOCUMENT_LINK)
+    document_type = columns.ChoiceFieldColumn()
+    vm = tables.Column(
+        linkify=True
+    )
+
+    tags = columns.TagColumn(
+        url_name='dcim:sitegroup_list'
+    )
+
+    class Meta(NetBoxTable.Meta):
+        model = VMDocument
+        fields = ('pk', 'id', 'name', 'document_type',  'size', 'filename', 'vm', 'comments', 'actions', 'created', 'last_updated', 'tags')
+        default_columns = ('name', 'document_type', 'vm', 'tags')
+
+class CircuitProviderDocumentTable(NetBoxTable):
+    name = tables.TemplateColumn(template_code=CIRCUIT_DOCUMENT_LINK)
+    document_type = columns.ChoiceFieldColumn()
+    provider = tables.Column(
+        linkify=True
+    )
+
+    tags = columns.TagColumn(
+        url_name='dcim:sitegroup_list'
+    )
+
+    class Meta(NetBoxTable.Meta):
+        model = CircuitDocument
+        fields = ('pk', 'id', 'name', 'document_type',  'size', 'filename', 'provider', 'comments', 'actions', 'created', 'last_updated', 'tags')
+        default_columns = ('name', 'document_type', 'provider', 'tags')
```

### Comparing `netbox-documents-0.6.3/netbox_documents/template_content.py` & `netbox_documents-0.6.4/netbox_documents/template_content.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from extras.plugins import PluginTemplateExtension
 from django.conf import settings
-from .models import SiteDocument, LocationDocument, DeviceDocument, DeviceTypeDocument, CircuitDocument 
+from .models import SiteDocument, LocationDocument, DeviceDocument, DeviceTypeDocument, CircuitDocument, VMDocument, CircuitProviderDocument
 
 plugin_settings = settings.PLUGINS_CONFIG.get('netbox_documents', {})
 
 class SiteDocumentList(PluginTemplateExtension):
     model = 'dcim.site'
 
     def left_page(self):
@@ -128,8 +128,59 @@
             return self.render('netbox_documents/circuitdocument_include.html', extra_context={
                 'circuit_documents': CircuitDocument.objects.filter(circuit=self.context['object']),
             })
 
         else:
             return ""
 
-template_extensions = [SiteDocumentList, LocationDocumentList, DeviceDocumentList, DeviceTypeDocumentList, CircuitDocumentList]
+class VMDocumentList(PluginTemplateExtension):
+    model = 'virtualization.virtualmachine'
+
+    def left_page(self):
+
+        if plugin_settings.get('enable_vm_documents') and plugin_settings.get('vm_documents_location') == 'left':
+
+            return self.render('netbox_documents/vmdocument_include.html', extra_context={
+                'vm_documents': VMDocument.objects.filter(vm=self.context['object']),
+            })
+
+        else:
+            return ""
+
+    def right_page(self):
+
+        if plugin_settings.get('enable_vm_documents') and plugin_settings.get('vm_documents_location') == 'right':
+
+            return self.render('netbox_documents/vmdocument_include.html', extra_context={
+                'vm_documents': VMDocument.objects.filter(vm=self.context['object']),
+            })
+
+        else:
+            return ""
+
+class CircuitProviderDocumentList(PluginTemplateExtension):
+    model = 'circuits.provider'
+
+    def left_page(self):
+
+        if plugin_settings.get('enable_circuit_provider_documents') and plugin_settings.get('circuit_provider_documents_location') == 'left':
+
+            return self.render('netbox_documents/circuitproviderdocument_include.html', extra_context={
+                'circuit_provider_documents': CircuitProviderDocument.objects.filter(provider=self.context['object']),
+            })
+
+        else:
+            return ""
+
+    def right_page(self):
+
+        if plugin_settings.get('enable_circuit_provider_documents') and plugin_settings.get('circuit_provider_documents_location') == 'right':
+
+            return self.render('netbox_documents/circuitproviderdocument_include.html', extra_context={
+                'circuit_provider_documents': CircuitProviderDocument.objects.filter(provider=self.context['object']),
+            })
+
+        else:
+            return ""
+
+
+template_extensions = [SiteDocumentList, LocationDocumentList, DeviceDocumentList, DeviceTypeDocumentList, CircuitDocumentList, VMDocumentList, CircuitProviderDocumentList]
```

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/circuitdocument.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/circuitdocument.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/circuitdocument_edit.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/circuitdocument_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/circuitdocument_include.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/circuitdocument_include.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/devicedocument.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/devicedocument.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/devicedocument_edit.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/devicedocument_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/devicedocument_include.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/devicedocument_include.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/devicetypedocument.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/devicetypedocument.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/devicetypedocument_edit.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/devicetypedocument_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/devicetypedocument_include.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/devicetypedocument_include.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/document_edit.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/document_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/locationdocument.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/locationdocument.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/locationdocument_edit.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/locationdocument_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/locationdocument_include.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/locationdocument_include.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/sitedocument.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/sitedocument.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/sitedocument_edit.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/sitedocument_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/templates/netbox_documents/sitedocument_include.html` & `netbox_documents-0.6.4/netbox_documents/templates/netbox_documents/sitedocument_include.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.6.3/netbox_documents/urls.py` & `netbox_documents-0.6.4/netbox_documents/urls.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,10 +50,30 @@
     path('circuit-document/add/', views.CircuitDocumentEditView.as_view(), name='circuitdocument_add'),
     path('circuit-document/<int:pk>/', views.CircuitDocumentView.as_view(), name='circuitdocument'),
     path('circuit-document/<int:pk>/edit/', views.CircuitDocumentEditView.as_view(), name='circuitdocument_edit'),
     path('circuit-document/<int:pk>/delete/', views.CircuitDocumentDeleteView.as_view(), name='circuitdocument_delete'),
     path('circuit-document/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='circuitdocument_changelog', kwargs={
         'model': models.CircuitDocument
     }), 
+
+    # VMDocument
+    path('vm-document/', views.VMDocumentListView.as_view(), name='vmdocument_list'),
+    path('vm-document/add/', views.VMDocumentEditView.as_view(), name='vmdocument_add'),
+    path('vm-document/<int:pk>/', views.VMDocumentView.as_view(), name='vmdocument'),
+    path('vm-document/<int:pk>/edit/', views.VMDocumentEditView.as_view(), name='vmdocument_edit'),
+    path('vm-document/<int:pk>/delete/', views.VMDocumentDeleteView.as_view(), name='vmdocument_delete'),
+    path('vm-document/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='vmdocument_changelog', kwargs={
+        'model': models.VMDocument
+    }), 
+
+    # CircuitProviderDocument
+    path('circuitprovider-document/', views.CircuitProviderDocumentListView.as_view(), name='circuitproviderdocument_list'),
+    path('circuitprovider-document/add/', views.CircuitProviderDocumentEditView.as_view(), name='circuitproviderdocument_add'),
+    path('circuitprovider-document/<int:pk>/', views.CircuitProviderDocumentView.as_view(), name='circuitproviderdocument'),
+    path('circuitprovider-document/<int:pk>/edit/', views.CircuitProviderDocumentEditView.as_view(), name='circuitproviderdocument_edit'),
+    path('circuitprovider-document/<int:pk>/delete/', views.CircuitProviderDocumentDeleteView.as_view(), name='circuitproviderdocument_delete'),
+    path('circuitprovider-document/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='circuitproviderdocument_changelog', kwargs={
+        'model': models.CircuitProviderDocument
+    }),    
     
 
 )
```

### Comparing `netbox-documents-0.6.3/netbox_documents/utils.py` & `netbox_documents-0.6.4/netbox_documents/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,18 @@
         path_prepend = instance.location.id
     if hasattr(instance, 'device'):
         path_prepend = instance.device.id
     if hasattr(instance, 'device_type'): 
         path_prepend = instance.device_type.id
     if hasattr(instance, 'circuit'):
         path_prepend = instance.circuit.id
+    if hasattr(instance, 'vm'):
+        path_prepend = instance.vm.id
+    if hasattr(instance, 'provider'):
+        path_prepend = instance.provider.id
 
     # Rename the file to the provided name, if any. Attempt to preserve the file extension.
     extension = filename.rsplit('.')[-1].lower()
     if instance.name and extension in ['bmp', 'gif', 'jpeg', 'jpg', 'png', 'pdf', 'txt', 'doc', 'docx', 'xls', 'xlsx', 'xlsm', 'tif', 'tiff']:
         filename = '.'.join([instance.name, extension])
     elif instance.name:
         filename = instance.name
```

### Comparing `netbox-documents-0.6.3/netbox_documents/views.py` & `netbox_documents-0.6.4/netbox_documents/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -94,8 +94,47 @@
 class CircuitDocumentEditView(generic.ObjectEditView):
     queryset = models.CircuitDocument.objects.all()
     form = forms.CircuitDocumentForm
 
     template_name = 'netbox_documents/circuitdocument_edit.html'
 
 class CircuitDocumentDeleteView(generic.ObjectDeleteView):
-    queryset = models.CircuitDocument.objects.all()
+    queryset = models.CircuitDocument.objects.all()
+
+
+### VMDocument
+class VMDocumentView(generic.ObjectView):
+    queryset = models.VMDocument.objects.all()
+
+class VMDocumentListView(generic.ObjectListView):
+    queryset = models.VMDocument.objects.all()
+    table = tables.VMDocumentTable
+    filterset = filtersets.VMDocumentFilterSet
+    filterset_form = forms.VMDocumentFilterForm
+
+class VMDocumentEditView(generic.ObjectEditView):
+    queryset = models.VMDocument.objects.all()
+    form = forms.VMDocumentForm
+
+    template_name = 'netbox_documents/vmdocument_edit.html'
+
+class VMDocumentDeleteView(generic.ObjectDeleteView):
+    queryset = models.VMDocument.objects.all()
+
+### CircuitProviderDocument
+class CircuitProviderDocumentView(generic.ObjectView):
+    queryset = models.CircuitProviderDocument.objects.all()
+
+class CircuitProviderDocumentListView(generic.ObjectListView):
+    queryset = models.CircuitProviderDocument.objects.all()
+    table = tables.CircuitProviderDocumentTable
+    filterset = filtersets.CircuitProviderDocumentFilterSet
+    filterset_form = forms.CircuitProviderDocumentFilterForm
+
+class CircuitProviderDocumentEditView(generic.ObjectEditView):
+    queryset = models.CircuitProviderDocument.objects.all()
+    form = forms.CircuitProviderDocumentForm
+
+    template_name = 'netbox_documents/circuitproviderdocument_edit.html'
+
+class CircuitProviderDocumentDeleteView(generic.ObjectDeleteView):
+    queryset = models.CircuitProviderDocument.objects.all()
```

### Comparing `netbox-documents-0.6.3/netbox_documents.egg-info/PKG-INFO` & `netbox_documents-0.6.4/netbox_documents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-documents
-Version: 0.6.3
+Version: 0.6.4
 Summary: Manage site, location, circuit and device diagrams and documents in Netbox
 Home-page: https://github.com/jasonyates/netbox-documents
 Author: Jason Yates
 Author-email: me@jasonyates.co.uk
 Keywords: netbox,netbox-plugin,plugin
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,25 +18,27 @@
 
 * Store documents against the following NetBox models:
    - Circuits
    - Devices
    - Device Types
    - Sites
    - Locations
+   - Virtual Machines
+   - Circuit Providers
 
 * Upload documents to your NetBox media/ folder or other Django supported storage method e.g. S3
 * Supports a wide array of common file types (bmp, gif, jpeg, jpg, png, pdf, txt, doc, docx, xls, xlsx, xlsm)
 * Store links to external URL's to save duplication of remote documents
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.6+       |      0.6.3     |
+|     3.6+       |      0.6.4     |
 |     3.5.x      |      0.6.0     |
 | 3.3.x - 3.4.x  |      0.5.1     |
 
 
 ## Installation
 
 A working installation of Netbox 3.3+ is required. 3.6+ is recommended. **NOTE: Netbox 3.5 introduced breaking changes for plugins, please use the correct plugin version for your netbox install.**
```

### Comparing `netbox-documents-0.6.3/netbox_documents.egg-info/SOURCES.txt` & `netbox_documents-0.6.4/netbox_documents.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements.txt
 setup.py
 netbox_documents/__init__.py
 netbox_documents/filtersets.py
 netbox_documents/forms.py
 netbox_documents/models.py
 netbox_documents/navigation.py
 netbox_documents/search.py
@@ -25,24 +26,32 @@
 netbox_documents/api/urls.py
 netbox_documents/api/views.py
 netbox_documents/migrations/0001_initial.py
 netbox_documents/migrations/0002_AddDeviceType.py
 netbox_documents/migrations/0003_alter_circuitdocument_options_and_more.py
 netbox_documents/migrations/0004_locationdocument.py
 netbox_documents/migrations/0005_alter_circuitdocument_external_url_and_more.py
+netbox_documents/migrations/0006_vmdocument.py
+netbox_documents/migrations/0007_circuitproviderdocument.py
 netbox_documents/migrations/__init__.py
 netbox_documents/templates/netbox_documents/circuitdocument.html
 netbox_documents/templates/netbox_documents/circuitdocument_edit.html
 netbox_documents/templates/netbox_documents/circuitdocument_include.html
+netbox_documents/templates/netbox_documents/circuitproviderdocument.html
+netbox_documents/templates/netbox_documents/circuitproviderdocument_edit.html
+netbox_documents/templates/netbox_documents/circuitproviderdocument_include.html
 netbox_documents/templates/netbox_documents/devicedocument.html
 netbox_documents/templates/netbox_documents/devicedocument_edit.html
 netbox_documents/templates/netbox_documents/devicedocument_include.html
 netbox_documents/templates/netbox_documents/devicetypedocument.html
 netbox_documents/templates/netbox_documents/devicetypedocument_edit.html
 netbox_documents/templates/netbox_documents/devicetypedocument_include.html
 netbox_documents/templates/netbox_documents/document_edit.html
 netbox_documents/templates/netbox_documents/locationdocument.html
 netbox_documents/templates/netbox_documents/locationdocument_edit.html
 netbox_documents/templates/netbox_documents/locationdocument_include.html
 netbox_documents/templates/netbox_documents/sitedocument.html
 netbox_documents/templates/netbox_documents/sitedocument_edit.html
-netbox_documents/templates/netbox_documents/sitedocument_include.html
+netbox_documents/templates/netbox_documents/sitedocument_include.html
+netbox_documents/templates/netbox_documents/vmdocument.html
+netbox_documents/templates/netbox_documents/vmdocument_edit.html
+netbox_documents/templates/netbox_documents/vmdocument_include.html
```

### Comparing `netbox-documents-0.6.3/setup.py` & `netbox_documents-0.6.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from setuptools import find_packages, setup
 
 from os import path
 top_level_directory = path.abspath(path.dirname(__file__))
 with open(path.join(top_level_directory, 'README.md'), encoding='utf-8') as file:
     long_description = file.read()
 
+with open(path.join(top_level_directory, 'requirements.txt')) as file:
+    required = file.read().splitlines()
 
 setup(
     name='netbox-documents',
-    version='0.6.3',
+    version='0.6.4',
     description='Manage site, location, circuit and device diagrams and documents in Netbox',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jason Yates',
     author_email='me@jasonyates.co.uk',
     url='https://github.com/jasonyates/netbox-documents',
-    install_requires=["drf_extra_fields>=3.7.0"],
+    install_requires=required,
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     keywords=['netbox', 'netbox-plugin', 'plugin'],
 )
```

