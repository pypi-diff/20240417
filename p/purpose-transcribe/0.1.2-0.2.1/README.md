# Comparing `tmp/purpose_transcribe-0.1.2.tar.gz` & `tmp/purpose_transcribe-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purpose_transcribe-0.1.2.tar", last modified: Mon Apr 15 20:37:21 2024, max compression
+gzip compressed data, was "purpose_transcribe-0.2.1.tar", last modified: Tue Apr 16 23:58:01 2024, max compression
```

## Comparing `purpose_transcribe-0.1.2.tar` & `purpose_transcribe-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 mo197      (504) staff       (20)        0 2024-04-15 20:37:21.907407 purpose_transcribe-0.1.2/
--rw-r--r--   0 mo197      (504) staff       (20)     1577 2024-04-15 18:49:51.000000 purpose_transcribe-0.1.2/LICENSE
--rw-r--r--   0 mo197      (504) staff       (20)       33 2024-04-15 18:40:20.000000 purpose_transcribe-0.1.2/MANIFEST.in
--rw-r--r--   0 mo197      (504) staff       (20)     2183 2024-04-15 20:37:21.907344 purpose_transcribe-0.1.2/PKG-INFO
--rw-r--r--   0 mo197      (504) staff       (20)     1516 2024-04-15 19:27:17.000000 purpose_transcribe-0.1.2/README.md
-drwxr-xr-x   0 mo197      (504) staff       (20)        0 2024-04-15 20:37:21.905008 purpose_transcribe-0.1.2/purpose_transcribe/
-drwxr-xr-x   0 mo197      (504) staff       (20)        0 2024-04-15 20:37:21.907117 purpose_transcribe-0.1.2/purpose_transcribe/purpose_transcribe.egg-info/
--rw-r--r--   0 mo197      (504) staff       (20)     2183 2024-04-15 20:37:21.000000 purpose_transcribe-0.1.2/purpose_transcribe/purpose_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 mo197      (504) staff       (20)      416 2024-04-15 20:37:21.000000 purpose_transcribe-0.1.2/purpose_transcribe/purpose_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 mo197      (504) staff       (20)        1 2024-04-15 20:37:21.000000 purpose_transcribe-0.1.2/purpose_transcribe/purpose_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 mo197      (504) staff       (20)       77 2024-04-15 20:37:21.000000 purpose_transcribe-0.1.2/purpose_transcribe/purpose_transcribe.egg-info/entry_points.txt
--rw-r--r--   0 mo197      (504) staff       (20)       21 2024-04-15 20:37:21.000000 purpose_transcribe-0.1.2/purpose_transcribe/purpose_transcribe.egg-info/requires.txt
--rw-r--r--   0 mo197      (504) staff       (20)        1 2024-04-15 20:37:21.000000 purpose_transcribe-0.1.2/purpose_transcribe/purpose_transcribe.egg-info/top_level.txt
--rw-r--r--   0 mo197      (504) staff       (20)      591 2024-04-15 20:37:21.907618 purpose_transcribe-0.1.2/setup.cfg
--rw-r--r--   0 mo197      (504) staff       (20)     1022 2024-04-15 20:35:48.000000 purpose_transcribe-0.1.2/setup.py
+drwxr-xr-x   0 mo197      (504) staff       (20)        0 2024-04-16 23:58:01.666574 purpose_transcribe-0.2.1/
+-rw-r--r--   0 mo197      (504) staff       (20)     1577 2024-04-15 18:49:51.000000 purpose_transcribe-0.2.1/LICENSE
+-rw-r--r--   0 mo197      (504) staff       (20)       33 2024-04-15 18:40:20.000000 purpose_transcribe-0.2.1/MANIFEST.in
+-rw-r--r--   0 mo197      (504) staff       (20)     2207 2024-04-16 23:58:01.666476 purpose_transcribe-0.2.1/PKG-INFO
+-rw-r--r--   0 mo197      (504) staff       (20)     1541 2024-04-16 23:37:48.000000 purpose_transcribe-0.2.1/README.md
+-rw-r--r--   0 mo197      (504) staff       (20)      561 2024-04-16 23:58:01.666820 purpose_transcribe-0.2.1/setup.cfg
+-rw-r--r--   0 mo197      (504) staff       (20)      992 2024-04-16 23:57:12.000000 purpose_transcribe-0.2.1/setup.py
+drwxr-xr-x   0 mo197      (504) staff       (20)        0 2024-04-16 23:58:01.663835 purpose_transcribe-0.2.1/src/
+drwxr-xr-x   0 mo197      (504) staff       (20)        0 2024-04-16 23:58:01.664918 purpose_transcribe-0.2.1/src/purpose_transcribe/
+-rw-r--r--   0 mo197      (504) staff       (20)        0 2024-04-16 23:47:02.000000 purpose_transcribe-0.2.1/src/purpose_transcribe/__init__.py
+-rw-r--r--   0 mo197      (504) staff       (20)      812 2024-04-16 23:54:20.000000 purpose_transcribe-0.2.1/src/purpose_transcribe/main.py
+-rw-r--r--   0 mo197      (504) staff       (20)      902 2024-04-16 23:37:38.000000 purpose_transcribe-0.2.1/src/purpose_transcribe/transcription.py
+-rw-r--r--   0 mo197      (504) staff       (20)      250 2024-04-16 23:37:38.000000 purpose_transcribe-0.2.1/src/purpose_transcribe/utils.py
+drwxr-xr-x   0 mo197      (504) staff       (20)        0 2024-04-16 23:58:01.666203 purpose_transcribe-0.2.1/src/purpose_transcribe.egg-info/
+-rw-r--r--   0 mo197      (504) staff       (20)     2207 2024-04-16 23:58:01.000000 purpose_transcribe-0.2.1/src/purpose_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 mo197      (504) staff       (20)      464 2024-04-16 23:58:01.000000 purpose_transcribe-0.2.1/src/purpose_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 mo197      (504) staff       (20)        1 2024-04-16 23:58:01.000000 purpose_transcribe-0.2.1/src/purpose_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 mo197      (504) staff       (20)       77 2024-04-16 23:58:01.000000 purpose_transcribe-0.2.1/src/purpose_transcribe.egg-info/entry_points.txt
+-rw-r--r--   0 mo197      (504) staff       (20)       21 2024-04-16 23:58:01.000000 purpose_transcribe-0.2.1/src/purpose_transcribe.egg-info/requires.txt
+-rw-r--r--   0 mo197      (504) staff       (20)       19 2024-04-16 23:58:01.000000 purpose_transcribe-0.2.1/src/purpose_transcribe.egg-info/top_level.txt
```

### Comparing `purpose_transcribe-0.1.2/LICENSE` & `purpose_transcribe-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `purpose_transcribe-0.1.2/PKG-INFO` & `purpose_transcribe-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purpose_transcribe
-Version: 0.1.2
+Version: 0.2.1
 Summary: A CLI tool for transcribing audio files
 Author: Mark Okello
 Author-email: markokello55@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -15,15 +15,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: openai-whisper
 
 # Purpose Transcribe
-A CLI tool for transcribing audio.
+A CLI tool for transcribing audio for the purpose project.
 ## Installation
 install Purpose Transcribe via pip:
 ```bash 
 pip install purpose_transcribe
 ```
 ## Usage
 To use the tool, navigate to the directory containing your audio files and run:
```

### Comparing `purpose_transcribe-0.1.2/README.md` & `purpose_transcribe-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Purpose Transcribe
-A CLI tool for transcribing audio.
+A CLI tool for transcribing audio for the purpose project.
 ## Installation
 install Purpose Transcribe via pip:
 ```bash 
 pip install purpose_transcribe
 ```
 ## Usage
 To use the tool, navigate to the directory containing your audio files and run:
@@ -44,8 +44,8 @@
 ```
 You will need a PyPI account to upload. Enter your username and password as prompted.
 Verify Installation
 Once uploaded, you can install your package using:
 
 ```bash
 pip install your_package
-```
+```
```

### Comparing `purpose_transcribe-0.1.2/purpose_transcribe/purpose_transcribe.egg-info/PKG-INFO` & `purpose_transcribe-0.2.1/src/purpose_transcribe.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purpose_transcribe
-Version: 0.1.2
+Version: 0.2.1
 Summary: A CLI tool for transcribing audio files
 Author: Mark Okello
 Author-email: markokello55@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -15,15 +15,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: openai-whisper
 
 # Purpose Transcribe
-A CLI tool for transcribing audio.
+A CLI tool for transcribing audio for the purpose project.
 ## Installation
 install Purpose Transcribe via pip:
 ```bash 
 pip install purpose_transcribe
 ```
 ## Usage
 To use the tool, navigate to the directory containing your audio files and run:
```

### Comparing `purpose_transcribe-0.1.2/setup.cfg` & `purpose_transcribe-0.2.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [metadata]
 name = purpose_transcribe
-version = 0.1.2
+version = 0.2.1
 author = Mark Okello
 author_email = markokello55@gmail.com
 description = Transcription Tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
-	= purpose_transcribe
+	= src
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	click
 	openai-whisper
 
 [options.packages.find]
-where = purpose_transcribe
+where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `purpose_transcribe-0.1.2/setup.py` & `purpose_transcribe-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 setup(
     name='purpose_transcribe',
-    version='0.1.2',
+    version='0.2.1',
     description='A CLI tool for transcribing audio files',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Mark Okello',
-    packages=find_packages(where="purpose_transcribe"),
-    package_dir={"": "purpose_transcribe"},
+    packages=find_packages(where="src"),
+    package_dir={"": "src"},
     include_package_data=True,
     install_requires=[
         'click',
         'openai-whisper'
     ],
     entry_points={
         'console_scripts': [
```

