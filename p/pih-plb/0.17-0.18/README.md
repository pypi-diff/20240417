# Comparing `tmp/pih-plb-0.17.tar.gz` & `tmp/pih-plb-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb-0.17.tar", last modified: Wed Apr 17 06:42:11 2024, max compression
+gzip compressed data, was "pih-plb-0.18.tar", last modified: Wed Apr 17 06:51:15 2024, max compression
```

## Comparing `pih-plb-0.17.tar` & `pih-plb-0.18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 06:42:11.233410 pih-plb-0.17/
--rw-rw-rw-   0        0        0      293 2024-04-17 06:42:11.202164 pih-plb-0.17/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 06:42:10.805558 pih-plb-0.17/PolibaseService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.17/PolibaseService/__init__.py
--rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.17/PolibaseService/__main__.py
--rw-rw-rw-   0        0        0    45741 2024-04-17 06:41:11.000000 pih-plb-0.17/PolibaseService/api.py
--rw-rw-rw-   0        0        0     3618 2024-04-17 06:41:18.000000 pih-plb-0.17/PolibaseService/const.py
--rw-rw-rw-   0        0        0    14873 2024-04-16 23:48:02.000000 pih-plb-0.17/PolibaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:42:11.170941 pih-plb-0.17/pih_plb.egg-info/
--rw-rw-rw-   0        0        0      293 2024-04-17 06:42:10.000000 pih-plb-0.17/pih_plb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-04-17 06:42:10.000000 pih-plb-0.17/pih_plb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 06:42:10.000000 pih-plb-0.17/pih_plb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-17 06:42:10.000000 pih-plb-0.17/pih_plb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-17 06:42:10.000000 pih-plb-0.17/pih_plb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-17 06:42:10.000000 pih-plb-0.17/pih_plb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 06:42:11.249051 pih-plb-0.17/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 06:51:16.050047 pih-plb-0.18/
+-rw-rw-rw-   0        0        0      293 2024-04-17 06:51:16.003171 pih-plb-0.18/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 06:51:15.627162 pih-plb-0.18/PolibaseService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.18/PolibaseService/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.18/PolibaseService/__main__.py
+-rw-rw-rw-   0        0        0    45741 2024-04-17 06:41:11.000000 pih-plb-0.18/PolibaseService/api.py
+-rw-rw-rw-   0        0        0     3618 2024-04-17 06:50:29.000000 pih-plb-0.18/PolibaseService/const.py
+-rw-rw-rw-   0        0        0    14907 2024-04-17 06:50:17.000000 pih-plb-0.18/PolibaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:51:15.971921 pih-plb-0.18/pih_plb.egg-info/
+-rw-rw-rw-   0        0        0      293 2024-04-17 06:51:14.000000 pih-plb-0.18/pih_plb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-17 06:51:14.000000 pih-plb-0.18/pih_plb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:51:14.000000 pih-plb-0.18/pih_plb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-17 06:51:14.000000 pih-plb-0.18/pih_plb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-17 06:51:14.000000 pih-plb-0.18/pih_plb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-17 06:51:14.000000 pih-plb-0.18/pih_plb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 06:51:16.065668 pih-plb-0.18/setup.cfg
```

### Comparing `pih-plb-0.17/PolibaseService/api.py` & `pih-plb-0.18/PolibaseService/api.py`

 * *Files identical despite different names*

### Comparing `pih-plb-0.17/PolibaseService/const.py` & `pih-plb-0.18/PolibaseService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih import A
 from pih.tools import j
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Polibase"
 
-VERSION: str = "0.17"
+VERSION: str = "0.18"
 
 HOST = A.CT_H.POLIBASE
 
 PACKAGES: tuple[str, ...] = ("oracledb",)
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
```

### Comparing `pih-plb-0.17/PolibaseService/service.py` & `pih-plb-0.18/PolibaseService/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,18 +299,20 @@
 
         def service_starts_handler() -> None:
             Api.init(DEBUG)
             Api.on_note_emailed_update_handler = on_note_emailed_update_handler
             Api.on_person_creation_or_update_handler = (
                 on_person_creation_or_update_handler
             )
+            Api.on_person_saldo_update_handler = on_person_saldo_update_handler
+            return 
             last_id: int | None = A.D_V.value(LAST_SALDO_OPERATION_ID_NAME, section=SD.name)
             if nn(last_id):
                 A.D.every(on_person_saldo_update_handler, Api.get_person_saldo_after_id(nnt(last_id)))
-            Api.on_person_saldo_update_handler = on_person_saldo_update_handler
+           
 
         A.SRV_A.serve(
             SD,
             service_call_handler,
             service_starts_handler,
             isolate=ISOLATED,
             as_standalone=as_standalone,
```

