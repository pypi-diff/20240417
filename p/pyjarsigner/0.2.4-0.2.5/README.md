# Comparing `tmp/pyjarsigner-0.2.4.tar.gz` & `tmp/pyjarsigner-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjarsigner-0.2.4.tar", last modified: Tue Aug 29 06:38:56 2023, max compression
+gzip compressed data, was "pyjarsigner-0.2.5.tar", max compression
```

## Comparing `pyjarsigner-0.2.4.tar` & `pyjarsigner-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,10 @@
-drwxr-xr-x   0 praseetha   (501) staff       (20)        0 2023-08-29 06:38:56.147511 pyjarsigner-0.2.4/
--rw-r--r--   0 praseetha   (501) staff       (20)     7651 2022-12-08 18:23:30.000000 pyjarsigner-0.2.4/LICENSE
--rw-r--r--   0 praseetha   (501) staff       (20)      989 2023-08-29 06:38:56.147596 pyjarsigner-0.2.4/PKG-INFO
-drwxr-xr-x   0 praseetha   (501) staff       (20)        0 2023-08-29 06:38:56.146421 pyjarsigner-0.2.4/pyjarsigner/
--rw-r--r--   0 praseetha   (501) staff       (20)       53 2022-12-08 18:23:30.000000 pyjarsigner-0.2.4/pyjarsigner/__init__.py
--rw-r--r--   0 praseetha   (501) staff       (20)    14935 2022-12-08 18:23:30.000000 pyjarsigner-0.2.4/pyjarsigner/change.py
--rw-r--r--   0 praseetha   (501) staff       (20)     4610 2022-12-08 18:23:30.000000 pyjarsigner-0.2.4/pyjarsigner/crypto.py
--rw-r--r--   0 praseetha   (501) staff       (20)     5706 2022-12-08 18:23:30.000000 pyjarsigner-0.2.4/pyjarsigner/dirutils.py
--rw-r--r--   0 praseetha   (501) staff       (20)     8242 2023-08-29 06:33:57.000000 pyjarsigner-0.2.4/pyjarsigner/jarutil.py
--rw-r--r--   0 praseetha   (501) staff       (20)    25246 2022-12-08 18:23:30.000000 pyjarsigner-0.2.4/pyjarsigner/manifest.py
-drwxr-xr-x   0 praseetha   (501) staff       (20)        0 2023-08-29 06:38:56.147371 pyjarsigner-0.2.4/pyjarsigner.egg-info/
--rw-r--r--   0 praseetha   (501) staff       (20)      989 2023-08-29 06:38:56.000000 pyjarsigner-0.2.4/pyjarsigner.egg-info/PKG-INFO
--rw-r--r--   0 praseetha   (501) staff       (20)      373 2023-08-29 06:38:56.000000 pyjarsigner-0.2.4/pyjarsigner.egg-info/SOURCES.txt
--rw-r--r--   0 praseetha   (501) staff       (20)        1 2023-08-29 06:38:56.000000 pyjarsigner-0.2.4/pyjarsigner.egg-info/dependency_links.txt
--rw-r--r--   0 praseetha   (501) staff       (20)        1 2022-12-08 18:30:32.000000 pyjarsigner-0.2.4/pyjarsigner.egg-info/not-zip-safe
--rw-r--r--   0 praseetha   (501) staff       (20)       17 2023-08-29 06:38:56.000000 pyjarsigner-0.2.4/pyjarsigner.egg-info/requires.txt
--rw-r--r--   0 praseetha   (501) staff       (20)       12 2023-08-29 06:38:56.000000 pyjarsigner-0.2.4/pyjarsigner.egg-info/top_level.txt
--rw-r--r--   0 praseetha   (501) staff       (20)      353 2023-08-29 06:38:56.147907 pyjarsigner-0.2.4/setup.cfg
--rw-r--r--   0 praseetha   (501) staff       (20)     1260 2023-08-29 06:38:49.000000 pyjarsigner-0.2.4/setup.py
+-rw-r--r--   0        0        0     7651 2022-12-08 18:23:30.658546 pyjarsigner-0.2.5/LICENSE
+-rw-r--r--   0        0        0      124 2024-04-17 17:00:13.454009 pyjarsigner-0.2.5/README.md
+-rw-r--r--   0        0        0       53 2022-12-08 18:23:30.659144 pyjarsigner-0.2.5/pyjarsigner/__init__.py
+-rw-r--r--   0        0        0    14935 2022-12-08 18:23:30.659362 pyjarsigner-0.2.5/pyjarsigner/change.py
+-rw-r--r--   0        0        0     4610 2022-12-08 18:23:30.659529 pyjarsigner-0.2.5/pyjarsigner/crypto.py
+-rw-r--r--   0        0        0     5706 2022-12-08 18:23:30.659704 pyjarsigner-0.2.5/pyjarsigner/dirutils.py
+-rw-r--r--   0        0        0     8242 2023-08-29 06:33:57.693330 pyjarsigner-0.2.5/pyjarsigner/jarutil.py
+-rw-r--r--   0        0        0    25246 2022-12-08 18:23:30.660210 pyjarsigner-0.2.5/pyjarsigner/manifest.py
+-rw-r--r--   0        0        0      618 2024-04-17 17:08:10.384752 pyjarsigner-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 pyjarsigner-0.2.5/PKG-INFO
```

### Comparing `pyjarsigner-0.2.4/LICENSE` & `pyjarsigner-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjarsigner-0.2.4/PKG-INFO` & `pyjarsigner-0.2.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pyjarsigner
-Version: 0.2.4
+Version: 0.2.5
 Summary: Pure Python3 implementation to sign JAR and APK files
-Home-page: https://github.com/appknox/pyjarsigner
+License: LGPL-3.0-only
+Keywords: appknox,pyjarsigner,jarsigner,android,apksigner
 Author: Subho Halder
 Author-email: sunny@appknox.com
-License: GNU Lesser General Public License
-Keywords: appknox pyjarsigner jarsigner android apksigner
-Platform: any
-Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-License-File: LICENSE
+Requires-Dist: M2Crypto (==0.38.0)
+Description-Content-Type: text/markdown
+
+# pyjarsigner
+
+Pure Python3 implementation to sign JAR and APK files which was inspired and borrowed from python-javatools.
 
-pure Python3 implementation to sign JAR and APK files which was inspired and borrowed from python-javatools
```

### Comparing `pyjarsigner-0.2.4/pyjarsigner/change.py` & `pyjarsigner-0.2.5/pyjarsigner/change.py`

 * *Files identical despite different names*

### Comparing `pyjarsigner-0.2.4/pyjarsigner/crypto.py` & `pyjarsigner-0.2.5/pyjarsigner/crypto.py`

 * *Files identical despite different names*

### Comparing `pyjarsigner-0.2.4/pyjarsigner/dirutils.py` & `pyjarsigner-0.2.5/pyjarsigner/dirutils.py`

 * *Files identical despite different names*

### Comparing `pyjarsigner-0.2.4/pyjarsigner/jarutil.py` & `pyjarsigner-0.2.5/pyjarsigner/jarutil.py`

 * *Files identical despite different names*

### Comparing `pyjarsigner-0.2.4/pyjarsigner/manifest.py` & `pyjarsigner-0.2.5/pyjarsigner/manifest.py`

 * *Files identical despite different names*

