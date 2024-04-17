# Comparing `tmp/simplenote_local-1.0.tar.gz` & `tmp/simplenote_local-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplenote_local-1.0.tar", last modified: Tue Apr 16 13:41:33 2024, max compression
+gzip compressed data, was "simplenote_local-1.0.1.tar", last modified: Tue Apr 16 14:14:27 2024, max compression
```

## Comparing `simplenote_local-1.0.tar` & `simplenote_local-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-16 13:41:33.445433 simplenote_local-1.0/
--rw-r--r--   0 norm       (502) staff       (20)     1076 2024-02-29 11:23:11.000000 simplenote_local-1.0/LICENSE
--rw-r--r--   0 norm       (502) staff       (20)     7536 2024-04-16 13:41:33.445242 simplenote_local-1.0/PKG-INFO
--rw-r--r--   0 norm       (502) staff       (20)     7024 2024-04-16 08:31:17.000000 simplenote_local-1.0/README.md
-drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-16 13:41:33.443493 simplenote_local-1.0/nv/
--rw-r--r--   0 norm       (502) staff       (20)        0 2024-02-29 11:31:47.000000 simplenote_local-1.0/nv/__init__.py
--rw-r--r--   0 norm       (502) staff       (20)    29466 2024-03-27 16:54:15.000000 simplenote_local-1.0/nv/nv.py
--rw-r--r--   0 norm       (502) staff       (20)       38 2024-04-16 13:41:33.445494 simplenote_local-1.0/setup.cfg
--rw-r--r--   0 norm       (502) staff       (20)      830 2024-04-16 13:41:29.000000 simplenote_local-1.0/setup.py
-drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-16 13:41:33.443955 simplenote_local-1.0/simplenote_local/
--rw-r--r--   0 norm       (502) staff       (20)    32547 2024-04-16 09:00:44.000000 simplenote_local-1.0/simplenote_local/__init__.py
--rw-r--r--   0 norm       (502) staff       (20)     7587 2024-04-16 09:05:24.000000 simplenote_local-1.0/simplenote_local/cli.py
--rw-r--r--   0 norm       (502) staff       (20)        0 2024-03-09 07:20:11.000000 simplenote_local-1.0/simplenote_local/note.py
-drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-16 13:41:33.444998 simplenote_local-1.0/simplenote_local.egg-info/
--rw-r--r--   0 norm       (502) staff       (20)     7536 2024-04-16 13:41:33.000000 simplenote_local-1.0/simplenote_local.egg-info/PKG-INFO
--rw-r--r--   0 norm       (502) staff       (20)      389 2024-04-16 13:41:33.000000 simplenote_local-1.0/simplenote_local.egg-info/SOURCES.txt
--rw-r--r--   0 norm       (502) staff       (20)        1 2024-04-16 13:41:33.000000 simplenote_local-1.0/simplenote_local.egg-info/dependency_links.txt
--rw-r--r--   0 norm       (502) staff       (20)       57 2024-04-16 13:41:33.000000 simplenote_local-1.0/simplenote_local.egg-info/entry_points.txt
--rw-r--r--   0 norm       (502) staff       (20)       57 2024-04-16 13:41:33.000000 simplenote_local-1.0/simplenote_local.egg-info/requires.txt
--rw-r--r--   0 norm       (502) staff       (20)       20 2024-04-16 13:41:33.000000 simplenote_local-1.0/simplenote_local.egg-info/top_level.txt
-drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-16 13:41:33.444821 simplenote_local-1.0/tests/
--rw-r--r--   0 norm       (502) staff       (20)      193 2024-03-09 12:03:31.000000 simplenote_local-1.0/tests/test_note.py
+drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-16 14:14:27.050388 simplenote_local-1.0.1/
+-rw-r--r--   0 norm       (502) staff       (20)     1076 2024-02-29 11:23:11.000000 simplenote_local-1.0.1/LICENSE
+-rw-r--r--   0 norm       (502) staff       (20)     7538 2024-04-16 14:14:27.050182 simplenote_local-1.0.1/PKG-INFO
+-rw-r--r--   0 norm       (502) staff       (20)     7024 2024-04-16 08:31:17.000000 simplenote_local-1.0.1/README.md
+drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-16 14:14:27.047795 simplenote_local-1.0.1/nv/
+-rw-r--r--   0 norm       (502) staff       (20)        0 2024-02-29 11:31:47.000000 simplenote_local-1.0.1/nv/__init__.py
+-rw-r--r--   0 norm       (502) staff       (20)    29466 2024-03-27 16:54:15.000000 simplenote_local-1.0.1/nv/nv.py
+-rw-r--r--   0 norm       (502) staff       (20)       38 2024-04-16 14:14:27.050441 simplenote_local-1.0.1/setup.cfg
+-rw-r--r--   0 norm       (502) staff       (20)      925 2024-04-16 14:12:25.000000 simplenote_local-1.0.1/setup.py
+drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-16 14:14:27.048568 simplenote_local-1.0.1/simplenote_local/
+-rw-r--r--   0 norm       (502) staff       (20)    32515 2024-04-16 14:10:42.000000 simplenote_local-1.0.1/simplenote_local/__init__.py
+-rw-r--r--   0 norm       (502) staff       (20)     7587 2024-04-16 09:05:24.000000 simplenote_local-1.0.1/simplenote_local/cli.py
+-rw-r--r--   0 norm       (502) staff       (20)       22 2024-04-16 14:11:59.000000 simplenote_local-1.0.1/simplenote_local/version.py
+drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-16 14:14:27.049720 simplenote_local-1.0.1/simplenote_local.egg-info/
+-rw-r--r--   0 norm       (502) staff       (20)     7538 2024-04-16 14:14:27.000000 simplenote_local-1.0.1/simplenote_local.egg-info/PKG-INFO
+-rw-r--r--   0 norm       (502) staff       (20)      392 2024-04-16 14:14:27.000000 simplenote_local-1.0.1/simplenote_local.egg-info/SOURCES.txt
+-rw-r--r--   0 norm       (502) staff       (20)        1 2024-04-16 14:14:27.000000 simplenote_local-1.0.1/simplenote_local.egg-info/dependency_links.txt
+-rw-r--r--   0 norm       (502) staff       (20)       57 2024-04-16 14:14:27.000000 simplenote_local-1.0.1/simplenote_local.egg-info/entry_points.txt
+-rw-r--r--   0 norm       (502) staff       (20)       57 2024-04-16 14:14:27.000000 simplenote_local-1.0.1/simplenote_local.egg-info/requires.txt
+-rw-r--r--   0 norm       (502) staff       (20)       20 2024-04-16 14:14:27.000000 simplenote_local-1.0.1/simplenote_local.egg-info/top_level.txt
+drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-16 14:14:27.049448 simplenote_local-1.0.1/tests/
+-rw-r--r--   0 norm       (502) staff       (20)      193 2024-03-09 12:03:31.000000 simplenote_local-1.0.1/tests/test_note.py
```

### Comparing `simplenote_local-1.0/LICENSE` & `simplenote_local-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simplenote_local-1.0/PKG-INFO` & `simplenote_local-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplenote_local
-Version: 1.0
+Version: 1.0.1
 Summary: Sync notes to/from simplenote.com
 Home-page: https://github.com/norm/simplenote-local
 Author: Mark Norman Francis
 Author-email: norm@201created.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `simplenote_local-1.0/README.md` & `simplenote_local-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `simplenote_local-1.0/nv/nv.py` & `simplenote_local-1.0.1/nv/nv.py`

 * *Files identical despite different names*

### Comparing `simplenote_local-1.0/setup.py` & `simplenote_local-1.0.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from setuptools import find_packages, setup
 
+with open('simplenote_local/version.py') as version_file:
+    exec(version_file.read())
+
 setup(
     name='simplenote_local',
-    version='1.0',
+    version=__version__,
 
     description = 'Sync notes to/from simplenote.com',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license = 'MIT',
     url = 'https://github.com/norm/simplenote-local',
```

### Comparing `simplenote_local-1.0/simplenote_local/__init__.py` & `simplenote_local-1.0.1/simplenote_local/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,21 +376,20 @@
         # <h1> tag as the note title (which may not be the first line of text
         # given global nav etc appearing first in source order)
         soup = BeautifulSoup(body, 'html.parser')
         first_header = soup.find('h1')
         is_html = len(soup.find_all()) > 0
         if first_header:
             first_header = first_header.string
-        if is_html:
-            if not raw:
-                body = markdownify(body).lstrip().rstrip()
-                body = re.sub('\n\n\n*', '\n\n', body)
-            title, body = Note.title_and_body(body)
-            if first_header:
-                title = first_header
+        if is_html and not raw:
+            body = markdownify(body).lstrip().rstrip()
+            body = re.sub('\n\n\n*', '\n\n', body)
+        title, body = Note.title_and_body(body)
+        if first_header:
+            title = first_header
 
         if matches:
             matching = self.find_matching_notes(matches)
             if matching:
                 note = matching[0]
                 note.body = body
                 note.modified = now
```

### Comparing `simplenote_local-1.0/simplenote_local/cli.py` & `simplenote_local-1.0.1/simplenote_local/cli.py`

 * *Files identical despite different names*

### Comparing `simplenote_local-1.0/simplenote_local.egg-info/PKG-INFO` & `simplenote_local-1.0.1/simplenote_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplenote_local
-Version: 1.0
+Version: 1.0.1
 Summary: Sync notes to/from simplenote.com
 Home-page: https://github.com/norm/simplenote-local
 Author: Mark Norman Francis
 Author-email: norm@201created.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

