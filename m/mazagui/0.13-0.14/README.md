# Comparing `tmp/mazagui-0.13.tar.gz` & `tmp/mazagui-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazagui-0.13.tar", last modified: Sat Mar  9 15:13:19 2024, max compression
+gzip compressed data, was "mazagui-0.14.tar", last modified: Wed Apr 17 15:27:05 2024, max compression
```

## Comparing `mazagui-0.13.tar` & `mazagui-0.14.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-09 15:13:19.388906 mazagui-0.13/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35148 2023-07-29 11:56:29.000000 mazagui-0.13/LICENSE.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2579 2024-03-09 15:13:19.388616 mazagui-0.13/PKG-INFO
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1878 2023-09-05 17:08:45.000000 mazagui-0.13/README.md
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       38 2024-03-09 15:13:19.389010 mazagui-0.13/setup.cfg
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1111 2024-03-09 15:12:12.000000 mazagui-0.13/setup.py
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-09 15:13:19.377829 mazagui-0.13/src/
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-09 15:13:19.383429 mazagui-0.13/src/mazagui/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   270398 2020-11-14 15:11:36.000000 mazagui-0.13/src/mazagui/MAZAlib.ico
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       20 2023-09-10 13:34:37.000000 mazagui-0.13/src/mazagui/__init__.py
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    36199 2024-03-09 14:53:12.000000 mazagui-0.13/src/mazagui/gui.py
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-09 15:13:19.387744 mazagui-0.13/src/mazagui.egg-info/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2579 2024-03-09 15:13:19.000000 mazagui-0.13/src/mazagui.egg-info/PKG-INFO
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      271 2024-03-09 15:13:19.000000 mazagui-0.13/src/mazagui.egg-info/SOURCES.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)        1 2024-03-09 15:13:19.000000 mazagui-0.13/src/mazagui.egg-info/dependency_links.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       37 2024-03-09 15:13:19.000000 mazagui-0.13/src/mazagui.egg-info/requires.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)        8 2024-03-09 15:13:19.000000 mazagui-0.13/src/mazagui.egg-info/top_level.txt
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:27:05.387460 mazagui-0.14/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35148 2023-07-29 11:56:29.000000 mazagui-0.14/LICENSE.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2847 2024-04-17 15:27:05.387213 mazagui-0.14/PKG-INFO
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2088 2024-04-17 15:24:07.000000 mazagui-0.14/README.md
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       38 2024-04-17 15:27:05.387554 mazagui-0.14/setup.cfg
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1234 2024-04-17 15:25:32.000000 mazagui-0.14/setup.py
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:27:05.377358 mazagui-0.14/src/
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:27:05.382639 mazagui-0.14/src/mazagui/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   270398 2020-11-14 15:11:36.000000 mazagui-0.14/src/mazagui/MAZAlib.ico
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       20 2023-09-10 13:34:37.000000 mazagui-0.14/src/mazagui/__init__.py
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    36199 2024-03-09 14:53:12.000000 mazagui-0.14/src/mazagui/gui.py
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:27:05.386375 mazagui-0.14/src/mazagui.egg-info/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2847 2024-04-17 15:27:05.000000 mazagui-0.14/src/mazagui.egg-info/PKG-INFO
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      271 2024-04-17 15:27:05.000000 mazagui-0.14/src/mazagui.egg-info/SOURCES.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)        1 2024-04-17 15:27:05.000000 mazagui-0.14/src/mazagui.egg-info/dependency_links.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       37 2024-04-17 15:27:05.000000 mazagui-0.14/src/mazagui.egg-info/requires.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)        8 2024-04-17 15:27:05.000000 mazagui-0.14/src/mazagui.egg-info/top_level.txt
```

### Comparing `mazagui-0.13/LICENSE.txt` & `mazagui-0.14/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mazagui-0.13/setup.py` & `mazagui-0.14/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 from setuptools import setup, find_packages
+import pip
 
-version='0.13'
+
+
+version='0.14'
 libName="mazagui"
 
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 short_description = "GUI for cross-platform 2d/3d image segmentation C++ library"
 
 installRequiresList=['mazalib','matplotlib','tk','Pillow','imageio']
 
+pip.main(['install'] + installRequiresList)
 
 setup(
 	name=libName,
 	version=version,
 	description=short_description,
 	long_description=long_description,
-	author='Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina',
+	long_description_content_type="text/markdown",
+	author='Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina, Andrey A. Ananev',
 	author_email='mathieu.gravey@unil.ch',
 	license='GPLv3',
 	packages=find_packages('src',include=['mazagui']),
 	package_dir={'': 'src'},
 	package_data={'mazagui': ['./MAZAlib.ico']},
 	classifiers=[
 		'Development Status :: 3 - Alpha',
```

### Comparing `mazagui-0.13/src/mazagui/MAZAlib.ico` & `mazagui-0.14/src/mazagui/MAZAlib.ico`

 * *Files identical despite different names*

### Comparing `mazagui-0.13/src/mazagui/gui.py` & `mazagui-0.14/src/mazagui/gui.py`

 * *Files identical despite different names*

