# Comparing `tmp/edurpa_google-1.0.2.tar.gz` & `tmp/edurpa_google-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edurpa_google-1.0.2.tar", last modified: Wed Apr 17 15:44:19 2024, max compression
+gzip compressed data, was "edurpa_google-1.0.3.tar", last modified: Wed Apr 17 15:54:04 2024, max compression
```

## Comparing `edurpa_google-1.0.2.tar` & `edurpa_google-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 15:44:19.265039 edurpa_google-1.0.2/
--rw-rw-rw-   0        0        0     1088 2024-02-07 12:41:53.000000 edurpa_google-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      527 2024-04-17 15:44:19.264142 edurpa_google-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-02-07 12:40:46.000000 edurpa_google-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 15:44:19.265039 edurpa_google-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1069 2024-04-17 15:44:01.000000 edurpa_google-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:44:19.225602 edurpa_google-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 15:44:19.225602 edurpa_google-1.0.2/src/EduRPA/
-drwxrwxrwx   0        0        0        0 2024-04-17 15:44:19.262314 edurpa_google-1.0.2/src/EduRPA/edurpa_google.egg-info/
--rw-rw-rw-   0        0        0      527 2024-04-17 15:44:19.000000 edurpa_google-1.0.2/src/EduRPA/edurpa_google.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2024-04-17 15:44:19.000000 edurpa_google-1.0.2/src/EduRPA/edurpa_google.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 15:44:19.000000 edurpa_google-1.0.2/src/EduRPA/edurpa_google.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-17 15:44:19.000000 edurpa_google-1.0.2/src/EduRPA/edurpa_google.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 15:44:19.000000 edurpa_google-1.0.2/src/EduRPA/edurpa_google.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 15:54:04.499942 edurpa_google-1.0.3/
+-rw-rw-rw-   0        0        0     1088 2024-02-07 12:41:53.000000 edurpa_google-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      527 2024-04-17 15:54:04.499942 edurpa_google-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-02-07 12:40:46.000000 edurpa_google-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 15:54:04.500945 edurpa_google-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1083 2024-04-17 15:54:01.000000 edurpa_google-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:54:04.475788 edurpa_google-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 15:54:04.475788 edurpa_google-1.0.3/src/EduRPA/
+drwxrwxrwx   0        0        0        0 2024-04-17 15:54:04.496159 edurpa_google-1.0.3/src/EduRPA/edurpa_google.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-04-17 15:54:04.000000 edurpa_google-1.0.3/src/EduRPA/edurpa_google.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2024-04-17 15:54:04.000000 edurpa_google-1.0.3/src/EduRPA/edurpa_google.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 15:54:04.000000 edurpa_google-1.0.3/src/EduRPA/edurpa_google.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-17 15:54:04.000000 edurpa_google-1.0.3/src/EduRPA/edurpa_google.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 15:54:04.000000 edurpa_google-1.0.3/src/EduRPA/edurpa_google.egg-info/top_level.txt
```

### Comparing `edurpa_google-1.0.2/LICENSE` & `edurpa_google-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edurpa_google-1.0.2/PKG-INFO` & `edurpa_google-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edurpa_google
-Version: 1.0.2
+Version: 1.0.3
 Summary: Education Google RPA Librabry For Education
 Home-page: https://github.com/edu-rpa/edu-rpa-library
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `edurpa_google-1.0.2/setup.py` & `edurpa_google-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,23 +11,23 @@
             str(requirement)
             for requirement
             in pkg_resources.parse_requirements(requirements)
         ]
 
 setuptools.setup(
     name="edurpa_google",
-    version="1.0.2",
+    version="1.0.3",
     author="david",
     author_email="davidhuynh0222@gmail.com",
     description="Education Google RPA Librabry For Education",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/edu-rpa/edu-rpa-library",
     package_dir={'': 'src/EduRPA/'},
-    packages=setuptools.find_packages(where='src'),
+    packages=setuptools.find_packages(where='src/EduRPA/Google'),
     classifiers=[
         "Programming Language :: Python :: 2",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires = install_requires,
 )
```

### Comparing `edurpa_google-1.0.2/src/EduRPA/edurpa_google.egg-info/PKG-INFO` & `edurpa_google-1.0.3/src/EduRPA/edurpa_google.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edurpa-google
-Version: 1.0.2
+Version: 1.0.3
 Summary: Education Google RPA Librabry For Education
 Home-page: https://github.com/edu-rpa/edu-rpa-library
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

