# Comparing `tmp/dotprompt-0.1.7.tar.gz` & `tmp/dotprompt-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotprompt-0.1.7.tar", last modified: Wed Apr 17 14:38:27 2024, max compression
+gzip compressed data, was "dotprompt-0.1.8.tar", last modified: Wed Apr 17 15:55:29 2024, max compression
```

## Comparing `dotprompt-0.1.7.tar` & `dotprompt-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:27.979536 dotprompt-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 14:38:17.000000 dotprompt-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44053 2024-04-17 14:38:27.975536 dotprompt-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-17 14:38:17.000000 dotprompt-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:27.975536 dotprompt-0.1.7/dotprompt/
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-17 14:38:17.000000 dotprompt-0.1.7/dotprompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-17 14:38:17.000000 dotprompt-0.1.7/dotprompt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-17 14:38:17.000000 dotprompt-0.1.7/dotprompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:27.975536 dotprompt-0.1.7/dotprompt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44053 2024-04-17 14:38:27.000000 dotprompt-0.1.7/dotprompt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-17 14:38:27.000000 dotprompt-0.1.7/dotprompt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:38:27.000000 dotprompt-0.1.7/dotprompt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 14:38:27.000000 dotprompt-0.1.7/dotprompt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 14:38:27.000000 dotprompt-0.1.7/dotprompt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-17 14:38:17.000000 dotprompt-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 14:38:27.979536 dotprompt-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-17 14:38:17.000000 dotprompt-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:55:29.825224 dotprompt-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 15:55:22.000000 dotprompt-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44053 2024-04-17 15:55:29.825224 dotprompt-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-17 15:55:22.000000 dotprompt-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:55:29.821224 dotprompt-0.1.8/dotprompt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-17 15:55:22.000000 dotprompt-0.1.8/dotprompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-17 15:55:22.000000 dotprompt-0.1.8/dotprompt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-17 15:55:22.000000 dotprompt-0.1.8/dotprompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:55:29.821224 dotprompt-0.1.8/dotprompt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44053 2024-04-17 15:55:29.000000 dotprompt-0.1.8/dotprompt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-17 15:55:29.000000 dotprompt-0.1.8/dotprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:55:29.000000 dotprompt-0.1.8/dotprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 15:55:29.000000 dotprompt-0.1.8/dotprompt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 15:55:29.000000 dotprompt-0.1.8/dotprompt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-17 15:55:22.000000 dotprompt-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:55:29.825224 dotprompt-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-17 15:55:22.000000 dotprompt-0.1.8/setup.py
```

### Comparing `dotprompt-0.1.7/LICENSE` & `dotprompt-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dotprompt-0.1.7/PKG-INFO` & `dotprompt-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotprompt
-Version: 0.1.7
+Version: 0.1.8
 Summary: Module to incorporate .prompt file to your python code for GenAI
 Author-email: AKoscianski <arnaud.koscianski@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dotprompt-0.1.7/README.md` & `dotprompt-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dotprompt-0.1.7/dotprompt/__init__.py` & `dotprompt-0.1.8/dotprompt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 import os
 import inspect
 import sys
 from .prompt import Prompt
 from .exceptions import PrompDirectoryNotFoundError, PromptError
 
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 
 IGNORED_EXT = ['py']
 
 
 logging.info("Loading prompt files")
 __prompt_dir =os.path.join(os.getcwd(), 'prompts')
 if not os.path.isdir(__prompt_dir):
+    logging.warning(f"Prompt directory \"prompts\" not found in {__prompt_dir}")
     not_found = True
     ROOT_DIR = os.path.abspath(os.curdir)
     caller_path = os.path.dirname(sys.argv[0])
+    logging.warning(f"Crawling from {caller_path}")
     while not_found:
         if "prompts" in os.listdir(caller_path):
             __prompt_dir = os.path.join(caller_path, "prompts")
             not_found = False
         elif caller_path == ROOT_DIR:
             raise PrompDirectoryNotFoundError(f"No prompt dir found in {ROOT_DIR}")
         caller_path = os.path.dirname(caller_path)
```

### Comparing `dotprompt-0.1.7/dotprompt/prompt.py` & `dotprompt-0.1.8/dotprompt/prompt.py`

 * *Files identical despite different names*

### Comparing `dotprompt-0.1.7/dotprompt.egg-info/PKG-INFO` & `dotprompt-0.1.8/dotprompt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotprompt
-Version: 0.1.7
+Version: 0.1.8
 Summary: Module to incorporate .prompt file to your python code for GenAI
 Author-email: AKoscianski <arnaud.koscianski@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dotprompt-0.1.7/pyproject.toml` & `dotprompt-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dotprompt"
-version = "0.1.7"
+version = "0.1.8"
 description = "Module to incorporate .prompt file to your python code for GenAI"
 readme = "README.md"
 authors = [{ name = "AKoscianski", email = "arnaud.koscianski@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -25,15 +25,15 @@
 [project.urls]
 Homepage = "https://github.com/Akoscianski/dotprompt"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver]
-current_version = "0.1.7"
+current_version = "0.1.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

