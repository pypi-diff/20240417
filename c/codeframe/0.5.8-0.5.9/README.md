# Comparing `tmp/codeframe-0.5.8.tar.gz` & `tmp/codeframe-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeframe-0.5.8.tar", last modified: Mon Apr 15 11:21:46 2024, max compression
+gzip compressed data, was "codeframe-0.5.9.tar", last modified: Wed Apr 17 13:52:46 2024, max compression
```

## Comparing `codeframe-0.5.8.tar` & `codeframe-0.5.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 11:21:46.859549 codeframe-0.5.8/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     2484 2024-04-15 11:21:46.859549 codeframe-0.5.8/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2025 2024-04-15 11:21:02.000000 codeframe-0.5.8/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 11:21:46.851549 codeframe-0.5.8/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11703 2024-04-15 08:56:26.000000 codeframe-0.5.8/bin/codeframe
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 11:21:46.855549 codeframe-0.5.8/codeframe/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-01-17 17:42:18.000000 codeframe-0.5.8/codeframe/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    10240 2024-04-09 08:16:32.000000 codeframe-0.5.8/codeframe/cmd_parser.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6895 2024-03-20 08:17:13.000000 codeframe-0.5.8/codeframe/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 11:21:46.855549 codeframe-0.5.8/codeframe/data/
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 11:21:46.855549 codeframe-0.5.8/codeframe/data/installation_files/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      461 2024-04-15 11:20:58.000000 codeframe-0.5.8/codeframe/data/installation_files/.bumpversion.cfg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       83 2024-04-15 11:20:58.000000 codeframe-0.5.8/codeframe/data/installation_files/.gitignore
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1845 2024-04-15 11:20:58.000000 codeframe-0.5.8/codeframe/data/installation_files/README.org
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-03-19 15:01:37.000000 codeframe-0.5.8/codeframe/data/installation_files/__init__.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 11:21:46.855549 codeframe-0.5.8/codeframe/data/installation_files/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11703 2024-04-15 11:20:58.000000 codeframe-0.5.8/codeframe/data/installation_files/bin/codeframe
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11703 2024-04-15 11:20:58.000000 codeframe-0.5.8/codeframe/data/installation_files/bin_codeframe.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 11:21:46.855549 codeframe-0.5.8/codeframe/data/installation_files/codeframe/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-04-15 11:20:58.000000 codeframe-0.5.8/codeframe/data/installation_files/codeframe/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3944 2024-04-15 11:20:58.000000 codeframe-0.5.8/codeframe/data/installation_files/distcheck.sh
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      291 2024-04-15 11:20:58.000000 codeframe-0.5.8/codeframe/data/installation_files/requirements.txt
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1861 2024-04-15 11:20:58.000000 codeframe-0.5.8/codeframe/data/installation_files/setup.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2024-03-19 14:47:38.000000 codeframe-0.5.8/codeframe/data/testing
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4075 2024-03-20 08:16:36.000000 codeframe-0.5.8/codeframe/df_table.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      633 2024-04-09 08:07:38.000000 codeframe-0.5.8/codeframe/fn_load.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9408 2024-04-15 11:07:07.000000 codeframe-0.5.8/codeframe/installation.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9460 2024-04-08 14:32:43.000000 codeframe-0.5.8/codeframe/interpreter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8898 2024-04-15 08:51:16.000000 codeframe-0.5.8/codeframe/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5135 2024-04-15 11:14:15.000000 codeframe-0.5.8/codeframe/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2897 2024-01-23 13:00:22.000000 codeframe-0.5.8/codeframe/topbar.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-15 11:21:46.000000 codeframe-0.5.8/codeframe/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 11:21:46.855549 codeframe-0.5.8/codeframe.egg-info/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     2484 2024-04-15 11:21:46.000000 codeframe-0.5.8/codeframe.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      990 2024-04-15 11:21:46.000000 codeframe-0.5.8/codeframe.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-15 11:21:46.000000 codeframe-0.5.8/codeframe.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       76 2024-04-15 11:21:46.000000 codeframe-0.5.8/codeframe.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2024-04-15 11:21:46.000000 codeframe-0.5.8/codeframe.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-15 11:21:46.859549 codeframe-0.5.8/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1861 2024-03-19 15:48:21.000000 codeframe-0.5.8/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-17 13:52:46.895927 codeframe-0.5.9/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     2484 2024-04-17 13:52:46.895927 codeframe-0.5.9/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2025 2024-04-17 13:52:41.000000 codeframe-0.5.9/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-17 13:52:46.891927 codeframe-0.5.9/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11768 2024-04-17 13:52:43.000000 codeframe-0.5.9/bin/codeframe
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-17 13:52:46.891927 codeframe-0.5.9/codeframe/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-01-17 17:42:18.000000 codeframe-0.5.9/codeframe/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11072 2024-04-17 13:50:37.000000 codeframe-0.5.9/codeframe/cmd_parser.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6917 2024-04-17 13:19:17.000000 codeframe-0.5.9/codeframe/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-17 13:52:46.895927 codeframe-0.5.9/codeframe/data/
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-17 13:52:46.895927 codeframe-0.5.9/codeframe/data/installation_files/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      461 2024-04-17 13:52:37.000000 codeframe-0.5.9/codeframe/data/installation_files/.bumpversion.cfg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       83 2024-04-17 13:52:37.000000 codeframe-0.5.9/codeframe/data/installation_files/.gitignore
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1845 2024-04-17 13:52:37.000000 codeframe-0.5.9/codeframe/data/installation_files/README.org
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-03-19 15:01:37.000000 codeframe-0.5.9/codeframe/data/installation_files/__init__.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-17 13:52:46.895927 codeframe-0.5.9/codeframe/data/installation_files/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11703 2024-04-17 13:52:37.000000 codeframe-0.5.9/codeframe/data/installation_files/bin/codeframe
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11768 2024-04-17 13:52:37.000000 codeframe-0.5.9/codeframe/data/installation_files/bin_codeframe.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-17 13:52:46.895927 codeframe-0.5.9/codeframe/data/installation_files/codeframe/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-04-17 13:52:37.000000 codeframe-0.5.9/codeframe/data/installation_files/codeframe/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3944 2024-04-17 13:52:37.000000 codeframe-0.5.9/codeframe/data/installation_files/distcheck.sh
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      291 2024-04-17 13:52:37.000000 codeframe-0.5.9/codeframe/data/installation_files/requirements.txt
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1861 2024-04-17 13:52:37.000000 codeframe-0.5.9/codeframe/data/installation_files/setup.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2024-03-19 14:47:38.000000 codeframe-0.5.9/codeframe/data/testing
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4075 2024-03-20 08:16:36.000000 codeframe-0.5.9/codeframe/df_table.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      919 2024-04-17 13:44:28.000000 codeframe-0.5.9/codeframe/fn_load.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9408 2024-04-15 11:07:07.000000 codeframe-0.5.9/codeframe/installation.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9994 2024-04-17 13:35:42.000000 codeframe-0.5.9/codeframe/interpreter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8898 2024-04-15 08:51:16.000000 codeframe-0.5.9/codeframe/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5135 2024-04-15 11:14:15.000000 codeframe-0.5.9/codeframe/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2897 2024-01-23 13:00:22.000000 codeframe-0.5.9/codeframe/topbar.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-17 13:52:46.000000 codeframe-0.5.9/codeframe/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-17 13:52:46.895927 codeframe-0.5.9/codeframe.egg-info/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     2484 2024-04-17 13:52:46.000000 codeframe-0.5.9/codeframe.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      990 2024-04-17 13:52:46.000000 codeframe-0.5.9/codeframe.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-17 13:52:46.000000 codeframe-0.5.9/codeframe.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       76 2024-04-17 13:52:46.000000 codeframe-0.5.9/codeframe.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2024-04-17 13:52:46.000000 codeframe-0.5.9/codeframe.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-17 13:52:46.895927 codeframe-0.5.9/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1861 2024-03-19 15:48:21.000000 codeframe-0.5.9/setup.py
```

### Comparing `codeframe-0.5.8/PKG-INFO` & `codeframe-0.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeframe
-Version: 0.5.8
+Version: 0.5.9
 Summary: Automatically created environment for python package
 Home-page: https://gitlab.com/jaromrax/codeframe
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `codeframe-0.5.8/README.md` & `codeframe-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.8/bin/codeframe` & `codeframe-0.5.9/codeframe/data/installation_files/bin/codeframe`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.8/codeframe/cmd_parser.py` & `codeframe-0.5.9/codeframe/cmd_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 #
 #
 import shlex
 import inspect
 import fnmatch
 from codeframe.version import __version__
 from codeframe import config
+#from codeframe.config import object_list
 from console import fg,bg
 import glob
 #
 #import importlib_resources
 import importlib
 import sys
 import os
 #from importlib import import_module
 #
 # Assuming dflist is a global variable
-dflist = ['df1', 'df2', 'df3', 'd11', 'd21','h11']
+
+#config.object_list = ['df1', 'df2', 'df3', 'd11', 'd21','h11']
 
 #############################################################
 #
 #############################################################
 
 
 
@@ -59,18 +61,18 @@
     if len(filescur)==0:
         asdqwe541 = 1
         #print("D... NO python FILES available in current directory (listpy)")
         # return None
         #files = filescur
     else:
         corenames = [ os.path.splitext(x)[0].split(pretext)[1] for x in filescur]
-        if DEBUG: print(f"D... modules available in CURR:\n          {corenames}")
+        if DEBUG: print(f"{fg.dimgray}D... modules available in CURR: {fg.default} {corenames}")
         # files = [x for x in files if x.find("pr_model_")!=0] # models- I exclude?
         files =  files + filescur
-        if DEBUG: print(f"i... modules available: \n{files}\n")
+        if DEBUG: print(f"{fg.dimgray}D... modules available:{fg.default}} {files}")
     return files
 
 
 
 
 
 #############################################################
@@ -108,30 +110,30 @@
         #print(f" ... searching /{intit}/ in {ffile} ")
 
         if (intit == construct):
             #print(f"P... got {ffile}")
             #print("i... trying to importlib:", item.GetTitle() )
             # UNimport module first - case there was an error there previously
             unloadname = f"{pretext}{intit}"
-            if DEBUG: print(f"D... module /{unloadname}/ ... ", end="")
+            if DEBUG: print(f"{fg.dimgray}D... module /{unloadname}/ ... {fg.default}", end="")
             try:
                 sys.modules.pop( unloadname ) # ffile[:-3]     f"pr_{construct}")
-                if DEBUG: print("... unloaded successfully, loading now...")
+                if DEBUG: print(f"{fg.dimggray}... unloaded successfully, loading now...{fg.default}")
             except:
-                if DEBUG: print("... not unloaded, loading now...")
+                if DEBUG: print(f"{fg.dimgray}... not unloaded, loading now...{fg.default}")
 
             # IMPORT
             #print("D... importing module")
             #module = importlib.import_module( ffile[:-3] ) # older
 
             spec = importlib.util.spec_from_file_location( pretext+intit, ffile )
             module = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(module)
 
-            if DEBUG: print("D... importing module DONE")
+            if DEBUG: print(f"{fg.dimgray}D... importing module DONE{fg.default}")
             #break
 
     return module
 # ---------------------------------------------------------------
 
 
 
@@ -193,56 +195,65 @@
     results = []
 
     if len(tokens)==0:
         results.append( func() )
         return results
 
     it = iter(tokens)
-    print("D... tokens:", tokens)
+    print(f"{fg.dimgray}D... tokens:{fg.default}", tokens)
     for token in it:
         if token.endswith('*') or '*' in token:
             # Handle the pattern matching by deferring execution until later
             args.append(token)
         elif token.startswith('-'):
             # Remove the '-' prefix
             flag = token.lstrip('-')
             value = next(it, None)
             # Attempt to match the flag to known parameters
             matched_params = [p for p in sig.parameters if p.startswith(flag)]
             if not matched_params:
+                print(f"X... ERROR - unknown flag {token}")
+                return []
                 raise ValueError(f"Unknown flag: {token}")
             if len(matched_params) > 1:
+                print(f"X... ERROR - ambiguous flag {token}")
+                return []
                 raise ValueError(f"Ambiguous flag: {token}")
             param_name = matched_params[0]
             param = sig.parameters[param_name]
             # Convert the value to the correct type based on the default value
             if param.default is not inspect.Parameter.empty and param.default is not None:
                 if isinstance(param.default, bool):
                     value = value.lower() in ('true', 'yes', '1')
                 else:
                     value = type(param.default)(value)
             elif param.default is None:
                 # If the default is None, we keep the value as a string
                 pass
             kwargs[param_name] = value
         else:
-            if DEBUG: print("D... appending ", token)
+            if DEBUG: print(f"{fg.dimgray}D... appending {fg.default}", token)
             args.append(token)
 
     for pattern in args:
-        if DEBUG: print("D... working on arg:", pattern)
-        # Run the function for each dataframe in dflist that matches the pattern
+        if DEBUG: print(f"{fg.dimgray}D... working on arg:{fg.default}", pattern)
+        matching_dfs=[]
+        # Run the function for each dataframe in config.object_list that matches the pattern
         if use_files:
-            if DEBUG: print("D... interpreting pattern as a file:", pattern)
+            if DEBUG: print(f"{fg.dimgray}D... interpreting pattern as a file:{fg.default}", pattern)
             matching_dfs = glob.glob( pattern )
-        elif pattern in dflist:
-            if DEBUG: print("D... argument {pattern}IS  in the list of allowed objects")
-            matching_dfs = fnmatch.filter(dflist, pattern)
+            if len(matching_dfs)==0:
+                print(f"{fg.red}X... no files match /{pattern}/{fg.default}")
+        elif pattern in config.object_list:
+            if DEBUG: print(f"{fg.dimgray}D... argument /{pattern}/ IS  in the list of allowed objects{fg.default}")
+            matching_dfs = fnmatch.filter(config.object_list, pattern)
+            if len(matching_dfs)==0:
+                print(f"{fg.red}X... no objects match /{pattern}/{fg.default}")
         else:
-            print("X... argument {pattern} NOT in the list of allowed objects")
+            print(f"{fg.red}X... argument /{pattern}/ IS NOT in the list of allowed objects:{fg.default}", config.object_list)
         #
         for dfname in matching_dfs:
             # Substitute '$' with the dataframe name for all kwargs
             modified_kwargs = {k: v.replace('$', dfname) if isinstance(v, str) and '$' in v else v
                                for k, v in kwargs.items()}
             try:
                 results.append(func(dfname, **modified_kwargs))
```

### Comparing `codeframe-0.5.8/codeframe/config.py` & `codeframe-0.5.9/codeframe/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         'history':'~/.config/codeframe/history',
         'quit':False         #
 }
 
 #================================== all global variables are recommended to store here
 global_variables_here = None
 
+object_list = ['df1']
 #================================== all global variables are recommended to store here
 
 #CFG_DEBUG = True
 CFG_DEBUG = False
 myPromptSession = None
 
 # ========================================= some general terminal OPS
```

### Comparing `codeframe-0.5.8/codeframe/data/installation_files/README.org` & `codeframe-0.5.9/codeframe/data/installation_files/README.org`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.8/codeframe/data/installation_files/bin/codeframe` & `codeframe-0.5.9/bin/codeframe`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.completion import NestedCompleter
 
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 
 # ========================
-SHOW_LOGO_TABLE = True
-SHOW_TIME = True
+SHOW_LOGO_TABLE = False
+SHOW_TIME = False
 SHOW_COMMAND_LINE = True
 RUN_MMAP_INPUT = True  #  INTERACTIVE MMAP-INTERACTIVE
 RUN_SELECT_FROM_TABLE = False
 
 termsize = os.get_terminal_size().columns
 
 # import pandas as pd
@@ -100,25 +100,28 @@
         print("i... RESET TERMINAL")
         os.system("reset")
         #terminal.clear()
         termsize = termsize2
         move_cursor(3, 1)
         #print("X")
 
-def main(projectname=None, debug=False, keyboard_remote_start = False, servermode = False):
+def main(projectname=None, debug=False, keyboard_remote_start = False, servermode = False, logo = False):
     """
     Main function of the project. When 'projectname' given: new project is created
 
     Parameters:
     projectname: THIS WILL GENERATE NEW PROJECT with these modules
     keyboard_remote_start: just start a standalone prompt
     servermode: wait for commands via mmap... to be used with -k
     """
     global RUN_SELECT_FROM_TABLE, SHOW_LOGO_TABLE, SHOW_TIME, RUN_MMAP_INPUT
 
+    SHOW_LOGO_TABLE = logo
+    SHOW_TIME = logo
+
     if not servermode: RUN_MMAP_INPUT = False
     # GLobal clear terminal
     if debug:
         print(__version__)
     #else:
 
     signal.signal(signal.SIGWINCH, handle_sigwinch)
```

### Comparing `codeframe-0.5.8/codeframe/data/installation_files/bin_codeframe.py` & `codeframe-0.5.9/codeframe/data/installation_files/bin_codeframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.completion import NestedCompleter
 
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 
 # ========================
-SHOW_LOGO_TABLE = True
-SHOW_TIME = True
+SHOW_LOGO_TABLE = False
+SHOW_TIME = False
 SHOW_COMMAND_LINE = True
 RUN_MMAP_INPUT = True  #  INTERACTIVE MMAP-INTERACTIVE
 RUN_SELECT_FROM_TABLE = False
 
 termsize = os.get_terminal_size().columns
 
 # import pandas as pd
@@ -100,25 +100,28 @@
         print("i... RESET TERMINAL")
         os.system("reset")
         #terminal.clear()
         termsize = termsize2
         move_cursor(3, 1)
         #print("X")
 
-def main(projectname=None, debug=False, keyboard_remote_start = False, servermode = False):
+def main(projectname=None, debug=False, keyboard_remote_start = False, servermode = False, logo = False):
     """
     Main function of the project. When 'projectname' given: new project is created
 
     Parameters:
     projectname: THIS WILL GENERATE NEW PROJECT with these modules
     keyboard_remote_start: just start a standalone prompt
     servermode: wait for commands via mmap... to be used with -k
     """
     global RUN_SELECT_FROM_TABLE, SHOW_LOGO_TABLE, SHOW_TIME, RUN_MMAP_INPUT
 
+    SHOW_LOGO_TABLE = logo
+    SHOW_TIME = logo
+
     if not servermode: RUN_MMAP_INPUT = False
     # GLobal clear terminal
     if debug:
         print(__version__)
     #else:
 
     signal.signal(signal.SIGWINCH, handle_sigwinch)
```

### Comparing `codeframe-0.5.8/codeframe/data/installation_files/distcheck.sh` & `codeframe-0.5.9/codeframe/data/installation_files/distcheck.sh`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.8/codeframe/data/installation_files/setup.py` & `codeframe-0.5.9/codeframe/data/installation_files/setup.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.8/codeframe/df_table.py` & `codeframe-0.5.9/codeframe/df_table.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.8/codeframe/fn_load.py` & `codeframe-0.5.9/codeframe/fn_load.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,16 +9,24 @@
   -  yes, but is there possible to do without?
      - ? for the sake of codeframe initial paradigm? or is that ok?
 
 """
 
 from fire import Fire
 from console import fg,bg
+from codeframe import config
+# I NEED TO UPDATE  -   config.object_list
 
 
-def load():  print("in load @ fn_load ... but this doeasnt happen normally")
-
 def main(*args,**kwargs):
-    print(f"D... @main @fn_load /{args}/{kwargs}/. module loaded, function called")
+    print(f"{fg.dimgray}D... main() @fn_lo: args/kwargs.../{args}/{kwargs}/{fg.default}")
+    #print(f"D... main() @fn_load: args/kwargs.../{args}/{kwargs}/")
+    if len(args)==0:
+        print("X... give me a file as a parameter...")
+        return None
+    # ===== loading
+    print(f"{fg.green}i... loading {args[0]}{fg.default}")
+    config.object_list.append( args[0] )
+
 
 if __name__=="__main__":
     Fire(main)
```

### Comparing `codeframe-0.5.8/codeframe/installation.py` & `codeframe-0.5.9/codeframe/installation.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.8/codeframe/interpreter.py` & `codeframe-0.5.9/codeframe/interpreter.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,30 @@
 from codeframe.config import  move_cursor
 import subprocess as sp
 from console import fg,bg
 import glob
 import shlex
 
 
-# SHELL COMMANDS with files as parameters
+# ===================================  all commands are in 2 main groups ===========
+#                     shell (just pass to shell)
+#                     local - each one needs to have its own module defined
+# SHELL COMMANDS with files as parameters (ll is extended here)
 KNOWN_COMMANDS_SHELL_FS = ['ls','ll','fdfind','head','tail','cat']
 # other shell commands
 KNOWN_COMMANDS_SHELL_OTHER = ['ag']
-# calling functions
-KNOWN_COMMANDS_LOCAL = ['zoom','unzoom','connect','reset']
+# call functions@fn_modules -  objects as parameters -  must be defined
+KNOWN_COMMANDS_LOCAL = ['lo','show','zoom','unzoom','connect','reset']
+# call functions@fn_modules - files as parameters
 KNOWN_COMMANDS_LOCAL_FS = ['load']
+#
+# ============================================================================= summary
 KNOWN_COMMANDS = KNOWN_COMMANDS_SHELL_FS + KNOWN_COMMANDS_LOCAL + KNOWN_COMMANDS_SHELL_OTHER + KNOWN_COMMANDS_LOCAL_FS
 
+
 #============================================= prepare for completions =======================
 # now create nested completion dict
 KNOWN_COMMANDS_DICT = {}
 for i in KNOWN_COMMANDS:
     KNOWN_COMMANDS_DICT[i]=None
 # now create special completion for filemanagement
 allfiles = glob.glob("*")
@@ -46,14 +53,17 @@
         print(f".../{inp}/==/{res}/..")
         if res==inp:
             break
         time.sleep(1)
 
 
 def exclude(cmd=""):
+    """
+    certain protection from malicious shell string...
+    """
     bad = False
     if cmd.find("&")>=0:  bad = True
     if cmd.find("|")>=0:  bad = True
     if cmd.find("'")>=0:  bad = True
     if cmd.find('$')>=0:  bad = True
     if cmd.find('%')>=0:  bad = True
     if cmd.find('#')>=0:  bad = True
@@ -229,34 +239,33 @@
 
             #if kw1 in KNOWN_COMMANDS_SHELL_OTHER:
             if kw1 in KNOWN_COMMANDS_SHELL_FS or kw1 in KNOWN_COMMANDS_SHELL_OTHER:
                 # replace some commands
                 if kw1=="ll": cmd = "ls -l "+kw2
                 run_or_die(cmd)
 
-            elif kw1 in KNOWN_COMMANDS_LOCAL: # zoom
-                # full control of cmd_parser ------- object list ----------
-                # func = getattr( cmd_parser, kw1) # WHEN ELSEWHERE
-                # --------- get the function from globals --------------------
-                func =  globals()[kw1] # WHEN HERE
-                # --------- HA! import a module fn_yrname
+            elif kw1 in KNOWN_COMMANDS_LOCAL: # zoom, show
+                ### full control of cmd_parser ------- object list ----------
+                ### func = getattr( cmd_parser, kw1) # WHEN ELSEWHERE
+                ### --------- get the function from globals --------------------
+                #func =  globals()[kw1] # WHEN HERE
+                ### --------- HA! import a module fn_yrname
                 func =  cmd_parser.str_func_to_func( kw1 )
                 func = func.main
                 res = cmd_parser.call_function_with_command( func , kw2)
                 for i in res: print("RES:",i) # print results
 
             elif kw1 in KNOWN_COMMANDS_LOCAL_FS:  # load
-                # ----- I need to do glob myself and call repetitively -------
-                # I try to import a module =======
-                #
-
-                # func = getattr( cmd_parser, kw1) # WHEN ELSEWHERE
-                # --------- get the function from globals --------------------
-                func =  globals()[kw1]
-                # --------- HA! import a module fn_yrname
+                ### ----- I need to do glob myself and call repetitively -------
+                ### I try to import a module =======
+                ###
+                ### func = getattr( cmd_parser, kw1) # WHEN ELSEWHERE
+                ### --------- get the function from globals --------------------
+                #func =  globals()[kw1]
+                ### --------- HA! import a module fn_yrname
                 func =  cmd_parser.str_func_to_func( kw1 )
                 func = func.main
 
                 # kw2_bis = iterate_star( kw2 )
                 #for i in kw2_bis:
                 res = cmd_parser.call_function_with_command( func , kw2, use_files=True)
                 #for i in res: print("RES:",i) # print results
```

### Comparing `codeframe-0.5.8/codeframe/key_enter.py` & `codeframe-0.5.9/codeframe/key_enter.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.8/codeframe/mmapwr.py` & `codeframe-0.5.9/codeframe/mmapwr.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.8/codeframe/topbar.py` & `codeframe-0.5.9/codeframe/topbar.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.8/codeframe.egg-info/PKG-INFO` & `codeframe-0.5.9/codeframe.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeframe
-Version: 0.5.8
+Version: 0.5.9
 Summary: Automatically created environment for python package
 Home-page: https://gitlab.com/jaromrax/codeframe
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `codeframe-0.5.8/codeframe.egg-info/SOURCES.txt` & `codeframe-0.5.9/codeframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.8/setup.py` & `codeframe-0.5.9/setup.py`

 * *Files identical despite different names*

