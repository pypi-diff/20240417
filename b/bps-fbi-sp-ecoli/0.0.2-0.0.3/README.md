# Comparing `tmp/bps_fbi_sp_ecoli-0.0.2.tar.gz` & `tmp/bps_fbi_sp_ecoli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bps_fbi_sp_ecoli-0.0.2.tar", last modified: Wed Apr 17 12:45:31 2024, max compression
+gzip compressed data, was "bps_fbi_sp_ecoli-0.0.3.tar", last modified: Wed Apr 17 13:39:23 2024, max compression
```

## Comparing `bps_fbi_sp_ecoli-0.0.2.tar` & `bps_fbi_sp_ecoli-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/
--rw-rw-r--   0 kloc      (1000) kloc      (1000)     1094 2024-03-11 14:17:36.000000 bps_fbi_sp_ecoli-0.0.2/LICENSE
--rw-rw-r--   0 kloc      (1000) kloc      (1000)      214 2024-04-15 13:54:59.000000 bps_fbi_sp_ecoli-0.0.2/MANIFEST.in
--rw-r--r--   0 kloc      (1000) kloc      (1000)     1686 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/PKG-INFO
--rw-r--r--   0 kloc      (1000) kloc      (1000)      815 2024-04-17 09:43:21.000000 bps_fbi_sp_ecoli-0.0.2/README.md
-drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/
--rw-r--r--   0 kloc      (1000) kloc      (1000)       22 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/__init__.py
--rw-r--r--   0 kloc      (1000) kloc      (1000)     7455 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/_modidx.py
-drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/config/
--rw-r--r--   0 kloc      (1000) kloc      (1000)      654 2024-04-15 13:52:00.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/config/config.default.env
--rw-r--r--   0 kloc      (1000) kloc      (1000)     1101 2024-04-15 13:52:00.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/config/config.default.yaml
--rw-r--r--   0 kloc      (1000) kloc      (1000)     8648 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/core.py
--rw-r--r--   0 kloc      (1000) kloc      (1000)     1922 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/hello_world.py
--rw-r--r--   0 kloc      (1000) kloc      (1000)     7043 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/helpers.py
--rw-r--r--   0 kloc      (1000) kloc      (1000)      947 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/qc_ecoli_pipeline.py
--rw-r--r--   0 kloc      (1000) kloc      (1000)     6837 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/run_bifrostecolipostkma.py
--rw-r--r--   0 kloc      (1000) kloc      (1000)     4371 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/run_qcecolisummary.py
-drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/scripts/
--rw-r--r--   0 kloc      (1000) kloc      (1000)        0 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/scripts/__init__.py
--rwxr-xr-x   0 kloc      (1000) kloc      (1000)     9168 2024-03-20 11:45:54.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/scripts/bifrostecolipostkma.py
--rwxr-xr-x   0 kloc      (1000) kloc      (1000)     1767 2024-04-08 11:03:21.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/scripts/qcecolisummary.py
-drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/
--rw-r--r--   0 kloc      (1000) kloc      (1000)     1686 2024-04-17 12:45:31.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/PKG-INFO
--rw-r--r--   0 kloc      (1000) kloc      (1000)      810 2024-04-17 12:45:31.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/SOURCES.txt
--rw-r--r--   0 kloc      (1000) kloc      (1000)        1 2024-04-17 12:45:31.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/dependency_links.txt
--rw-r--r--   0 kloc      (1000) kloc      (1000)      309 2024-04-17 12:45:31.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/entry_points.txt
--rw-r--r--   0 kloc      (1000) kloc      (1000)        1 2024-04-17 09:45:29.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/not-zip-safe
--rw-r--r--   0 kloc      (1000) kloc      (1000)       54 2024-04-17 12:45:31.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/requires.txt
--rw-r--r--   0 kloc      (1000) kloc      (1000)       53 2024-04-17 12:45:31.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/top_level.txt
--rw-r--r--   0 kloc      (1000) kloc      (1000)     1125 2024-04-17 12:45:09.000000 bps_fbi_sp_ecoli-0.0.2/settings.ini
--rw-r--r--   0 kloc      (1000) kloc      (1000)       38 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/setup.cfg
--rw-rw-r--   0 kloc      (1000) kloc      (1000)     2606 2024-04-08 07:25:39.000000 bps_fbi_sp_ecoli-0.0.2/setup.py
+drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 13:39:23.861580 bps_fbi_sp_ecoli-0.0.3/
+-rw-rw-r--   0 kloc      (1000) kloc      (1000)     1094 2024-03-11 14:17:36.000000 bps_fbi_sp_ecoli-0.0.3/LICENSE
+-rw-rw-r--   0 kloc      (1000) kloc      (1000)      214 2024-04-15 13:54:59.000000 bps_fbi_sp_ecoli-0.0.3/MANIFEST.in
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     1710 2024-04-17 13:39:23.861580 bps_fbi_sp_ecoli-0.0.3/PKG-INFO
+-rw-r--r--   0 kloc      (1000) kloc      (1000)      815 2024-04-17 09:43:21.000000 bps_fbi_sp_ecoli-0.0.3/README.md
+drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 13:39:23.861580 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/
+-rw-r--r--   0 kloc      (1000) kloc      (1000)       22 2024-04-17 13:39:19.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/__init__.py
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     7455 2024-04-17 13:39:19.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/_modidx.py
+drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 13:39:23.861580 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/config/
+-rw-r--r--   0 kloc      (1000) kloc      (1000)      654 2024-04-15 13:52:00.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/config/config.default.env
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     1101 2024-04-15 13:52:00.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/config/config.default.yaml
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     8648 2024-04-17 13:39:19.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/core.py
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     1922 2024-04-17 13:39:19.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/hello_world.py
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     7043 2024-04-17 13:39:19.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/helpers.py
+-rw-r--r--   0 kloc      (1000) kloc      (1000)      947 2024-04-17 13:39:19.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/qc_ecoli_pipeline.py
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     6837 2024-04-17 13:39:19.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/run_bifrostecolipostkma.py
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     4371 2024-04-17 13:39:19.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/run_qcecolisummary.py
+drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 13:39:23.861580 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/scripts/
+-rw-r--r--   0 kloc      (1000) kloc      (1000)        0 2024-04-17 13:39:19.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/scripts/__init__.py
+-rwxr-xr-x   0 kloc      (1000) kloc      (1000)     9168 2024-03-20 11:45:54.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/scripts/bifrostecolipostkma.py
+-rwxr-xr-x   0 kloc      (1000) kloc      (1000)     1767 2024-04-08 11:03:21.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/scripts/qcecolisummary.py
+drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 13:39:23.861580 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli.egg-info/
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     1710 2024-04-17 13:39:23.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli.egg-info/PKG-INFO
+-rw-r--r--   0 kloc      (1000) kloc      (1000)      810 2024-04-17 13:39:23.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli.egg-info/SOURCES.txt
+-rw-r--r--   0 kloc      (1000) kloc      (1000)        1 2024-04-17 13:39:23.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli.egg-info/dependency_links.txt
+-rw-r--r--   0 kloc      (1000) kloc      (1000)      309 2024-04-17 13:39:23.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli.egg-info/entry_points.txt
+-rw-r--r--   0 kloc      (1000) kloc      (1000)        1 2024-04-17 09:45:29.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli.egg-info/not-zip-safe
+-rw-r--r--   0 kloc      (1000) kloc      (1000)       63 2024-04-17 13:39:23.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli.egg-info/requires.txt
+-rw-r--r--   0 kloc      (1000) kloc      (1000)       51 2024-04-17 13:39:23.000000 bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli.egg-info/top_level.txt
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     1175 2024-04-17 13:39:19.000000 bps_fbi_sp_ecoli-0.0.3/settings.ini
+-rw-r--r--   0 kloc      (1000) kloc      (1000)       38 2024-04-17 13:39:23.861580 bps_fbi_sp_ecoli-0.0.3/setup.cfg
+-rw-rw-r--   0 kloc      (1000) kloc      (1000)     2606 2024-04-08 07:25:39.000000 bps_fbi_sp_ecoli-0.0.3/setup.py
```

### Comparing `bps_fbi_sp_ecoli-0.0.2/LICENSE` & `bps_fbi_sp_ecoli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/PKG-INFO` & `bps_fbi_sp_ecoli-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bps_fbi_sp_ecoli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Species specific scripts for ecoli
 Home-page: https://github.com/ssi-dk/bps_fbi_sp_ecoli
 Author: kalilamali
 Author-email: kloc@ssi.dk
 License: MIT License
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -19,14 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastcore
 Requires-Dist: python_dotenv
 Requires-Dist: envyaml
 Requires-Dist: pandas
 Requires-Dist: requests
+Requires-Dist: openpyxl
 Provides-Extra: dev
 
 # bps_fbi_sp_ecoli
 
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
```

### Comparing `bps_fbi_sp_ecoli-0.0.2/README.md` & `bps_fbi_sp_ecoli-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/_modidx.py` & `bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/_modidx.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/config/config.default.env` & `bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/config/config.default.env`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/config/config.default.yaml` & `bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/config/config.default.yaml`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/core.py` & `bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/core.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/hello_world.py` & `bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/hello_world.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/helpers.py` & `bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/helpers.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/qc_ecoli_pipeline.py` & `bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/qc_ecoli_pipeline.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/run_bifrostecolipostkma.py` & `bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/run_bifrostecolipostkma.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/run_qcecolisummary.py` & `bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/run_qcecolisummary.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/scripts/bifrostecolipostkma.py` & `bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/scripts/bifrostecolipostkma.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/scripts/qcecolisummary.py` & `bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli/scripts/qcecolisummary.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/PKG-INFO` & `bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bps_fbi_sp_ecoli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Species specific scripts for ecoli
 Home-page: https://github.com/ssi-dk/bps_fbi_sp_ecoli
 Author: kalilamali
 Author-email: kloc@ssi.dk
 License: MIT License
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -19,14 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastcore
 Requires-Dist: python_dotenv
 Requires-Dist: envyaml
 Requires-Dist: pandas
 Requires-Dist: requests
+Requires-Dist: openpyxl
 Provides-Extra: dev
 
 # bps_fbi_sp_ecoli
 
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
```

### Comparing `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/SOURCES.txt` & `bps_fbi_sp_ecoli-0.0.3/bps_fbi_sp_ecoli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.2/settings.ini` & `bps_fbi_sp_ecoli-0.0.3/settings.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = bps_fbi_sp_ecoli
 lib_name = bps_fbi_sp_ecoli
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = MIT
 black_formatting = 1
 doc_path = _docs
 lib_path = bps_fbi_sp_ecoli
 nbs_path = nbs
 recursive = True
@@ -22,15 +22,17 @@
 author_email = kloc@ssi.dk
 copyright = 2024 onwards, kalilamali
 description = Species specific scripts for ecoli
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = ssi-dk
-requirements = fastcore python_dotenv envyaml pandas requests
+requirements = fastcore
+pip_requirements = python_dotenv envyaml pandas requests openpyxl
+conda_requirements = 
 console_scripts = 
 	core_hello_world=bps_fbi_sp_ecoli.core:cli
 	hello_two_world=bps_fbi_sp_ecoli.hello_world:cli
 	FBI_run_bifrostecolipostkma=bps_fbi_sp_ecoli.run_bifrostecolipostkma:cli
 	FBI_run_qcecolisummary=bps_fbi_sp_ecoli.run_qcecolisummary:cli
 readme_nb = index.ipynb
 allowed_metadata_keys =
```

### Comparing `bps_fbi_sp_ecoli-0.0.2/setup.py` & `bps_fbi_sp_ecoli-0.0.3/setup.py`

 * *Files identical despite different names*
