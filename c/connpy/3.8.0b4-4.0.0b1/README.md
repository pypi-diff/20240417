# Comparing `tmp/connpy-3.8.0b4.tar.gz` & `tmp/connpy-4.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.8.0b4.tar", last modified: Tue Dec 19 21:27:08 2023, max compression
+gzip compressed data, was "connpy-4.0.0b1.tar", last modified: Wed Apr 17 19:29:52 2024, max compression
```

## Comparing `connpy-3.8.0b4.tar` & `connpy-4.0.0b1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 21:27:08.196219 connpy-3.8.0b4/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-12-19 21:26:58.000000 connpy-3.8.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2023-12-19 21:27:08.196219 connpy-3.8.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11012 2023-12-19 21:26:58.000000 connpy-3.8.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 21:27:08.196219 connpy-3.8.0b4/connpy/
--rw-r--r--   0 runner    (1001) docker     (127)    10546 2023-12-19 21:26:58.000000 connpy-3.8.0b4/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-12-19 21:26:58.000000 connpy-3.8.0b4/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-19 21:26:58.000000 connpy-3.8.0b4/connpy/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24698 2023-12-19 21:26:58.000000 connpy-3.8.0b4/connpy/ai.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5102 2023-12-19 21:26:58.000000 connpy-3.8.0b4/connpy/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7896 2023-12-19 21:26:58.000000 connpy-3.8.0b4/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16082 2023-12-19 21:26:58.000000 connpy-3.8.0b4/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    74171 2023-12-19 21:26:58.000000 connpy-3.8.0b4/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    32826 2023-12-19 21:26:58.000000 connpy-3.8.0b4/connpy/core.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5897 2023-12-19 21:26:58.000000 connpy-3.8.0b4/connpy/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 21:27:08.196219 connpy-3.8.0b4/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2023-12-19 21:27:08.000000 connpy-3.8.0b4/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-12-19 21:27:08.000000 connpy-3.8.0b4/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 21:27:08.000000 connpy-3.8.0b4/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-19 21:27:08.000000 connpy-3.8.0b4/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-19 21:27:08.000000 connpy-3.8.0b4/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-19 21:27:08.000000 connpy-3.8.0b4/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-12-19 21:27:08.196219 connpy-3.8.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-19 21:26:58.000000 connpy-3.8.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:29:52.115888 connpy-4.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-17 19:29:47.000000 connpy-4.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12164 2024-04-17 19:29:52.115888 connpy-4.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-04-17 19:29:47.000000 connpy-4.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:29:52.115888 connpy-4.0.0b1/connpy/
+-rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24698 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5102 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7896 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16208 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    74522 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32826 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/core.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1572 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7133 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:29:52.115888 connpy-4.0.0b1/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12164 2024-04-17 19:29:52.000000 connpy-4.0.0b1/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 19:29:52.000000 connpy-4.0.0b1/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:29:52.000000 connpy-4.0.0b1/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 19:29:52.000000 connpy-4.0.0b1/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-17 19:29:52.000000 connpy-4.0.0b1/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 19:29:52.000000 connpy-4.0.0b1/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-17 19:29:52.115888 connpy-4.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 19:29:47.000000 connpy-4.0.0b1/setup.py
```

### Comparing `connpy-3.8.0b4/LICENSE` & `connpy-4.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.8.0b4/PKG-INFO` & `connpy-4.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.8.0b4
+Version: 4.0.0b1
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
@@ -23,14 +23,17 @@
 Requires-Dist: pycryptodome
 Requires-Dist: Flask
 Requires-Dist: pyfzf
 Requires-Dist: waitress
 Requires-Dist: PyYAML
 Requires-Dist: openai
 Requires-Dist: rich
+Requires-Dist: protobuf
+Requires-Dist: google_api_python_client
+Requires-Dist: google_auth_oauthlib
 
 # Conn
 [![](https://img.shields.io/pypi/v/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/pyversions/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/l/connpy.svg?style=flat-square)](https://github.com/fluzzi/connpy/blob/main/LICENSE)
 [![](https://img.shields.io/pypi/dm/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 
@@ -95,14 +98,15 @@
   export          Export connection folder to Yaml file
   import          Import connection folder to config from Yaml file
   ai              Make request to an AI
   run             Run scripts or commands on nodes
   api             Start and stop connpy api
   plugin          Manage plugins
   config          Manage app config
+  sync            Sync config with Google
 ```
 
 ### Manage profiles:
 ```
 usage: conn profile [-h] (--add | --del | --mod | --show) profile
 
 positional arguments:
```

### Comparing `connpy-3.8.0b4/README.md` & `connpy-4.0.0b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
   export          Export connection folder to Yaml file
   import          Import connection folder to config from Yaml file
   ai              Make request to an AI
   run             Run scripts or commands on nodes
   api             Start and stop connpy api
   plugin          Manage plugins
   config          Manage app config
+  sync            Sync config with Google
 ```
 
 ### Manage profiles:
 ```
 usage: conn profile [-h] (--add | --del | --mod | --show) profile
 
 positional arguments:
```

### Comparing `connpy-3.8.0b4/connpy/__init__.py` & `connpy-4.0.0b1/connpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 #!/usr/bin/env python3
 '''
 ## Connection manager
 
 Connpy is a connection manager that allows you to store nodes to connect them fast and password free.
 
 ### Features
-    - You can generate profiles and reference them from nodes using @profilename 
-      so you dont need to edit multiple nodes when changing password or other 
-      information.
-    - Nodes can be stored on @folder or @subfolder@folder to organize your 
-      devices. Then can be referenced using node@subfolder@folder or node@folder
-    - If you have too many nodes. Get completion script using: conn config 
-      --completion, or use fzf installing pyfzf and running conn config --fzf true
+    - You can generate profiles and reference them from nodes using @profilename so you dont
+      need to edit multiple nodes when changing password or other information.
+    - Nodes can be stored on @folder or @subfolder@folder to organize your devices. Then can 
+      be referenced using node@subfolder@folder or node@folder
+    - If you have too many nodes. Get completion script using: conn config --completion.
+      Or use fzf installing pyfzf and running conn config --fzf true
+    - Create in bulk, copy, move, export and import nodes for easy management.
+    - Run automation scripts in network devices.
+    - use GPT AI to help you manage your devices.
+    - Add plugins with your own scripts.
     - Much more!
 
 ### Usage
 ```
 usage: conn [-h] [--add | --del | --mod | --show | --debug] [node|folder] [--sftp]
        conn {profile,move,mv,copy,cp,list,ls,bulk,export,import,ai,run,api,plugin,config} ...
 
@@ -43,14 +46,15 @@
   export          Export connection folder to Yaml file
   import          Import connection folder to config from Yaml file
   ai              Make request to an AI
   run             Run scripts or commands on nodes
   api             Start and stop connpy api
   plugin          Manage plugins
   config          Manage app config
+  sync            Sync config with Google
 ```
 
 ###   Manage profiles
 ```
 usage: conn profile [-h] (--add | --del | --mod | --show) profile
 
 positional arguments:
```

### Comparing `connpy-3.8.0b4/connpy/ai.py` & `connpy-4.0.0b1/connpy/ai.py`

 * *Files identical despite different names*

### Comparing `connpy-3.8.0b4/connpy/api.py` & `connpy-4.0.0b1/connpy/api.py`

 * *Files identical despite different names*

### Comparing `connpy-3.8.0b4/connpy/completion.py` & `connpy-4.0.0b1/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.8.0b4/connpy/configfile.py` & `connpy-4.0.0b1/connpy/configfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 #Imports
 import json
 import os
 import re
 from Crypto.PublicKey import RSA
 from pathlib import Path
 from copy import deepcopy
+from .hooks import ConfigHook
+
 
 
 #functions and classes
 
 class configfile:
     ''' This class generates a configfile object. Containts a dictionary storing, config, nodes and profiles, normaly used by connection manager.
 
@@ -101,23 +103,28 @@
                 f.close()
                 os.chmod(conf, 0o600)
         jsonconf = open(conf)
         jsondata = json.load(jsonconf)
         jsonconf.close()
         return jsondata
 
+    @ConfigHook
     def _saveconfig(self, conf):
         #Save config file
         newconfig = {"config":{}, "connections": {}, "profiles": {}}
         newconfig["config"] = self.config
         newconfig["connections"] = self.connections
         newconfig["profiles"] = self.profiles
-        with open(conf, "w") as f:
-            json.dump(newconfig, f, indent = 4)
-            f.close()
+        try:
+            with open(conf, "w") as f:
+                json.dump(newconfig, f, indent = 4)
+                f.close()
+        except:
+            return 1
+        return 0
 
     def _createkey(self, keyfile):
         #Create key file
         key = RSA.generate(2048)
         with open(keyfile,'wb') as f:
             f.write(key.export_key('PEM'))
             f.close()
```

### Comparing `connpy-3.8.0b4/connpy/connapp.py` & `connpy-4.0.0b1/connpy/connapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,17 +155,27 @@
         configcrud.add_argument("--completion", dest="completion", nargs=1, choices=["bash","zsh"], action=self._store_type, help="Get terminal completion configuration for conn")
         configcrud.add_argument("--configfolder", dest="configfolder", nargs=1, action=self._store_type, help="Set the default location for config file", metavar="FOLDER")
         configcrud.add_argument("--openai-org", dest="organization", nargs=1, action=self._store_type, help="Set openai organization", metavar="ORGANIZATION")
         configcrud.add_argument("--openai-api-key", dest="api_key", nargs=1, action=self._store_type, help="Set openai api_key", metavar="API_KEY")
         configcrud.add_argument("--openai-model", dest="model", nargs=1, action=self._store_type, help="Set openai model", metavar="MODEL")
         configparser.set_defaults(func=self._func_others)
         #Add plugins
-        file_path = self.config.defaultdir + "/plugins"
         self.plugins = Plugins()
-        self.plugins._import_plugins_to_argparse(file_path, subparsers)
+        try:
+            core_path = os.path.dirname(os.path.realpath(__file__)) + "/core_plugins"
+            self.plugins._import_plugins_to_argparse(core_path, subparsers)
+        except:
+            pass
+        try:
+            file_path = self.config.defaultdir + "/plugins"
+            self.plugins._import_plugins_to_argparse(file_path, subparsers)
+        except:
+            pass
+        for preload in self.plugins.preloads.values():
+            preload.Preload(self)
         #Generate helps
         nodeparser.usage = self._help("usage", subparsers)
         nodeparser.epilog = self._help("end", subparsers)
         nodeparser.help = self._help("node")
         #Manage sys arguments
         self.commands = list(subparsers.choices.keys())
         profilecmds = []
```

### Comparing `connpy-3.8.0b4/connpy/core.py` & `connpy-4.0.0b1/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-3.8.0b4/connpy/plugins.py` & `connpy-4.0.0b1/connpy/plugins.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import argparse
 import os
 
 class Plugins:
     def __init__(self):
         self.plugins = {}
         self.plugin_parsers = {}
+        self.preloads = {}
 
     def verify_script(self, file_path):
         """
         Verifies that a given Python script meets specific structural requirements.
 
         This function checks a Python script for compliance with predefined structural 
         rules. It ensures that the script contains only allowed top-level elements 
@@ -24,15 +25,15 @@
 
         ### Returns:
             - str: A message indicating the type of violation if the script doesn't meet 
                  the requirements, or False if all requirements are met.
 
         ### Verifications:
             - The presence of only allowed top-level elements.
-            - The existence of two specific classes: 'Parser' and 'Entrypoint'.
+            - The existence of two specific classes: 'Parser' and 'Entrypoint'. and/or specific class: Preload.
             - 'Parser' class must only have an '__init__' method and must assign 'self.parser'
               and 'self.description'.
             - 'Entrypoint' class must have an '__init__' method accepting specific arguments.
 
         If any of these checks fail, the function returns an error message indicating 
         the reason. If the script passes all checks, the function returns False, 
         indicating successful verification.
@@ -45,16 +46,18 @@
             source_code = file.read()
 
         try:
             tree = ast.parse(source_code)
         except SyntaxError as e:
             return f"Syntax error in file: {e}"
 
-        required_classes = {'Parser', 'Entrypoint'}
-        found_classes = set()
+
+        has_parser = False
+        has_entrypoint = False
+        has_preload = False
 
         for node in tree.body:
             # Allow only function definitions, class definitions, and pass statements at top-level
             if isinstance(node, ast.If):
                 # Check for the 'if __name__ == "__main__":' block
                 if not (isinstance(node.test, ast.Compare) and
                         isinstance(node.test.left, ast.Name) and
@@ -62,37 +65,50 @@
                         isinstance(node.test.comparators[0], ast.Str) and
                         node.test.comparators[0].s == '__main__'):
                     return "Only __name__ == __main__ If is allowed"
 
             elif not isinstance(node, (ast.FunctionDef, ast.ClassDef, ast.Import, ast.ImportFrom, ast.Pass)):
                 return f"Plugin can only have pass, functions, classes and imports. {node} is not allowed"  # Reject any other AST types
 
-            if isinstance(node, ast.ClassDef) and node.name in required_classes:
-                found_classes.add(node.name)
+            if isinstance(node, ast.ClassDef):
 
                 if node.name == 'Parser':
+                    has_parser = True
                     # Ensure Parser class has only the __init__ method and assigns self.parser
                     if not all(isinstance(method, ast.FunctionDef) and method.name == '__init__' for method in node.body):
                         return "Parser class should only have __init__ method"
 
                     # Check if 'self.parser' and 'self.description' are assigned in __init__ method
                     init_method = node.body[0]
                     assigned_attrs = [target.attr for expr in init_method.body if isinstance(expr, ast.Assign) for target in expr.targets if isinstance(target, ast.Attribute) and isinstance(target.value, ast.Name) and target.value.id == 'self']
                     if 'parser' not in assigned_attrs or 'description' not in assigned_attrs:
                         return "Parser class should set self.parser and self.description" # 'self.parser' or 'self.description' not assigned in __init__
 
                 elif node.name == 'Entrypoint':
+                    has_entrypoint = True
                     init_method = next((item for item in node.body if isinstance(item, ast.FunctionDef) and item.name == '__init__'), None)
                     if not init_method or len(init_method.args.args) != 4:  # self, args, parser, conapp
-                        return "Entrypoint class should accept only arguments: args, parser and connapp"  # 'Entrypoint' __init__ does not have correct signature
+                        return "Entrypoint class should have method __init__ and accept only arguments: args, parser and connapp"  # 'Entrypoint' __init__ does not have correct signature
+
+                elif node.name == 'Preload':
+                    has_preload = True
+                    init_method = next((item for item in node.body if isinstance(item, ast.FunctionDef) and item.name == '__init__'), None)
+                    if not init_method or len(init_method.args.args) != 2:  # self, connapp
+                        return "Preload class should have method __init__ and accept only argument: connapp"  # 'Preload' __init__ does not have correct signature
+
+        # Applying the combination logic based on class presence
+        if has_parser and not has_entrypoint:
+            return "Parser requires Entrypoint class to be present."
+        elif has_entrypoint and not has_parser:
+            return "Entrypoint requires Parser class to be present."
+    
+        if not (has_parser or has_entrypoint or has_preload):
+            return "No valid class (Parser, Entrypoint, or Preload) found."
 
-        if required_classes == found_classes:
-            return False
-        else:
-            return "Classes Entrypoint and Parser are mandatory"
+        return False  # All requirements met, no error
 
     def _import_from_path(self, path):
         spec = importlib.util.spec_from_file_location("module.name", path)
         module = importlib.util.module_from_spec(spec)
         sys.modules["module.name"] = module
         spec.loader.exec_module(module)
         return module
@@ -104,13 +120,17 @@
                 root_filename = os.path.splitext(filename)[0]
                 if root_filename in commands:
                     continue
                 # Construct the full path
                 filepath = os.path.join(directory, filename)
                 check_file = self.verify_script(filepath)
                 if check_file:
+                    print(f"Failed to load plugin: {filename}. Reason: {check_file}")
                     continue
                 else:
                     self.plugins[root_filename] = self._import_from_path(filepath)
-                    self.plugin_parsers[root_filename] = self.plugins[root_filename].Parser()
-                    subparsers.add_parser(root_filename, parents=[self.plugin_parsers[root_filename].parser], add_help=False, description=self.plugin_parsers[root_filename].description)
+                    if hasattr(self.plugins[root_filename], "Parser"):
+                        self.plugin_parsers[root_filename] = self.plugins[root_filename].Parser()
+                        subparsers.add_parser(root_filename, parents=[self.plugin_parsers[root_filename].parser], add_help=False, description=self.plugin_parsers[root_filename].description)
+                    if hasattr(self.plugins[root_filename], "Preload"):
+                        self.preloads[root_filename] = self.plugins[root_filename]
```

### Comparing `connpy-3.8.0b4/connpy.egg-info/PKG-INFO` & `connpy-4.0.0b1/connpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.8.0b4
+Version: 4.0.0b1
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
@@ -23,14 +23,17 @@
 Requires-Dist: pycryptodome
 Requires-Dist: Flask
 Requires-Dist: pyfzf
 Requires-Dist: waitress
 Requires-Dist: PyYAML
 Requires-Dist: openai
 Requires-Dist: rich
+Requires-Dist: protobuf
+Requires-Dist: google_api_python_client
+Requires-Dist: google_auth_oauthlib
 
 # Conn
 [![](https://img.shields.io/pypi/v/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/pyversions/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/l/connpy.svg?style=flat-square)](https://github.com/fluzzi/connpy/blob/main/LICENSE)
 [![](https://img.shields.io/pypi/dm/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 
@@ -95,14 +98,15 @@
   export          Export connection folder to Yaml file
   import          Import connection folder to config from Yaml file
   ai              Make request to an AI
   run             Run scripts or commands on nodes
   api             Start and stop connpy api
   plugin          Manage plugins
   config          Manage app config
+  sync            Sync config with Google
 ```
 
 ### Manage profiles:
 ```
 usage: conn profile [-h] (--add | --del | --mod | --show) profile
 
 positional arguments:
```

### Comparing `connpy-3.8.0b4/setup.cfg` & `connpy-4.0.0b1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 	pycryptodome
 	Flask
 	pyfzf
 	waitress
 	PyYAML
 	openai
 	rich
+	protobuf
+	google_api_python_client
+	google_auth_oauthlib
 
 [options.entry_points]
 console_scripts = 
 	conn = connpy.__main__:main
 	connpy = connpy.__main__:main
 	connpy-completion-helper = connpy.completion:main
```

