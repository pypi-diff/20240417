# Comparing `tmp/ToolsStr-1.1.1.tar.gz` & `tmp/toolsstr-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ToolsStr-1.1.1.tar", last modified: Thu Apr 11 11:25:28 2024, max compression
+gzip compressed data, was "toolsstr-1.1.2.tar", last modified: Wed Apr 17 10:33:56 2024, max compression
```

## Comparing `ToolsStr-1.1.1.tar` & `toolsstr-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 11:25:28.595883 ToolsStr-1.1.1/
--rw-rw-rw-   0        0        0     1094 2024-04-09 13:17:14.000000 ToolsStr-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      532 2024-04-11 11:25:28.590887 ToolsStr-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 11:25:28.587907 ToolsStr-1.1.1/ToolsStr.egg-info/
--rw-rw-rw-   0        0        0      532 2024-04-11 11:25:28.000000 ToolsStr-1.1.1/ToolsStr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-04-11 11:25:28.000000 ToolsStr-1.1.1/ToolsStr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 11:25:28.000000 ToolsStr-1.1.1/ToolsStr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 11:25:28.000000 ToolsStr-1.1.1/ToolsStr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 11:25:28.595883 ToolsStr-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      788 2024-04-11 11:24:22.000000 ToolsStr-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:25:28.581879 ToolsStr-1.1.1/toolsstr/
--rw-rw-rw-   0        0        0        0 2024-04-11 10:51:20.000000 ToolsStr-1.1.1/toolsstr/__init__.py
--rw-rw-rw-   0        0        0      260 2024-04-11 10:29:14.000000 ToolsStr-1.1.1/toolsstr/pystrtools.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:33:56.955086 toolsstr-1.1.2/
+-rw-rw-rw-   0        0        0     1094 2024-04-09 13:17:14.000000 toolsstr-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      532 2024-04-17 10:33:56.952087 toolsstr-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 10:33:56.665085 toolsstr-1.1.2/ToolsStr/
+-rw-rw-rw-   0        0        0       31 2024-04-16 20:37:46.000000 toolsstr-1.1.2/ToolsStr/__init__.py
+-rw-rw-rw-   0        0        0     1006 2024-04-16 22:15:25.000000 toolsstr-1.1.2/ToolsStr/toolsstr.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:33:56.948088 toolsstr-1.1.2/ToolsStr.egg-info/
+-rw-rw-rw-   0        0        0      532 2024-04-17 10:33:56.000000 toolsstr-1.1.2/ToolsStr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-04-17 10:33:56.000000 toolsstr-1.1.2/ToolsStr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 10:33:56.000000 toolsstr-1.1.2/ToolsStr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-17 10:33:56.000000 toolsstr-1.1.2/ToolsStr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 10:33:56.956088 toolsstr-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      788 2024-04-17 10:29:34.000000 toolsstr-1.1.2/setup.py
```

### Comparing `ToolsStr-1.1.1/LICENSE` & `toolsstr-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ToolsStr-1.1.1/PKG-INFO` & `toolsstr-1.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ToolsStr
-Version: 1.1.1
+Version: 1.1.2
 Summary: A small package for keyboard typing in Python
 Author: Amirmahdi Mohammadi
 Author-email: amirmahdi21r21@gmail.com
 Keywords: python,type,master,toolsstr,rubika,library,strtools
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ToolsStr-1.1.1/ToolsStr.egg-info/PKG-INFO` & `toolsstr-1.1.2/ToolsStr.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ToolsStr
-Version: 1.1.1
+Version: 1.1.2
 Summary: A small package for keyboard typing in Python
 Author: Amirmahdi Mohammadi
 Author-email: amirmahdi21r21@gmail.com
 Keywords: python,type,master,toolsstr,rubika,library,strtools
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ToolsStr-1.1.1/setup.py` & `toolsstr-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
         name="ToolsStr", 
-        version='1.1.1',
+        version='1.1.2',
         author="Amirmahdi Mohammadi",
         author_email="amirmahdi21r21@gmail.com",
         description='A small package for keyboard typing in Python',
         long_description='Keyboard Typing . . .\n\nMy GitHub page: https://gitHub.com/FrameworkPython',
         packages=find_packages(),
         
         install_requires=[],
```

