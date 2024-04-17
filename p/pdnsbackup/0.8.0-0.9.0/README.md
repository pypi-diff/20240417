# Comparing `tmp/pdnsbackup-0.8.0.tar.gz` & `tmp/pdnsbackup-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdnsbackup-0.8.0.tar", last modified: Mon Oct  9 06:14:56 2023, max compression
+gzip compressed data, was "pdnsbackup-0.9.0.tar", last modified: Tue Oct 17 18:42:35 2023, max compression
```

## Comparing `pdnsbackup-0.8.0.tar` & `pdnsbackup-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 06:14:56.781954 pdnsbackup-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-10-09 06:14:33.000000 pdnsbackup-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-09 06:14:33.000000 pdnsbackup-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2023-10-09 06:14:56.781954 pdnsbackup-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2023-10-09 06:14:33.000000 pdnsbackup-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 06:14:56.781954 pdnsbackup-0.8.0/pdnsbackup/
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2023-10-09 06:14:33.000000 pdnsbackup-0.8.0/pdnsbackup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-10-09 06:14:33.000000 pdnsbackup-0.8.0/pdnsbackup/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-09 06:14:33.000000 pdnsbackup-0.8.0/pdnsbackup/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8394 2023-10-09 06:14:33.000000 pdnsbackup-0.8.0/pdnsbackup/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2023-10-09 06:14:33.000000 pdnsbackup-0.8.0/pdnsbackup/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 06:14:56.781954 pdnsbackup-0.8.0/pdnsbackup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2023-10-09 06:14:56.000000 pdnsbackup-0.8.0/pdnsbackup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-10-09 06:14:56.000000 pdnsbackup-0.8.0/pdnsbackup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 06:14:56.000000 pdnsbackup-0.8.0/pdnsbackup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-09 06:14:56.000000 pdnsbackup-0.8.0/pdnsbackup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-10-09 06:14:56.000000 pdnsbackup-0.8.0/pdnsbackup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-09 06:14:56.000000 pdnsbackup-0.8.0/pdnsbackup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-09 06:14:56.781954 pdnsbackup-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-10-09 06:14:56.000000 pdnsbackup-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 06:14:56.781954 pdnsbackup-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-10-09 06:14:33.000000 pdnsbackup-0.8.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2023-10-09 06:14:33.000000 pdnsbackup-0.8.0/tests/test_export_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2023-10-09 06:14:33.000000 pdnsbackup-0.8.0/tests/test_export_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-10-09 06:14:33.000000 pdnsbackup-0.8.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2023-10-09 06:14:33.000000 pdnsbackup-0.8.0/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 18:42:35.921693 pdnsbackup-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-10-17 18:42:08.000000 pdnsbackup-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-17 18:42:08.000000 pdnsbackup-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2023-10-17 18:42:35.921693 pdnsbackup-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2023-10-17 18:42:08.000000 pdnsbackup-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 18:42:35.921693 pdnsbackup-0.9.0/pdnsbackup/
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2023-10-17 18:42:08.000000 pdnsbackup-0.9.0/pdnsbackup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-10-17 18:42:08.000000 pdnsbackup-0.9.0/pdnsbackup/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-17 18:42:08.000000 pdnsbackup-0.9.0/pdnsbackup/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8394 2023-10-17 18:42:08.000000 pdnsbackup-0.9.0/pdnsbackup/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2023-10-17 18:42:08.000000 pdnsbackup-0.9.0/pdnsbackup/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 18:42:35.921693 pdnsbackup-0.9.0/pdnsbackup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2023-10-17 18:42:35.000000 pdnsbackup-0.9.0/pdnsbackup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2023-10-17 18:42:35.000000 pdnsbackup-0.9.0/pdnsbackup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 18:42:35.000000 pdnsbackup-0.9.0/pdnsbackup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-17 18:42:35.000000 pdnsbackup-0.9.0/pdnsbackup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-10-17 18:42:35.000000 pdnsbackup-0.9.0/pdnsbackup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-17 18:42:35.000000 pdnsbackup-0.9.0/pdnsbackup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-17 18:42:35.921693 pdnsbackup-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-10-17 18:42:35.000000 pdnsbackup-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 18:42:35.921693 pdnsbackup-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2023-10-17 18:42:08.000000 pdnsbackup-0.9.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2023-10-17 18:42:08.000000 pdnsbackup-0.9.0/tests/test_export_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2023-10-17 18:42:08.000000 pdnsbackup-0.9.0/tests/test_export_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2023-10-17 18:42:08.000000 pdnsbackup-0.9.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2023-10-17 18:42:08.000000 pdnsbackup-0.9.0/tests/test_parser.py
```

### Comparing `pdnsbackup-0.8.0/LICENSE` & `pdnsbackup-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdnsbackup-0.8.0/PKG-INFO` & `pdnsbackup-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdnsbackup
-Version: 0.8.0
+Version: 0.9.0
 Summary: Backup tool for PowerDNS database
 Home-page: https://github.com/dmachard/python-pdnsbackup
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
 Keywords: powerdns pdns database backup
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pdnsbackup-0.8.0/README.md` & `pdnsbackup-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pdnsbackup-0.8.0/pdnsbackup/__init__.py` & `pdnsbackup-0.9.0/pdnsbackup/__init__.py`

 * *Files identical despite different names*

### Comparing `pdnsbackup-0.8.0/pdnsbackup/backend.py` & `pdnsbackup-0.9.0/pdnsbackup/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,10 +30,10 @@
                 r = await cur.fetchall()
                 records = list(r)
                 logger.info("gmysql - %s records fetched..." % (len(records)))
         except Exception as e:
             logger.error("fetch - %s" % e)
         finally:
             if conn is not None:
-                conn.close()
+                await conn.ensure_closed()
             logger.debug("gmysql - connection closed")
     return records
```

### Comparing `pdnsbackup-0.8.0/pdnsbackup/config.yml` & `pdnsbackup-0.9.0/pdnsbackup/config.yml`

 * *Files identical despite different names*

### Comparing `pdnsbackup-0.8.0/pdnsbackup/export.py` & `pdnsbackup-0.9.0/pdnsbackup/export.py`

 * *Files identical despite different names*

### Comparing `pdnsbackup-0.8.0/pdnsbackup/parser.py` & `pdnsbackup-0.9.0/pdnsbackup/parser.py`

 * *Files identical despite different names*

### Comparing `pdnsbackup-0.8.0/pdnsbackup.egg-info/PKG-INFO` & `pdnsbackup-0.9.0/pdnsbackup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdnsbackup
-Version: 0.8.0
+Version: 0.9.0
 Summary: Backup tool for PowerDNS database
 Home-page: https://github.com/dmachard/python-pdnsbackup
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
 Keywords: powerdns pdns database backup
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pdnsbackup-0.8.0/setup.py` & `pdnsbackup-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
     
 KEYWORDS = ('powerdns pdns database backup')
 
 setuptools.setup(
     name="pdnsbackup",
-    version="0.8.0",
+    version="0.9.0",
     author="Denis MACHARD",
     author_email="d.machard@gmail.com",
     description="Backup tool for PowerDNS database",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/dmachard/python-pdnsbackup",
     packages=['pdnsbackup'],
```

### Comparing `pdnsbackup-0.8.0/tests/test_config.py` & `pdnsbackup-0.9.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pdnsbackup-0.8.0/tests/test_export_file.py` & `pdnsbackup-0.9.0/tests/test_export_file.py`

 * *Files identical despite different names*

### Comparing `pdnsbackup-0.8.0/tests/test_export_metrics.py` & `pdnsbackup-0.9.0/tests/test_export_metrics.py`

 * *Files identical despite different names*

### Comparing `pdnsbackup-0.8.0/tests/test_parser.py` & `pdnsbackup-0.9.0/tests/test_parser.py`

 * *Files identical despite different names*

