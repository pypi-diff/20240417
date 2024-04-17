# Comparing `tmp/bps_fbi_sp_ecoli-0.0.1.tar.gz` & `tmp/bps_fbi_sp_ecoli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bps_fbi_sp_ecoli-0.0.1.tar", last modified: Mon Apr 15 14:26:11 2024, max compression
+gzip compressed data, was "bps_fbi_sp_ecoli-0.0.2.tar", last modified: Wed Apr 17 12:45:31 2024, max compression
```

## Comparing `bps_fbi_sp_ecoli-0.0.1.tar` & `bps_fbi_sp_ecoli-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-15 14:26:11.859686 bps_fbi_sp_ecoli-0.0.1/
--rw-rw-r--   0 kloc      (1000) kloc      (1000)     1094 2024-03-11 14:17:36.000000 bps_fbi_sp_ecoli-0.0.1/LICENSE
--rw-rw-r--   0 kloc      (1000) kloc      (1000)      214 2024-04-15 13:54:59.000000 bps_fbi_sp_ecoli-0.0.1/MANIFEST.in
--rw-r--r--   0 kloc      (1000) kloc      (1000)     5076 2024-04-15 14:26:11.859686 bps_fbi_sp_ecoli-0.0.1/PKG-INFO
--rw-r--r--   0 kloc      (1000) kloc      (1000)     4255 2024-04-15 14:16:49.000000 bps_fbi_sp_ecoli-0.0.1/README.md
-drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-15 14:26:11.859686 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/
--rw-r--r--   0 kloc      (1000) kloc      (1000)       22 2024-04-15 14:16:37.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/__init__.py
--rw-r--r--   0 kloc      (1000) kloc      (1000)     7463 2024-04-15 14:16:37.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/_modidx.py
-drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-15 14:26:11.859686 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/config/
--rw-r--r--   0 kloc      (1000) kloc      (1000)      654 2024-04-15 13:52:00.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/config/config.default.env
--rw-r--r--   0 kloc      (1000) kloc      (1000)     1101 2024-04-15 13:52:00.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/config/config.default.yaml
--rw-r--r--   0 kloc      (1000) kloc      (1000)     8648 2024-04-15 14:16:36.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/core.py
--rw-r--r--   0 kloc      (1000) kloc      (1000)     1922 2024-04-15 14:16:36.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/hello_world.py
--rw-r--r--   0 kloc      (1000) kloc      (1000)     7043 2024-04-15 14:16:36.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/helpers.py
--rw-r--r--   0 kloc      (1000) kloc      (1000)      947 2024-04-15 14:16:37.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/qc_ecoli_pipeline.py
--rw-r--r--   0 kloc      (1000) kloc      (1000)     6837 2024-04-15 14:16:37.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/run_bifrostecolipostkma.py
--rw-r--r--   0 kloc      (1000) kloc      (1000)     4371 2024-04-15 14:16:37.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/run_qcecolisummary.py
-drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-15 14:26:11.859686 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/scripts/
--rw-r--r--   0 kloc      (1000) kloc      (1000)        0 2024-04-15 14:16:37.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/scripts/__init__.py
--rwxr-xr-x   0 kloc      (1000) kloc      (1000)     9168 2024-03-20 11:45:54.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/scripts/bifrostecolipostkma.py
--rwxr-xr-x   0 kloc      (1000) kloc      (1000)     1767 2024-04-08 11:03:21.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/scripts/qcecolisummary.py
-drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-15 14:26:11.859686 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli.egg-info/
--rw-r--r--   0 kloc      (1000) kloc      (1000)     5076 2024-04-15 14:26:11.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli.egg-info/PKG-INFO
--rw-r--r--   0 kloc      (1000) kloc      (1000)      810 2024-04-15 14:26:11.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli.egg-info/SOURCES.txt
--rw-r--r--   0 kloc      (1000) kloc      (1000)        1 2024-04-15 14:26:11.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli.egg-info/dependency_links.txt
--rw-r--r--   0 kloc      (1000) kloc      (1000)      309 2024-04-15 14:26:11.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli.egg-info/entry_points.txt
--rw-r--r--   0 kloc      (1000) kloc      (1000)        1 2024-04-15 14:08:04.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli.egg-info/not-zip-safe
--rw-r--r--   0 kloc      (1000) kloc      (1000)       45 2024-04-15 14:26:11.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli.egg-info/requires.txt
--rw-r--r--   0 kloc      (1000) kloc      (1000)       53 2024-04-15 14:26:11.000000 bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli.egg-info/top_level.txt
--rw-r--r--   0 kloc      (1000) kloc      (1000)     1241 2024-04-15 13:53:00.000000 bps_fbi_sp_ecoli-0.0.1/settings.ini
--rw-r--r--   0 kloc      (1000) kloc      (1000)       38 2024-04-15 14:26:11.859686 bps_fbi_sp_ecoli-0.0.1/setup.cfg
--rw-rw-r--   0 kloc      (1000) kloc      (1000)     2606 2024-04-08 07:25:39.000000 bps_fbi_sp_ecoli-0.0.1/setup.py
+drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/
+-rw-rw-r--   0 kloc      (1000) kloc      (1000)     1094 2024-03-11 14:17:36.000000 bps_fbi_sp_ecoli-0.0.2/LICENSE
+-rw-rw-r--   0 kloc      (1000) kloc      (1000)      214 2024-04-15 13:54:59.000000 bps_fbi_sp_ecoli-0.0.2/MANIFEST.in
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     1686 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/PKG-INFO
+-rw-r--r--   0 kloc      (1000) kloc      (1000)      815 2024-04-17 09:43:21.000000 bps_fbi_sp_ecoli-0.0.2/README.md
+drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/
+-rw-r--r--   0 kloc      (1000) kloc      (1000)       22 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/__init__.py
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     7455 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/_modidx.py
+drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/config/
+-rw-r--r--   0 kloc      (1000) kloc      (1000)      654 2024-04-15 13:52:00.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/config/config.default.env
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     1101 2024-04-15 13:52:00.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/config/config.default.yaml
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     8648 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/core.py
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     1922 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/hello_world.py
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     7043 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/helpers.py
+-rw-r--r--   0 kloc      (1000) kloc      (1000)      947 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/qc_ecoli_pipeline.py
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     6837 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/run_bifrostecolipostkma.py
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     4371 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/run_qcecolisummary.py
+drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/scripts/
+-rw-r--r--   0 kloc      (1000) kloc      (1000)        0 2024-04-17 12:45:10.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/scripts/__init__.py
+-rwxr-xr-x   0 kloc      (1000) kloc      (1000)     9168 2024-03-20 11:45:54.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/scripts/bifrostecolipostkma.py
+-rwxr-xr-x   0 kloc      (1000) kloc      (1000)     1767 2024-04-08 11:03:21.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/scripts/qcecolisummary.py
+drwxr-xr-x   0 kloc      (1000) kloc      (1000)        0 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     1686 2024-04-17 12:45:31.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/PKG-INFO
+-rw-r--r--   0 kloc      (1000) kloc      (1000)      810 2024-04-17 12:45:31.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/SOURCES.txt
+-rw-r--r--   0 kloc      (1000) kloc      (1000)        1 2024-04-17 12:45:31.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/dependency_links.txt
+-rw-r--r--   0 kloc      (1000) kloc      (1000)      309 2024-04-17 12:45:31.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/entry_points.txt
+-rw-r--r--   0 kloc      (1000) kloc      (1000)        1 2024-04-17 09:45:29.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/not-zip-safe
+-rw-r--r--   0 kloc      (1000) kloc      (1000)       54 2024-04-17 12:45:31.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/requires.txt
+-rw-r--r--   0 kloc      (1000) kloc      (1000)       53 2024-04-17 12:45:31.000000 bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/top_level.txt
+-rw-r--r--   0 kloc      (1000) kloc      (1000)     1125 2024-04-17 12:45:09.000000 bps_fbi_sp_ecoli-0.0.2/settings.ini
+-rw-r--r--   0 kloc      (1000) kloc      (1000)       38 2024-04-17 12:45:31.079002 bps_fbi_sp_ecoli-0.0.2/setup.cfg
+-rw-rw-r--   0 kloc      (1000) kloc      (1000)     2606 2024-04-08 07:25:39.000000 bps_fbi_sp_ecoli-0.0.2/setup.py
```

### Comparing `bps_fbi_sp_ecoli-0.0.1/LICENSE` & `bps_fbi_sp_ecoli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/_modidx.py` & `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/bps_fbi_sp_ecoli',
-                'doc_host': 'https://kalilamali.github.io',
-                'git_url': 'https://github.com/kalilamali/bps_fbi_sp_ecoli',
+                'doc_host': 'https://ssi-dk.github.io',
+                'git_url': 'https://github.com/ssi-dk/bps_fbi_sp_ecoli',
                 'lib_path': 'bps_fbi_sp_ecoli'},
   'syms': { 'bps_fbi_sp_ecoli.core': { 'bps_fbi_sp_ecoli.core.cli': ('core.html#cli', 'bps_fbi_sp_ecoli/core.py'),
                                        'bps_fbi_sp_ecoli.core.get_config': ('core.html#get_config', 'bps_fbi_sp_ecoli/core.py'),
                                        'bps_fbi_sp_ecoli.core.get_samplesheet': ('core.html#get_samplesheet', 'bps_fbi_sp_ecoli/core.py'),
                                        'bps_fbi_sp_ecoli.core.hello_world': ('core.html#hello_world', 'bps_fbi_sp_ecoli/core.py'),
                                        'bps_fbi_sp_ecoli.core.set_env_variables': ( 'core.html#set_env_variables',
                                                                                     'bps_fbi_sp_ecoli/core.py'),
```

### Comparing `bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/config/config.default.env` & `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/config/config.default.env`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/config/config.default.yaml` & `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/config/config.default.yaml`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/core.py` & `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     DEV_MODE = True
 
 PROJECT_DIR = os.getcwd()  # override value in dev mode
 if PROJECT_DIR.endswith("nbs"):
     DEV_MODE = True
     PROJECT_DIR = os.path.split(PROJECT_DIR)[0]
 
-# %% ../nbs/00_core.ipynb 11
+# %% ../nbs/00_core.ipynb 12
 # standard libs
 import os
 import re
 
 # Common to template
 # add into settings.ini, requirements, package name is python-dotenv, for conda build ensure `conda config --add channels conda-forge`
 import dotenv  # for loading config from .env files, https://pypi.org/project/python-dotenv/
@@ -48,15 +48,15 @@
 )
 from fastcore.script import (
     call_parse,
 )  # for @call_parse, https://fastcore.fast.ai/script
 
 # Project specific libraries
 
-# %% ../nbs/00_core.ipynb 14
+# %% ../nbs/00_core.ipynb 15
 import importlib
 import importlib.util
 
 
 def set_env_variables(config_path: str, overide_env_vars: bool = True) -> bool:
     # Load dot env sets environmental values from a file, if the value already exists it will not be overwritten unless override is set to True.
     # If we have multiple .env files then we need to apply the one which we want to take precedence last with overide.
@@ -75,15 +75,15 @@
 
     # 2. set values from file:
     if os.path.isfile(config_path):
         dotenv.load_dotenv(config_path, override=overide_env_vars)
 
     return True
 
-# %% ../nbs/00_core.ipynb 16
+# %% ../nbs/00_core.ipynb 17
 import importlib
 import importlib.util
 
 
 def get_config(config_path: str = None, overide_env_vars: bool = True) -> dict:
     if config_path is None:
         config_path = ""
@@ -99,28 +99,28 @@
         os.environ.get(
             "CORE_YAML_CONFIG_FILE", f"{PACKAGE_DIR}/config/config.default.yaml"
         ),
         strict=False,
     ).export()
     return config
 
-# %% ../nbs/00_core.ipynb 18
+# %% ../nbs/00_core.ipynb 19
 # create a os.PathLike object
 config = get_config(os.environ.get("CORE_CONFIG_FILE", ""))
 
-# %% ../nbs/00_core.ipynb 20
+# %% ../nbs/00_core.ipynb 21
 def show_project_env_vars(config: dict) -> None:
     # Prints out all the project environment variables
     # This is useful for debugging and seeing what is being set
     for k, v in config.items():
         # If ENV var starts with PROJECTNAME_ then print
         if k.startswith(config["CORE_PROJECT_VARIABLE_PREFIX"]):
             print(f"{k}={v}")
 
-# %% ../nbs/00_core.ipynb 23
+# %% ../nbs/00_core.ipynb 24
 import pandas as pd
 
 
 def get_samplesheet(sample_sheet_config: dict) -> pd.DataFrame:
     # Load the sample sheet into a pandas dataframe
     # If columns is not None then it will only load those columns
     # If the sample sheet is a csv then it will load it as a csv, otherwise it will assume it's a tsv
@@ -186,19 +186,19 @@
     if columns is not None:
         df = df[columns]
 
     # Clean the df of any extra rows that can be caused by empty lines in the sample sheet
     df = df.dropna(how="all")
     return df
 
-# %% ../nbs/00_core.ipynb 25
+# %% ../nbs/00_core.ipynb 26
 def hello_world(name: str = "Not given") -> str:
     return f"Hello World! My name is {name}"
 
-# %% ../nbs/00_core.ipynb 29
+# %% ../nbs/00_core.ipynb 30
 from fastcore.script import call_parse
 
 
 @call_parse
 def cli(
     name: str,  # Your name
     config_file: str = None,  # config file to set env vars from
```

### Comparing `bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/hello_world.py` & `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/hello_world.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/helpers.py` & `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/helpers.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/qc_ecoli_pipeline.py` & `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/qc_ecoli_pipeline.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/run_bifrostecolipostkma.py` & `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/run_bifrostecolipostkma.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/run_qcecolisummary.py` & `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/run_qcecolisummary.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/scripts/bifrostecolipostkma.py` & `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/scripts/bifrostecolipostkma.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli/scripts/qcecolisummary.py` & `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli/scripts/qcecolisummary.py`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.1/bps_fbi_sp_ecoli.egg-info/SOURCES.txt` & `bps_fbi_sp_ecoli-0.0.2/bps_fbi_sp_ecoli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bps_fbi_sp_ecoli-0.0.1/setup.py` & `bps_fbi_sp_ecoli-0.0.2/setup.py`

 * *Files identical despite different names*

