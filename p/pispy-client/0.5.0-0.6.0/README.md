# Comparing `tmp/pispy-client-0.5.0.tar.gz` & `tmp/pispy_client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pispy-client-0.5.0.tar", last modified: Fri Apr 12 15:22:32 2024, max compression
+gzip compressed data, was "pispy_client-0.6.0.tar", last modified: Wed Apr 17 09:09:35 2024, max compression
```

## Comparing `pispy-client-0.5.0.tar` & `pispy_client-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-12 15:22:32.658897 pispy-client-0.5.0/
--rw-r--r--   0 davep      (501) staff       (20)     2403 2024-04-12 15:22:32.658781 pispy-client-0.5.0/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)     1108 2024-04-10 13:45:14.000000 pispy-client-0.5.0/README.md
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-12 15:22:32.656562 pispy-client-0.5.0/pispy/
--rw-r--r--   0 davep      (501) staff       (20)      403 2024-04-12 15:20:43.000000 pispy-client-0.5.0/pispy/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)      378 2024-04-10 13:45:14.000000 pispy-client-0.5.0/pispy/__main__.py
--rw-r--r--   0 davep      (501) staff       (20)     1935 2024-04-12 09:50:20.000000 pispy-client-0.5.0/pispy/app.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-12 15:22:32.656816 pispy-client-0.5.0/pispy/data/
--rw-r--r--   0 davep      (501) staff       (20)      331 2024-04-11 08:19:00.000000 pispy-client-0.5.0/pispy/data/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     7041 2024-04-12 15:02:03.000000 pispy-client-0.5.0/pispy/data/package.py
--rw-r--r--   0 davep      (501) staff       (20)        0 2024-04-10 13:45:14.000000 pispy-client-0.5.0/pispy/py.typed
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-12 15:22:32.657079 pispy-client-0.5.0/pispy/widgets/
--rw-r--r--   0 davep      (501) staff       (20)      325 2024-04-11 08:19:00.000000 pispy-client-0.5.0/pispy/widgets/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     8776 2024-04-12 15:20:26.000000 pispy-client-0.5.0/pispy/widgets/package_info.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-12 15:22:32.658211 pispy-client-0.5.0/pispy_client.egg-info/
--rw-r--r--   0 davep      (501) staff       (20)     2403 2024-04-12 15:22:32.000000 pispy-client-0.5.0/pispy_client.egg-info/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      417 2024-04-12 15:22:32.000000 pispy-client-0.5.0/pispy_client.egg-info/SOURCES.txt
--rw-r--r--   0 davep      (501) staff       (20)        1 2024-04-12 15:22:32.000000 pispy-client-0.5.0/pispy_client.egg-info/dependency_links.txt
--rw-r--r--   0 davep      (501) staff       (20)       45 2024-04-12 15:22:32.000000 pispy-client-0.5.0/pispy_client.egg-info/entry_points.txt
--rw-r--r--   0 davep      (501) staff       (20)       22 2024-04-12 15:22:32.000000 pispy-client-0.5.0/pispy_client.egg-info/requires.txt
--rw-r--r--   0 davep      (501) staff       (20)        6 2024-04-12 15:22:32.000000 pispy-client-0.5.0/pispy_client.egg-info/top_level.txt
--rw-r--r--   0 davep      (501) staff       (20)      124 2024-04-11 08:19:00.000000 pispy-client-0.5.0/pyproject.toml
--rw-r--r--   0 davep      (501) staff       (20)     1404 2024-04-12 15:22:32.659229 pispy-client-0.5.0/setup.cfg
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-17 09:09:35.907362 pispy_client-0.6.0/
+-rw-r--r--   0 davep      (501) staff       (20)     2112 2024-04-17 09:09:35.907264 pispy_client-0.6.0/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      817 2024-04-17 09:08:30.000000 pispy_client-0.6.0/README.md
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-17 09:09:35.905654 pispy_client-0.6.0/pispy/
+-rw-r--r--   0 davep      (501) staff       (20)      403 2024-04-17 09:08:35.000000 pispy_client-0.6.0/pispy/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     1730 2024-04-13 14:14:19.000000 pispy_client-0.6.0/pispy/__main__.py
+-rw-r--r--   0 davep      (501) staff       (20)     2300 2024-04-16 11:31:24.000000 pispy_client-0.6.0/pispy/app.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-17 09:09:35.905881 pispy_client-0.6.0/pispy/data/
+-rw-r--r--   0 davep      (501) staff       (20)      331 2024-04-11 08:19:00.000000 pispy_client-0.6.0/pispy/data/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     7041 2024-04-12 15:02:03.000000 pispy_client-0.6.0/pispy/data/package.py
+-rw-r--r--   0 davep      (501) staff       (20)        0 2024-04-10 13:45:14.000000 pispy_client-0.6.0/pispy/py.typed
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-17 09:09:35.906159 pispy_client-0.6.0/pispy/widgets/
+-rw-r--r--   0 davep      (501) staff       (20)      346 2024-04-16 11:31:24.000000 pispy_client-0.6.0/pispy/widgets/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)    12632 2024-04-17 08:58:33.000000 pispy_client-0.6.0/pispy/widgets/package_information.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-17 09:09:35.907029 pispy_client-0.6.0/pispy_client.egg-info/
+-rw-r--r--   0 davep      (501) staff       (20)     2112 2024-04-17 09:09:35.000000 pispy_client-0.6.0/pispy_client.egg-info/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      424 2024-04-17 09:09:35.000000 pispy_client-0.6.0/pispy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 davep      (501) staff       (20)        1 2024-04-17 09:09:35.000000 pispy_client-0.6.0/pispy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 davep      (501) staff       (20)       45 2024-04-17 09:09:35.000000 pispy_client-0.6.0/pispy_client.egg-info/entry_points.txt
+-rw-r--r--   0 davep      (501) staff       (20)       22 2024-04-17 09:09:35.000000 pispy_client-0.6.0/pispy_client.egg-info/requires.txt
+-rw-r--r--   0 davep      (501) staff       (20)        6 2024-04-17 09:09:35.000000 pispy_client-0.6.0/pispy_client.egg-info/top_level.txt
+-rw-r--r--   0 davep      (501) staff       (20)      124 2024-04-11 08:19:00.000000 pispy_client-0.6.0/pyproject.toml
+-rw-r--r--   0 davep      (501) staff       (20)     1404 2024-04-17 09:09:35.907682 pispy_client-0.6.0/setup.cfg
```

### Comparing `pispy-client-0.5.0/PKG-INFO` & `pispy_client-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pispy-client
-Version: 0.5.0
+Version: 0.6.0
 Summary: A terminal-based Python package index inspector
 Home-page: https://github.com/davep/pispy
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -30,42 +30,41 @@
 Requires-Dist: textual>=0.56.4
 Requires-Dist: httpx
 
 # PISpy
 
 ## Introduction
 
-PISpy aims to be a simple but useful [PyPi](https://pypi.org/) lookup client
-for the Terminal, built with [Textual](https://textual.textualize.io/).
+PISpy aims to be a simple but useful [PyPI](https://pypi.org/) lookup client
+for the terminal.
 
 ## Installation
 
-PISPy is a full-screen terminal-based tool and is best installed using
-[`pipx`](https://pypa.github.io/pipx/):
+### pipx
+
+The package can be installed using [`pipx`](https://pypa.github.io/pipx/):
 
 ```sh
 $ pipx install pispy-client
 ```
 
-## Running
-
-Once installed, just run `pispy` from your shell.
+### Homebrew
 
-![PISpy lookup up Textual](https://raw.githubusercontent.com/davep/pispy/main/img/pispy.png)
+The package can be installed using Homebrew. Use the following commands to
+install:
 
-## Naming
+```sh
+$ brew tap davep/homebrew
+$ brew install pispy
+```
 
-> Wait! What? Is this pispy or pispy-client? Why the two names?
+## Running
 
-Well... when I started hacking this together I went to check if PyPi had a
-package called `pispy` and it didn't, so I steamed ahead with that. Only
-when I came to add the package to PyPi did it say it wouldn't let me because
-it was too similar to another package.
+Once installed, just run `pispy` from your shell.
 
-So... package name is `pispy-client` but the content is `pispy`.
+![PISpy lookup up Tinboard](https://raw.githubusercontent.com/davep/pispy/main/img/pispy.png)
 
-## Work in progress
+![PISpy lookup up Tinboard](https://raw.githubusercontent.com/davep/pispy/main/img/pispy-description.png)
 
-PISpy is currently a work in progress. I'm still figuring out what it should
-do and how; but for now it provides a simple package lookup interface.
+![PISpy lookup up Tinboard](https://raw.githubusercontent.com/davep/pispy/main/img/pispy-wheel.png)
 
 [//]: # (README.md ends here)
```

### Comparing `pispy-client-0.5.0/pispy/app.py` & `pispy_client-0.6.0/pispy/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Textual imports.
 from textual import on
 from textual.app import App, ComposeResult
 from textual.widgets import Input
 
 ##############################################################################
 # Local imports.
-from .widgets import PackageInfo
+from .widgets import PackageInformation
 
 
 ##############################################################################
 class PISpy(App[None]):
     """The main application class."""
 
     CSS = """
@@ -21,50 +21,64 @@
             visibility: hidden;
         }
 
         &.-tall {
             height: 1;
         }
     }
+
+    Screen:inline {
+        height: 50vh;
+
+        Input {
+            display: none;
+        }
+    }
     """
 
     BINDINGS = [("escape", "quit", "Quit")]
     """The main application bindings."""
 
     ENABLE_COMMAND_PALETTE = False
     """Disable the command palette."""
 
+    def __init__(self, initial_package: str | None) -> None:
+        """Initialise the application.
+
+        Args:
+            initial_package: The initial package to look up.
+        """
+        super().__init__()
+        self._package = initial_package
+
     def compose(self) -> ComposeResult:
         """Compose the stats screen.
 
         Returns:
             The stats screen's layout.
         """
         yield Input(placeholder="Name of the package to look up in PyPI")
-        yield PackageInfo()
+        yield PackageInformation()
 
-    def on_mount(self) -> None:
-        """Configure the screen once loaded up."""
-        self.query_one(Input).focus()
+    async def on_mount(self) -> None:
+        """Pre-fill the display if a package is passed on the command line."""
+        if self._package is not None:
+            await self.run_action(f"lookup('{self._package}')")
 
     @on(Input.Submitted)
-    async def lookup_package(self) -> None:
+    def lookup_package(self) -> None:
         """React to the user hitting enter in the input field."""
-        await self.query_one(PackageInfo).show(self.query_one(Input).value)
+        if self.query_one(PackageInformation).show(self.query_one(Input).value):
+            self.query_one(PackageInformation).focus()
 
-    async def action_lookup(self, package: str) -> None:
+    def action_lookup(self, package: str) -> None:
         """React to a hyperlink of a project being clicked on.
 
         Args:
             package: The name of the package to look up.
         """
         self.query_one(Input).value = package
         self.query_one(Input).cursor_position = len(package)
-        await self.lookup_package()
-
-##############################################################################
-def run() -> None:
-    """Run the application."""
-    PISpy().run()
+        self.lookup_package()
 
 
 ### app.py ends here
```

### Comparing `pispy-client-0.5.0/pispy/data/package.py` & `pispy_client-0.6.0/pispy/data/package.py`

 * *Files identical despite different names*

### Comparing `pispy-client-0.5.0/pispy_client.egg-info/PKG-INFO` & `pispy_client-0.6.0/pispy_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pispy-client
-Version: 0.5.0
+Version: 0.6.0
 Summary: A terminal-based Python package index inspector
 Home-page: https://github.com/davep/pispy
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -30,42 +30,41 @@
 Requires-Dist: textual>=0.56.4
 Requires-Dist: httpx
 
 # PISpy
 
 ## Introduction
 
-PISpy aims to be a simple but useful [PyPi](https://pypi.org/) lookup client
-for the Terminal, built with [Textual](https://textual.textualize.io/).
+PISpy aims to be a simple but useful [PyPI](https://pypi.org/) lookup client
+for the terminal.
 
 ## Installation
 
-PISPy is a full-screen terminal-based tool and is best installed using
-[`pipx`](https://pypa.github.io/pipx/):
+### pipx
+
+The package can be installed using [`pipx`](https://pypa.github.io/pipx/):
 
 ```sh
 $ pipx install pispy-client
 ```
 
-## Running
-
-Once installed, just run `pispy` from your shell.
+### Homebrew
 
-![PISpy lookup up Textual](https://raw.githubusercontent.com/davep/pispy/main/img/pispy.png)
+The package can be installed using Homebrew. Use the following commands to
+install:
 
-## Naming
+```sh
+$ brew tap davep/homebrew
+$ brew install pispy
+```
 
-> Wait! What? Is this pispy or pispy-client? Why the two names?
+## Running
 
-Well... when I started hacking this together I went to check if PyPi had a
-package called `pispy` and it didn't, so I steamed ahead with that. Only
-when I came to add the package to PyPi did it say it wouldn't let me because
-it was too similar to another package.
+Once installed, just run `pispy` from your shell.
 
-So... package name is `pispy-client` but the content is `pispy`.
+![PISpy lookup up Tinboard](https://raw.githubusercontent.com/davep/pispy/main/img/pispy.png)
 
-## Work in progress
+![PISpy lookup up Tinboard](https://raw.githubusercontent.com/davep/pispy/main/img/pispy-description.png)
 
-PISpy is currently a work in progress. I'm still figuring out what it should
-do and how; but for now it provides a simple package lookup interface.
+![PISpy lookup up Tinboard](https://raw.githubusercontent.com/davep/pispy/main/img/pispy-wheel.png)
 
 [//]: # (README.md ends here)
```

### Comparing `pispy-client-0.5.0/setup.cfg` & `pispy_client-0.6.0/setup.cfg`

 * *Files identical despite different names*

