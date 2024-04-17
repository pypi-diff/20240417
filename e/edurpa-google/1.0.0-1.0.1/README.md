# Comparing `tmp/edurpa_google-1.0.0.tar.gz` & `tmp/edurpa_google-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edurpa_google-1.0.0.tar", last modified: Wed Apr 17 15:30:10 2024, max compression
+gzip compressed data, was "edurpa_google-1.0.1.tar", last modified: Wed Apr 17 15:41:29 2024, max compression
```

## Comparing `edurpa_google-1.0.0.tar` & `edurpa_google-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 15:30:10.531556 edurpa_google-1.0.0/
--rw-rw-rw-   0        0        0     1088 2024-02-07 12:41:53.000000 edurpa_google-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      527 2024-04-17 15:30:10.531556 edurpa_google-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-02-07 12:40:46.000000 edurpa_google-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 15:30:10.531556 edurpa_google-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1061 2024-04-17 15:29:39.000000 edurpa_google-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:30:10.501168 edurpa_google-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 15:30:10.505558 edurpa_google-1.0.0/src/edurpa_google/
--rw-rw-rw-   0        0        0    13083 2024-04-17 14:40:59.000000 edurpa_google-1.0.0/src/edurpa_google/Classroom.py
--rw-rw-rw-   0        0        0     1549 2024-04-17 15:02:59.000000 edurpa_google-1.0.0/src/edurpa_google/CustomOAuth.py
--rw-rw-rw-   0        0        0    11939 2024-04-17 14:40:59.000000 edurpa_google-1.0.0/src/edurpa_google/Form.py
--rw-rw-rw-   0        0        0      313 2024-04-17 14:41:36.000000 edurpa_google-1.0.0/src/edurpa_google/Utils.py
--rw-rw-rw-   0        0        0       22 2024-04-17 15:12:01.000000 edurpa_google-1.0.0/src/edurpa_google/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:30:10.529301 edurpa_google-1.0.0/src/edurpa_google.egg-info/
--rw-rw-rw-   0        0        0      527 2024-04-17 15:30:10.000000 edurpa_google-1.0.0/src/edurpa_google.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2024-04-17 15:30:10.000000 edurpa_google-1.0.0/src/edurpa_google.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 15:30:10.000000 edurpa_google-1.0.0/src/edurpa_google.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-17 15:30:10.000000 edurpa_google-1.0.0/src/edurpa_google.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-17 15:30:10.000000 edurpa_google-1.0.0/src/edurpa_google.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 15:41:29.349195 edurpa_google-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2024-02-07 12:41:53.000000 edurpa_google-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      527 2024-04-17 15:41:29.349195 edurpa_google-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-02-07 12:40:46.000000 edurpa_google-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 15:41:29.349195 edurpa_google-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1061 2024-04-17 15:41:21.000000 edurpa_google-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:41:29.314850 edurpa_google-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 15:41:29.348606 edurpa_google-1.0.1/src/edurpa_google.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-04-17 15:41:29.000000 edurpa_google-1.0.1/src/edurpa_google.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-04-17 15:41:29.000000 edurpa_google-1.0.1/src/edurpa_google.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 15:41:29.000000 edurpa_google-1.0.1/src/edurpa_google.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-17 15:41:29.000000 edurpa_google-1.0.1/src/edurpa_google.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 15:41:29.000000 edurpa_google-1.0.1/src/edurpa_google.egg-info/top_level.txt
```

### Comparing `edurpa_google-1.0.0/LICENSE` & `edurpa_google-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edurpa_google-1.0.0/PKG-INFO` & `edurpa_google-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edurpa_google
-Version: 1.0.0
+Version: 1.0.1
 Summary: Education Google RPA Librabry For Education
 Home-page: https://github.com/edu-rpa/edu-rpa-library
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `edurpa_google-1.0.0/setup.py` & `edurpa_google-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             str(requirement)
             for requirement
             in pkg_resources.parse_requirements(requirements)
         ]
 
 setuptools.setup(
     name="edurpa_google",
-    version="1.0.0",
+    version="1.0.1",
     author="david",
     author_email="davidhuynh0222@gmail.com",
     description="Education Google RPA Librabry For Education",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/edu-rpa/edu-rpa-library",
     package_dir={'': 'src'},
```

### Comparing `edurpa_google-1.0.0/src/edurpa_google.egg-info/PKG-INFO` & `edurpa_google-1.0.1/src/edurpa_google.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edurpa-google
-Version: 1.0.0
+Version: 1.0.1
 Summary: Education Google RPA Librabry For Education
 Home-page: https://github.com/edu-rpa/edu-rpa-library
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

