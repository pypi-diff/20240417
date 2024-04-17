# Comparing `tmp/satorisynapse-0.0.2.tar.gz` & `tmp/satorisynapse-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/satorisynapse-0.0.2.tar", last modified: Wed Apr 17 20:24:51 2024, max compression
+gzip compressed data, was "satorisynapse-0.0.3.tar", last modified: Wed Apr 17 21:00:32 2024, max compression
```

## Comparing `satorisynapse-0.0.2.tar` & `satorisynapse-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 20:24:38.000000 satorisynapse-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/satorisynapse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/satorisynapse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/satorisynapse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/satorisynapse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/satorisynapse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/satorisynapse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-17 20:24:38.000000 satorisynapse-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:00:32.940129 satorisynapse-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-17 21:00:28.000000 satorisynapse-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-17 21:00:32.940129 satorisynapse-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 21:00:28.000000 satorisynapse-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:00:32.936129 satorisynapse-0.0.3/satorisynapse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:00:32.940129 satorisynapse-0.0.3/satorisynapse/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:00:28.000000 satorisynapse-0.0.3/satorisynapse/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-17 21:00:28.000000 satorisynapse-0.0.3/satorisynapse/lib/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-17 21:00:28.000000 satorisynapse-0.0.3/satorisynapse/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-17 21:00:28.000000 satorisynapse-0.0.3/satorisynapse/lib/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 21:00:28.000000 satorisynapse-0.0.3/satorisynapse/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:00:32.940129 satorisynapse-0.0.3/satorisynapse/synapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:00:28.000000 satorisynapse-0.0.3/satorisynapse/synapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-17 21:00:28.000000 satorisynapse-0.0.3/satorisynapse/synapse/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7968 2024-04-17 21:00:28.000000 satorisynapse-0.0.3/satorisynapse/synapse/threaded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:00:32.940129 satorisynapse-0.0.3/satorisynapse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-17 21:00:32.000000 satorisynapse-0.0.3/satorisynapse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-17 21:00:32.000000 satorisynapse-0.0.3/satorisynapse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 21:00:32.000000 satorisynapse-0.0.3/satorisynapse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 21:00:32.000000 satorisynapse-0.0.3/satorisynapse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 21:00:32.000000 satorisynapse-0.0.3/satorisynapse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 21:00:32.940129 satorisynapse-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-17 21:00:28.000000 satorisynapse-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `satorisynapse-0.0.2/PKG-INFO` & `satorisynapse-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.2
+Version: 0.0.3
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
+Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
-License: UNKNOWN
-Download-URL: https://github.com/SatoriNetwork/satorisynapse
-Description: # Synapse
-        p2p for Satori
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Synapse
+p2p for Satori
```

### Comparing `satorisynapse-0.0.2/satorisynapse.egg-info/PKG-INFO` & `satorisynapse-0.0.3/satorisynapse.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.2
+Version: 0.0.3
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
+Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
-License: UNKNOWN
-Download-URL: https://github.com/SatoriNetwork/satorisynapse
-Description: # Synapse
-        p2p for Satori
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Synapse
+p2p for Satori
```

### Comparing `satorisynapse-0.0.2/setup.py` & `satorisynapse-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def get_name():
     return 'satorisynapse'
 
 
 def get_version():
-    return '0.0.2'
+    return '0.0.3'
 
 
 def get_requirements():
     requirements = get_here('requirements.txt')
     if os.path.isfile(requirements):
         with open(requirements, 'r') as f:
             return f.read().splitlines()
```

