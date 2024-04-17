# Comparing `tmp/cook_builder-0.0.9.tar.gz` & `tmp/cook_builder-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cook_builder-0.0.9.tar", last modified: Thu Apr 11 18:43:50 2024, max compression
+gzip compressed data, was "cook_builder-0.1.0.tar", last modified: Wed Apr 17 19:42:29 2024, max compression
```

## Comparing `cook_builder-0.0.9.tar` & `cook_builder-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-11 18:43:50.453547 cook_builder-0.0.9/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.0.9/LICENSE
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2981 2024-04-11 18:43:50.453547 cook_builder-0.0.9/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      851 2024-04-02 19:02:19.000000 cook_builder-0.0.9/README.md
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-11 18:43:50.449546 cook_builder-0.0.9/cook/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        0 2024-02-10 12:15:45.000000 cook_builder-0.0.9/cook/__init__.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1710 2024-04-11 18:40:16.000000 cook_builder-0.0.9/cook/cli.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     5742 2024-04-02 18:20:44.000000 cook_builder-0.0.9/cook/configuration.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3491 2024-04-11 18:43:27.000000 cook_builder-0.0.9/cook/cook.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      369 2024-04-11 18:43:27.000000 cook_builder-0.0.9/cook/logger.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1342 2024-04-02 18:46:13.000000 cook_builder-0.0.9/cook/recipe.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      936 2024-03-09 09:22:10.000000 cook_builder-0.0.9/cook/rsync.py
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-11 18:43:50.453547 cook_builder-0.0.9/cook_builder.egg-info/
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2981 2024-04-11 18:43:50.000000 cook_builder-0.0.9/cook_builder.egg-info/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      358 2024-04-11 18:43:50.000000 cook_builder-0.0.9/cook_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-04-11 18:43:50.000000 cook_builder-0.0.9/cook_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       39 2024-04-11 18:43:50.000000 cook_builder-0.0.9/cook_builder.egg-info/entry_points.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       27 2024-04-11 18:43:50.000000 cook_builder-0.0.9/cook_builder.egg-info/requires.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-04-11 18:43:50.000000 cook_builder-0.0.9/cook_builder.egg-info/top_level.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      983 2024-04-11 18:43:22.000000 cook_builder-0.0.9/pyproject.toml
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-11 18:43:50.453547 cook_builder-0.0.9/setup.cfg
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-17 19:42:29.190290 cook_builder-0.1.0/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.1.0/LICENSE
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2980 2024-04-17 19:42:29.190290 cook_builder-0.1.0/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      851 2024-04-14 13:06:12.000000 cook_builder-0.1.0/README.md
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-17 19:42:29.190290 cook_builder-0.1.0/cook/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      250 2024-04-17 17:21:28.000000 cook_builder-0.1.0/cook/__init__.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      780 2024-04-15 19:53:48.000000 cook_builder-0.1.0/cook/build_server.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1619 2024-04-15 19:53:48.000000 cook_builder-0.1.0/cook/cli.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     5827 2024-04-17 17:49:40.000000 cook_builder-0.1.0/cook/configuration.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2591 2024-04-17 17:35:46.000000 cook_builder-0.1.0/cook/cook.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      150 2024-04-16 14:39:30.000000 cook_builder-0.1.0/cook/exception.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1988 2024-04-17 18:00:59.000000 cook_builder-0.1.0/cook/executors.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      924 2024-04-13 11:15:16.000000 cook_builder-0.1.0/cook/logger.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1079 2024-04-17 17:21:33.000000 cook_builder-0.1.0/cook/main.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1030 2024-04-13 20:33:00.000000 cook_builder-0.1.0/cook/recipe.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3441 2024-04-17 17:42:46.000000 cook_builder-0.1.0/cook/rsync.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      382 2024-04-13 14:06:50.000000 cook_builder-0.1.0/cook/watchers.py
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-17 19:42:29.190290 cook_builder-0.1.0/cook_builder.egg-info/
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2980 2024-04-17 19:42:29.000000 cook_builder-0.1.0/cook_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      445 2024-04-17 19:42:29.000000 cook_builder-0.1.0/cook_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-04-17 19:42:29.000000 cook_builder-0.1.0/cook_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-17 19:42:29.000000 cook_builder-0.1.0/cook_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       27 2024-04-17 19:42:29.000000 cook_builder-0.1.0/cook_builder.egg-info/requires.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-04-17 19:42:29.000000 cook_builder-0.1.0/cook_builder.egg-info/top_level.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1110 2024-04-17 19:42:03.000000 cook_builder-0.1.0/pyproject.toml
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-17 19:42:29.190290 cook_builder-0.1.0/setup.cfg
```

### Comparing `cook_builder-0.0.9/LICENSE` & `cook_builder-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cook_builder-0.0.9/PKG-INFO` & `cook_builder-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.0.9
+Version: 0.1.0
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/serweryn617/cook
 Project-URL: Issues, https://github.com/serweryn617/cook/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `cook_builder-0.0.9/README.md` & `cook_builder-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cook_builder-0.0.9/cook/cli.py` & `cook_builder-0.1.0/cook/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,46 @@
 import argparse
 import pathlib
 
-from .cook import Cook
-from .recipe import Recipe
-from .configuration import Configuration
+from .main import main, settings
 
 
 def parse_user_args(user_args):
     res = {}
     for arg in user_args:
         key, value = arg.split('=')
         res[key] = value
     return res
 
 
-def main():
-    epilog_text = '\n'.join((
-        'example usage:',
-        '  %(prog)s my_project name=latest -p ./example/ -b local',
-    ))
+def cli():
+    global settings
+
+    epilog_text = '\n'.join(
+        (
+            'example usage:',
+            '  %(prog)s my_project name=latest -p ./example/ -b local',
+        )
+    )
 
     parser = argparse.ArgumentParser(
-        description='Build script aggregator and remote executor',
-        epilog=epilog_text,
-        formatter_class=argparse.RawDescriptionHelpFormatter
+        description='Build script aggregator and remote executor', epilog=epilog_text, formatter_class=argparse.RawDescriptionHelpFormatter
     )
 
     parser.add_argument('-p', '--recipe_path', default='.', help='Path to directory containing `recipe.py` file.')
     parser.add_argument('-b', '--build_server', help='Build server to use. Uses value of `default_build_server` if left unspecified.')
+    parser.add_argument('-r', '--rich_output', action='store_true')
     parser.add_argument('project', nargs='?', help='Project to build. Uses value of `default_project` if left unspecified.')
     parser.add_argument('user_args', nargs='*', default=[], help='User arguments. Can be used in recipe file. Format: `key=value`')
 
     args = parser.parse_args()
-    recipe_base_path = pathlib.Path.cwd() / args.recipe_path
-    build_server = args.build_server
+    settings.recipe_base_path = (pathlib.Path.cwd() / args.recipe_path).resolve()
+    settings.build_server = args.build_server
     if args.project and '=' in args.project:
-        project = None
-        args.user_args.append(args.project)
+        settings.project = None
+        args.user_args.insert(0, args.project)
     else:
-        project = args.project
-    user_args = parse_user_args(args.user_args)
-
-    recipe = Recipe(recipe_base_path, user_args)
-    recipe.load()
-
-    configuration = Configuration(recipe)
-    configuration.setup(project, build_server)
-
-    cook = Cook(recipe, configuration)
-    cook.cook()
-
+        settings.project = args.project
+    settings.user_args.update(parse_user_args(args.user_args))
+    settings.rich_output = args.rich_output
 
-if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `cook_builder-0.0.9/cook_builder.egg-info/PKG-INFO` & `cook_builder-0.1.0/cook_builder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.0.9
+Version: 0.1.0
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/serweryn617/cook
 Project-URL: Issues, https://github.com/serweryn617/cook/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

