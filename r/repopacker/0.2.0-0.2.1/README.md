# Comparing `tmp/repopacker-0.2.0.tar.gz` & `tmp/repopacker-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repopacker-0.2.0.tar", max compression
+gzip compressed data, was "repopacker-0.2.1.tar", max compression
```

## Comparing `repopacker-0.2.0.tar` & `repopacker-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-08-27 15:47:00.195111 repopacker-0.2.0/LICENSE
--rw-r--r--   0        0        0     4927 2023-08-28 15:30:08.779960 repopacker-0.2.0/README.md
--rw-r--r--   0        0        0      575 2023-09-08 00:13:15.372574 repopacker-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-26 18:48:40.982504 repopacker-0.2.0/repopacker/__init__.py
--rw-r--r--   0        0        0     1562 2023-08-27 00:20:03.608379 repopacker-0.2.0/repopacker/add.py
--rw-r--r--   0        0        0      723 2023-08-27 00:32:32.612296 repopacker-0.2.0/repopacker/clean.py
--rw-r--r--   0        0        0     1171 2023-08-27 17:25:04.229700 repopacker-0.2.0/repopacker/commands.py
--rw-r--r--   0        0        0     2131 2023-09-08 00:07:41.590760 repopacker-0.2.0/repopacker/config.py
--rw-r--r--   0        0        0       54 2023-09-08 00:13:10.237265 repopacker-0.2.0/repopacker/constants.py
--rw-r--r--   0        0        0     1575 2023-08-27 16:20:17.912792 repopacker-0.2.0/repopacker/download.py
--rw-r--r--   0        0        0      772 2023-08-27 00:21:15.799977 repopacker-0.2.0/repopacker/git.py
--rw-r--r--   0        0        0      179 2023-08-27 00:17:30.161405 repopacker-0.2.0/repopacker/init_cmd.py
--rw-r--r--   0        0        0      334 2023-08-27 00:22:25.092326 repopacker-0.2.0/repopacker/list_cmd.py
--rw-r--r--   0        0        0      639 2023-08-27 01:34:41.295073 repopacker-0.2.0/repopacker/main.py
--rw-r--r--   0        0        0     1008 2023-09-08 00:11:12.570558 repopacker-0.2.0/repopacker/pack.py
--rw-r--r--   0        0        0     1427 2023-08-27 00:21:50.348771 repopacker-0.2.0/repopacker/remove.py
--rw-r--r--   0        0        0      754 2023-08-27 17:27:40.079139 repopacker-0.2.0/repopacker/types.py
--rw-r--r--   0        0        0     1834 2023-08-27 16:19:43.532300 repopacker-0.2.0/repopacker/unpack.py
--rw-r--r--   0        0        0     2077 2023-09-08 00:09:13.004029 repopacker-0.2.0/repopacker/utils.py
--rw-r--r--   0        0        0     5473 1970-01-01 00:00:00.000000 repopacker-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-27 15:47:00.195111 repopacker-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5286 2023-09-08 01:36:37.839470 repopacker-0.2.1/README.md
+-rw-r--r--   0        0        0      575 2024-04-17 15:41:33.791756 repopacker-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-26 18:48:40.982504 repopacker-0.2.1/repopacker/__init__.py
+-rw-r--r--   0        0        0     1562 2023-08-27 00:20:03.608379 repopacker-0.2.1/repopacker/add.py
+-rw-r--r--   0        0        0      723 2023-08-27 00:32:32.612296 repopacker-0.2.1/repopacker/clean.py
+-rw-r--r--   0        0        0     1171 2023-08-27 17:25:04.229700 repopacker-0.2.1/repopacker/commands.py
+-rw-r--r--   0        0        0     2131 2023-09-08 00:07:41.590760 repopacker-0.2.1/repopacker/config.py
+-rw-r--r--   0        0        0       54 2024-04-17 15:41:36.670415 repopacker-0.2.1/repopacker/constants.py
+-rw-r--r--   0        0        0     1575 2023-08-27 16:20:17.912792 repopacker-0.2.1/repopacker/download.py
+-rw-r--r--   0        0        0      772 2023-08-27 00:21:15.799977 repopacker-0.2.1/repopacker/git.py
+-rw-r--r--   0        0        0      179 2023-08-27 00:17:30.161405 repopacker-0.2.1/repopacker/init_cmd.py
+-rw-r--r--   0        0        0      334 2023-08-27 00:22:25.092326 repopacker-0.2.1/repopacker/list_cmd.py
+-rw-r--r--   0        0        0      639 2023-08-27 01:34:41.295073 repopacker-0.2.1/repopacker/main.py
+-rw-r--r--   0        0        0     1008 2023-09-08 01:28:21.343203 repopacker-0.2.1/repopacker/pack.py
+-rw-r--r--   0        0        0     1427 2023-08-27 00:21:50.348771 repopacker-0.2.1/repopacker/remove.py
+-rw-r--r--   0        0        0      754 2023-08-27 17:27:40.079139 repopacker-0.2.1/repopacker/types.py
+-rw-r--r--   0        0        0     1834 2023-08-27 16:19:43.532300 repopacker-0.2.1/repopacker/unpack.py
+-rw-r--r--   0        0        0     2077 2023-09-08 00:09:13.004029 repopacker-0.2.1/repopacker/utils.py
+-rw-r--r--   0        0        0     5883 1970-01-01 00:00:00.000000 repopacker-0.2.1/PKG-INFO
```

### Comparing `repopacker-0.2.0/LICENSE` & `repopacker-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repopacker-0.2.0/README.md` & `repopacker-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -82,16 +82,16 @@
   can create a zip file,
 
   ```bash
   repopacker pack repopack.zip
   ```
 
   You should upload this to an accessible location such as [dropbox](https://www.dropbox.com)
-  or [Zenodo](https://zenodo.org/). Add the link to the `downloadpath` in the `.repopacker.json`.
-  Optionally you can also
+  or [Zenodo](https://zenodo.org/). 
+  Optionally you can also add the link to the `downloadpath` in the `.repopacker.json`.
 
 - **Unpack:** Populate directories with large files in their original locations,
 
   ```bash
   repopacker unpack repopack.zip
   ```
 
@@ -154,11 +154,19 @@
 
   ```bash
   repopacker clean
   ```
 
 ## Gotchas
 
+- RepoPacker will attempt to zip your files into a single zip making it poorly
+suited to extremely large files (more than 100GB will probably become unwieldy).
+
+- To verify the integrity of zip files, RepoPacker will perform a checksum of the 
+zipped file before unpacking. This can be slow for large zips. You can disable this
+behavior by modifying the config.
+
 - RepoPacker is not directly integrated with Git meaning any operations which update
   the file tree (like `git mv`) will not be known to RepoPacker.
-  You must remove files these files and re-add
+  You must remove these files and re-add
   them using RepoPacker for them to be properly tracked.
+
```

### Comparing `repopacker-0.2.0/pyproject.toml` & `repopacker-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "repopacker"
-version = "0.2.0" # remember to change in constants.py
+version = "0.2.1" # remember to change in constants.py
 description = "A low-tech solution to large files in Git"
 authors = ["Kevin Course <kevin.course@mail.utoronto.ca>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `repopacker-0.2.0/repopacker/add.py` & `repopacker-0.2.1/repopacker/add.py`

 * *Files identical despite different names*

### Comparing `repopacker-0.2.0/repopacker/clean.py` & `repopacker-0.2.1/repopacker/clean.py`

 * *Files identical despite different names*

### Comparing `repopacker-0.2.0/repopacker/commands.py` & `repopacker-0.2.1/repopacker/commands.py`

 * *Files identical despite different names*

### Comparing `repopacker-0.2.0/repopacker/config.py` & `repopacker-0.2.1/repopacker/config.py`

 * *Files identical despite different names*

### Comparing `repopacker-0.2.0/repopacker/download.py` & `repopacker-0.2.1/repopacker/download.py`

 * *Files identical despite different names*

### Comparing `repopacker-0.2.0/repopacker/git.py` & `repopacker-0.2.1/repopacker/git.py`

 * *Files identical despite different names*

### Comparing `repopacker-0.2.0/repopacker/main.py` & `repopacker-0.2.1/repopacker/main.py`

 * *Files identical despite different names*

### Comparing `repopacker-0.2.0/repopacker/pack.py` & `repopacker-0.2.1/repopacker/pack.py`

 * *Files identical despite different names*

### Comparing `repopacker-0.2.0/repopacker/remove.py` & `repopacker-0.2.1/repopacker/remove.py`

 * *Files identical despite different names*

### Comparing `repopacker-0.2.0/repopacker/types.py` & `repopacker-0.2.1/repopacker/types.py`

 * *Files identical despite different names*

### Comparing `repopacker-0.2.0/repopacker/unpack.py` & `repopacker-0.2.1/repopacker/unpack.py`

 * *Files identical despite different names*

### Comparing `repopacker-0.2.0/repopacker/utils.py` & `repopacker-0.2.1/repopacker/utils.py`

 * *Files identical despite different names*

### Comparing `repopacker-0.2.0/PKG-INFO` & `repopacker-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: repopacker
-Version: 0.2.0
+Version: 0.2.1
 Summary: A low-tech solution to large files in Git
 License: GPL-3.0-or-later
 Author: Kevin Course
 Author-email: kevin.course@mail.utoronto.ca
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # RepoPacker
 
@@ -97,16 +98,16 @@
   can create a zip file,
 
   ```bash
   repopacker pack repopack.zip
   ```
 
   You should upload this to an accessible location such as [dropbox](https://www.dropbox.com)
-  or [Zenodo](https://zenodo.org/). Add the link to the `downloadpath` in the `.repopacker.json`.
-  Optionally you can also
+  or [Zenodo](https://zenodo.org/). 
+  Optionally you can also add the link to the `downloadpath` in the `.repopacker.json`.
 
 - **Unpack:** Populate directories with large files in their original locations,
 
   ```bash
   repopacker unpack repopack.zip
   ```
 
@@ -169,12 +170,20 @@
 
   ```bash
   repopacker clean
   ```
 
 ## Gotchas
 
+- RepoPacker will attempt to zip your files into a single zip making it poorly
+suited to extremely large files (more than 100GB will probably become unwieldy).
+
+- To verify the integrity of zip files, RepoPacker will perform a checksum of the 
+zipped file before unpacking. This can be slow for large zips. You can disable this
+behavior by modifying the config.
+
 - RepoPacker is not directly integrated with Git meaning any operations which update
   the file tree (like `git mv`) will not be known to RepoPacker.
-  You must remove files these files and re-add
+  You must remove these files and re-add
   them using RepoPacker for them to be properly tracked.
 
+
```

