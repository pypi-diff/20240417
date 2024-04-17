# Comparing `tmp/yente-3.8.7.tar.gz` & `tmp/yente-3.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yente-3.8.7.tar", last modified: Wed Apr 17 08:16:31 2024, max compression
+gzip compressed data, was "yente-3.8.8.tar", last modified: Wed Apr 17 08:16:54 2024, max compression
```

## Comparing `yente-3.8.7.tar` & `yente-3.8.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:31.707814 yente-3.8.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 08:14:51.000000 yente-3.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-17 08:14:51.000000 yente-3.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-17 08:16:31.707814 yente-3.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-17 08:14:51.000000 yente-3.8.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:16:31.707814 yente-3.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-17 08:14:51.000000 yente-3.8.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:31.699814 yente-3.8.7/yente/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:14:51.000000 yente-3.8.7/yente/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-17 08:14:51.000000 yente-3.8.7/yente/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-17 08:14:51.000000 yente-3.8.7/yente/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:31.703814 yente-3.8.7/yente/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-17 08:14:51.000000 yente-3.8.7/yente/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-17 08:14:51.000000 yente-3.8.7/yente/data/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-17 08:14:51.000000 yente-3.8.7/yente/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-17 08:14:51.000000 yente-3.8.7/yente/data/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-17 08:14:51.000000 yente-3.8.7/yente/data/freebase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-17 08:14:51.000000 yente-3.8.7/yente/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-17 08:14:51.000000 yente-3.8.7/yente/data/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-17 08:14:51.000000 yente-3.8.7/yente/data/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-17 08:14:51.000000 yente-3.8.7/yente/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:14:51.000000 yente-3.8.7/yente/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-17 08:14:51.000000 yente-3.8.7/yente/reindex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:31.703814 yente-3.8.7/yente/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-17 08:14:51.000000 yente-3.8.7/yente/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:31.703814 yente-3.8.7/yente/routers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:14:51.000000 yente-3.8.7/yente/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-17 08:14:51.000000 yente-3.8.7/yente/routers/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-17 08:14:51.000000 yente-3.8.7/yente/routers/match.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-04-17 08:14:51.000000 yente-3.8.7/yente/routers/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-17 08:14:51.000000 yente-3.8.7/yente/routers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-17 08:14:51.000000 yente-3.8.7/yente/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 08:14:51.000000 yente-3.8.7/yente/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:31.707814 yente-3.8.7/yente/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:14:51.000000 yente-3.8.7/yente/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-17 08:14:51.000000 yente-3.8.7/yente/search/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-17 08:14:51.000000 yente-3.8.7/yente/search/indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-17 08:14:51.000000 yente-3.8.7/yente/search/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-17 08:14:51.000000 yente-3.8.7/yente/search/nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-17 08:14:51.000000 yente-3.8.7/yente/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-17 08:14:51.000000 yente-3.8.7/yente/search/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-17 08:14:51.000000 yente-3.8.7/yente/search/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 08:14:51.000000 yente-3.8.7/yente/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-17 08:14:51.000000 yente-3.8.7/yente/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-17 08:14:51.000000 yente-3.8.7/yente/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:31.707814 yente-3.8.7/yente.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-17 08:16:31.000000 yente-3.8.7/yente.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-17 08:16:31.000000 yente-3.8.7/yente.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:16:31.000000 yente-3.8.7/yente.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 08:16:31.000000 yente-3.8.7/yente.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:16:31.000000 yente-3.8.7/yente.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:15:43.000000 yente-3.8.7/yente.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-17 08:16:31.000000 yente-3.8.7/yente.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 08:16:31.000000 yente-3.8.7/yente.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.137381 yente-3.8.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 08:15:08.000000 yente-3.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-17 08:15:08.000000 yente-3.8.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-17 08:16:54.137381 yente-3.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-17 08:15:08.000000 yente-3.8.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:16:54.137381 yente-3.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-17 08:15:08.000000 yente-3.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.129381 yente-3.8.8/yente/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:15:08.000000 yente-3.8.8/yente/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-17 08:15:08.000000 yente-3.8.8/yente/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-17 08:15:08.000000 yente-3.8.8/yente/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.133381 yente-3.8.8/yente/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/freebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-17 08:15:08.000000 yente-3.8.8/yente/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:15:08.000000 yente-3.8.8/yente/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-17 08:15:08.000000 yente-3.8.8/yente/reindex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.133381 yente-3.8.8/yente/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-17 08:15:08.000000 yente-3.8.8/yente/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.133381 yente-3.8.8/yente/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:15:08.000000 yente-3.8.8/yente/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-17 08:15:08.000000 yente-3.8.8/yente/routers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-17 08:15:08.000000 yente-3.8.8/yente/routers/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-04-17 08:15:08.000000 yente-3.8.8/yente/routers/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-17 08:15:08.000000 yente-3.8.8/yente/routers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-17 08:15:08.000000 yente-3.8.8/yente/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 08:15:08.000000 yente-3.8.8/yente/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.137381 yente-3.8.8/yente/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 08:15:08.000000 yente-3.8.8/yente/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-17 08:15:08.000000 yente-3.8.8/yente/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-17 08:15:08.000000 yente-3.8.8/yente/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.137381 yente-3.8.8/yente.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:16:01.000000 yente-3.8.8/yente.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/top_level.txt
```

### Comparing `yente-3.8.7/LICENSE` & `yente-3.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/PKG-INFO` & `yente-3.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.8.7
+Version: 3.8.8
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: followthemoney==3.5.9
```

### Comparing `yente-3.8.7/README.md` & `yente-3.8.8/README.md`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/setup.py` & `yente-3.8.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="yente",
-    version="3.8.7",
+    version="3.8.8",
     url="https://opensanctions.org/docs/api/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="OpenSanctions",
     author_email="info@opensanctions.org",
     packages=find_packages(exclude=["examples", "tests"]),
```

### Comparing `yente-3.8.7/yente/app.py` & `yente-3.8.8/yente/app.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/cli.py` & `yente-3.8.8/yente/cli.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/data/__init__.py` & `yente-3.8.8/yente/data/__init__.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/data/common.py` & `yente-3.8.8/yente/data/common.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/data/dataset.py` & `yente-3.8.8/yente/data/dataset.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/data/entity.py` & `yente-3.8.8/yente/data/entity.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/data/freebase.py` & `yente-3.8.8/yente/data/freebase.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/data/loader.py` & `yente-3.8.8/yente/data/loader.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/data/manifest.py` & `yente-3.8.8/yente/data/manifest.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/data/util.py` & `yente-3.8.8/yente/data/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from prefixdate.precision import Precision
 from contextlib import asynccontextmanager
 from typing import AsyncGenerator, Dict, List, Iterable, Optional, Set
 from rigour.text.scripts import is_modern_alphabet
 from rigour.text.distance import levenshtein
 from fingerprints import remove_types, clean_name_light
 from nomenklatura.util import fingerprint_name, names_word_list
+from yente.settings import HTTP_PROXY
 
 
 @lru_cache(maxsize=5000)
 def _metaphone_cached(word: str) -> str:
     return metaphone(word)
 
 
@@ -126,11 +127,12 @@
         return path
     return None
 
 
 @asynccontextmanager
 async def httpx_session() -> AsyncGenerator[httpx.AsyncClient, None]:
     transport = httpx.AsyncHTTPTransport(retries=3)
+    proxy = HTTP_PROXY if HTTP_PROXY != "" else None
     async with httpx.AsyncClient(
-        transport=transport, http2=True, timeout=None
+        transport=transport, http2=True, timeout=None, proxy=proxy
     ) as client:
         yield client
```

### Comparing `yente-3.8.7/yente/logs.py` & `yente-3.8.8/yente/logs.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/resources/favicon.ico` & `yente-3.8.8/yente/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/routers/admin.py` & `yente-3.8.8/yente/routers/admin.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/routers/match.py` & `yente-3.8.8/yente/routers/match.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,17 @@
         title="Score threshold for results to be considered matches",
     ),
     cutoff: float = Query(
         settings.SCORE_CUTOFF,
         title="Lower bound of score for results to be returned at all",
     ),
     algorithm: str = Query(settings.DEFAULT_ALGORITHM, title=ALGO_HELP),
+    include_dataset: List[str] = Query(
+        [], title="Only include the given datasets in results"
+    ),
     exclude_schema: List[str] = Query(
         [], title="Remove the given types of entities from results"
     ),
     exclude_dataset: List[str] = Query(
         [], title="Remove the given datasets from results"
     ),
     topics: List[str] = Query(
@@ -140,14 +143,15 @@
         try:
             entity = Entity.from_example(example)
             query = entity_query(
                 ds,
                 entity,
                 filters=filters,
                 fuzzy=fuzzy,
+                include_dataset=include_dataset,
                 exclude_schema=exclude_schema,
                 exclude_dataset=exclude_dataset,
                 changed_since=changed_since,
             )
         except Exception as exc:
             log.info("Cannot parse example entity: %s" % str(exc))
             raise HTTPException(
```

### Comparing `yente-3.8.7/yente/routers/reconcile.py` & `yente-3.8.8/yente/routers/reconcile.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/routers/search.py` & `yente-3.8.8/yente/routers/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,17 @@
 async def search(
     response: Response,
     q: str = Query("", title="Query text"),
     dataset: str = PATH_DATASET,
     schema: str = Query(
         settings.BASE_SCHEMA, title="Types of entities that can match the search"
     ),
+    include_dataset: List[str] = Query(
+        [], title="Only include the given datasets in results"
+    ),
     exclude_schema: List[str] = Query(
         [], title="Remove the given types of entities from results"
     ),
     exclude_dataset: List[str] = Query(
         [], title="Remove the given datasets from results"
     ),
     changed_since: Optional[str] = Query(
@@ -105,14 +108,15 @@
     query = text_query(
         ds,
         schema_obj,
         q,
         filters=filters,
         fuzzy=fuzzy,
         simple=simple,
+        include_dataset=include_dataset,
         exclude_schema=exclude_schema,
         exclude_dataset=exclude_dataset,
         changed_since=changed_since,
     )
     aggregations = facet_aggregations([f.value for f in facets])
     resp = await search_entities(
         query,
```

### Comparing `yente-3.8.7/yente/routers/util.py` & `yente-3.8.8/yente/routers/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/scoring.py` & `yente-3.8.8/yente/scoring.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/search/base.py` & `yente-3.8.8/yente/search/base.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/search/indexer.py` & `yente-3.8.8/yente/search/indexer.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/search/mapping.py` & `yente-3.8.8/yente/search/mapping.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/search/nested.py` & `yente-3.8.8/yente/search/nested.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/search/queries.py` & `yente-3.8.8/yente/search/queries.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,21 +17,27 @@
 
 
 def filter_query(
     shoulds: List[Clause],
     dataset: Optional[Dataset] = None,
     schema: Optional[Schema] = None,
     filters: FilterDict = {},
+    include_dataset: List[str] = [],
     exclude_schema: List[str] = [],
     exclude_dataset: List[str] = [],
     changed_since: Optional[str] = None,
 ) -> Clause:
     filterqs: List[Clause] = []
     if dataset is not None:
-        ds = [d for d in dataset.dataset_names if d not in exclude_dataset]
+        ds = [
+            d
+            for d in dataset.dataset_names
+            if (len(include_dataset) == 0 or d in include_dataset)
+            and d not in exclude_dataset
+        ]
         filterqs.append({"terms": {"datasets": ds}})
     if schema is not None:
         schemata = schema.matchable_schemata
         if not schema.matchable:
             schemata.update(schema.descendants)
         names = [s.name for s in schemata]
         filterqs.append({"terms": {"schema": names}})
@@ -72,27 +78,28 @@
         if fuzzy:
             match[NAMES_FIELD]["fuzziness"] = "AUTO"
         shoulds.append({"match": match})
     for key in index_name_keys(names):
         term = {NAME_KEY_FIELD: {"value": key, "boost": 4.0}}
         shoulds.append({"term": term})
     for token in set(index_name_parts(names)):
-        term = {NAME_PART_FIELD: {"value": token, 'boost': 1.0}}
+        term = {NAME_PART_FIELD: {"value": token, "boost": 1.0}}
         shoulds.append({"term": term})
     for phoneme in set(phonetic_names(names)):
         term = {NAME_PHONETIC_FIELD: {"value": phoneme, "boost": 0.8}}
         shoulds.append({"term": term})
     return shoulds
 
 
 def entity_query(
     dataset: Dataset,
     entity: EntityProxy,
     filters: FilterDict = {},
     fuzzy: bool = True,
+    include_dataset: List[str] = [],
     exclude_schema: List[str] = [],
     exclude_dataset: List[str] = [],
     changed_since: Optional[str] = None,
 ) -> Clause:
     shoulds: List[Clause] = names_query(entity, fuzzy=fuzzy)
     for prop, value in entity.itervalues():
         if prop.type == registry.name or not prop.matchable:
@@ -106,27 +113,29 @@
             shoulds.append({"match": {"text": value}})
 
     return filter_query(
         shoulds,
         filters=filters,
         dataset=dataset,
         schema=entity.schema,
+        include_dataset=include_dataset,
         exclude_schema=exclude_schema,
         exclude_dataset=exclude_dataset,
         changed_since=changed_since,
     )
 
 
 def text_query(
     dataset: Dataset,
     schema: Schema,
     query: str,
     filters: FilterDict = {},
     fuzzy: bool = False,
     simple: bool = False,
+    include_dataset: List[str] = [],
     exclude_schema: List[str] = [],
     exclude_dataset: List[str] = [],
     changed_since: Optional[str] = None,
 ) -> Clause:
     if not len(query.strip()):
         should: Clause = {"match_all": {}}
     elif simple:
@@ -152,14 +161,15 @@
         }
         # log.info("Query", should=should)
     return filter_query(
         [should],
         dataset=dataset,
         schema=schema,
         filters=filters,
+        include_dataset=include_dataset,
         exclude_schema=exclude_schema,
         exclude_dataset=exclude_dataset,
         changed_since=changed_since,
     )
 
 
 def prefix_query(
```

### Comparing `yente-3.8.7/yente/search/search.py` & `yente-3.8.8/yente/search/search.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/search/status.py` & `yente-3.8.8/yente/search/status.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente/settings.py` & `yente-3.8.8/yente/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def env_str(name: str, default: str) -> str:
     """Ensure the env returns a string even on Windows (#100)."""
     value = stringify(env.get(name))
     return default if value is None else value
 
 
-VERSION = "3.8.7"
+VERSION = "3.8.8"
 AUTHOR = "OpenSanctions"
 HOME_PAGE = "https://www.opensanctions.org"
 EMAIL = "info@opensanctions.org"
 CONTACT = {"name": AUTHOR, "url": HOME_PAGE, "email": EMAIL}
 
 TITLE = env_str("YENTE_TITLE", "yente")
 DESCRIPTION = """
@@ -109,14 +109,18 @@
 BASE_SCHEMA = "Thing"
 PORT = int(env_str("YENTE_PORT", env_str("PORT", "8000")))
 UPDATE_TOKEN = env_str("YENTE_UPDATE_TOKEN", "unsafe-default")
 CACHE_HEADERS = {
     "Cache-Control": "public; max-age=3600",
     "X-Robots-Tag": "none",
 }
+
+# Set a proxy for outgoing HTTP requests:
+HTTP_PROXY = env_str("YENTE_HTTP_PROXY", "")
+
 # How many results to return per page of search results max:
 MAX_PAGE = 500
 
 # How many entities to accept in a /match batch at most:
 MAX_BATCH = int(env_str("YENTE_MAX_BATCH", "100"))
 MAX_RESULTS = 9999
 MAX_OFFSET = MAX_RESULTS - MAX_PAGE
```

### Comparing `yente-3.8.7/yente/util.py` & `yente-3.8.8/yente/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente.egg-info/PKG-INFO` & `yente-3.8.8/yente.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.8.7
+Version: 3.8.8
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: followthemoney==3.5.9
```

### Comparing `yente-3.8.7/yente.egg-info/SOURCES.txt` & `yente-3.8.8/yente.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yente-3.8.7/yente.egg-info/requires.txt` & `yente-3.8.8/yente.egg-info/requires.txt`

 * *Files identical despite different names*

