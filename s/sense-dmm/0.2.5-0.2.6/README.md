# Comparing `tmp/sense_dmm-0.2.5.tar.gz` & `tmp/sense_dmm-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sense_dmm-0.2.5.tar", last modified: Wed Apr 17 12:37:22 2024, max compression
+gzip compressed data, was "sense_dmm-0.2.6.tar", last modified: Wed Apr 17 13:09:00 2024, max compression
```

## Comparing `sense_dmm-0.2.5.tar` & `sense_dmm-0.2.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.216601 sense_dmm-0.2.5/
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)    11309 2024-04-17 12:17:46.000000 sense_dmm-0.2.5/LICENSE
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)     1304 2024-04-17 12:37:22.214601 sense_dmm-0.2.5/PKG-INFO
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)      568 2024-01-29 16:06:36.000000 sense_dmm-0.2.5/README.md
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1297 2024-04-17 12:36:12.000000 sense_dmm-0.2.5/pyproject.toml
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)       38 2024-04-17 12:37:22.216601 sense_dmm-0.2.5/setup.cfg
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.148598 sense_dmm-0.2.5/src/
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.147598 sense_dmm-0.2.5/src/dmm/
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.164599 sense_dmm-0.2.5/src/dmm/daemons/
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-14 15:26:01.000000 sense_dmm-0.2.5/src/dmm/daemons/__init__.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     5480 2024-03-08 16:09:55.000000 sense_dmm-0.2.5/src/dmm/daemons/core.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1564 2024-03-25 13:31:18.000000 sense_dmm-0.2.5/src/dmm/daemons/fts.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1669 2024-03-27 11:29:44.000000 sense_dmm-0.2.5/src/dmm/daemons/rucio.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     4267 2024-03-27 11:26:17.000000 sense_dmm-0.2.5/src/dmm/daemons/sense.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      890 2024-02-23 14:11:39.000000 sense_dmm-0.2.5/src/dmm/daemons/sites.py
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.170599 sense_dmm-0.2.5/src/dmm/db/
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)        0 2023-02-03 00:49:09.000000 sense_dmm-0.2.5/src/dmm/db/__init__.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     2995 2024-03-22 14:47:08.000000 sense_dmm-0.2.5/src/dmm/db/models.py
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)     1729 2024-03-05 17:10:58.000000 sense_dmm-0.2.5/src/dmm/db/session.py
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.173599 sense_dmm-0.2.5/src/dmm/frontend/
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-14 15:26:02.000000 sense_dmm-0.2.5/src/dmm/frontend/__init__.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1505 2024-03-27 11:22:32.000000 sense_dmm-0.2.5/src/dmm/frontend/frontend.py
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.180600 sense_dmm-0.2.5/src/dmm/main/
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-14 15:26:02.000000 sense_dmm-0.2.5/src/dmm/main/__init__.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     3080 2024-04-17 12:36:38.000000 sense_dmm-0.2.5/src/dmm/main/dmm.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      882 2024-03-05 16:44:49.000000 sense_dmm-0.2.5/src/dmm/main/orchestrator.py
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.193600 sense_dmm-0.2.5/src/dmm/utils/
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-14 15:26:02.000000 sense_dmm-0.2.5/src/dmm/utils/__init__.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     2084 2024-02-23 14:10:31.000000 sense_dmm-0.2.5/src/dmm/utils/config.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     3260 2024-03-05 16:47:50.000000 sense_dmm-0.2.5/src/dmm/utils/db.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     3005 2024-03-05 19:27:05.000000 sense_dmm-0.2.5/src/dmm/utils/fts.py
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)     3311 2024-04-08 14:00:30.000000 sense_dmm-0.2.5/src/dmm/utils/monit.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)    11182 2024-03-27 11:30:31.000000 sense_dmm-0.2.5/src/dmm/utils/sense.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     2506 2024-03-03 18:02:36.000000 sense_dmm-0.2.5/src/dmm/utils/siterm.py
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.212601 sense_dmm-0.2.5/src/sense_dmm.egg-info/
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)     1304 2024-04-17 12:37:22.000000 sense_dmm-0.2.5/src/sense_dmm.egg-info/PKG-INFO
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      765 2024-04-17 12:37:22.000000 sense_dmm-0.2.5/src/sense_dmm.egg-info/SOURCES.txt
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        1 2024-04-17 12:37:22.000000 sense_dmm-0.2.5/src/sense_dmm.egg-info/dependency_links.txt
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)       42 2024-04-17 12:37:22.000000 sense_dmm-0.2.5/src/sense_dmm.egg-info/entry_points.txt
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)       83 2024-04-17 12:37:22.000000 sense_dmm-0.2.5/src/sense_dmm.egg-info/requires.txt
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        4 2024-04-17 12:37:22.000000 sense_dmm-0.2.5/src/sense_dmm.egg-info/top_level.txt
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 13:09:00.283856 sense_dmm-0.2.6/
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)    11309 2024-04-17 12:17:46.000000 sense_dmm-0.2.6/LICENSE
+-rw-r--r--   0 aaarora  (31749) aaarora  (31749)     1304 2024-04-17 13:09:00.281855 sense_dmm-0.2.6/PKG-INFO
+-rw-r--r--   0 aaarora  (31749) aaarora  (31749)      568 2024-01-29 16:06:36.000000 sense_dmm-0.2.6/README.md
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1297 2024-04-17 13:05:56.000000 sense_dmm-0.2.6/pyproject.toml
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)       38 2024-04-17 13:09:00.283856 sense_dmm-0.2.6/setup.cfg
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 13:09:00.216853 sense_dmm-0.2.6/src/
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 13:09:00.215853 sense_dmm-0.2.6/src/dmm/
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 13:09:00.231854 sense_dmm-0.2.6/src/dmm/daemons/
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-14 15:26:01.000000 sense_dmm-0.2.6/src/dmm/daemons/__init__.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     5480 2024-03-08 16:09:55.000000 sense_dmm-0.2.6/src/dmm/daemons/core.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1564 2024-03-25 13:31:18.000000 sense_dmm-0.2.6/src/dmm/daemons/fts.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1669 2024-03-27 11:29:44.000000 sense_dmm-0.2.6/src/dmm/daemons/rucio.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     4267 2024-03-27 11:26:17.000000 sense_dmm-0.2.6/src/dmm/daemons/sense.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      890 2024-02-23 14:11:39.000000 sense_dmm-0.2.6/src/dmm/daemons/sites.py
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 13:09:00.237854 sense_dmm-0.2.6/src/dmm/db/
+-rw-r--r--   0 aaarora  (31749) aaarora  (31749)        0 2023-02-03 00:49:09.000000 sense_dmm-0.2.6/src/dmm/db/__init__.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     2995 2024-03-22 14:47:08.000000 sense_dmm-0.2.6/src/dmm/db/models.py
+-rw-r--r--   0 aaarora  (31749) aaarora  (31749)     1729 2024-03-05 17:10:58.000000 sense_dmm-0.2.6/src/dmm/db/session.py
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 13:09:00.240854 sense_dmm-0.2.6/src/dmm/frontend/
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-14 15:26:02.000000 sense_dmm-0.2.6/src/dmm/frontend/__init__.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1647 2024-04-17 13:04:54.000000 sense_dmm-0.2.6/src/dmm/frontend/frontend.py
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 13:09:00.247854 sense_dmm-0.2.6/src/dmm/main/
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-14 15:26:02.000000 sense_dmm-0.2.6/src/dmm/main/__init__.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     3079 2024-04-17 13:08:06.000000 sense_dmm-0.2.6/src/dmm/main/dmm.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      882 2024-03-05 16:44:49.000000 sense_dmm-0.2.6/src/dmm/main/orchestrator.py
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 13:09:00.260855 sense_dmm-0.2.6/src/dmm/utils/
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-14 15:26:02.000000 sense_dmm-0.2.6/src/dmm/utils/__init__.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     2084 2024-02-23 14:10:31.000000 sense_dmm-0.2.6/src/dmm/utils/config.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     3260 2024-03-05 16:47:50.000000 sense_dmm-0.2.6/src/dmm/utils/db.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     3005 2024-03-05 19:27:05.000000 sense_dmm-0.2.6/src/dmm/utils/fts.py
+-rw-r--r--   0 aaarora  (31749) aaarora  (31749)     3311 2024-04-08 14:00:30.000000 sense_dmm-0.2.6/src/dmm/utils/monit.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)    11182 2024-03-27 11:30:31.000000 sense_dmm-0.2.6/src/dmm/utils/sense.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     2506 2024-03-03 18:02:36.000000 sense_dmm-0.2.6/src/dmm/utils/siterm.py
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 13:09:00.279856 sense_dmm-0.2.6/src/sense_dmm.egg-info/
+-rw-r--r--   0 aaarora  (31749) aaarora  (31749)     1304 2024-04-17 13:09:00.000000 sense_dmm-0.2.6/src/sense_dmm.egg-info/PKG-INFO
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      765 2024-04-17 13:09:00.000000 sense_dmm-0.2.6/src/sense_dmm.egg-info/SOURCES.txt
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        1 2024-04-17 13:09:00.000000 sense_dmm-0.2.6/src/sense_dmm.egg-info/dependency_links.txt
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)       42 2024-04-17 13:09:00.000000 sense_dmm-0.2.6/src/sense_dmm.egg-info/entry_points.txt
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)       83 2024-04-17 13:09:00.000000 sense_dmm-0.2.6/src/sense_dmm.egg-info/requires.txt
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        4 2024-04-17 13:09:00.000000 sense_dmm-0.2.6/src/sense_dmm.egg-info/top_level.txt
```

### Comparing `sense_dmm-0.2.5/LICENSE` & `sense_dmm-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/PKG-INFO` & `sense_dmm-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sense-dmm
-Version: 0.2.5
+Version: 0.2.6
 Summary: Data Movement Manager for Rucio SENSE interoperatio prototype
 Author-email: Aashay Arora <aaarora@ucsd.edu>
 Project-URL: Homepage, https://github.com/aashayarora/rucio-sense-dmm
 Project-URL: Issues, https://github.com/aashayarora/rucio-sense-dmm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sense_dmm-0.2.5/README.md` & `sense_dmm-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/pyproject.toml` & `sense_dmm-0.2.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "etc",
     "tests",
     "assets"
 ]
 
 [project]
 name = "sense-dmm"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Aashay Arora", email="aaarora@ucsd.edu" },
 ]
 dependencies = [
     "sense-o-api==1.31",
     "sqlalchemy",
     "psycopg2-binary",
```

### Comparing `sense_dmm-0.2.5/src/dmm/daemons/core.py` & `sense_dmm-0.2.6/src/dmm/daemons/core.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/dmm/daemons/fts.py` & `sense_dmm-0.2.6/src/dmm/daemons/fts.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/dmm/daemons/rucio.py` & `sense_dmm-0.2.6/src/dmm/daemons/rucio.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/dmm/daemons/sense.py` & `sense_dmm-0.2.6/src/dmm/daemons/sense.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/dmm/daemons/sites.py` & `sense_dmm-0.2.6/src/dmm/daemons/sites.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/dmm/db/models.py` & `sense_dmm-0.2.6/src/dmm/db/models.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/dmm/db/session.py` & `sense_dmm-0.2.6/src/dmm/db/session.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/dmm/frontend/frontend.py` & `sense_dmm-0.2.6/src/dmm/frontend/frontend.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from flask import Flask, Response, render_template
 import logging
 import json
+import os
 
 from dmm.db.session import databased
 from dmm.utils.db import get_request_from_id, get_request_cursor
 
-frontend_app = Flask(__name__, template_folder="templates")
+current_directory = os.path.dirname(os.path.abspath(__file__))
+templates_folder = os.path.join(current_directory, "templates")
+frontend_app = Flask(__name__, template_folder=templates_folder)
 
 @frontend_app.route("/query/<rule_id>", methods=["GET"])
 @databased
 def handle_client(rule_id, session=None):
     logging.info(f"Received request for rule_id: {rule_id}")
     try:
         req = get_request_from_id(rule_id, session=session)
```

### Comparing `sense_dmm-0.2.5/src/dmm/main/dmm.py` & `sense_dmm-0.2.6/src/dmm/main/dmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,14 @@
 from dmm.daemons.rucio import preparer, rucio_modifier, finisher
 from dmm.daemons.fts import fts_modifier
 from dmm.daemons.sense import status_updater, stager, provision, sense_modifier, canceller, deleter
 from dmm.daemons.core import decider, allocator
 from dmm.daemons.sites import refresh_site_db, free_unused_endpoints
 from dmm.frontend.frontend import frontend_app
 
-logging.basicConfig(
-    format="(%(threadName)s) [%(asctime)s] %(levelname)s: %(message)s",
-    datefmt="%m-%d-%Y %H:%M:%S %p",
-    level=logging.DEBUG,
-    handlers=[logging.FileHandler(filename="/var/log/dmm.log"), logging.StreamHandler(sys.stdout)]
-)
-
 class DMM:
     def __init__(self):
         self.host = config_get("dmm", "host")
         self.port = config_get_int("dmm", "port")
         self.cert = config_get("dmm", "cert")
         self.key = config_get("dmm", "key")
 
@@ -79,9 +72,16 @@
                 finisher: {"client": self.rucio_client}
             }
             fork(self.rucio_daemon_frequency, self.lock, rucio_daemons)
 
         serve(frontend_app, port=self.port, host=self.host)
 
 def main():
+    logging.basicConfig(
+    format="(%(threadName)s) [%(asctime)s] %(levelname)s: %(message)s",
+    datefmt="%m-%d-%Y %H:%M:%S %p",
+    level=logging.DEBUG,
+    handlers=[logging.FileHandler(filename="dmm.log"), logging.StreamHandler(sys.stdout)]
+    )
+
     dmm = DMM()
     dmm.start()
```

### Comparing `sense_dmm-0.2.5/src/dmm/main/orchestrator.py` & `sense_dmm-0.2.6/src/dmm/main/orchestrator.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/dmm/utils/config.py` & `sense_dmm-0.2.6/src/dmm/utils/config.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/dmm/utils/db.py` & `sense_dmm-0.2.6/src/dmm/utils/db.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/dmm/utils/fts.py` & `sense_dmm-0.2.6/src/dmm/utils/fts.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/dmm/utils/monit.py` & `sense_dmm-0.2.6/src/dmm/utils/monit.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/dmm/utils/sense.py` & `sense_dmm-0.2.6/src/dmm/utils/sense.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/dmm/utils/siterm.py` & `sense_dmm-0.2.6/src/dmm/utils/siterm.py`

 * *Files identical despite different names*

### Comparing `sense_dmm-0.2.5/src/sense_dmm.egg-info/PKG-INFO` & `sense_dmm-0.2.6/src/sense_dmm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sense-dmm
-Version: 0.2.5
+Version: 0.2.6
 Summary: Data Movement Manager for Rucio SENSE interoperatio prototype
 Author-email: Aashay Arora <aaarora@ucsd.edu>
 Project-URL: Homepage, https://github.com/aashayarora/rucio-sense-dmm
 Project-URL: Issues, https://github.com/aashayarora/rucio-sense-dmm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sense_dmm-0.2.5/src/sense_dmm.egg-info/SOURCES.txt` & `sense_dmm-0.2.6/src/sense_dmm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

