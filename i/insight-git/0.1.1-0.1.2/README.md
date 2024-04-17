# Comparing `tmp/insight-git-0.1.1.tar.gz` & `tmp/insight_git-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insight-git-0.1.1.tar", last modified: Wed Apr  3 18:51:25 2024, max compression
+gzip compressed data, was "insight_git-0.1.2.tar", last modified: Wed Apr 17 06:52:44 2024, max compression
```

## Comparing `insight-git-0.1.1.tar` & `insight_git-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:51:25.332921 insight-git-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-03 18:51:20.000000 insight-git-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-03 18:51:25.332921 insight-git-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-03 18:51:20.000000 insight-git-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:51:25.324921 insight-git-0.1.1/insight_git/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugin_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:51:25.328920 insight-git-0.1.1/insight_git/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugins/branch_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugins/commit_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugins/commit_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugins/contributors_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugins/git_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:51:25.328920 insight-git-0.1.1/insight_git.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-03 18:51:25.000000 insight-git-0.1.1/insight_git.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-03 18:51:25.000000 insight-git-0.1.1/insight_git.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:51:25.000000 insight-git-0.1.1/insight_git.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-03 18:51:25.000000 insight-git-0.1.1/insight_git.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-03 18:51:25.000000 insight-git-0.1.1/insight_git.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 18:51:25.000000 insight-git-0.1.1/insight_git.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-03 18:51:20.000000 insight-git-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:51:25.332921 insight-git-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:51:25.328920 insight-git-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_branch_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_commit_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_commit_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_contributors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_git_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:52:44.845985 insight_git-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-17 06:52:38.000000 insight_git-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-17 06:52:44.845985 insight_git-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-17 06:52:38.000000 insight_git-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:52:44.841985 insight_git-0.1.2/insight_git/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-17 06:52:38.000000 insight_git-0.1.2/insight_git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-17 06:52:38.000000 insight_git-0.1.2/insight_git/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-17 06:52:38.000000 insight_git-0.1.2/insight_git/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-17 06:52:38.000000 insight_git-0.1.2/insight_git/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-17 06:52:38.000000 insight_git-0.1.2/insight_git/plugin_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:52:44.841985 insight_git-0.1.2/insight_git/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:52:38.000000 insight_git-0.1.2/insight_git/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-17 06:52:38.000000 insight_git-0.1.2/insight_git/plugins/branch_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-17 06:52:38.000000 insight_git-0.1.2/insight_git/plugins/commit_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-17 06:52:38.000000 insight_git-0.1.2/insight_git/plugins/commit_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-17 06:52:38.000000 insight_git-0.1.2/insight_git/plugins/contributors_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-17 06:52:38.000000 insight_git-0.1.2/insight_git/plugins/git_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:52:44.841985 insight_git-0.1.2/insight_git/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    75034 2024-04-17 06:52:38.000000 insight_git-0.1.2/insight_git/resources/graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-17 06:52:38.000000 insight_git-0.1.2/insight_git/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:52:44.845985 insight_git-0.1.2/insight_git.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-17 06:52:44.000000 insight_git-0.1.2/insight_git.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-17 06:52:44.000000 insight_git-0.1.2/insight_git.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:52:44.000000 insight_git-0.1.2/insight_git.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-17 06:52:44.000000 insight_git-0.1.2/insight_git.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-17 06:52:44.000000 insight_git-0.1.2/insight_git.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 06:52:44.000000 insight_git-0.1.2/insight_git.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-17 06:52:38.000000 insight_git-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:52:44.845985 insight_git-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:52:44.845985 insight_git-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-17 06:52:38.000000 insight_git-0.1.2/tests/test_branch_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-17 06:52:38.000000 insight_git-0.1.2/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-17 06:52:38.000000 insight_git-0.1.2/tests/test_commit_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-17 06:52:38.000000 insight_git-0.1.2/tests/test_commit_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-17 06:52:38.000000 insight_git-0.1.2/tests/test_contributors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-17 06:52:38.000000 insight_git-0.1.2/tests/test_git_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 06:52:38.000000 insight_git-0.1.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-17 06:52:38.000000 insight_git-0.1.2/tests/tests.py
```

### Comparing `insight-git-0.1.1/LICENSE.txt` & `insight_git-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/PKG-INFO` & `insight_git-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insight-git
-Version: 0.1.1
+Version: 0.1.2
 Summary: Insight Git analyzes Git repositories to present comprehensive statistics.
 Author-email: "André F. Costa" <afmcosta@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andrecosta99/insight-git
 Project-URL: Documentation, https://andrecosta99.github.io/insight-git/
 Project-URL: Repository, https://github.com/andrecosta99/insight-git
 Keywords: git,analysis,commit,education
@@ -37,18 +37,17 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest>=8.0; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocstrings; extra == "dev"
 
-
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Tests](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml/badge.svg)](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml)
-[![codecov](https://codecov.io/gh/andrecosta99/insight-git/branch/master/graph/badge.svg)](https://codecov.io/gh/andrecosta99/insight-git)
+[![Tests](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/andrecosta99/insight-git/branch/main/graph/badge.svg)](https://codecov.io/gh/andrecosta99/insight-git)
 [![Docs](https://img.shields.io/badge/docs-click%20here-blue.svg)](https://andrecosta99.github.io/insight-git/)
 [![PyPI version](https://badge.fury.io/py/insight-git.svg)](https://badge.fury.io/py/insight-git)
 ![GitHub last commit](https://img.shields.io/github/last-commit/andrecosta99/insight-git)
 ![GitHub forks](https://img.shields.io/github/forks/andrecosta99/insight-git)
 
 
 # Insight Git
```

### Comparing `insight-git-0.1.1/README.md` & `insight_git-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Tests](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml/badge.svg)](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml)
-[![codecov](https://codecov.io/gh/andrecosta99/insight-git/branch/master/graph/badge.svg)](https://codecov.io/gh/andrecosta99/insight-git)
+[![Tests](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/andrecosta99/insight-git/branch/main/graph/badge.svg)](https://codecov.io/gh/andrecosta99/insight-git)
 [![Docs](https://img.shields.io/badge/docs-click%20here-blue.svg)](https://andrecosta99.github.io/insight-git/)
 [![PyPI version](https://badge.fury.io/py/insight-git.svg)](https://badge.fury.io/py/insight-git)
 ![GitHub last commit](https://img.shields.io/github/last-commit/andrecosta99/insight-git)
 ![GitHub forks](https://img.shields.io/github/forks/andrecosta99/insight-git)
 
 
 # Insight Git
```

### Comparing `insight-git-0.1.1/insight_git/__main__.py` & `insight_git-0.1.2/insight_git/__main__.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/insight_git/callbacks.py` & `insight_git-0.1.2/insight_git/callbacks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,112 @@
 import dash_bootstrap_components as dbc
 from dash import Input, Output, State, callback, html
 from dash.exceptions import PreventUpdate
 
 from .plugin_loader import load_plugins
 from .utils import clone_remote_repo
 
-# Mapping of plugin identifiers to their display titles
-PLUGIN_TITLES = {
-    "git_statistics": "Git Statistics",
-    "commit_graph": "Commit Graph",
-    "branch_information": "Branch Information",
-    "commit_type": "Commit Type",
-    "contributors": "Project Contributors",
-    "code_quality": "Python Code Quality",
-}
+
+def generate_plugin_titles():
+    """
+    Dynamically generates titles for plugins based on their function names.
+    Converts snake_case to Title Case for display purposes.
+
+    Returns:
+        dict: A dictionary mapping plugin function names to their titles.
+    """
+    plugins = load_plugins()
+    titles = {}
+    for plugin_name in plugins.keys():
+        title = plugin_name.replace("_", " ").title()
+        titles[plugin_name] = title
+    return titles
+
+
+PLUGIN_TITLES = generate_plugin_titles()
 
 
 @callback(
     Output("url-error-message", "children"),
     Output("plugin-error-message", "children"),
     Input("load-repo-button", "n_clicks"),
     State("repo-input", "value"),
     State("plugin-selector", "value"),
     prevent_initial_call=True,
 )
 def validate_input(n_clicks, url, selected_plugins):
     """
-    Validates the input fields. Checks if the repository URL is entered
-    and at least one plugin is selected. Returns error messages accordingly.
+    Validates user input for the repository URL and selected plugins.
+    Returns error messages if validation fails.
 
     Args:
-        n_clicks (int): The number of times the load repository button was clicked.
-        url (str): The URL of the Git repository.
-        selected_plugins (list): The selected plugins.
+        n_clicks (int): Number of times the 'Load Repository' button was clicked.
+        url (str): URL of the Git repository entered by the user.
+        selected_plugins (list): List of selected plugins.
 
     Returns:
-        tuple: Tuple containing URL error message and plugin error message.
+        tuple: A tuple containing URL error message and plugin error message.
     """
-    url_error = ""
-    plugin_error = ""
+    url_error, plugin_error = "", ""
     if not url:
         url_error = "Please enter a repository URL."
     if not selected_plugins:
         plugin_error = "Please select at least one plugin."
     return url_error, plugin_error
 
 
 def register_callbacks(app):
     """
-    Registers callbacks in the application. Handles the interactions in the application,
-    including validating inputs and updating the plugin output area based on the
-    selected plugins and repository URL.
+    Registers the necessary callbacks for the Dash app.
+    This function sets up the interaction between UI elements and data processing.
 
     Args:
-        app (Dash app): The Dash application instance where callbacks will be registered.
+        app (Dash app): Instance of the Dash app.
     """
 
     @app.callback(
         Output("plugin-output-area", "children"),
         [Input("load-repo-button", "n_clicks")],
         [State("repo-input", "value"), State("plugin-selector", "value")],
     )
     def update_plugin_output(n_clicks, repo_url, selected_plugins):
         """
-        Updates the plugin output based on user interactions. Clones the repository,
-        loads the selected plugins, and updates the output area with the results
-        from each plugin.
+        Updates the plugin output area based on user interactions.
+        Clones the Git repository, loads the selected plugins,
+        and displays the plugin outputs.
 
         Args:
-            n_clicks (int): The number of times the load repository button was clicked.
-            repo_url (str): The URL of the Git repository to analyze.
-            selected_plugins (list): The selected plugins for analysis.
+            n_clicks (int): Number of times the 'Load Repository' button was clicked.
+            repo_url (str): URL of the Git repository to be analyzed.
+            selected_plugins (list): List of plugins selected by the user.
 
         Returns:
-            list: A list of Dash components representing the output from each selected plugin.
+            list: A list of Dash components representing the output from each plugin.
         """
         if n_clicks is None or n_clicks < 1 or not repo_url or not selected_plugins:
             raise PreventUpdate
 
         loading_message = html.Div(
-            "Data is updated",
+            "Data updated...",
             style={"textAlign": "center", "marginTop": "14px", "marginBottom": "20px"},
         )
 
         repo_path = clone_remote_repo(repo_url)
         if repo_path is None:
             return [html.Div("Failed to clone the repository.")]
 
-        plugins = load_plugins()
         plugin_outputs = [loading_message]
 
+        plugins = load_plugins()
         for plugin_name in selected_plugins:
             plugin_function = plugins.get(plugin_name)
             if plugin_function:
                 try:
                     plugin_output = plugin_function(repo_path)
-                    card_title = PLUGIN_TITLES.get(
-                        plugin_name, plugin_name.replace("_", " ").title()
-                    )
+                    card_title = PLUGIN_TITLES.get(plugin_name)
                     card = dbc.Card(
                         [dbc.CardHeader(card_title), dbc.CardBody([plugin_output])],
                         className="mb-4",
                     )
                     plugin_outputs.append(card)
                 except Exception as e:
                     plugin_outputs.append(html.Div(f"Error loading {plugin_name}: {e}"))
```

### Comparing `insight-git-0.1.1/insight_git/layout.py` & `insight_git-0.1.2/insight_git/layout.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,38 @@
+import base64
+from importlib.resources import files
+
 import dash_bootstrap_components as dbc
 from dash import dcc, html
 
 from .plugin_loader import load_plugins
 
 
-# Function to create the layout of the Dash app
 def create_layout(app):
     plugins = load_plugins()  # Loads available plugins
     plugin_options = [
-        {
-            "label": plugin.replace("_", " ").title(),
-            "value": plugin,
-        }  # Format plugins for dropdown
+        {"label": plugin.replace("_", " ").title(), "value": plugin}
         for plugin in plugins.keys()
     ]
 
+    resource_path = files("insight_git.resources").joinpath("graph.png")
+    encoded_image = base64.b64encode(resource_path.read_bytes()).decode("ascii")
+    image_html = html.Img(
+        src=f"data:image/png;base64,{encoded_image}",
+        style={"height": "24px", "marginRight": "5px"},
+    )
+
     # Define the navigation bar with logo and title
     navbar = dbc.Navbar(
         dbc.Container(
             [
                 dbc.Row(
                     [
-                        dbc.Col(
-                            html.Img(
-                                src="https://assets.streamlinehq.com/image/private/w_200,h_200,ar_1/f_auto/v1/icons/freebies-freemojis/objects/objects/bar-chart-f5c5npy7d6s2nmc8ttmgxd.png?_a=DAJFJtWIZAAC",
-                                height="30px",
-                                className="me-3",
-                            )
-                        ),
-                        dbc.Col(dbc.NavbarBrand("Insight Git", className="ms-2")),
+                        dbc.Col(dbc.NavbarBrand(image_html, className="me-2")),
+                        dbc.Col(dbc.NavbarBrand("Insight Gits", className="ms-2")),
                     ],
                     align="center",
                     className="g-0",
                 ),
             ],
             fluid=True,
         ),
@@ -85,13 +85,13 @@
                     ),
                     dbc.Row(
                         dbc.Col(plugin_error_message, width=12, lg=8), justify="center"
                     ),
                     dbc.Row(dbc.Col(submit_button, width=12, lg=8), justify="center"),
                     dbc.Row(dbc.Col(plugin_output_area, md=8), justify="center"),
                 ],
-                fluid=True,  # Container uses the entire horizontal space
+                fluid=True,
             ),
         ]
     )
 
-    return layout  # Returns the defined layout for the app
+    return layout
```

### Comparing `insight-git-0.1.1/insight_git/plugin_loader.py` & `insight_git-0.1.2/insight_git/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/insight_git/plugins/branch_information.py` & `insight_git-0.1.2/insight_git/plugins/branch_information.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/insight_git/plugins/commit_graph.py` & `insight_git-0.1.2/insight_git/plugins/commit_graph.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/insight_git/plugins/commit_type.py` & `insight_git-0.1.2/insight_git/plugins/commit_type.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/insight_git/plugins/contributors_info.py` & `insight_git-0.1.2/insight_git/plugins/contributors_info.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/insight_git/plugins/git_statistics.py` & `insight_git-0.1.2/insight_git/plugins/git_statistics.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/insight_git/utils.py` & `insight_git-0.1.2/insight_git/utils.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/insight_git.egg-info/PKG-INFO` & `insight_git-0.1.2/insight_git.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insight-git
-Version: 0.1.1
+Version: 0.1.2
 Summary: Insight Git analyzes Git repositories to present comprehensive statistics.
 Author-email: "André F. Costa" <afmcosta@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andrecosta99/insight-git
 Project-URL: Documentation, https://andrecosta99.github.io/insight-git/
 Project-URL: Repository, https://github.com/andrecosta99/insight-git
 Keywords: git,analysis,commit,education
@@ -37,18 +37,17 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest>=8.0; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocstrings; extra == "dev"
 
-
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Tests](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml/badge.svg)](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml)
-[![codecov](https://codecov.io/gh/andrecosta99/insight-git/branch/master/graph/badge.svg)](https://codecov.io/gh/andrecosta99/insight-git)
+[![Tests](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/andrecosta99/insight-git/branch/main/graph/badge.svg)](https://codecov.io/gh/andrecosta99/insight-git)
 [![Docs](https://img.shields.io/badge/docs-click%20here-blue.svg)](https://andrecosta99.github.io/insight-git/)
 [![PyPI version](https://badge.fury.io/py/insight-git.svg)](https://badge.fury.io/py/insight-git)
 ![GitHub last commit](https://img.shields.io/github/last-commit/andrecosta99/insight-git)
 ![GitHub forks](https://img.shields.io/github/forks/andrecosta99/insight-git)
 
 
 # Insight Git
```

### Comparing `insight-git-0.1.1/insight_git.egg-info/SOURCES.txt` & `insight_git-0.1.2/insight_git.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 insight_git.egg-info/top_level.txt
 insight_git/plugins/__init__.py
 insight_git/plugins/branch_information.py
 insight_git/plugins/commit_graph.py
 insight_git/plugins/commit_type.py
 insight_git/plugins/contributors_info.py
 insight_git/plugins/git_statistics.py
+insight_git/resources/graph.png
 tests/test_branch_information.py
 tests/test_callbacks.py
 tests/test_commit_graph.py
 tests/test_commit_type.py
 tests/test_contributors.py
 tests/test_git_statistics.py
-tests/test_main.py
+tests/test_main.py
+tests/tests.py
```

### Comparing `insight-git-0.1.1/pyproject.toml` & `insight_git-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
-requires = ["setuptools>=58.0.0", "wheel"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "insight-git"
-version = "0.1.1"
+version = "0.1.2"
 description = "Insight Git analyzes Git repositories to present comprehensive statistics."
 authors = [{name = "André F. Costa", email = "afmcosta@gmail.com"}]
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
 keywords = ["git", "analysis", "commit", "education"]
 classifiers = [
@@ -100,7 +100,10 @@
     "env",
     "venv",
     ".eggs",
     "*.egg",
     "docs"
 ]
 docstring-convention = "google"
+
+[tool.setuptools.package-data]
+insight_git = ["resources/*"]
```

### Comparing `insight-git-0.1.1/tests/test_branch_information.py` & `insight_git-0.1.2/tests/test_branch_information.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/tests/test_callbacks.py` & `insight_git-0.1.2/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/tests/test_commit_graph.py` & `insight_git-0.1.2/tests/test_commit_graph.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/tests/test_commit_type.py` & `insight_git-0.1.2/tests/test_commit_type.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/tests/test_contributors.py` & `insight_git-0.1.2/tests/test_contributors.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/tests/test_git_statistics.py` & `insight_git-0.1.2/tests/test_git_statistics.py`

 * *Files identical despite different names*

### Comparing `insight-git-0.1.1/tests/test_main.py` & `insight_git-0.1.2/tests/test_main.py`

 * *Files identical despite different names*

