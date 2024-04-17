# Comparing `tmp/spyglass_cli-0.1.1-py3-none-any.whl.zip` & `tmp/spyglass_cli-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 10469 bytes, number of entries: 13
--rw-r--r--  2.0 unx     3064 b- defN 24-Apr-15 20:25 spyglass/app.py
--rw-r--r--  2.0 unx     1396 b- defN 24-Apr-15 20:24 spyglass/database.py
--rw-r--r--  2.0 unx      517 b- defN 24-Mar-10 14:39 spyglass/utils.py
+Zip file size: 10481 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     3082 b- defN 24-Apr-17 20:57 spyglass/app.py
+-rw-r--r--  2.0 unx     1405 b- defN 24-Apr-17 20:58 spyglass/database.py
+-rw-r--r--  2.0 unx      517 b- defN 24-Apr-17 20:58 spyglass/utils.py
 -rw-r--r--  2.0 unx     3175 b- defN 24-Apr-06 13:25 spyglass/__pycache__/database.cpython-311.pyc
 -rwxr-xr-x  2.0 unx     2943 b- defN 24-Mar-10 14:39 spyglass/__pycache__/database.cpython-312.pyc
 -rw-r--r--  2.0 unx     1429 b- defN 24-Apr-06 13:25 spyglass/__pycache__/utils.cpython-311.pyc
 -rwxr-xr-x  2.0 unx     1404 b- defN 24-Mar-10 14:39 spyglass/__pycache__/utils.cpython-312.pyc
--rwxr-xr-x  2.0 unx     1523 b- defN 24-Apr-17 20:56 spyglass_cli-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1013 b- defN 24-Apr-17 20:56 spyglass_cli-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 20:56 spyglass_cli-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 24-Apr-17 20:56 spyglass_cli-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-17 20:56 spyglass_cli-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1134 b- defN 24-Apr-17 20:56 spyglass_cli-0.1.1.dist-info/RECORD
-13 files, 17746 bytes uncompressed, 8549 bytes compressed:  51.8%
+-rwxr-xr-x  2.0 unx     1523 b- defN 24-Apr-17 20:58 spyglass_cli-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1013 b- defN 24-Apr-17 20:58 spyglass_cli-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 20:58 spyglass_cli-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 24-Apr-17 20:58 spyglass_cli-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-17 20:58 spyglass_cli-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1134 b- defN 24-Apr-17 20:58 spyglass_cli-0.1.2.dist-info/RECORD
+13 files, 17773 bytes uncompressed, 8561 bytes compressed:  51.8%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: spyglass/__pycache__/utils.cpython-311.pyc
 Comment: 
 
 Filename: spyglass/__pycache__/utils.cpython-312.pyc
 Comment: 
 
-Filename: spyglass_cli-0.1.1.dist-info/LICENSE
+Filename: spyglass_cli-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: spyglass_cli-0.1.1.dist-info/METADATA
+Filename: spyglass_cli-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: spyglass_cli-0.1.1.dist-info/WHEEL
+Filename: spyglass_cli-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: spyglass_cli-0.1.1.dist-info/entry_points.txt
+Filename: spyglass_cli-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: spyglass_cli-0.1.1.dist-info/top_level.txt
+Filename: spyglass_cli-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: spyglass_cli-0.1.1.dist-info/RECORD
+Filename: spyglass_cli-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spyglass/app.py

```diff
@@ -2,16 +2,16 @@
 from pathlib import Path
 import subprocess
 
 import inquirer
 import typer
 from icecream import ic
 
-from database import Shelf
-from utils import die, Project
+from spyglass.database import Shelf
+from spyglass.utils import die, Project
 
 
 app = typer.Typer()
 project_subcommand = typer.Typer()
 app.add_typer(project_subcommand, name='project')
 
 entries: list[Project] = []
```

## spyglass/database.py

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 import platform
 
 import shelve as shelf
 
-from utils import die, Project
+from spyglass.utils import die, Project
 
 
 
 class Shelf:
     def __init__(self, filename: str):
         self.file: Path = None
         self.db = None
```

## Comparing `spyglass_cli-0.1.1.dist-info/LICENSE` & `spyglass_cli-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `spyglass_cli-0.1.1.dist-info/METADATA` & `spyglass_cli-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyglass-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Project management cli tool written in python
 Author-email: Jovan Djokic-Sumarac <sumarac@protonmail.com>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/sumarac/spyglass
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `spyglass_cli-0.1.1.dist-info/RECORD` & `spyglass_cli-0.1.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-spyglass/app.py,sha256=33IaOZr2glbJfI5wXi_v9jb6yAC8Sme8XR8Zn9xOtfE,3064
-spyglass/database.py,sha256=Y8mOU9VfjbUkQvNLnTDqycVbtqX1S6spvQ2QPOtsBLc,1396
+spyglass/app.py,sha256=LVOn3Tul2DTOZ5jHz4vVeZ8AuBuRjHmG8Z3rdRJWpok,3082
+spyglass/database.py,sha256=D6qDsvXghpWpVilGA3ISaVEzTgplyvs_48lvkM-x17w,1405
 spyglass/utils.py,sha256=Uf7I9lPvZcIaEVxEAIQhvjDjx4XRiTse7fhesFq38tw,517
 spyglass/__pycache__/database.cpython-311.pyc,sha256=os0oGPeMzgln7gEhm4BO8j_BzMF92DQBzHjL17KPqHc,3175
 spyglass/__pycache__/database.cpython-312.pyc,sha256=O9gVjuhB4Qts6lgC0yPvtl5bIYiT2_y_328j1c2xEbw,2943
 spyglass/__pycache__/utils.cpython-311.pyc,sha256=fYbfdFCyQC6YWw2rzbkk1D8jvmYtIo6m9y27X6flP90,1429
 spyglass/__pycache__/utils.cpython-312.pyc,sha256=iEztJHW6RELKMDbrazazK9vh3X-lrEzmbpjBjtj8Zpc,1404
-spyglass_cli-0.1.1.dist-info/LICENSE,sha256=6HUoGk1LfJqPgG5J4PjpnbEXN-qy-OtnNnGVZcoBVBk,1523
-spyglass_cli-0.1.1.dist-info/METADATA,sha256=8Fx5AIcqgtpOKStwIqXcq0VO59V3aYEe83jTjSg_QL8,1013
-spyglass_cli-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-spyglass_cli-0.1.1.dist-info/entry_points.txt,sha256=6lX2JC4SFdC4REpEKkNnQMUhl5xWntBZE63Rh9dt4Ds,47
-spyglass_cli-0.1.1.dist-info/top_level.txt,sha256=bCMuU4Cf9XNHucle5vDbOreq499MjFzsxKTR8qaj69M,9
-spyglass_cli-0.1.1.dist-info/RECORD,,
+spyglass_cli-0.1.2.dist-info/LICENSE,sha256=6HUoGk1LfJqPgG5J4PjpnbEXN-qy-OtnNnGVZcoBVBk,1523
+spyglass_cli-0.1.2.dist-info/METADATA,sha256=IjYllHFlR_Lx9JmUcwE3XB4Z-z2uia0btYi4PYvvLOA,1013
+spyglass_cli-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+spyglass_cli-0.1.2.dist-info/entry_points.txt,sha256=6lX2JC4SFdC4REpEKkNnQMUhl5xWntBZE63Rh9dt4Ds,47
+spyglass_cli-0.1.2.dist-info/top_level.txt,sha256=bCMuU4Cf9XNHucle5vDbOreq499MjFzsxKTR8qaj69M,9
+spyglass_cli-0.1.2.dist-info/RECORD,,
```
