# Comparing `tmp/pih-plb-0.16.tar.gz` & `tmp/pih-plb-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb-0.16.tar", last modified: Wed Apr 17 06:01:55 2024, max compression
+gzip compressed data, was "pih-plb-0.17.tar", last modified: Wed Apr 17 06:42:11 2024, max compression
```

## Comparing `pih-plb-0.16.tar` & `pih-plb-0.17.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 06:01:55.706368 pih-plb-0.16/
--rw-rw-rw-   0        0        0      293 2024-04-17 06:01:55.659489 pih-plb-0.16/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 06:01:55.298030 pih-plb-0.16/PolibaseService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.16/PolibaseService/__init__.py
--rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.16/PolibaseService/__main__.py
--rw-rw-rw-   0        0        0    45743 2024-04-16 23:44:39.000000 pih-plb-0.16/PolibaseService/api.py
--rw-rw-rw-   0        0        0     3618 2024-04-17 05:59:44.000000 pih-plb-0.16/PolibaseService/const.py
--rw-rw-rw-   0        0        0    14873 2024-04-16 23:48:02.000000 pih-plb-0.16/PolibaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:01:55.628245 pih-plb-0.16/pih_plb.egg-info/
--rw-rw-rw-   0        0        0      293 2024-04-17 06:01:54.000000 pih-plb-0.16/pih_plb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-04-17 06:01:55.000000 pih-plb-0.16/pih_plb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 06:01:54.000000 pih-plb-0.16/pih_plb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-17 06:01:54.000000 pih-plb-0.16/pih_plb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-17 06:01:54.000000 pih-plb-0.16/pih_plb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-17 06:01:54.000000 pih-plb-0.16/pih_plb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 06:01:55.706368 pih-plb-0.16/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 06:42:11.233410 pih-plb-0.17/
+-rw-rw-rw-   0        0        0      293 2024-04-17 06:42:11.202164 pih-plb-0.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 06:42:10.805558 pih-plb-0.17/PolibaseService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.17/PolibaseService/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.17/PolibaseService/__main__.py
+-rw-rw-rw-   0        0        0    45741 2024-04-17 06:41:11.000000 pih-plb-0.17/PolibaseService/api.py
+-rw-rw-rw-   0        0        0     3618 2024-04-17 06:41:18.000000 pih-plb-0.17/PolibaseService/const.py
+-rw-rw-rw-   0        0        0    14873 2024-04-16 23:48:02.000000 pih-plb-0.17/PolibaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:42:11.170941 pih-plb-0.17/pih_plb.egg-info/
+-rw-rw-rw-   0        0        0      293 2024-04-17 06:42:10.000000 pih-plb-0.17/pih_plb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-17 06:42:10.000000 pih-plb-0.17/pih_plb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:42:10.000000 pih-plb-0.17/pih_plb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-17 06:42:10.000000 pih-plb-0.17/pih_plb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-17 06:42:10.000000 pih-plb-0.17/pih_plb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-17 06:42:10.000000 pih-plb-0.17/pih_plb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 06:42:11.249051 pih-plb-0.17/setup.cfg
```

### Comparing `pih-plb-0.16/PolibaseService/api.py` & `pih-plb-0.17/PolibaseService/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import oracledb
 from oracledb import SessionPool, DatabaseError, Cursor
 
 import ipih
 from pih import A, PIHThread
 from PolibaseService.const import HOST
 
-if not A.D.contains(A.SYS.host(), HOST.name):
-    oracledb.init_oracle_client(lib_dir=r"C:\instantclient")
+#if not A.D.contains(A.SYS.host(), HOST.name):
+#oracledb.init_oracle_client(lib_dir=r"C:\instantclient")
 
 
 from pih.consts.errors import Error
 from PolibaseService.const import *
 from pih.collections import (
     PolibasePersonVisit,
     PolibasePersonVisitSearchCritery,
```

### Comparing `pih-plb-0.16/PolibaseService/const.py` & `pih-plb-0.17/PolibaseService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih import A
 from pih.tools import j
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Polibase"
 
-VERSION: str = "0.16"
+VERSION: str = "0.17"
 
 HOST = A.CT_H.POLIBASE
 
 PACKAGES: tuple[str, ...] = ("oracledb",)
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
```

### Comparing `pih-plb-0.16/PolibaseService/service.py` & `pih-plb-0.17/PolibaseService/service.py`

 * *Files identical despite different names*

