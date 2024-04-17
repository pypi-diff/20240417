# Comparing `tmp/tinyfetch-0.0.6.tar.gz` & `tmp/tinyfetch-0.0.7.tar.gz`

## Comparing `tinyfetch-0.0.6.tar` & `tinyfetch-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 tinyfetch-0.0.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 tinyfetch-0.0.6/.github/workflows/test.yml
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinyfetch-0.0.6/src/tinyfetch/__init__.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 tinyfetch-0.0.6/src/tinyfetch/cli.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 tinyfetch-0.0.6/src/tinyfetch/core.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 tinyfetch-0.0.6/src/tinyfetch/module.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfetch-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 tinyfetch-0.0.6/tests/test.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 tinyfetch-0.0.6/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 tinyfetch-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 tinyfetch-0.0.6/README.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 tinyfetch-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 tinyfetch-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 tinyfetch-0.0.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 tinyfetch-0.0.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinyfetch-0.0.7/src/tinyfetch/__init__.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 tinyfetch-0.0.7/src/tinyfetch/cli.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 tinyfetch-0.0.7/src/tinyfetch/core.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 tinyfetch-0.0.7/src/tinyfetch/module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfetch-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 tinyfetch-0.0.7/tests/test.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 tinyfetch-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 tinyfetch-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 tinyfetch-0.0.7/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 tinyfetch-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 tinyfetch-0.0.7/PKG-INFO
```

### Comparing `tinyfetch-0.0.6/.github/workflows/publish.yml` & `tinyfetch-0.0.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.6/.github/workflows/test.yml` & `tinyfetch-0.0.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.6/src/tinyfetch/cli.py` & `tinyfetch-0.0.7/src/tinyfetch/cli.py`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.6/src/tinyfetch/core.py` & `tinyfetch-0.0.7/src/tinyfetch/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from tinyfetch import module
-from tinyfetch.module import Color, ASCII_LOGO
+from tinyfetch.module import ASCII_LOGO, Color
 
 modules_list = [
     module.Space,
     module.UserHost,
     module.SplitLine,
     module.PythonVersion,
     module.PIPVersion,
```

### Comparing `tinyfetch-0.0.6/src/tinyfetch/module.py` & `tinyfetch-0.0.7/src/tinyfetch/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,41 @@
-import sys
 import csv
 import getpass
 import os
 import platform
+import sys
 from dataclasses import dataclass, field
 from enum import Enum
 from pathlib import Path
 from typing import Union
 
 BOLD = "\u001b[1m"
 RESET = "\u001b[0m"
-
-
-class Color(Enum):
-    red = "\u001b[31m"
-    green = "\u001b[32m"
-    yellow = "\u001b[33m"
-    blue = "\u001b[34m"
-    magenta = "\u001b[35m"
-    cyan = "\u001b[36m"
-    white = "\u001b[37m"
-
-
 ASCII_LOGO = [
     "            ",
     "     ___    ",
     "    (.. \   ",
     "    (<> |   ",
     "   //  \ \  ",
     "  ( |  | /| ",
     " _/\ __)/_) ",
     " \/-____\/  ",
 ]
 
 
+class Color(Enum):
+    red = "\u001b[31m"
+    green = "\u001b[32m"
+    yellow = "\u001b[33m"
+    blue = "\u001b[34m"
+    magenta = "\u001b[35m"
+    cyan = "\u001b[36m"
+    white = "\u001b[37m"
+
+
 @dataclass
 class Module:
     title: Union[str, None] = field(init=False, default=None)
     value: str = field(init=False)
     title_color: str = field(default=Color["white"])
     no_color: bool = field(default=False)
```

### Comparing `tinyfetch-0.0.6/.gitignore` & `tinyfetch-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.6/LICENSE.txt` & `tinyfetch-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.6/README.md` & `tinyfetch-0.0.7/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -4,49 +4,49 @@
 ![PyPI - Version](https://img.shields.io/pypi/v/tinyfetch)
 ![GitHub License](https://img.shields.io/github/license/beucismis/tinyfetch)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/beucismis/tinyfetch/test.yml?label=test)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/beucismis/tinyfetch/publish.yml?label=publish)
 
 Python and system information command-line fetch tool.
 
-```console
+```
 $ tinyfetch
 
-beucismis@thinkpad
-------------------
-Python Version: 3.11.2
-PIP Version: 24.0
-PIP Packages: 8
-Implementation: CPython
-Compiler: GCC 12.2.0
+     ___     beucismis@thinkpad-devuan
+    (.. \    -------------------------
+    (<> |    Python Version: 3.11.2
+   //  \ \   PIP Version: 24.0
+  ( |  | /|  PIP Packages: 341
+ _/\ __)/_)  Implementation: CPython
+ \/-____\/   Compiler: GCC 12.2.0
 
-Kernel: Linux-6.1.0-18-amd64
-OS: Devuan GNU/Linux 5 (daedalus) x86_64
+             Kernel: Linux-6.1.0-18-amd64
+             OS: Devuan GNU/Linux 5 (daedalus) x86_64
 ```
 
-Output like this!
+Output like this! Also, tux ASCII logo is inspired by [fastfetch](https://github.com/fastfetch-cli/fastfetch). Thanks!
 
 ## Installation
 
-```console
+```
 pip install -U tinyfetch
 ```
 
 ## Documentation
 
-```console
+```
 $ tinyfetch --help
 
-usage: tinyfetch [-h] [--title-color {red,green,yellow,blue,magenta,cyan}] [--no-color] [--version]
+usage: tinyfetch [-h] [--title-color {red,green,yellow,blue,magenta,cyan,white}] [--no-color] [--version]
 
 Python and system information command-line fetch tool
 
 options:
   -h, --help            show this help message and exit
-  --title-color {red,green,yellow,blue,magenta,cyan}
+  --title-color {red,green,yellow,blue,magenta,cyan,white}
                         set default the title color
   --no-color            turn off all colors and disables
   --version             show program's version number and exit
 ```
 
 ## License
```

### Comparing `tinyfetch-0.0.6/pyproject.toml` & `tinyfetch-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.6/PKG-INFO` & `tinyfetch-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tinyfetch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python and system information command-line fetch tool
 Project-URL: Source, https://github.com/beucismis/tinyfetch
 Project-URL: Issues, https://github.com/beucismis/tinyfetch/issues
 Project-URL: Documentation, https://github.com/beucismis/tinyfetch?tab=readme-ov-file#documentation
 Author-email: beucismis <beucismis@tutamail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -27,49 +27,49 @@
 ![PyPI - Version](https://img.shields.io/pypi/v/tinyfetch)
 ![GitHub License](https://img.shields.io/github/license/beucismis/tinyfetch)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/beucismis/tinyfetch/test.yml?label=test)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/beucismis/tinyfetch/publish.yml?label=publish)
 
 Python and system information command-line fetch tool.
 
-```console
+```
 $ tinyfetch
 
-beucismis@thinkpad
-------------------
-Python Version: 3.11.2
-PIP Version: 24.0
-PIP Packages: 8
-Implementation: CPython
-Compiler: GCC 12.2.0
+     ___     beucismis@thinkpad-devuan
+    (.. \    -------------------------
+    (<> |    Python Version: 3.11.2
+   //  \ \   PIP Version: 24.0
+  ( |  | /|  PIP Packages: 341
+ _/\ __)/_)  Implementation: CPython
+ \/-____\/   Compiler: GCC 12.2.0
 
-Kernel: Linux-6.1.0-18-amd64
-OS: Devuan GNU/Linux 5 (daedalus) x86_64
+             Kernel: Linux-6.1.0-18-amd64
+             OS: Devuan GNU/Linux 5 (daedalus) x86_64
 ```
 
-Output like this!
+Output like this! Also, tux ASCII logo is inspired by [fastfetch](https://github.com/fastfetch-cli/fastfetch). Thanks!
 
 ## Installation
 
-```console
+```
 pip install -U tinyfetch
 ```
 
 ## Documentation
 
-```console
+```
 $ tinyfetch --help
 
-usage: tinyfetch [-h] [--title-color {red,green,yellow,blue,magenta,cyan}] [--no-color] [--version]
+usage: tinyfetch [-h] [--title-color {red,green,yellow,blue,magenta,cyan,white}] [--no-color] [--version]
 
 Python and system information command-line fetch tool
 
 options:
   -h, --help            show this help message and exit
-  --title-color {red,green,yellow,blue,magenta,cyan}
+  --title-color {red,green,yellow,blue,magenta,cyan,white}
                         set default the title color
   --no-color            turn off all colors and disables
   --version             show program's version number and exit
 ```
 
 ## License
```

