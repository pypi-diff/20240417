# Comparing `tmp/hearthstone-9.2.0.tar.gz` & `tmp/hearthstone-9.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-9.2.0.tar", last modified: Wed Apr 17 07:33:11 2024, max compression
+gzip compressed data, was "hearthstone-9.2.1.tar", last modified: Wed Apr 17 07:50:27 2024, max compression
```

## Comparing `hearthstone-9.2.0.tar` & `hearthstone-9.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:33:11.173920 hearthstone-9.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-17 07:33:07.000000 hearthstone-9.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-17 07:33:11.173920 hearthstone-9.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-17 07:33:07.000000 hearthstone-9.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:33:11.173920 hearthstone-9.2.0/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    61702 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:33:11.173920 hearthstone-9.2.0/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-17 07:33:07.000000 hearthstone-9.2.0/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:33:11.173920 hearthstone-9.2.0/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-17 07:33:11.000000 hearthstone-9.2.0/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-17 07:33:11.000000 hearthstone-9.2.0/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:33:11.000000 hearthstone-9.2.0/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 07:33:11.000000 hearthstone-9.2.0/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 07:33:11.000000 hearthstone-9.2.0/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:33:11.000000 hearthstone-9.2.0/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-17 07:33:11.173920 hearthstone-9.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-17 07:33:07.000000 hearthstone-9.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:50:27.041378 hearthstone-9.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-17 07:50:23.000000 hearthstone-9.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-17 07:50:27.041378 hearthstone-9.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-17 07:50:23.000000 hearthstone-9.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:50:27.041378 hearthstone-9.2.1/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 07:50:23.000000 hearthstone-9.2.1/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-17 07:50:23.000000 hearthstone-9.2.1/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12893 2024-04-17 07:50:23.000000 hearthstone-9.2.1/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-17 07:50:23.000000 hearthstone-9.2.1/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-17 07:50:23.000000 hearthstone-9.2.1/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-17 07:50:23.000000 hearthstone-9.2.1/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61702 2024-04-17 07:50:23.000000 hearthstone-9.2.1/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-04-17 07:50:23.000000 hearthstone-9.2.1/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-17 07:50:23.000000 hearthstone-9.2.1/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 07:50:23.000000 hearthstone-9.2.1/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:50:27.041378 hearthstone-9.2.1/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-04-17 07:50:23.000000 hearthstone-9.2.1/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-17 07:50:23.000000 hearthstone-9.2.1/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:50:27.041378 hearthstone-9.2.1/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-17 07:50:27.000000 hearthstone-9.2.1/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-17 07:50:27.000000 hearthstone-9.2.1/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:50:27.000000 hearthstone-9.2.1/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 07:50:27.000000 hearthstone-9.2.1/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 07:50:27.000000 hearthstone-9.2.1/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:50:27.000000 hearthstone-9.2.1/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-17 07:50:27.041378 hearthstone-9.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-17 07:50:23.000000 hearthstone-9.2.1/setup.py
```

### Comparing `hearthstone-9.2.0/LICENSE` & `hearthstone-9.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.0/PKG-INFO` & `hearthstone-9.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 9.2.0
+Version: 9.2.1
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,20 @@
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/hearthsim/python-hearthstone/ci.yml?branch=master)](https://github.com/HearthSim/python-hearthstone/actions/workflows/ci.yml)
 [![PyPI](https://img.shields.io/pypi/v/hearthstone.svg)](https://pypi.org/project/hearthstone/)
 
 A Hearthstone Python library containing:
 
 * A CardDefs.xml parser (`hearthstone.cardxml`)
 * A DbfXml parser (`hearthstone.dbf`)
+* A deck code encoder and decoder (`hearthstone.deckstrings`)
 * Hearthstone enums as IntEnum (`hearthstone.enums`)
 
-The log parser previously in `hearthstone.hslog` has moved to the
-[python-hslog project](https://github.com/HearthSim/python-hslog).
-
-The CardDefs.xml data for the latest build is available in the
+The CardDefs.xml data for the latest build can optionally be installed from the
 [python-hearthstone-data repository](https://github.com/HearthSim/python-hearthstone-data)
-or on PyPI with `pip install hearthstone_data`.
+or on PyPI with `pip install hearthstone_data`. Otherwise, they will be download at runtime.
 
 
 ## Requirements
 
 * Python 3.6+
 * lxml
```

### Comparing `hearthstone-9.2.0/README.md` & `hearthstone-9.2.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/hearthsim/python-hearthstone/ci.yml?branch=master)](https://github.com/HearthSim/python-hearthstone/actions/workflows/ci.yml)
 [![PyPI](https://img.shields.io/pypi/v/hearthstone.svg)](https://pypi.org/project/hearthstone/)
 
 A Hearthstone Python library containing:
 
 * A CardDefs.xml parser (`hearthstone.cardxml`)
 * A DbfXml parser (`hearthstone.dbf`)
+* A deck code encoder and decoder (`hearthstone.deckstrings`)
 * Hearthstone enums as IntEnum (`hearthstone.enums`)
 
-The log parser previously in `hearthstone.hslog` has moved to the
-[python-hslog project](https://github.com/HearthSim/python-hslog).
-
-The CardDefs.xml data for the latest build is available in the
+The CardDefs.xml data for the latest build can optionally be installed from the
 [python-hearthstone-data repository](https://github.com/HearthSim/python-hearthstone-data)
-or on PyPI with `pip install hearthstone_data`.
+or on PyPI with `pip install hearthstone_data`. Otherwise, they will be download at runtime.
 
 
 ## Requirements
 
 * Python 3.6+
 * lxml
```

### Comparing `hearthstone-9.2.0/hearthstone/bountyxml.py` & `hearthstone-9.2.1/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.0/hearthstone/cardxml.py` & `hearthstone-9.2.1/hearthstone/cardxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,15 +393,18 @@
 cardid_cache: dict = {}
 dbf_cache: dict = {}
 
 
 XML_URL = "https://api.hearthstonejson.com/v1/latest/CardDefs.xml"
 
 
-def _bootstrap_from_web(url: str, parse: Callable[[Iterator[Tuple[str, Any]]], None]):
+def _bootstrap_from_web(parse: Callable[[Iterator[Tuple[str, Any]]], None], url=None):
+	if url is None:
+		url = XML_URL
+
 	with tempfile.TemporaryFile(mode="rb+") as fp:
 		if download_to_tempfile_retry(url, fp):
 			fp.flush()
 			fp.seek(0)
 
 			parse(ElementTree.iterparse(fp, events=("start", "end",)))
 
@@ -442,15 +445,15 @@
 			has_lib = True
 			try:
 				import hearthstone_data  # noqa: F401
 			except ImportError:
 				has_lib = False
 
 			if not has_lib:
-				_bootstrap_from_web(url or XML_URL, parse)
+				_bootstrap_from_web(parse, url=url)
 
 		if not db:
 			_bootstrap_from_library(parse, path=path)
 
 		cache[cache_key] = (db, None)
 
 	return cache[cache_key]
```

### Comparing `hearthstone-9.2.0/hearthstone/dbf.py` & `hearthstone-9.2.1/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.0/hearthstone/deckstrings.py` & `hearthstone-9.2.1/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.0/hearthstone/entities.py` & `hearthstone-9.2.1/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.0/hearthstone/enums.py` & `hearthstone-9.2.1/hearthstone/enums.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.0/hearthstone/mercenaryxml.py` & `hearthstone-9.2.1/hearthstone/mercenaryxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,17 +187,20 @@
 
 mercenary_cache: Dict[Tuple[str, str], Tuple[Dict[int, MercenaryXML], Any]] = {}
 
 
 XML_URL = "https://api.hearthstonejson.com/v1/latest/MercenaryDefs.xml"
 
 
-def _bootstrap_from_web(parse: Callable[[Iterator[Tuple[str, Any]]], None]):
+def _bootstrap_from_web(parse: Callable[[Iterator[Tuple[str, Any]]], None], url=None):
+	if url is None:
+		url = XML_URL
+
 	with tempfile.TemporaryFile(mode="rb+") as fp:
-		if download_to_tempfile_retry(XML_URL, fp):
+		if download_to_tempfile_retry(url, fp):
 			fp.flush()
 			fp.seek(0)
 
 			parse(ElementTree.iterparse(fp, events=("start", "end",)))
 
 
 def _bootstrap_from_library(parse: Callable[[Iterator[Tuple[str, Any]]], None], path=None):
@@ -206,15 +209,15 @@
 	if path is None:
 		path = get_mercenarydefs_path()
 
 	with open(path, "rb") as f:
 		parse(ElementTree.iterparse(f, events=("start", "end",)))
 
 
-def load(path=None, locale="enUS"):
+def load(locale="enUS", path=None, url=None):
 	cache_key = (path, locale)
 	if cache_key not in mercenary_cache:
 		db = {}
 
 		def parse(context: Iterator[Tuple[str, Any]]):
 			nonlocal db
 			root = None
@@ -228,15 +231,15 @@
 					merc.locale = locale
 					db[merc.id] = merc
 
 					elem.clear()  # type: ignore
 					root.clear()  # type: ignore
 
 		if path is None:
-			_bootstrap_from_web(parse)
+			_bootstrap_from_web(parse, url=url)
 
 		if not db:
 			_bootstrap_from_library(parse, path=path)
 
 		mercenary_cache[cache_key] = (db, None)
 
 	return mercenary_cache[cache_key]
```

### Comparing `hearthstone-9.2.0/hearthstone/stringsfile.py` & `hearthstone-9.2.1/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.0/hearthstone/utils/__init__.py` & `hearthstone-9.2.1/hearthstone/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.0/hearthstone/xmlutils.py` & `hearthstone-9.2.1/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.0/hearthstone.egg-info/PKG-INFO` & `hearthstone-9.2.1/hearthstone.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 9.2.0
+Version: 9.2.1
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,20 @@
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/hearthsim/python-hearthstone/ci.yml?branch=master)](https://github.com/HearthSim/python-hearthstone/actions/workflows/ci.yml)
 [![PyPI](https://img.shields.io/pypi/v/hearthstone.svg)](https://pypi.org/project/hearthstone/)
 
 A Hearthstone Python library containing:
 
 * A CardDefs.xml parser (`hearthstone.cardxml`)
 * A DbfXml parser (`hearthstone.dbf`)
+* A deck code encoder and decoder (`hearthstone.deckstrings`)
 * Hearthstone enums as IntEnum (`hearthstone.enums`)
 
-The log parser previously in `hearthstone.hslog` has moved to the
-[python-hslog project](https://github.com/HearthSim/python-hslog).
-
-The CardDefs.xml data for the latest build is available in the
+The CardDefs.xml data for the latest build can optionally be installed from the
 [python-hearthstone-data repository](https://github.com/HearthSim/python-hearthstone-data)
-or on PyPI with `pip install hearthstone_data`.
+or on PyPI with `pip install hearthstone_data`. Otherwise, they will be download at runtime.
 
 
 ## Requirements
 
 * Python 3.6+
 * lxml
```

### Comparing `hearthstone-9.2.0/hearthstone.egg-info/SOURCES.txt` & `hearthstone-9.2.1/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.0/setup.cfg` & `hearthstone-9.2.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 9.2.0
+version = 9.2.1
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

