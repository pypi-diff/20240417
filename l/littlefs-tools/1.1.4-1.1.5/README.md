# Comparing `tmp/littlefs_tools-1.1.4.tar.gz` & `tmp/littlefs_tools-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "littlefs_tools-1.1.4.tar", last modified: Thu Jan 11 19:09:21 2024, max compression
+gzip compressed data, was "littlefs_tools-1.1.5.tar", last modified: Tue Apr 16 23:22:08 2024, max compression
```

## Comparing `littlefs_tools-1.1.4.tar` & `littlefs_tools-1.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 19:09:21.486540 littlefs_tools-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-11 19:09:18.000000 littlefs_tools-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-01-11 19:09:21.486540 littlefs_tools-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-01-11 19:09:18.000000 littlefs_tools-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 19:09:21.482540 littlefs_tools-1.1.4/littlefs_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-11 19:09:18.000000 littlefs_tools-1.1.4/littlefs_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-01-11 19:09:18.000000 littlefs_tools-1.1.4/littlefs_tools/littlefs_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 19:09:21.486540 littlefs_tools-1.1.4/littlefs_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-01-11 19:09:21.000000 littlefs_tools-1.1.4/littlefs_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-11 19:09:21.000000 littlefs_tools-1.1.4/littlefs_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 19:09:21.000000 littlefs_tools-1.1.4/littlefs_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-11 19:09:21.000000 littlefs_tools-1.1.4/littlefs_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-11 19:09:21.000000 littlefs_tools-1.1.4/littlefs_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-11 19:09:21.000000 littlefs_tools-1.1.4/littlefs_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 19:09:21.486540 littlefs_tools-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-01-11 19:09:18.000000 littlefs_tools-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:22:08.672497 littlefs_tools-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-16 23:22:06.000000 littlefs_tools-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-16 23:22:08.672497 littlefs_tools-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-16 23:22:06.000000 littlefs_tools-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:22:08.672497 littlefs_tools-1.1.5/littlefs_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 23:22:06.000000 littlefs_tools-1.1.5/littlefs_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-16 23:22:06.000000 littlefs_tools-1.1.5/littlefs_tools/littlefs_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:22:08.672497 littlefs_tools-1.1.5/littlefs_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-16 23:22:08.000000 littlefs_tools-1.1.5/littlefs_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-16 23:22:08.000000 littlefs_tools-1.1.5/littlefs_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 23:22:08.000000 littlefs_tools-1.1.5/littlefs_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-16 23:22:08.000000 littlefs_tools-1.1.5/littlefs_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 23:22:08.000000 littlefs_tools-1.1.5/littlefs_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 23:22:08.000000 littlefs_tools-1.1.5/littlefs_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 23:22:08.672497 littlefs_tools-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-16 23:22:06.000000 littlefs_tools-1.1.5/setup.py
```

### Comparing `littlefs_tools-1.1.4/LICENSE` & `littlefs_tools-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `littlefs_tools-1.1.4/PKG-INFO` & `littlefs_tools-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: littlefs_tools
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python package to create littleFS filesystem image binaries
 Home-page: https://github.com/vppillai/littlefs_tools
 Author: Vysakh P Pillai
-Author-email: vysakhpillai@embeddedinn.xyz
+Author-email: vysakhpillai@embeddedinn.com
 License: MIT
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Filesystems
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `littlefs_tools-1.1.4/README.md` & `littlefs_tools-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `littlefs_tools-1.1.4/littlefs_tools/littlefs_tools.py` & `littlefs_tools-1.1.5/littlefs_tools/littlefs_tools.py`

 * *Files identical despite different names*

### Comparing `littlefs_tools-1.1.4/littlefs_tools.egg-info/PKG-INFO` & `littlefs_tools-1.1.5/littlefs_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: littlefs-tools
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python package to create littleFS filesystem image binaries
 Home-page: https://github.com/vppillai/littlefs_tools
 Author: Vysakh P Pillai
-Author-email: vysakhpillai@embeddedinn.xyz
+Author-email: vysakhpillai@embeddedinn.com
 License: MIT
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Filesystems
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `littlefs_tools-1.1.4/setup.py` & `littlefs_tools-1.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="littlefs_tools",
-    version="1.1.4",
+    version="1.1.5",
     description="Python package to create littleFS filesystem image binaries",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vppillai/littlefs_tools",
     author="Vysakh P Pillai",
-    author_email="vysakhpillai@embeddedinn.xyz",
+    author_email="vysakhpillai@embeddedinn.com",
     license="MIT",
     packages=["littlefs_tools"],
     install_requires=["littlefs-python", "colorama"],
     entry_points={
         "console_scripts": [
             "littlefs_list=littlefs_tools.littlefs_tools:list_files",
             "littlefs_create=littlefs_tools.littlefs_tools:create_image",
             "littlefs_extract=littlefs_tools.littlefs_tools:extract_files",
         ],
     },
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Topic :: Scientific/Engineering",
         "Topic :: System :: Filesystems",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
```

