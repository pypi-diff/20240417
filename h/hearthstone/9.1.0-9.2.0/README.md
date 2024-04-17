# Comparing `tmp/hearthstone-9.1.0.tar.gz` & `tmp/hearthstone-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-9.1.0.tar", last modified: Tue Apr 16 15:05:14 2024, max compression
+gzip compressed data, was "hearthstone-9.2.0.tar", last modified: Wed Apr 17 07:33:11 2024, max compression
```

## Comparing `hearthstone-9.1.0.tar` & `hearthstone-9.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:05:14.468963 hearthstone-9.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-16 15:05:08.000000 hearthstone-9.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-16 15:05:14.468963 hearthstone-9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-16 15:05:08.000000 hearthstone-9.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:05:14.468963 hearthstone-9.1.0/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12804 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    61527 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:05:14.468963 hearthstone-9.1.0/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:05:14.468963 hearthstone-9.1.0/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-16 15:05:14.000000 hearthstone-9.1.0/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-16 15:05:14.000000 hearthstone-9.1.0/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:05:14.000000 hearthstone-9.1.0/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 15:05:14.000000 hearthstone-9.1.0/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 15:05:14.000000 hearthstone-9.1.0/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:05:14.000000 hearthstone-9.1.0/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-16 15:05:14.468963 hearthstone-9.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-16 15:05:08.000000 hearthstone-9.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:33:11.173920 hearthstone-9.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-17 07:33:07.000000 hearthstone-9.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-17 07:33:11.173920 hearthstone-9.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-17 07:33:07.000000 hearthstone-9.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:33:11.173920 hearthstone-9.2.0/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61702 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:33:11.173920 hearthstone-9.2.0/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:33:11.173920 hearthstone-9.2.0/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-17 07:33:11.000000 hearthstone-9.2.0/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-17 07:33:11.000000 hearthstone-9.2.0/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:33:11.000000 hearthstone-9.2.0/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 07:33:11.000000 hearthstone-9.2.0/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 07:33:11.000000 hearthstone-9.2.0/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:33:11.000000 hearthstone-9.2.0/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-17 07:33:11.173920 hearthstone-9.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-17 07:33:07.000000 hearthstone-9.2.0/setup.py
```

### Comparing `hearthstone-9.1.0/LICENSE` & `hearthstone-9.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-9.1.0/PKG-INFO` & `hearthstone-9.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 9.1.0
+Version: 9.2.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-9.1.0/README.md` & `hearthstone-9.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-9.1.0/hearthstone/bountyxml.py` & `hearthstone-9.2.0/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.1.0/hearthstone/cardxml.py` & `hearthstone-9.2.0/hearthstone/cardxml.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,17 +393,17 @@
 cardid_cache: dict = {}
 dbf_cache: dict = {}
 
 
 XML_URL = "https://api.hearthstonejson.com/v1/latest/CardDefs.xml"
 
 
-def _bootstrap_from_web(parse: Callable[[Iterator[Tuple[str, Any]]], None]):
+def _bootstrap_from_web(url: str, parse: Callable[[Iterator[Tuple[str, Any]]], None]):
 	with tempfile.TemporaryFile(mode="rb+") as fp:
-		if download_to_tempfile_retry(XML_URL, fp):
+		if download_to_tempfile_retry(url, fp):
 			fp.flush()
 			fp.seek(0)
 
 			parse(ElementTree.iterparse(fp, events=("start", "end",)))
 
 
 def _bootstrap_from_library(parse: Callable[[Iterator[Tuple[str, Any]]], None], path=None):
@@ -412,15 +412,15 @@
 	if path is None:
 		path = get_carddefs_path()
 
 	with open(path, "rb") as f:
 		parse(ElementTree.iterparse(f, events=("start", "end",)))
 
 
-def _load(path, locale, cache, attr):
+def _load(path, locale, cache, attr, url=None):
 	cache_key = (path, locale)
 	if cache_key not in cache:
 		db = {}
 
 		def parse(context: Iterator[Tuple[str, Any]]):
 			nonlocal db
 			root = None
@@ -442,23 +442,23 @@
 			has_lib = True
 			try:
 				import hearthstone_data  # noqa: F401
 			except ImportError:
 				has_lib = False
 
 			if not has_lib:
-				_bootstrap_from_web(parse)
+				_bootstrap_from_web(url or XML_URL, parse)
 
 		if not db:
 			_bootstrap_from_library(parse, path=path)
 
 		cache[cache_key] = (db, None)
 
 	return cache[cache_key]
 
 
-def load(path=None, locale="enUS"):
-	return _load(path, locale, cardid_cache, "id")
+def load(path=None, locale="enUS", url=None):
+	return _load(path, locale, cardid_cache, "id", url)
 
 
-def load_dbf(path=None, locale="enUS"):
-	return _load(path, locale, dbf_cache, "dbf_id")
+def load_dbf(path=None, locale="enUS", url=None):
+	return _load(path, locale, dbf_cache, "dbf_id", url)
```

### Comparing `hearthstone-9.1.0/hearthstone/dbf.py` & `hearthstone-9.2.0/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.1.0/hearthstone/deckstrings.py` & `hearthstone-9.2.0/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.1.0/hearthstone/entities.py` & `hearthstone-9.2.0/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.1.0/hearthstone/enums.py` & `hearthstone-9.2.0/hearthstone/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1013,18 +1013,23 @@
 	PIECE_OF_CTHUN = 1477
 	AVFACTION = 2323
 	AVRANK = 2324
 	MERCS_DISCOVER = 2665
 	TOPDECK = 377
 
 	# Missing/guessed, only present in logs
+	# Note: the names of these can change at any time!
 	WEAPON = 334
 	DISCARD_CARDS = 890
 	BATTLEGROUNDS_HERO_ARMOR_TIER = 1723
 	BATTLEGROUNDS_DARKMOON_PRIZE_TURN = 1735
+	EXCAVATE_COUNTER = 2822
+	BACON_ELEMENTAL_PLAY_COUNTER = 2878
+	IS_BACON_POOL_SPELL = 3081
+	IS_BACON_DUOS_POOL_SPELL = 3166
 
 	CANT_BE_EXHAUSTED = 244
 	CANT_EXHAUST = 226
 	CANT_TARGET = 228
 	CANT_DESTROY = 229
 	# Enum number changed
 	# HISTORY_PROXY_NO_BIG_CARD = 427
```

### Comparing `hearthstone-9.1.0/hearthstone/mercenaryxml.py` & `hearthstone-9.2.0/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.1.0/hearthstone/stringsfile.py` & `hearthstone-9.2.0/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.1.0/hearthstone/utils/__init__.py` & `hearthstone-9.2.0/hearthstone/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.1.0/hearthstone/xmlutils.py` & `hearthstone-9.2.0/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.1.0/hearthstone.egg-info/PKG-INFO` & `hearthstone-9.2.0/hearthstone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 9.1.0
+Version: 9.2.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-9.1.0/hearthstone.egg-info/SOURCES.txt` & `hearthstone-9.2.0/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-9.1.0/setup.cfg` & `hearthstone-9.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 9.1.0
+version = 9.2.0
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

