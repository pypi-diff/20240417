# Comparing `tmp/satorisynapse-0.0.1.tar.gz` & `tmp/satorisynapse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/satorisynapse-0.0.1.tar", last modified: Wed Apr 17 20:05:04 2024, max compression
+gzip compressed data, was "dist/satorisynapse-0.0.2.tar", last modified: Wed Apr 17 20:24:51 2024, max compression
```

## Comparing `satorisynapse-0.0.1.tar` & `satorisynapse-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:05:04.000000 satorisynapse-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-17 20:05:04.000000 satorisynapse-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 20:04:50.000000 satorisynapse-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:05:04.000000 satorisynapse-0.0.1/satorisynapse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-17 20:05:04.000000 satorisynapse-0.0.1/satorisynapse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-17 20:05:04.000000 satorisynapse-0.0.1/satorisynapse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 20:05:04.000000 satorisynapse-0.0.1/satorisynapse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 20:05:04.000000 satorisynapse-0.0.1/satorisynapse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:05:04.000000 satorisynapse-0.0.1/satorisynapse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:05:04.000000 satorisynapse-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-17 20:04:50.000000 satorisynapse-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 20:24:38.000000 satorisynapse-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/satorisynapse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/satorisynapse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/satorisynapse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/satorisynapse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/satorisynapse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/satorisynapse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:24:51.000000 satorisynapse-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-17 20:24:38.000000 satorisynapse-0.0.2/setup.py
```

### Comparing `satorisynapse-0.0.1/PKG-INFO` & `satorisynapse-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.1
+Version: 0.0.2
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 License: UNKNOWN
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Description: # Synapse
         p2p for Satori
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `satorisynapse-0.0.1/satorisynapse.egg-info/PKG-INFO` & `satorisynapse-0.0.2/satorisynapse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.1
+Version: 0.0.2
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 License: UNKNOWN
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Description: # Synapse
         p2p for Satori
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `satorisynapse-0.0.1/setup.py` & `satorisynapse-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def get_name():
     return 'satorisynapse'
 
 
 def get_version():
-    return '0.0.1'
+    return '0.0.2'
 
 
 def get_requirements():
     requirements = get_here('requirements.txt')
     if os.path.isfile(requirements):
         with open(requirements, 'r') as f:
             return f.read().splitlines()
@@ -37,15 +37,15 @@
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     packages=[f'{get_name()}.{p}' for p in find_packages(where=get_name())],
     install_requires=get_requirements(),
     dependency_links=[
         'git+https://github.com/SatoriNetwork/python-evrmorelib.git#egg=python-evrmorelib'
     ],
-    python_requires='>=3.9.5',
+    python_requires='>=3.7',
     author='Jordan Miller',
     author_email="jordan@satorinet.io",
     url=f'https://github.com/SatoriNetwork/{get_name()}',
     download_url=f'https://github.com/SatoriNetwork/{get_name()}',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

