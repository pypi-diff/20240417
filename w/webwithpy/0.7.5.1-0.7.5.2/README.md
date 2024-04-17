# Comparing `tmp/webwithpy-0.7.5.1.tar.gz` & `tmp/webwithpy-0.7.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webwithpy-0.7.5.1.tar", max compression
+gzip compressed data, was "webwithpy-0.7.5.2.tar", max compression
```

## Comparing `webwithpy-0.7.5.1.tar` & `webwithpy-0.7.5.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.5.1/LICENSE
--rw-r--r--   0        0        0     1021 2024-04-09 09:13:10.442038 webwithpy-0.7.5.1/README.md
--rw-r--r--   0        0        0      571 2024-04-10 09:36:54.271747 webwithpy-0.7.5.1/pyproject.toml
--rw-r--r--   0        0        0      163 2024-04-10 07:14:22.692581 webwithpy-0.7.5.1/webwithpy/__init__.py
--rw-r--r--   0        0        0      362 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/app.py
--rw-r--r--   0        0        0     1657 2024-04-10 09:29:34.540380 webwithpy-0.7.5.1/webwithpy/commands.py
--rw-r--r--   0        0        0      726 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/exeptions/HttpExceptions.py
--rw-r--r--   0        0        0      807 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/exeptions/RouteExceptions.py
--rw-r--r--   0        0        0      895 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/exeptions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/helper/__init__.py
--rw-r--r--   0        0        0      321 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/helper/async_handler.py
--rw-r--r--   0        0        0      204 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/html/__init__.py
--rw-r--r--   0        0        0       33 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/html/data/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/html/data/ast.py
--rw-r--r--   0        0        0      467 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/html/data/token.py
--rw-r--r--   0        0        0    16701 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/html/forms.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/html/helpers/__init__.py
--rw-r--r--   0        0        0      101 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/html/helpers/str_helper.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/html/html_exception/__init__.py
--rw-r--r--   0        0        0       40 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/html/html_exception/exceptions.py
--rw-r--r--   0        0        0     4357 2024-04-09 09:26:12.477690 webwithpy-0.7.5.1/webwithpy/html/lexer.py
--rw-r--r--   0        0        0     2034 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/html/parser.py
--rw-r--r--   0        0        0     4461 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/html/pyhtml.py
--rw-r--r--   0        0        0     3910 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/html/renderer.py
--rw-r--r--   0        0        0       53 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/http/__init__.py
--rw-r--r--   0        0        0      798 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/http/cookies.py
--rw-r--r--   0        0        0     3039 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/http/handler.py
--rw-r--r--   0        0        0      485 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/http/redirect.py
--rw-r--r--   0        0        0     5347 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/http/request.py
--rw-r--r--   0        0        0     3874 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/http/response.py
--rw-r--r--   0        0        0      751 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/http/urls.py
--rw-r--r--   0        0        0       99 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/__init__.py
--rw-r--r--   0        0        0     6260 2024-04-10 09:16:23.493948 webwithpy-0.7.5.1/webwithpy/orm/auth.py
--rw-r--r--   0        0        0     3644 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/core.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/dialect/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/dialect/base.py
--rw-r--r--   0        0        0     1764 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/dialect/mysql.py
--rw-r--r--   0        0        0     1763 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/dialect/sqlite.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/drivers/__init__.py
--rw-r--r--   0        0        0     1178 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/drivers/driver.py
--rw-r--r--   0        0        0     2803 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/drivers/mysql.py
--rw-r--r--   0        0        0     2801 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/drivers/sqlite.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/helpers/__init__.py
--rw-r--r--   0        0        0     1550 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/helpers/settings.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/objects/__init__.py
--rw-r--r--   0        0        0     5432 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/objects/objects.py
--rw-r--r--   0        0        0     5122 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/orm/objects/query.py
--rw-r--r--   0        0        0     1082 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/persistence.py
--rw-r--r--   0        0        0       70 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/routing/__init__.py
--rw-r--r--   0        0        0     1785 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/routing/methods.py
--rw-r--r--   0        0        0     5832 2024-04-10 09:03:15.499903 webwithpy-0.7.5.1/webwithpy/routing/router.py
--rw-r--r--   0        0        0     1213 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/static/form.css
--rw-r--r--   0        0        0     1161 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/static/improved_reg_form.css
--rw-r--r--   0        0        0       63 2024-04-10 08:42:40.770674 webwithpy-0.7.5.1/webwithpy/tests/__init__.py
--rw-r--r--   0        0        0      139 2024-04-10 08:42:07.174512 webwithpy-0.7.5.1/webwithpy/tests/case.py
--rw-r--r--   0        0        0      557 2024-04-10 08:29:49.054933 webwithpy-0.7.5.1/webwithpy/tests/helper.py
--rw-r--r--   0        0        0     2759 2024-04-09 07:43:04.000000 webwithpy-0.7.5.1/webwithpy/webwithpy.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 webwithpy-0.7.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.5.2/LICENSE
+-rw-r--r--   0        0        0     1021 2024-04-09 09:13:10.442038 webwithpy-0.7.5.2/README.md
+-rw-r--r--   0        0        0      571 2024-04-17 06:44:34.429056 webwithpy-0.7.5.2/pyproject.toml
+-rw-r--r--   0        0        0      163 2024-04-10 07:14:22.692581 webwithpy-0.7.5.2/webwithpy/__init__.py
+-rw-r--r--   0        0        0      362 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/app.py
+-rw-r--r--   0        0        0     1767 2024-04-16 08:57:26.313852 webwithpy-0.7.5.2/webwithpy/commands.py
+-rw-r--r--   0        0        0      726 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/exeptions/HttpExceptions.py
+-rw-r--r--   0        0        0      807 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/exeptions/RouteExceptions.py
+-rw-r--r--   0        0        0      895 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/exeptions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/helper/__init__.py
+-rw-r--r--   0        0        0      321 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/helper/async_handler.py
+-rw-r--r--   0        0        0      204 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/html/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/html/data/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/html/data/ast.py
+-rw-r--r--   0        0        0      467 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/html/data/token.py
+-rw-r--r--   0        0        0    16701 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/html/forms.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/html/helpers/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/html/helpers/str_helper.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/html/html_exception/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/html/html_exception/exceptions.py
+-rw-r--r--   0        0        0     4357 2024-04-09 09:26:12.477690 webwithpy-0.7.5.2/webwithpy/html/lexer.py
+-rw-r--r--   0        0        0     2034 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/html/parser.py
+-rw-r--r--   0        0        0     4474 2024-04-17 06:43:23.397315 webwithpy-0.7.5.2/webwithpy/html/pyhtml.py
+-rw-r--r--   0        0        0     3910 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/html/renderer.py
+-rw-r--r--   0        0        0       53 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/http/__init__.py
+-rw-r--r--   0        0        0      798 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/http/cookies.py
+-rw-r--r--   0        0        0     3039 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/http/handler.py
+-rw-r--r--   0        0        0      485 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/http/redirect.py
+-rw-r--r--   0        0        0     5347 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/http/request.py
+-rw-r--r--   0        0        0     3874 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/http/response.py
+-rw-r--r--   0        0        0      751 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/http/urls.py
+-rw-r--r--   0        0        0       99 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/__init__.py
+-rw-r--r--   0        0        0     6260 2024-04-10 09:16:23.493948 webwithpy-0.7.5.2/webwithpy/orm/auth.py
+-rw-r--r--   0        0        0     3644 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/core.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/dialect/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/dialect/base.py
+-rw-r--r--   0        0        0     1764 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/dialect/mysql.py
+-rw-r--r--   0        0        0     1763 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/dialect/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/drivers/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/drivers/driver.py
+-rw-r--r--   0        0        0     2803 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/drivers/mysql.py
+-rw-r--r--   0        0        0     2801 2024-04-16 09:17:10.218673 webwithpy-0.7.5.2/webwithpy/orm/drivers/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/helpers/__init__.py
+-rw-r--r--   0        0        0     1550 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/helpers/settings.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/objects/__init__.py
+-rw-r--r--   0        0        0     5432 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/objects/objects.py
+-rw-r--r--   0        0        0     5122 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/orm/objects/query.py
+-rw-r--r--   0        0        0     1082 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/persistence.py
+-rw-r--r--   0        0        0       70 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/routing/__init__.py
+-rw-r--r--   0        0        0     1785 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/routing/methods.py
+-rw-r--r--   0        0        0     5832 2024-04-16 08:53:43.003920 webwithpy-0.7.5.2/webwithpy/routing/router.py
+-rw-r--r--   0        0        0     1213 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/static/form.css
+-rw-r--r--   0        0        0     1161 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/static/improved_reg_form.css
+-rw-r--r--   0        0        0       63 2024-04-10 08:42:40.770674 webwithpy-0.7.5.2/webwithpy/tests/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-10 08:42:07.174512 webwithpy-0.7.5.2/webwithpy/tests/case.py
+-rw-r--r--   0        0        0      557 2024-04-10 08:29:49.054933 webwithpy-0.7.5.2/webwithpy/tests/helper.py
+-rw-r--r--   0        0        0     2759 2024-04-09 07:43:04.000000 webwithpy-0.7.5.2/webwithpy/webwithpy.py
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 webwithpy-0.7.5.2/PKG-INFO
```

### Comparing `webwithpy-0.7.5.1/LICENSE` & `webwithpy-0.7.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/README.md` & `webwithpy-0.7.5.2/README.md`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/pyproject.toml` & `webwithpy-0.7.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "webwithpy"
 readme = "README.md"
-version = "0.7.5.1"
+version = "0.7.5.2"
 description = ""
 authors = ["Sven Keimpema"]
 packages = [{include = "webwithpy/**/*.*", format = ["wheel", "sdist"]}]
 
 [tool.poetry.scripts]
 webwithpy = "webwithpy:cli"
```

### Comparing `webwithpy-0.7.5.1/webwithpy/commands.py` & `webwithpy-0.7.5.2/webwithpy/commands.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import sys
+
 from .routing.router import Router
 from .webwithpy import run_server
-from pydoc import importfile
+import runpy
 import click
 import os
 
 
 @click.group()
 def cli():
     """My package's command-line interface."""
@@ -31,37 +33,41 @@
     return False
 
 
 def find_main_file():
     dirs = get_dirs()
     for directory in dirs:
         if directory_contains_main(directory):
-            return directory + "/__main__.py"
+            return directory
 
     if directory_contains_main(os.getcwd()):
-        return os.getcwd() + "/__main__.py"
+        return os.getcwd()
 
     raise Exception("No __main__.py files found")
 
 
+def load_main_module(directory: str) -> None:
+    sys.path.insert(1, directory)
+    runpy.run_path("__main__.py", run_name="__main__")
+
+
 @cli.command()
 @click.option("--host", default="127.0.0.1", help="hostname of the webserver")
 @click.option("--port", default=8000, help="port to the web server")
 def start(host: str, port: int):
     # import __main__ file
     main_file = find_main_file()
-    importfile(main_file)
-
+    load_main_module(main_file)
     # run server at cli host, port
     run_server(host, port)
 
 
 @cli.command()
 def test():
     # make sure the router is set to testing, so we can also send requests to testing functions
     Router.testing = True
 
     # import __main__ file
     main_file = find_main_file()
-    importfile(main_file)
+    load_main_module(main_file)
 
     run_server()
```

### Comparing `webwithpy-0.7.5.1/webwithpy/exeptions/HttpExceptions.py` & `webwithpy-0.7.5.2/webwithpy/exeptions/HttpExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/exeptions/RouteExceptions.py` & `webwithpy-0.7.5.2/webwithpy/exeptions/RouteExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/exeptions/__init__.py` & `webwithpy-0.7.5.2/webwithpy/exeptions/__init__.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/html/data/ast.py` & `webwithpy-0.7.5.2/webwithpy/html/data/ast.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/html/forms.py` & `webwithpy-0.7.5.2/webwithpy/html/forms.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/html/lexer.py` & `webwithpy-0.7.5.2/webwithpy/html/lexer.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/html/parser.py` & `webwithpy-0.7.5.2/webwithpy/html/parser.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/html/pyhtml.py` & `webwithpy-0.7.5.2/webwithpy/html/pyhtml.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,32 +25,30 @@
 
 class Form(HtmlTag):
     def __init__(self, *tags: str | HtmlTag, **attrs):
         self.attrs = self.set_dict_attrs(attrs)
         self.tags = tags
 
     def __str__(self):
-        return (
-            f"<form enctype=multipart/form-data {self.attrs}>{''.join([tag.__str__() for tag in self.tags])}</form>"
-        )
+        return f"<form enctype=multipart/form-data {self.attrs}>{''.join([tag.__str__() for tag in self.tags])}</form>"
 
 
 class Label(HtmlTag):
     def __init__(self, *tags: str | HtmlTag, **attrs):
         self.attrs = self.set_dict_attrs(attrs)
         self.tags = tags
 
     def __str__(self):
         return f"<label {self.attrs}> {''.join(self.tags.__str__())} </label>"
 
 
 class Input(HtmlTag):
     def __init__(
-            self,
-            **attrs: Any,
+        self,
+        **attrs: Any,
     ):
         self.attrs = self.set_dict_attrs(attrs)
 
     def __str__(self):
         return f"<input {self.attrs}/>"
 
 
@@ -74,14 +72,17 @@
             f"<div class={self._class} {self.attrs}>"
             f" {''.join([tag.__str__() for tag in self.tags])}</div>"
         )
 
 
 class Img(HtmlTag):
     def __init__(self, image_bytes: bytes, image_type: str, **attrs: str):
+        if image_bytes is None:
+            self.attrs = self.set_dict_attrs(attrs)
+
         encoded_image_data = base64.b64encode(image_bytes)
         str_encoded_image_data = encoded_image_data.decode('utf-8')
         src = f'data:image/{image_type};base64,{str_encoded_image_data}'
         attrs.update({'src': src})
         self.attrs = self.set_dict_attrs(attrs)
 
     def __str__(self):
@@ -127,19 +128,19 @@
 
 class A(HtmlTag):
     """
     Html <a> </a> tag in python
     """
 
     def __init__(
-            self,
-            *tags: str | HtmlTag,
-            _class: str = "",
-            _href: str = "",
-            **attrs: str,
+        self,
+        *tags: str | HtmlTag,
+        _class: str = "",
+        _href: str = "",
+        **attrs: str,
     ):
         self._class = self.set_tag(f"class='{_class}'", _class)
         self._href = self.set_tag(f'href="{_href}"', _href)
         self.tags = tags
         self.attrs = self.set_dict_attrs(attrs)
 
     def __str__(self):
@@ -148,19 +149,19 @@
 
 class P(HtmlTag):
     """
     Html <p> </p> tag in python
     """
 
     def __init__(
-            self,
-            text: str = "",
-            _class: str = "",
-            _href: str = "",
-            **attrs: str,
+        self,
+        text: str = "",
+        _class: str = "",
+        _href: str = "",
+        **attrs: str,
     ):
         self.text = text
         self._class = self.set_tag(f"class='{_class}'", _class)
         self._href = self.set_tag(f'href="{_href}"', _href)
         self.attrs = self.set_dict_attrs(attrs)
 
     def __str__(self):
```

### Comparing `webwithpy-0.7.5.1/webwithpy/html/renderer.py` & `webwithpy-0.7.5.2/webwithpy/html/renderer.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/http/cookies.py` & `webwithpy-0.7.5.2/webwithpy/http/cookies.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/http/handler.py` & `webwithpy-0.7.5.2/webwithpy/http/handler.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/http/request.py` & `webwithpy-0.7.5.2/webwithpy/http/request.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/http/response.py` & `webwithpy-0.7.5.2/webwithpy/http/response.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/http/urls.py` & `webwithpy-0.7.5.2/webwithpy/http/urls.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/orm/auth.py` & `webwithpy-0.7.5.2/webwithpy/orm/auth.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/orm/core.py` & `webwithpy-0.7.5.2/webwithpy/orm/core.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/orm/dialect/base.py` & `webwithpy-0.7.5.2/webwithpy/orm/dialect/base.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/orm/dialect/mysql.py` & `webwithpy-0.7.5.2/webwithpy/orm/dialect/mysql.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/orm/dialect/sqlite.py` & `webwithpy-0.7.5.2/webwithpy/orm/dialect/sqlite.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/orm/drivers/driver.py` & `webwithpy-0.7.5.2/webwithpy/orm/drivers/driver.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/orm/drivers/mysql.py` & `webwithpy-0.7.5.2/webwithpy/orm/drivers/mysql.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/orm/drivers/sqlite.py` & `webwithpy-0.7.5.2/webwithpy/orm/drivers/sqlite.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/orm/helpers/settings.py` & `webwithpy-0.7.5.2/webwithpy/orm/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/orm/objects/objects.py` & `webwithpy-0.7.5.2/webwithpy/orm/objects/objects.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/orm/objects/query.py` & `webwithpy-0.7.5.2/webwithpy/orm/objects/query.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/persistence.py` & `webwithpy-0.7.5.2/webwithpy/persistence.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/routing/methods.py` & `webwithpy-0.7.5.2/webwithpy/routing/methods.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/routing/router.py` & `webwithpy-0.7.5.2/webwithpy/routing/router.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/static/form.css` & `webwithpy-0.7.5.2/webwithpy/static/form.css`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/static/improved_reg_form.css` & `webwithpy-0.7.5.2/webwithpy/static/improved_reg_form.css`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/tests/helper.py` & `webwithpy-0.7.5.2/webwithpy/tests/helper.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/webwithpy/webwithpy.py` & `webwithpy-0.7.5.2/webwithpy/webwithpy.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.5.1/PKG-INFO` & `webwithpy-0.7.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webwithpy
-Version: 0.7.5.1
+Version: 0.7.5.2
 Summary: 
 Author: Sven Keimpema
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

