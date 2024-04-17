# Comparing `tmp/robotframework-xlibrary-10.0.1.tar.gz` & `tmp/robotframework-xlibrary-11.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robotframework-xlibrary-10.0.1.tar", last modified: Thu Apr 11 06:34:12 2024, max compression
+gzip compressed data, was "dist\robotframework-xlibrary-11.0.0.tar", last modified: Wed Apr 17 07:36:25 2024, max compression
```

## Comparing `robotframework-xlibrary-10.0.1.tar` & `robotframework-xlibrary-11.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 06:34:12.000000 robotframework-xlibrary-10.0.1/
--rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-10.0.1/LICENSE
--rw-rw-rw-   0        0        0     1585 2024-04-11 06:34:12.000000 robotframework-xlibrary-10.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-03-18 09:46:55.000000 robotframework-xlibrary-10.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 06:34:12.000000 robotframework-xlibrary-10.0.1/setup.cfg
--rw-rw-rw-   0        0        0      780 2024-04-11 06:32:50.000000 robotframework-xlibrary-10.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:34:12.000000 robotframework-xlibrary-10.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-11 06:34:12.000000 robotframework-xlibrary-10.0.1/src/XLibrary/
--rw-rw-rw-   0        0        0     1532 2024-04-11 04:31:20.000000 robotframework-xlibrary-10.0.1/src/XLibrary/__init__.py
--rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-10.0.1/src/XLibrary/main.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:34:12.000000 robotframework-xlibrary-10.0.1/src/XLibrary/submodule1/
--rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-10.0.1/src/XLibrary/submodule1/__init__.py
--rw-rw-rw-   0        0        0     4248 2024-04-11 04:31:16.000000 robotframework-xlibrary-10.0.1/src/XLibrary/submodule1/module1.py
--rw-rw-rw-   0        0        0     1306 2024-04-11 06:19:22.000000 robotframework-xlibrary-10.0.1/src/XLibrary/submodule1/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:34:12.000000 robotframework-xlibrary-10.0.1/src/XLibrary/submodule2/
--rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-10.0.1/src/XLibrary/submodule2/__init__.py
--rw-rw-rw-   0        0        0      312 2024-03-18 09:34:30.000000 robotframework-xlibrary-10.0.1/src/XLibrary/submodule2/module1.py
--rw-rw-rw-   0        0        0      261 2024-03-18 09:34:30.000000 robotframework-xlibrary-10.0.1/src/XLibrary/submodule2/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:34:12.000000 robotframework-xlibrary-10.0.1/src/robotframework_xlibrary.egg-info/
--rw-rw-rw-   0        0        0     1585 2024-04-11 06:34:12.000000 robotframework-xlibrary-10.0.1/src/robotframework_xlibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-11 06:34:12.000000 robotframework-xlibrary-10.0.1/src/robotframework_xlibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 06:34:12.000000 robotframework-xlibrary-10.0.1/src/robotframework_xlibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-11 06:34:12.000000 robotframework-xlibrary-10.0.1/src/robotframework_xlibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 06:34:12.000000 robotframework-xlibrary-10.0.1/src/robotframework_xlibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/
+-rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-11.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1588 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-03-18 09:46:55.000000 robotframework-xlibrary-11.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      783 2024-04-17 07:35:37.000000 robotframework-xlibrary-11.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/XLibrary/
+-rw-rw-rw-   0        0        0     1114 2024-04-17 07:26:57.000000 robotframework-xlibrary-11.0.0/src/XLibrary/__init__.py
+-rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-11.0.0/src/XLibrary/main.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule1/
+-rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule1/__init__.py
+-rw-rw-rw-   0        0        0     4248 2024-04-11 04:31:16.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule1/module1.py
+-rw-rw-rw-   0        0        0     5643 2024-04-17 07:20:47.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule1/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule2/
+-rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule2/__init__.py
+-rw-rw-rw-   0        0        0     1774 2024-04-13 12:59:03.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule2/module1.py
+-rw-rw-rw-   0        0        0      261 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule2/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/
+-rw-rw-rw-   0        0        0     1588 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/top_level.txt
```

### Comparing `robotframework-xlibrary-10.0.1/PKG-INFO` & `robotframework-xlibrary-11.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 10.0.1
-Summary: Test Library for robotframework-xlibrary
+Version: 11.0.0
+Summary: Test Custom Library robotframework-xlibrary
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `robotframework-xlibrary-10.0.1/README.md` & `robotframework-xlibrary-11.0.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-10.0.1/setup.py` & `robotframework-xlibrary-11.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="robotframework-xlibrary",
-    version="10.0.1",
+    version="11.0.0",
     author="Tassana Khrueawan",
     author_email="tassana.khr@gmail.com",
-    description="Test Library for robotframework-xlibrary",
+    description="Test Custom Library robotframework-xlibrary",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Khrx1999/robotframework-xlibrary.git",
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     install_requires=[
         'robotframework>=3.0',
```

### Comparing `robotframework-xlibrary-10.0.1/src/XLibrary/__init__.py` & `robotframework-xlibrary-11.0.0/src/XLibrary/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,27 +16,17 @@
 class XLibrary(
     MainClass,
     XPrint, 
     XDrint,
     Module21,
     Module22
     ):
-    """ XLibrary เป็น Library Custom ขึ้้นมาใช้เองโดยเฉพาะ 
-
-
-
-        | Click Element |    Key            |
-        | Click Element |    Text="Text"    |
-
-        ตัวกำหนดตำแหน่งที่สามารถใช้ได้:
-
-        | *Locator*    | *Description*                      |
-        | key          | key ของอิลิเมนต์ FlutterDriver.       |
-        | text         | ข้อความของอิลิเมนต์.                   |
-
+    """ 
+    *` XLibrary เป็น Library Custom ขึ้้นมาใช้เองโดยเฉพาะ`*
+    *`Create By Tassana Khrueawan`*
     """
 
 
     def TTTTTT(self):
         """ พิมพ์ข้อความ 'Hello, world!' ลงในคอนโซล แบบไม่ได้แอดคีย์ """
         print("Hello, world! เทสภาษาไทยfdsafadsfsadfdsafdsa")
```

### Comparing `robotframework-xlibrary-10.0.1/src/XLibrary/submodule1/module1.py` & `robotframework-xlibrary-11.0.0/src/XLibrary/submodule1/module1.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-10.0.1/src/robotframework_xlibrary.egg-info/PKG-INFO` & `robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 10.0.1
-Summary: Test Library for robotframework-xlibrary
+Version: 11.0.0
+Summary: Test Custom Library robotframework-xlibrary
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `robotframework-xlibrary-10.0.1/src/robotframework_xlibrary.egg-info/SOURCES.txt` & `robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

