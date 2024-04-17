# Comparing `tmp/DodonaCLI-2024.3.5.tar.gz` & `tmp/dodonacli-2024.4.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DodonaCLI-2024.3.5.tar", last modified: Tue Mar  5 22:24:23 2024, max compression
+gzip compressed data, was "dodonacli-2024.4.17.tar", last modified: Wed Apr 17 20:28:39 2024, max compression
```

## Comparing `DodonaCLI-2024.3.5.tar` & `dodonacli-2024.4.17.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:24:23.277324 DodonaCLI-2024.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:24:23.269324 DodonaCLI-2024.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:24:23.269324 DodonaCLI-2024.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/.github/workflows/prevent_outside_pr_master.yml
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:24:23.277324 DodonaCLI-2024.3.5/DodonaCLI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-03-05 22:24:23.000000 DodonaCLI-2024.3.5/DodonaCLI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-05 22:24:23.000000 DodonaCLI-2024.3.5/DodonaCLI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 22:24:23.000000 DodonaCLI-2024.3.5/DodonaCLI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-05 22:24:23.000000 DodonaCLI-2024.3.5/DodonaCLI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-05 22:24:23.000000 DodonaCLI-2024.3.5/DodonaCLI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-05 22:24:23.000000 DodonaCLI-2024.3.5/DodonaCLI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-03-05 22:24:23.277324 DodonaCLI-2024.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:24:23.273324 DodonaCLI-2024.3.5/dodonacli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:24:23.273324 DodonaCLI-2024.3.5/dodonacli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/commands/cli_next.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/commands/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/commands/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/commands/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/commands/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/commands/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/commands/up.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:24:23.273324 DodonaCLI-2024.3.5/dodonacli/source/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/source/get_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/source/interactive_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/source/pretty_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    14471 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/source/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/source/set_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli/source/syntax_checker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1457 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/dodonacli_completion_script.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:24:23.277324 DodonaCLI-2024.3.5/man-page/
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/man-page/dodonacli.1
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/man-page/dodonacli.1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-05 22:24:15.000000 DodonaCLI-2024.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 22:24:23.277324 DodonaCLI-2024.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.546408 dodonacli-2024.4.17/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.538407 dodonacli-2024.4.17/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.538407 dodonacli-2024.4.17/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/.github/workflows/prevent_outside_pr_master.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.542407 dodonacli-2024.4.17/DodonaCLI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-04-17 20:28:39.000000 dodonacli-2024.4.17/DodonaCLI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-17 20:28:39.000000 dodonacli-2024.4.17/DodonaCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:28:39.000000 dodonacli-2024.4.17/DodonaCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 20:28:39.000000 dodonacli-2024.4.17/DodonaCLI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-17 20:28:39.000000 dodonacli-2024.4.17/DodonaCLI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 20:28:39.000000 dodonacli-2024.4.17/DodonaCLI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-04-17 20:28:39.546408 dodonacli-2024.4.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.542407 dodonacli-2024.4.17/dodonacli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.542407 dodonacli-2024.4.17/dodonacli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/cli_next.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/up.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.542407 dodonacli-2024.4.17/dodonacli/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/interactive_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/pretty_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14473 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/set_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/syntax_checker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli_completion_script.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.542407 dodonacli-2024.4.17/man-page/
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/man-page/dodonacli.1
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/man-page/dodonacli.1.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:28:39.546408 dodonacli-2024.4.17/setup.cfg
```

### Comparing `DodonaCLI-2024.3.5/.github/workflows/publish.yml` & `dodonacli-2024.4.17/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/.github/workflows/publish_test.yml` & `dodonacli-2024.4.17/.github/workflows/publish_test.yml`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/DodonaCLI.egg-info/PKG-INFO` & `dodonacli-2024.4.17/DodonaCLI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DodonaCLI
-Version: 2024.3.5
+Version: 2024.4.17
 Summary: A CLI tool for Dodona
 Author-email: Bram Windey <windey.bram@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Bram Windey
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `DodonaCLI-2024.3.5/DodonaCLI.egg-info/SOURCES.txt` & `dodonacli-2024.4.17/DodonaCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/LICENSE` & `dodonacli-2024.4.17/LICENSE`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/PKG-INFO` & `dodonacli-2024.4.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DodonaCLI
-Version: 2024.3.5
+Version: 2024.4.17
 Summary: A CLI tool for Dodona
 Author-email: Bram Windey <windey.bram@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Bram Windey
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `DodonaCLI-2024.3.5/README.md` & `dodonacli-2024.4.17/README.md`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/dodonacli/commands/cli_next.py` & `dodonacli-2024.4.17/dodonacli/commands/cli_next.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 def get_next_exercise(config, connection, headers, reverse, unsolved):
     from dodonacli.source import get_data, pretty_print
 
     # Get all exercises of selected series
     exercise_data_json = get_data.exercises_data(
-        connection, headers, config['serie_id'], config['serie_token'] or ""
+        connection, headers, config['serie_id'], f"/?token={config['serie_token']}" if config['serie_token'] else ""
     )
 
     # Calculate some needed values
     id_list = [exercise['id'] for exercise in exercise_data_json]
     previous_id = config['exercise_id']
     previous_id_index = id_list.index(int(previous_id))
 
@@ -103,14 +103,18 @@
         with open(f"boilerplate.{file_extension}", "w") as boilerplate_file:
             boilerplate_file.write(boilerplate)
 
     return config
 
 
 def get_next_series(config, connection, headers, reverse, unsolved):
+    if config['serie_token']:
+        print("\nSorry, you can't use 'next' when inside a hidden series.\n")
+        return config
+
     from dodonacli.source import get_data, pretty_print
     # Get all series of selected course
     series_data_json = get_data.series_data(
         connection, headers, config['course_id']
     )
 
     # Take only necessary info from the large json
```

### Comparing `DodonaCLI-2024.3.5/dodonacli/commands/display.py` & `dodonacli-2024.4.17/dodonacli/commands/display.py`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/dodonacli/commands/info.py` & `dodonacli-2024.4.17/dodonacli/commands/info.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     if [ "$3" == "sub" ]; then
         COMPREPLY=( $(compgen -W "load display --help" -- "$2")  )
 
     elif [ "$3" == "display" ]; then
         COMPREPLY=( $(compgen -W "--force --help" -- "$2") )
 
     elif [ "$3" == "info" ]; then
-        COMPREPLY=( $(compgen -W "version changelog github check-update"))
+        COMPREPLY=( $(compgen -W "version changelog completion github check-update" -- "$2"))
 
     elif [ "$3" == "select" ]; then
         COMPREPLY=( $(compgen -W "--other --hidden --help" -- "$2") )
 
     elif [ "$3" == "next" ]; then
         COMPREPLY=( $(compgen -W "--reverse --unsolved --help" -- "$2") )
 
@@ -84,15 +84,14 @@
 
     else
         COMPREPLY=( $(compgen -W "--help") )
     fi
 }
 
 complete -F _dodona dodona
-
         """
     )
 
 
 @click.command(help='Link to the GitHub page of DodonaCLI. Can be handy for the README page, manpages,'
                     ' Issues (bug reports) and pull requests.')
 def github():
@@ -103,22 +102,25 @@
 
 @click.command(help='Changelog for the latest version.')
 def changelog():
     from rich.markdown import Markdown
     from dodonacli.source import pretty_console
 
     changelog_raw = """
-- Added support for hashbangs when using exercise links (post -l)
-- Fixed a bug where links to detached exercises didn't work
-- Added completion sub-command to print out the bash-completion-script
-- Optimised imports to gain quite a lot of speed when not making a request to Dodona
-- Small update to printing forcefully of exercise description (is now indented). More is planned.
-
+- Fixed inconsistent aligning on 'dodona sub view'
+- Improved the syntax-checker for:
+    - Java, now supports multiple classes by compiling all .java-files in the current directory
+    - JavaScript, switched from jshint to node to check syntax, which most JS-devs will have installed already
+- Fixed a wrong link that prevented you from using 'dodona next' inside a hidden series
+- Added check to prevent you from going to a 'next' course when you're in a hidden one, I feel this is a good change, if you disagree, let me know on GitHub
+- Fixed the bash completion script to correctly complete after 'dodona info'
+- Improved the sentence under this one to be more friendly.
 
-As always, use the "--help" flag after every command and sub-command to learn more.
+As always, you can use the "--help" flag after every command and sub-command to learn more.
+Happy coding!
     """
     md = Markdown(changelog_raw)
     pretty_console.console.print(md)
 
 
 def get_dodonacli_version():
     from importlib import metadata
```

### Comparing `DodonaCLI-2024.3.5/dodonacli/commands/post.py` & `dodonacli-2024.4.17/dodonacli/commands/post.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 @click.option("-l", "--use-link",
               help="Post your solutionfile to the link at the first line of your solutionfile. "
                    "This is inspired by plugins for editors as VSCode for Dodona.",
               is_flag=True, default=False)
 @click.option("-c", "--check",
               help="Check the file you provided if the syntax is valid for the programming language "
                    "associated with the exercise. Currently supported languages: bash, python, java, "
-                   "javascript.",
+                   "javascript. For Java files, it will use javac to compile all *.java files that "
+                   "don't have 'test' in them.",
               is_flag=True, default=False)
 @click.argument('file', type=click.Path(exists=True, file_okay=True, dir_okay=False, resolve_path=True))
 def post(file, use_link, check):
     import http.client
     from dodonacli.source import set_data, get_data, syntax_checker
 
     # Read configs in
```

### Comparing `DodonaCLI-2024.3.5/dodonacli/commands/select.py` & `dodonacli-2024.4.17/dodonacli/commands/select.py`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/dodonacli/commands/submission.py` & `dodonacli-2024.4.17/dodonacli/commands/submission.py`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/dodonacli/commands/up.py` & `dodonacli-2024.4.17/dodonacli/commands/up.py`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/dodonacli/main.py` & `dodonacli-2024.4.17/dodonacli/main.py`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/dodonacli/source/get_data.py` & `dodonacli-2024.4.17/dodonacli/source/get_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import datetime
 import http.client
 import json
 import os
 import platform
 import socket
 
 from . import set_data, interactive_tutorial
```

### Comparing `DodonaCLI-2024.3.5/dodonacli/source/interactive_tutorial.py` & `dodonacli-2024.4.17/dodonacli/source/interactive_tutorial.py`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/dodonacli/source/pretty_print.py` & `dodonacli-2024.4.17/dodonacli/source/pretty_print.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,12 +350,13 @@
         if res_status == 200:
             exercise_name = json.loads(result).get('name') or "[i]unkown[/i]"
         else:
             exercise_name = "[i]unable to get info about exercise[/i]"
 
         pretty_console.console.print(
             f"\t{accepted_emoji}  [link={submission['url'].rstrip('.json')}]#{len(json_data) - i: <2}[/link]"
-            f"\t{status}"
-            f"\t\t\t{exercise_name}"
+            f"\t{status: <25}"
+            f"\t{exercise_name}"
         )
+
     connection.close()
     print()
```

### Comparing `DodonaCLI-2024.3.5/dodonacli/source/set_data.py` & `dodonacli-2024.4.17/dodonacli/source/set_data.py`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/dodonacli/source/syntax_checker.py` & `dodonacli-2024.4.17/dodonacli/source/syntax_checker.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import os
+import shutil
 import subprocess
 import tempfile
-import shutil
 
 
 def check_syntax(file: str, language: str) -> bool:
     """
     Check the syntax of the code in the file using external tools
     :param file: Filename containing the code to check
     :param language: Programming language to determine what tool to use
@@ -53,19 +54,32 @@
         print("\nNo idea what's going wrong, but something definitly is going wrong:\n" + str(e))
         return False
 
 
 def check_java_syntax(file: str) -> bool:
     temp_dir = tempfile.mkdtemp()
     try:
-        subprocess.run(['javac', '-d', temp_dir, file], check=True)
+        directory = os.path.dirname(file)
+        java_files = [file for file in os.listdir(directory) if file.endswith('.java') and not "test" in file.lower()]
+        if not java_files:
+            return False  # No Java files found in the directory
+
+        # Construct the list of Java files with their full paths
+        java_files_with_paths = [os.path.join(directory, file) for file in java_files]
+
+        subprocess.run(['javac', '-d', temp_dir] + java_files_with_paths, check=True)
+
+        # Remove temporary directory
         shutil.rmtree(temp_dir, ignore_errors=True)
         return True
+
     except subprocess.CalledProcessError as cpe:
+        # This error will happen if there was something wrong with the Java syntax
         return False
+
     except FileNotFoundError:
         # This will only occur if javac isn't installed.
         # Click will detect that the user gave an invalid file before this function is called
         print("\nTo check the syntax, 'javac' is called with your file. It appears however, that "
               "the Java compiler isn't installed on your system. Please install it: https://openjdk.org/install/")
         return False
     except Exception as e:
@@ -73,23 +87,23 @@
         return False
     finally:
         shutil.rmtree(temp_dir, ignore_errors=True)
 
 
 def check_javascript_syntax(file: str) -> bool:
     try:
-        subprocess.run(['jshint', file], check=True)
+        subprocess.run(['node', '-c', file], check=True)
         return True
     except subprocess.CalledProcessError as cpe:
         return False
     except FileNotFoundError:
         # This will only occur if jshint isn't installed.
         # Click will detect that the user gave an invalid file before this function is called
-        print("\nTo check the syntax, 'jshint' is called with your file. It appears however, that "
-              "this program isn't installed on your system. Please install it using npm: npm install -g jshint")
+        print("\nTo check the syntax, 'node' is called with your file. It appears however, that "
+              "this program isn't installed on your system. Please install it: https://nodejs.org/en/learn/getting-started/how-to-install-nodejs")
         return False
     except Exception as e:
         print("\nNo idea what's going wrong, but something definitly is going wrong:\n" + str(e))
         return False
 
 
 def check_haskell_syntax(file: str) -> bool:
```

### Comparing `DodonaCLI-2024.3.5/dodonacli_completion_script.sh` & `dodonacli-2024.4.17/dodonacli_completion_script.sh`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     if [ "$3" == "sub" ]; then
         COMPREPLY=( $(compgen -W "load display --help" -- "$2")  )
 
     elif [ "$3" == "display" ]; then
         COMPREPLY=( $(compgen -W "--force --help" -- "$2") )
 
     elif [ "$3" == "info" ]; then
-        COMPREPLY=( $(compgen -W "version changelog completion github check-update"))
+        COMPREPLY=( $(compgen -W "version changelog completion github check-update" -- "$2"))
 
     elif [ "$3" == "select" ]; then
         COMPREPLY=( $(compgen -W "--other --hidden --help" -- "$2") )
 
     elif [ "$3" == "next" ]; then
         COMPREPLY=( $(compgen -W "--reverse --unsolved --help" -- "$2") )
```

### Comparing `DodonaCLI-2024.3.5/man-page/dodonacli.1` & `dodonacli-2024.4.17/man-page/dodonacli.1`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/man-page/dodonacli.1.gz` & `dodonacli-2024.4.17/man-page/dodonacli.1.gz`

 * *Files identical despite different names*

### Comparing `DodonaCLI-2024.3.5/pyproject.toml` & `dodonacli-2024.4.17/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DodonaCLI"
-version = "2024.3.5"
+version = "2024.4.17"
 authors = [
     { name = "Bram Windey", email = "windey.bram@gmail.com" },
 ]
 description = "A CLI tool for Dodona"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
```

