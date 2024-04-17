# Comparing `tmp/macnotesapp-0.6.0.tar.gz` & `tmp/macnotesapp-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macnotesapp-0.6.0.tar", max compression
+gzip compressed data, was "macnotesapp-0.6.1.tar", max compression
```

## Comparing `macnotesapp-0.6.0.tar` & `macnotesapp-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2023-08-21 03:41:17.620013 macnotesapp-0.6.0/LICENSE
--rw-r--r--   0        0        0     7750 2024-04-13 21:24:04.058980 macnotesapp-0.6.0/README.md
--rw-r--r--   0        0        0      235 2023-08-21 03:41:17.622887 macnotesapp-0.6.0/macnotesapp/__init__.py
--rw-r--r--   0        0        0      108 2023-08-21 03:41:17.623129 macnotesapp-0.6.0/macnotesapp/__main__.py
--rw-r--r--   0        0        0       43 2024-04-13 21:28:01.028684 macnotesapp-0.6.0/macnotesapp/_version.py
--rw-r--r--   0        0        0       53 2023-08-21 03:41:17.623603 macnotesapp-0.6.0/macnotesapp/cli/__init__.py
--rw-r--r--   0        0        0    15167 2023-08-22 13:47:29.871421 macnotesapp-0.6.0/macnotesapp/cli/cli.py
--rw-r--r--   0        0        0     2848 2023-08-22 14:26:32.748205 macnotesapp-0.6.0/macnotesapp/cli/cli_config.py
--rw-r--r--   0        0        0     8287 2023-08-21 03:41:17.624527 macnotesapp-0.6.0/macnotesapp/cli/cli_help.py
--rw-r--r--   0        0        0      305 2023-08-21 03:41:17.624760 macnotesapp-0.6.0/macnotesapp/cli/cli_param_types.py
--rw-r--r--   0        0        0     8588 2023-08-21 03:41:17.625096 macnotesapp-0.6.0/macnotesapp/cli/click_rich_echo.py
--rw-r--r--   0        0        0      754 2023-08-21 03:41:17.625426 macnotesapp-0.6.0/macnotesapp/cli/readable.py
--rw-r--r--   0        0        0      509 2023-08-22 14:17:02.413122 macnotesapp-0.6.0/macnotesapp/logging.py
--rw-r--r--   0        0        0    13597 2023-08-21 03:41:17.625813 macnotesapp-0.6.0/macnotesapp/macnotesapp.applescript
--rw-r--r--   0        0        0    13931 2023-08-21 03:41:17.626047 macnotesapp-0.6.0/macnotesapp/macnotesapp_applescript.py
--rw-r--r--   0        0        0    28440 2023-08-22 14:17:02.414155 macnotesapp-0.6.0/macnotesapp/notesapp.py
--rw-r--r--   0        0        0      453 2023-08-22 14:17:02.415119 macnotesapp-0.6.0/macnotesapp/script_loader.py
--rw-r--r--   0        0        0      893 2023-08-22 14:17:02.415924 macnotesapp-0.6.0/macnotesapp/utils.py
--rw-r--r--   0        0        0     1396 2024-04-13 21:28:01.029850 macnotesapp-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     9106 1970-01-01 00:00:00.000000 macnotesapp-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-21 03:41:17.620013 macnotesapp-0.6.1/LICENSE
+-rw-r--r--   0        0        0     7750 2024-04-13 21:24:04.058980 macnotesapp-0.6.1/README.md
+-rw-r--r--   0        0        0      235 2023-08-21 03:41:17.622887 macnotesapp-0.6.1/macnotesapp/__init__.py
+-rw-r--r--   0        0        0      108 2023-08-21 03:41:17.623129 macnotesapp-0.6.1/macnotesapp/__main__.py
+-rw-r--r--   0        0        0       43 2024-04-17 04:04:25.650872 macnotesapp-0.6.1/macnotesapp/_version.py
+-rw-r--r--   0        0        0       53 2023-08-21 03:41:17.623603 macnotesapp-0.6.1/macnotesapp/cli/__init__.py
+-rw-r--r--   0        0        0    15167 2023-08-22 13:47:29.871421 macnotesapp-0.6.1/macnotesapp/cli/cli.py
+-rw-r--r--   0        0        0     2848 2023-08-22 14:26:32.748205 macnotesapp-0.6.1/macnotesapp/cli/cli_config.py
+-rw-r--r--   0        0        0     8287 2023-08-21 03:41:17.624527 macnotesapp-0.6.1/macnotesapp/cli/cli_help.py
+-rw-r--r--   0        0        0      305 2023-08-21 03:41:17.624760 macnotesapp-0.6.1/macnotesapp/cli/cli_param_types.py
+-rw-r--r--   0        0        0     8588 2023-08-21 03:41:17.625096 macnotesapp-0.6.1/macnotesapp/cli/click_rich_echo.py
+-rw-r--r--   0        0        0      754 2023-08-21 03:41:17.625426 macnotesapp-0.6.1/macnotesapp/cli/readable.py
+-rw-r--r--   0        0        0      509 2023-08-22 14:17:02.413122 macnotesapp-0.6.1/macnotesapp/logging.py
+-rw-r--r--   0        0        0    13597 2023-08-21 03:41:17.625813 macnotesapp-0.6.1/macnotesapp/macnotesapp.applescript
+-rw-r--r--   0        0        0    13931 2023-08-21 03:41:17.626047 macnotesapp-0.6.1/macnotesapp/macnotesapp_applescript.py
+-rw-r--r--   0        0        0    28440 2023-08-22 14:17:02.414155 macnotesapp-0.6.1/macnotesapp/notesapp.py
+-rw-r--r--   0        0        0      453 2023-08-22 14:17:02.415119 macnotesapp-0.6.1/macnotesapp/script_loader.py
+-rw-r--r--   0        0        0      893 2023-08-22 14:17:02.415924 macnotesapp-0.6.1/macnotesapp/utils.py
+-rw-r--r--   0        0        0     1412 2024-04-17 04:04:25.653218 macnotesapp-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     9194 1970-01-01 00:00:00.000000 macnotesapp-0.6.1/PKG-INFO
```

### Comparing `macnotesapp-0.6.0/LICENSE` & `macnotesapp-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.6.0/README.md` & `macnotesapp-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.6.0/macnotesapp/cli/cli.py` & `macnotesapp-0.6.1/macnotesapp/cli/cli.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.6.0/macnotesapp/cli/cli_config.py` & `macnotesapp-0.6.1/macnotesapp/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.6.0/macnotesapp/cli/cli_help.py` & `macnotesapp-0.6.1/macnotesapp/cli/cli_help.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.6.0/macnotesapp/cli/click_rich_echo.py` & `macnotesapp-0.6.1/macnotesapp/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.6.0/macnotesapp/cli/readable.py` & `macnotesapp-0.6.1/macnotesapp/cli/readable.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.6.0/macnotesapp/macnotesapp.applescript` & `macnotesapp-0.6.1/macnotesapp/macnotesapp.applescript`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.6.0/macnotesapp/macnotesapp_applescript.py` & `macnotesapp-0.6.1/macnotesapp/macnotesapp_applescript.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.6.0/macnotesapp/notesapp.py` & `macnotesapp-0.6.1/macnotesapp/notesapp.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.6.0/macnotesapp/utils.py` & `macnotesapp-0.6.1/macnotesapp/utils.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.6.0/pyproject.toml` & `macnotesapp-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "macnotesapp"
-version = "0.6.0"
+version = "0.6.1"
 description = "Work with Apple MacOS Notes.app from the command line. Also includes python interface for scripting Notes.app from your own python code."
 authors = ["Rhet Turnbull <rturnbull@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/RhetTbull/macnotesapp"
 repository = "https://github.com/RhetTbull/macnotesapp"
 keywords = ["cli", "mac", "macos"]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12" # pyinstaller requires python < 3.12
+python = ">=3.9,<3.13" # pyinstaller requires python < 3.12
 py-applescript = "^1.0.3"
 click = "^8.1.2"
 rich = "^12.4.4"
 markdown2 = "^2.4.3"
 toml = "^0.10.2"
 questionary = "^1.10.0"
 wheel = "^0.37.1"
 readability-lxml = "^0.8.1"
 requests = "^2.28.1"
 validators = "^0.20.0"
 markdownify = "^0.11.6"
 pyobjc-framework-ScriptingBridge = "^9.0.1"
 xdg = "^6.0.0"
 lxml-html-clean = "^0.1.1"
+lxml = "^5.2.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 cogapp = "^3.3.0"
 wheel = "^0.37.1"
 build = "^0.8.0"
 pyinstaller = "^5.7"
```

### Comparing `macnotesapp-0.6.0/PKG-INFO` & `macnotesapp-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: macnotesapp
-Version: 0.6.0
+Version: 0.6.1
 Summary: Work with Apple MacOS Notes.app from the command line. Also includes python interface for scripting Notes.app from your own python code.
 Home-page: https://github.com/RhetTbull/macnotesapp
 License: MIT
 Keywords: cli,mac,macos
 Author: Rhet Turnbull
 Author-email: rturnbull@gmail.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.2,<9.0.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: lxml-html-clean (>=0.1.1,<0.2.0)
 Requires-Dist: markdown2 (>=2.4.3,<3.0.0)
 Requires-Dist: markdownify (>=0.11.6,<0.12.0)
 Requires-Dist: py-applescript (>=1.0.3,<2.0.0)
 Requires-Dist: pyobjc-framework-ScriptingBridge (>=9.0.1,<10.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: readability-lxml (>=0.8.1,<0.9.0)
```

