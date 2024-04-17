# Comparing `tmp/kettlebells-0.2.8.tar.gz` & `tmp/kettlebells-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kettlebells-0.2.8.tar", max compression
+gzip compressed data, was "kettlebells-0.2.9.tar", max compression
```

## Comparing `kettlebells-0.2.8.tar` & `kettlebells-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-09-30 22:28:20.349166 kettlebells-0.2.8/LICENSE
--rw-r--r--   0        0        0     6737 2023-10-14 22:50:48.771402 kettlebells-0.2.8/README.org
--rw-r--r--   0        0        0      786 2023-10-14 22:52:22.737306 kettlebells-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       22 2023-10-14 22:52:15.032617 kettlebells-0.2.8/src/kettlebells/__init__.py
--rw-r--r--   0        0        0     5182 2023-10-14 22:39:16.992508 kettlebells-0.2.8/src/kettlebells/__main__.py
--rw-r--r--   0        0        0       54 2023-09-30 22:28:20.545196 kettlebells-0.2.8/src/kettlebells/console.py
--rw-r--r--   0        0        0     4311 2023-10-14 21:59:38.630598 kettlebells-0.2.8/src/kettlebells/constants.py
--rw-r--r--   0        0        0     3401 2023-10-10 04:41:19.105224 kettlebells-0.2.8/src/kettlebells/database.py
--rw-r--r--   0        0        0     4050 2023-10-14 22:47:00.907592 kettlebells-0.2.8/src/kettlebells/stats.py
--rw-r--r--   0        0        0    12364 2023-10-14 22:00:06.580354 kettlebells-0.2.8/src/kettlebells/workouts.py
--rw-r--r--   0        0        0     7472 1970-01-01 00:00:00.000000 kettlebells-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-09-30 22:28:20.349166 kettlebells-0.2.9/LICENSE
+-rw-r--r--   0        0        0     6737 2023-10-14 22:50:48.771402 kettlebells-0.2.9/README.org
+-rw-r--r--   0        0        0      786 2023-10-14 22:56:48.640159 kettlebells-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-10-14 22:56:48.643529 kettlebells-0.2.9/src/kettlebells/__init__.py
+-rw-r--r--   0        0        0     5182 2023-10-14 22:55:47.440307 kettlebells-0.2.9/src/kettlebells/__main__.py
+-rw-r--r--   0        0        0       54 2023-09-30 22:28:20.545196 kettlebells-0.2.9/src/kettlebells/console.py
+-rw-r--r--   0        0        0     4311 2023-10-14 21:59:38.630598 kettlebells-0.2.9/src/kettlebells/constants.py
+-rw-r--r--   0        0        0     3401 2023-10-10 04:41:19.105224 kettlebells-0.2.9/src/kettlebells/database.py
+-rw-r--r--   0        0        0     4050 2023-10-14 22:47:00.907592 kettlebells-0.2.9/src/kettlebells/stats.py
+-rw-r--r--   0        0        0    12364 2023-10-14 22:00:06.580354 kettlebells-0.2.9/src/kettlebells/workouts.py
+-rw-r--r--   0        0        0     7472 1970-01-01 00:00:00.000000 kettlebells-0.2.9/PKG-INFO
```

### Comparing `kettlebells-0.2.8/LICENSE` & `kettlebells-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kettlebells-0.2.8/README.org` & `kettlebells-0.2.9/README.org`

 * *Files identical despite different names*

### Comparing `kettlebells-0.2.8/pyproject.toml` & `kettlebells-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kettlebells"
-version = "0.2.8"
+version = "0.2.9"
 description = "A CLI tool to create, save, and track progress of kettlebell workouts."
 authors = ["Russell Helmstedter <rhelmstedter@gmail.com>"]
 readme = "README.org"
 homepage = "https://github.com/rhelmstedter/kettlebells/"
 repository = "https://github.com/rhelmstedter/kettlebells/"
 keywords = ["CLI", "kettlebells", "fitness"]
```

### Comparing `kettlebells-0.2.8/src/kettlebells/__main__.py` & `kettlebells-0.2.9/src/kettlebells/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     sort: Annotated[
         str,
         typer.Option(
             "--sort",
             "-s",
             help="Sort the table. Possible arguments: weight moved, reps, density."
         ),
-    ] = "weight moved",
+    ] = "weight-moved",
 ) -> None:
     """Display a table of the top ten workouts in database."""
     data = read_database(KETTLEBELLS_DB)
     console.print(top_ten_workouts(data, sort))
 
 
 if __name__ == "__main__":
```

### Comparing `kettlebells-0.2.8/src/kettlebells/constants.py` & `kettlebells-0.2.9/src/kettlebells/constants.py`

 * *Files identical despite different names*

### Comparing `kettlebells-0.2.8/src/kettlebells/database.py` & `kettlebells-0.2.9/src/kettlebells/database.py`

 * *Files identical despite different names*

### Comparing `kettlebells-0.2.8/src/kettlebells/stats.py` & `kettlebells-0.2.9/src/kettlebells/stats.py`

 * *Files identical despite different names*

### Comparing `kettlebells-0.2.8/src/kettlebells/workouts.py` & `kettlebells-0.2.9/src/kettlebells/workouts.py`

 * *Files identical despite different names*

### Comparing `kettlebells-0.2.8/PKG-INFO` & `kettlebells-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kettlebells
-Version: 0.2.8
+Version: 0.2.9
 Summary: A CLI tool to create, save, and track progress of kettlebell workouts.
 Home-page: https://github.com/rhelmstedter/kettlebells/
 Keywords: CLI,kettlebells,fitness
 Author: Russell Helmstedter
 Author-email: rhelmstedter@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

