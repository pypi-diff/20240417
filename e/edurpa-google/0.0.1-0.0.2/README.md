# Comparing `tmp/EduRPA.Google-0.0.1.tar.gz` & `tmp/EduRPA-Google-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EduRPA.Google-0.0.1.tar", last modified: Wed Apr 17 14:52:32 2024, max compression
+gzip compressed data, was "EduRPA-Google-0.0.2.tar", last modified: Wed Apr 17 15:04:31 2024, max compression
```

## Comparing `EduRPA.Google-0.0.1.tar` & `EduRPA-Google-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 14:52:32.892197 EduRPA.Google-0.0.1/
--rw-rw-rw-   0        0        0     1088 2024-02-07 12:41:53.000000 EduRPA.Google-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      527 2024-04-17 14:52:32.890275 EduRPA.Google-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-02-07 12:40:46.000000 EduRPA.Google-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 14:52:32.892197 EduRPA.Google-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1061 2024-04-17 14:51:46.000000 EduRPA.Google-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:52:32.855246 EduRPA.Google-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 14:52:32.890275 EduRPA.Google-0.0.1/src/EduRPA.Google.egg-info/
--rw-rw-rw-   0        0        0      527 2024-04-17 14:52:32.000000 EduRPA.Google-0.0.1/src/EduRPA.Google.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-17 14:52:32.000000 EduRPA.Google-0.0.1/src/EduRPA.Google.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 14:52:32.000000 EduRPA.Google-0.0.1/src/EduRPA.Google.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-17 14:52:32.000000 EduRPA.Google-0.0.1/src/EduRPA.Google.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 14:52:32.000000 EduRPA.Google-0.0.1/src/EduRPA.Google.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 15:04:31.209911 EduRPA-Google-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2024-02-07 12:41:53.000000 EduRPA-Google-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      527 2024-04-17 15:04:31.206551 EduRPA-Google-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-02-07 12:40:46.000000 EduRPA-Google-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 15:04:31.209911 EduRPA-Google-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1061 2024-04-17 15:00:56.000000 EduRPA-Google-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:04:31.162157 EduRPA-Google-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 15:04:31.177932 EduRPA-Google-0.0.2/src/EduRPA-Google/
+-rw-rw-rw-   0        0        0    13083 2024-04-17 14:40:59.000000 EduRPA-Google-0.0.2/src/EduRPA-Google/Classroom.py
+-rw-rw-rw-   0        0        0     1549 2024-04-17 15:02:59.000000 EduRPA-Google-0.0.2/src/EduRPA-Google/CustomOAuth.py
+-rw-rw-rw-   0        0        0    11939 2024-04-17 14:40:59.000000 EduRPA-Google-0.0.2/src/EduRPA-Google/Form.py
+-rw-rw-rw-   0        0        0      313 2024-04-17 14:41:36.000000 EduRPA-Google-0.0.2/src/EduRPA-Google/Utils.py
+-rw-rw-rw-   0        0        0       22 2024-04-17 14:58:41.000000 EduRPA-Google-0.0.2/src/EduRPA-Google/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:04:31.206551 EduRPA-Google-0.0.2/src/EduRPA_Google.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-04-17 15:04:31.000000 EduRPA-Google-0.0.2/src/EduRPA_Google.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2024-04-17 15:04:31.000000 EduRPA-Google-0.0.2/src/EduRPA_Google.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 15:04:31.000000 EduRPA-Google-0.0.2/src/EduRPA_Google.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-17 15:04:31.000000 EduRPA-Google-0.0.2/src/EduRPA_Google.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-17 15:04:31.000000 EduRPA-Google-0.0.2/src/EduRPA_Google.egg-info/top_level.txt
```

### Comparing `EduRPA.Google-0.0.1/LICENSE` & `EduRPA-Google-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EduRPA.Google-0.0.1/PKG-INFO` & `EduRPA-Google-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: EduRPA.Google
-Version: 0.0.1
+Name: EduRPA-Google
+Version: 0.0.2
 Summary: Education Google RPA Librabry For Education
 Home-page: https://github.com/edu-rpa/edu-rpa-library
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EduRPA.Google-0.0.1/setup.py` & `EduRPA-Google-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     install_requires = [
             str(requirement)
             for requirement
             in pkg_resources.parse_requirements(requirements)
         ]
 
 setuptools.setup(
-    name="EduRPA.Google",
-    version="0.0.1",
+    name="EduRPA-Google",
+    version="0.0.2",
     author="david",
     author_email="davidhuynh0222@gmail.com",
     description="Education Google RPA Librabry For Education",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/edu-rpa/edu-rpa-library",
     package_dir={'': 'src'},
```

### Comparing `EduRPA.Google-0.0.1/src/EduRPA.Google.egg-info/PKG-INFO` & `EduRPA-Google-0.0.2/src/EduRPA_Google.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: EduRPA.Google
-Version: 0.0.1
+Name: EduRPA-Google
+Version: 0.0.2
 Summary: Education Google RPA Librabry For Education
 Home-page: https://github.com/edu-rpa/edu-rpa-library
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

