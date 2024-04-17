# Comparing `tmp/pih-plb-0.19.tar.gz` & `tmp/pih-plb-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb-0.19.tar", last modified: Wed Apr 17 13:39:24 2024, max compression
+gzip compressed data, was "pih-plb-0.20.tar", last modified: Wed Apr 17 14:42:04 2024, max compression
```

## Comparing `pih-plb-0.19.tar` & `pih-plb-0.20.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 13:39:24.502004 pih-plb-0.19/
--rw-rw-rw-   0        0        0      293 2024-04-17 13:39:24.455132 pih-plb-0.19/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 13:39:24.007730 pih-plb-0.19/PolibaseService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.19/PolibaseService/__init__.py
--rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.19/PolibaseService/__main__.py
--rw-rw-rw-   0        0        0    45743 2024-04-17 06:56:35.000000 pih-plb-0.19/PolibaseService/api.py
--rw-rw-rw-   0        0        0     3618 2024-04-17 13:38:42.000000 pih-plb-0.19/PolibaseService/const.py
--rw-rw-rw-   0        0        0    14886 2024-04-17 13:38:35.000000 pih-plb-0.19/PolibaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-17 13:39:24.423882 pih-plb-0.19/pih_plb.egg-info/
--rw-rw-rw-   0        0        0      293 2024-04-17 13:39:23.000000 pih-plb-0.19/pih_plb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-04-17 13:39:23.000000 pih-plb-0.19/pih_plb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 13:39:23.000000 pih-plb-0.19/pih_plb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-17 13:39:23.000000 pih-plb-0.19/pih_plb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-17 13:39:23.000000 pih-plb-0.19/pih_plb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-17 13:39:23.000000 pih-plb-0.19/pih_plb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 13:39:24.518998 pih-plb-0.19/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 14:42:04.564057 pih-plb-0.20/
+-rw-rw-rw-   0        0        0      293 2024-04-17 14:42:04.548434 pih-plb-0.20/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 14:42:04.170349 pih-plb-0.20/PolibaseService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.20/PolibaseService/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.20/PolibaseService/__main__.py
+-rw-rw-rw-   0        0        0    45781 2024-04-17 14:41:03.000000 pih-plb-0.20/PolibaseService/api.py
+-rw-rw-rw-   0        0        0     3618 2024-04-17 14:41:15.000000 pih-plb-0.20/PolibaseService/const.py
+-rw-rw-rw-   0        0        0    14886 2024-04-17 13:38:35.000000 pih-plb-0.20/PolibaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:42:04.501557 pih-plb-0.20/pih_plb.egg-info/
+-rw-rw-rw-   0        0        0      293 2024-04-17 14:42:03.000000 pih-plb-0.20/pih_plb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-17 14:42:03.000000 pih-plb-0.20/pih_plb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 14:42:03.000000 pih-plb-0.20/pih_plb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-17 14:42:03.000000 pih-plb-0.20/pih_plb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-17 14:42:03.000000 pih-plb-0.20/pih_plb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-17 14:42:03.000000 pih-plb-0.20/pih_plb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 14:42:04.579679 pih-plb-0.20/setup.cfg
```

### Comparing `pih-plb-0.19/PolibaseService/api.py` & `pih-plb-0.20/PolibaseService/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import oracledb
 from oracledb import SessionPool, DatabaseError, Cursor
 
 import ipih
 from pih import A, PIHThread
 from PolibaseService.const import HOST
 
-if not A.D.contains(A.SYS.host(), HOST.name):
+if A.D.contains(A.SYS.host(), HOST.name):
+    oracledb.init_oracle_client()
+else:
     oracledb.init_oracle_client(lib_dir=r"C:\instantclient")
 
 
 from pih.consts.errors import Error
 from PolibaseService.const import *
 from pih.collections import (
     PolibasePersonVisit,
```

### Comparing `pih-plb-0.19/PolibaseService/const.py` & `pih-plb-0.20/PolibaseService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih import A
 from pih.tools import j
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Polibase"
 
-VERSION: str = "0.19"
+VERSION: str = "0.20"
 
 HOST = A.CT_H.POLIBASE
 
 PACKAGES: tuple[str, ...] = ("oracledb",)
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
```

### Comparing `pih-plb-0.19/PolibaseService/service.py` & `pih-plb-0.20/PolibaseService/service.py`

 * *Files identical despite different names*

