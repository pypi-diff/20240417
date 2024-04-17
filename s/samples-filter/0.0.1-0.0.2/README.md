# Comparing `tmp/samples-filter-0.0.1.tar.gz` & `tmp/samples-filter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samples-filter-0.0.1.tar", last modified: Wed Apr 17 10:58:57 2024, max compression
+gzip compressed data, was "samples-filter-0.0.2.tar", last modified: Wed Apr 17 14:47:16 2024, max compression
```

## Comparing `samples-filter-0.0.1.tar` & `samples-filter-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 10:58:57.133293 samples-filter-0.0.1/
--rw-r--r--   0 r         (1000) r         (1001)     1087 2024-04-17 10:58:48.000000 samples-filter-0.0.1/LICENSE.txt
--rw-rw-r--   0 r         (1000) r         (1001)     4354 2024-04-17 10:58:57.133293 samples-filter-0.0.1/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1001)     3651 2024-04-17 10:58:48.000000 samples-filter-0.0.1/README.md
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 10:58:57.129294 samples-filter-0.0.1/objects/
--rw-r--r--   0 r         (1000) r         (1001)     1261 2024-04-17 10:58:48.000000 samples-filter-0.0.1/objects/__init__.py
--rw-r--r--   0 r         (1000) r         (1001)     1434 2024-04-17 10:58:48.000000 samples-filter-0.0.1/objects/__main__.py
--rw-r--r--   0 r         (1000) r         (1001)     2206 2024-04-17 10:58:48.000000 samples-filter-0.0.1/objects/cli.py
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 10:58:57.133293 samples-filter-0.0.1/samples_filter.egg-info/
--rw-rw-r--   0 r         (1000) r         (1001)     4354 2024-04-17 10:58:57.000000 samples-filter-0.0.1/samples_filter.egg-info/PKG-INFO
--rw-rw-r--   0 r         (1000) r         (1001)      315 2024-04-17 10:58:57.000000 samples-filter-0.0.1/samples_filter.egg-info/SOURCES.txt
--rw-rw-r--   0 r         (1000) r         (1001)        1 2024-04-17 10:58:57.000000 samples-filter-0.0.1/samples_filter.egg-info/dependency_links.txt
--rw-rw-r--   0 r         (1000) r         (1001)       56 2024-04-17 10:58:57.000000 samples-filter-0.0.1/samples_filter.egg-info/entry_points.txt
--rw-rw-r--   0 r         (1000) r         (1001)        6 2024-04-17 10:58:57.000000 samples-filter-0.0.1/samples_filter.egg-info/requires.txt
--rw-rw-r--   0 r         (1000) r         (1001)        8 2024-04-17 10:58:57.000000 samples-filter-0.0.1/samples_filter.egg-info/top_level.txt
--rw-rw-r--   0 r         (1000) r         (1001)       38 2024-04-17 10:58:57.133293 samples-filter-0.0.1/setup.cfg
--rw-r--r--   0 r         (1000) r         (1001)     2519 2024-04-17 10:58:48.000000 samples-filter-0.0.1/setup.py
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 14:47:16.054175 samples-filter-0.0.2/
+-rw-r--r--   0 r         (1000) r         (1001)     1087 2024-04-17 14:47:01.000000 samples-filter-0.0.2/LICENSE.txt
+-rw-rw-r--   0 r         (1000) r         (1001)     4339 2024-04-17 14:47:16.054175 samples-filter-0.0.2/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1001)     3636 2024-04-17 14:47:01.000000 samples-filter-0.0.2/README.md
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 14:47:16.050175 samples-filter-0.0.2/objects/
+-rw-r--r--   0 r         (1000) r         (1001)     1261 2024-04-17 14:47:01.000000 samples-filter-0.0.2/objects/__init__.py
+-rw-r--r--   0 r         (1000) r         (1001)     1434 2024-04-17 14:47:01.000000 samples-filter-0.0.2/objects/__main__.py
+-rw-r--r--   0 r         (1000) r         (1001)     2423 2024-04-17 14:47:01.000000 samples-filter-0.0.2/objects/cli.py
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 14:47:16.054175 samples-filter-0.0.2/samples_filter.egg-info/
+-rw-rw-r--   0 r         (1000) r         (1001)     4339 2024-04-17 14:47:15.000000 samples-filter-0.0.2/samples_filter.egg-info/PKG-INFO
+-rw-rw-r--   0 r         (1000) r         (1001)      315 2024-04-17 14:47:16.000000 samples-filter-0.0.2/samples_filter.egg-info/SOURCES.txt
+-rw-rw-r--   0 r         (1000) r         (1001)        1 2024-04-17 14:47:15.000000 samples-filter-0.0.2/samples_filter.egg-info/dependency_links.txt
+-rw-rw-r--   0 r         (1000) r         (1001)       61 2024-04-17 14:47:15.000000 samples-filter-0.0.2/samples_filter.egg-info/entry_points.txt
+-rw-rw-r--   0 r         (1000) r         (1001)        6 2024-04-17 14:47:15.000000 samples-filter-0.0.2/samples_filter.egg-info/requires.txt
+-rw-rw-r--   0 r         (1000) r         (1001)        8 2024-04-17 14:47:15.000000 samples-filter-0.0.2/samples_filter.egg-info/top_level.txt
+-rw-rw-r--   0 r         (1000) r         (1001)       38 2024-04-17 14:47:16.054175 samples-filter-0.0.2/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1001)     2524 2024-04-17 14:47:01.000000 samples-filter-0.0.2/setup.py
```

### Comparing `samples-filter-0.0.1/LICENSE.txt` & `samples-filter-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `samples-filter-0.0.1/PKG-INFO` & `samples-filter-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samples-filter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Command-line filter for GitHub repositories that contain "samples", instead of real project or framework or library
 Home-page: https://github.com/h1alexbel/samples-filter
 Author: Aliaksei Bialiauski
 Author-email: aliaksei.bialiauski@hey.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -32,15 +32,15 @@
 Samples-filter is a command-line filter
 for GitHub repositories that contain `samples`,
 instead of real project or framework or library.
 E.g. [leeowenowen/rxjava-examples](https://github.com/leeowenowen/rxjava-examples),
 [streaming-with-flink/examples-java](https://github.com/streaming-with-flink/examples-java),
 [redisson/redisson-examples](https://github.com/redisson/redisson-examples).
 
-**Motivation**. During work on [cam](https://github.com/yegor256/cam) project,
+**Motivation**. During the work on [cam](https://github.com/yegor256/cam) project,
 where we're building datasets with open source Java programs,
 we [discovered](https://github.com/yegor256/cam/issues/227)
 the need for filtering repositories that contain
 not a real code, but rather samples, tutorials or examples.
 This repository is portable command-line tool that filters those
 sample repositories.
 
@@ -71,21 +71,21 @@
 
 Fork repository, make changes, send us a [pull request](https://www.yegor256.com/2014/04/15/github-guidelines.html).
 We will review your changes and apply them to the `master` branch shortly,
 provided they don't violate our quality standards. To avoid frustration,
 before sending us your pull request please run full build:
 
 ```bash
-..
+make install test check
 ```
 
 To set up virtual environment use this set of commands:
 
 ```bash
 python3 -m venv $(pwd)
 source $(pwd)/venv/bin/activate
 ```
 
 You will need [Python 3.9+](https://www.python.org/downloads/release/python-390)
-and [pip](https://pypi.org/project/pip) installed.
+installed.
```

### Comparing `samples-filter-0.0.1/README.md` & `samples-filter-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Samples-filter is a command-line filter
 for GitHub repositories that contain `samples`,
 instead of real project or framework or library.
 E.g. [leeowenowen/rxjava-examples](https://github.com/leeowenowen/rxjava-examples),
 [streaming-with-flink/examples-java](https://github.com/streaming-with-flink/examples-java),
 [redisson/redisson-examples](https://github.com/redisson/redisson-examples).
 
-**Motivation**. During work on [cam](https://github.com/yegor256/cam) project,
+**Motivation**. During the work on [cam](https://github.com/yegor256/cam) project,
 where we're building datasets with open source Java programs,
 we [discovered](https://github.com/yegor256/cam/issues/227)
 the need for filtering repositories that contain
 not a real code, but rather samples, tutorials or examples.
 This repository is portable command-line tool that filters those
 sample repositories.
 
@@ -53,19 +53,19 @@
 
 Fork repository, make changes, send us a [pull request](https://www.yegor256.com/2014/04/15/github-guidelines.html).
 We will review your changes and apply them to the `master` branch shortly,
 provided they don't violate our quality standards. To avoid frustration,
 before sending us your pull request please run full build:
 
 ```bash
-..
+make install test check
 ```
 
 To set up virtual environment use this set of commands:
 
 ```bash
 python3 -m venv $(pwd)
 source $(pwd)/venv/bin/activate
 ```
 
 You will need [Python 3.9+](https://www.python.org/downloads/release/python-390)
-and [pip](https://pypi.org/project/pip) installed.
+installed.
```

### Comparing `samples-filter-0.0.1/objects/__init__.py` & `samples-filter-0.0.2/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.0.1/objects/__main__.py` & `samples-filter-0.0.2/objects/__main__.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.0.1/objects/cli.py` & `samples-filter-0.0.2/objects/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,38 +27,46 @@
 
 import typer
 
 from objects import NAME, VERSION
 
 app = typer.Typer()
 
-# @todo #1:45min Add support for --repositories and --out parameter.
-#  We should add support to our cli to handle two options: --repositories,
-#  and --out. Both indicate the name of the file to read/create.
-# @todo #1:25min Clean parameters that we don't need.
-#  Let's remove parameters that we don't really need in this cli.
-#  Less parameters we will have, the better.
-#  Don't forget to remove this puzzle.
 def _version_callback(value: bool) -> None:
     if value:
-        typer.echo(f"{NAME} v{VERSION}")
+        typer.echo(f"{VERSION}")
         raise typer.Exit()
 
+@app.command()
+def filter(
+    repositories: str = typer.Option(..., "--repositories", help="Path to the repositories file."),
+    out: str = typer.Option(..., "--out", help="Path to the output file.")
+):
+    """
+    Filter repositories.
+    """
+    typer.echo(f"Filtering {repositories}...")
+    # @todo #10:45min Filter the repositories using general-like interface.
+    #  We should execute filtering here using some general interface, so
+    #  it would easy to use either LLM or ML filters.
+    # @todo #10:35min Create {out} file with output result.
+    #  We should create file with provided name for {out}.
+    #  Don't forget to remove this puzzle.
+    typer.echo(f"Saving output to {out}")
+
 
 # Run it.
 @app.callback()
 def main(
         # pylint: disable=unused-argument
         version: Optional[bool] = typer.Option(
             None,
             "--version",
-            "-v",
             help="Show the application's version and exit.",
             callback=_version_callback,
             is_eager=True,
         )
 ) -> None:
-    """
-    Respond in interface
-    :param version: Cli version
+    f"""
+    {NAME}
     """
     return
```

### Comparing `samples-filter-0.0.1/samples_filter.egg-info/PKG-INFO` & `samples-filter-0.0.2/samples_filter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samples-filter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Command-line filter for GitHub repositories that contain "samples", instead of real project or framework or library
 Home-page: https://github.com/h1alexbel/samples-filter
 Author: Aliaksei Bialiauski
 Author-email: aliaksei.bialiauski@hey.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -32,15 +32,15 @@
 Samples-filter is a command-line filter
 for GitHub repositories that contain `samples`,
 instead of real project or framework or library.
 E.g. [leeowenowen/rxjava-examples](https://github.com/leeowenowen/rxjava-examples),
 [streaming-with-flink/examples-java](https://github.com/streaming-with-flink/examples-java),
 [redisson/redisson-examples](https://github.com/redisson/redisson-examples).
 
-**Motivation**. During work on [cam](https://github.com/yegor256/cam) project,
+**Motivation**. During the work on [cam](https://github.com/yegor256/cam) project,
 where we're building datasets with open source Java programs,
 we [discovered](https://github.com/yegor256/cam/issues/227)
 the need for filtering repositories that contain
 not a real code, but rather samples, tutorials or examples.
 This repository is portable command-line tool that filters those
 sample repositories.
 
@@ -71,21 +71,21 @@
 
 Fork repository, make changes, send us a [pull request](https://www.yegor256.com/2014/04/15/github-guidelines.html).
 We will review your changes and apply them to the `master` branch shortly,
 provided they don't violate our quality standards. To avoid frustration,
 before sending us your pull request please run full build:
 
 ```bash
-..
+make install test check
 ```
 
 To set up virtual environment use this set of commands:
 
 ```bash
 python3 -m venv $(pwd)
 source $(pwd)/venv/bin/activate
 ```
 
 You will need [Python 3.9+](https://www.python.org/downloads/release/python-390)
-and [pip](https://pypi.org/project/pip) installed.
+installed.
```

### Comparing `samples-filter-0.0.1/setup.py` & `samples-filter-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     version=actual,
     packages=find_packages(),
     install_requires=[
         'typer'
     ],
     entry_points={
         'console_scripts': [
-            'samples-filter=objects.run.py:main',
+            'samples-filter=objects.__main__.py:main',
         ],
     },
     author='Aliaksei Bialiauski',
     author_email='aliaksei.bialiauski@hey.com',
     description=
     'Command-line filter for GitHub repositories that contain "samples",'
     ' instead of real project or framework or library',
```

