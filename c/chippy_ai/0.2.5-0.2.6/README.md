# Comparing `tmp/chippy_ai-0.2.5.tar.gz` & `tmp/chippy_ai-0.2.6.tar.gz`

## Comparing `chippy_ai-0.2.5.tar` & `chippy_ai-0.2.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/MANIFEST.in
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/setup.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/build/lib/chip/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/build/lib/chip/config.ini
--rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/build/lib/chip/main.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/build/lib/chippy_ai/__init__.py
--rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/build/lib/chippy_ai/main.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip.egg-info/PKG-INFO
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip.egg-info/entry_points.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip.egg-info/top_level.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip_ai.egg-info/PKG-INFO
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip_ai.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip_ai.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip_ai.egg-info/entry_points.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip_ai.egg-info/top_level.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/.gitignore
--rw-r--r--   0        0        0     9743 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/README.MD
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/config.ini
--rw-r--r--   0        0        0    13460 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/main.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/pyproject.toml
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/cheats/git.txt
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/cheats/shell.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai.egg-info/PKG-INFO
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai.egg-info/entry_points.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai.egg-info/top_level.txt
--rw-r--r--   0        0        0   340261 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/images/chip1.png
--rw-r--r--   0        0        0   376104 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/images/chip2.png
--rw-r--r--   0        0        0   798043 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/images/demo.gif
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/LICENSE
--rw-r--r--   0        0        0     9323 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/MANIFEST.in
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/setup.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/build/lib/chip/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/build/lib/chip/config.ini
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/build/lib/chip/main.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/build/lib/chippy_ai/__init__.py
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/build/lib/chippy_ai/main.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip.egg-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip.egg-info/top_level.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip_ai.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip_ai.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip_ai.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip_ai.egg-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip_ai.egg-info/top_level.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/.gitignore
+-rw-r--r--   0        0        0     9743 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/README.MD
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/config.ini
+-rw-r--r--   0        0        0    13460 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/main.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/pyproject.toml
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/cheats/git.txt
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/cheats/shell.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/env/placeholder.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai.egg-info/entry_points.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai.egg-info/top_level.txt
+-rw-r--r--   0        0        0   340261 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/images/chip1.png
+-rw-r--r--   0        0        0   376104 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/images/chip2.png
+-rw-r--r--   0        0        0   798043 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/images/demo.gif
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/LICENSE
+-rw-r--r--   0        0        0     9323 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/PKG-INFO
```

### Comparing `chippy_ai-0.2.5/setup.py` & `chippy_ai-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.5/.github/workflows/publish.yml` & `chippy_ai-0.2.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.5/build/lib/chip/main.py` & `chippy_ai-0.2.6/build/lib/chip/main.py`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.5/build/lib/chippy_ai/main.py` & `chippy_ai-0.2.6/build/lib/chippy_ai/main.py`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.5/chippy_ai/README.MD` & `chippy_ai-0.2.6/chippy_ai/README.MD`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.5/chippy_ai/main.py` & `chippy_ai-0.2.6/chippy_ai/main.py`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.5/chippy_ai/pyproject.toml` & `chippy_ai-0.2.6/chippy_ai/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chippy_ai"
-version = "0.2.5"
+version = "0.2.6"
 description = "A small example package"
 readme = "README.md"
 authors = [{ name = "Alex Behrens", email = "alexanderbbehrens@gmail.com" }]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `chippy_ai-0.2.5/chippy_ai/cheats/git.txt` & `chippy_ai-0.2.6/chippy_ai/cheats/git.txt`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.5/chippy_ai/cheats/shell.txt` & `chippy_ai-0.2.6/chippy_ai/cheats/shell.txt`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.5/images/chip1.png` & `chippy_ai-0.2.6/images/chip1.png`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.5/images/chip2.png` & `chippy_ai-0.2.6/images/chip2.png`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.5/images/demo.gif` & `chippy_ai-0.2.6/images/demo.gif`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.5/LICENSE` & `chippy_ai-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.5/README.md` & `chippy_ai-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.5/pyproject.toml` & `chippy_ai-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chippy_ai"
-version = "0.2.5"
+version = "0.2.6"
 description = "A small example package"
 readme = "README.md"
 authors = [{ name = "Alex Behrens", email = "alexanderbbehrens@gmail.com" }]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `chippy_ai-0.2.5/PKG-INFO` & `chippy_ai-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: chippy_ai
-Version: 0.2.5
+Version: 0.2.6
 Summary: A small example package
 Project-URL: Homepage, https://github.com/alexbehrens/chip
 Project-URL: Issues, https://github.com/alexbehrens/chip/issues
 Author-email: Alex Behrens <alexanderbbehrens@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

