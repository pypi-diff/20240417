# Comparing `tmp/algorin_cli-0.0.1.tar.gz` & `tmp/algorin-cli-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algorin_cli-0.0.1.tar", last modified: Wed Apr 17 21:02:33 2024, max compression
+gzip compressed data, was "algorin-cli-0.1.tar", last modified: Wed Apr 17 21:46:52 2024, max compression
```

## Comparing `algorin_cli-0.0.1.tar` & `algorin-cli-0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:02:33.789106 algorin_cli-0.0.1/
--rw-r--r--   0 1064331    (502) staff       (20)     7653 2024-04-17 21:02:33.787983 algorin_cli-0.0.1/PKG-INFO
--rw-r--r--   0 1064331    (502) staff       (20)       33 2024-04-17 19:58:47.000000 algorin_cli-0.0.1/README.md
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:02:33.750984 algorin_cli-0.0.1/algorin/
--rw-r--r--   0 1064331    (502) staff       (20)      425 2024-04-17 20:22:58.000000 algorin_cli-0.0.1/algorin/__init__.py
--rw-r--r--   0 1064331    (502) staff       (20)     1021 2024-04-17 18:41:07.000000 algorin_cli-0.0.1/algorin/chatbot.py
--rw-r--r--   0 1064331    (502) staff       (20)     1021 2024-04-17 18:41:17.000000 algorin_cli-0.0.1/algorin/file_extractor.py
--rw-r--r--   0 1064331    (502) staff       (20)     1834 2024-04-17 18:41:13.000000 algorin_cli-0.0.1/algorin/main.py
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:02:33.770443 algorin_cli-0.0.1/algorin_cli.egg-info/
--rw-r--r--   0 1064331    (502) staff       (20)     7653 2024-04-17 21:02:33.000000 algorin_cli-0.0.1/algorin_cli.egg-info/PKG-INFO
--rw-r--r--   0 1064331    (502) staff       (20)      361 2024-04-17 21:02:33.000000 algorin_cli-0.0.1/algorin_cli.egg-info/SOURCES.txt
--rw-r--r--   0 1064331    (502) staff       (20)        1 2024-04-17 21:02:33.000000 algorin_cli-0.0.1/algorin_cli.egg-info/dependency_links.txt
--rw-r--r--   0 1064331    (502) staff       (20)     3831 2024-04-17 21:02:33.000000 algorin_cli-0.0.1/algorin_cli.egg-info/requires.txt
--rw-r--r--   0 1064331    (502) staff       (20)       14 2024-04-17 21:02:33.000000 algorin_cli-0.0.1/algorin_cli.egg-info/top_level.txt
--rw-r--r--   0 1064331    (502) staff       (20)       38 2024-04-17 21:02:33.789215 algorin_cli-0.0.1/setup.cfg
--rw-r--r--   0 1064331    (502) staff       (20)      705 2024-04-17 21:02:20.000000 algorin_cli-0.0.1/setup.py
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:02:33.778802 algorin_cli-0.0.1/tests/
--rw-r--r--   0 1064331    (502) staff       (20)      178 2024-04-17 20:21:38.000000 algorin_cli-0.0.1/tests/__init__.py
--rw-r--r--   0 1064331    (502) staff       (20)      546 2024-04-17 20:22:40.000000 algorin_cli-0.0.1/tests/test_chatbot.py
--rw-r--r--   0 1064331    (502) staff       (20)      769 2024-04-17 20:22:47.000000 algorin_cli-0.0.1/tests/test_file_extractor.py
--rw-r--r--   0 1064331    (502) staff       (20)      631 2024-04-17 20:22:52.000000 algorin_cli-0.0.1/tests/test_main.py
+drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:46:52.948705 algorin-cli-0.1/
+-rw-r--r--   0 1064331    (502) staff       (20)     7651 2024-04-17 21:46:52.948022 algorin-cli-0.1/PKG-INFO
+-rw-r--r--   0 1064331    (502) staff       (20)       33 2024-04-17 19:58:47.000000 algorin-cli-0.1/README.md
+drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:46:52.927391 algorin-cli-0.1/algorin-cli/
+-rw-r--r--   0 1064331    (502) staff       (20)      425 2024-04-17 20:22:58.000000 algorin-cli-0.1/algorin-cli/__init__.py
+-rw-r--r--   0 1064331    (502) staff       (20)     1021 2024-04-17 18:41:07.000000 algorin-cli-0.1/algorin-cli/chatbot.py
+-rw-r--r--   0 1064331    (502) staff       (20)     1021 2024-04-17 18:41:17.000000 algorin-cli-0.1/algorin-cli/file_extractor.py
+-rw-r--r--   0 1064331    (502) staff       (20)     1834 2024-04-17 18:41:13.000000 algorin-cli-0.1/algorin-cli/main.py
+drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:46:52.931923 algorin-cli-0.1/algorin_cli.egg-info/
+-rw-r--r--   0 1064331    (502) staff       (20)     7651 2024-04-17 21:46:52.000000 algorin-cli-0.1/algorin_cli.egg-info/PKG-INFO
+-rw-r--r--   0 1064331    (502) staff       (20)      377 2024-04-17 21:46:52.000000 algorin-cli-0.1/algorin_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 1064331    (502) staff       (20)        1 2024-04-17 21:46:52.000000 algorin-cli-0.1/algorin_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 1064331    (502) staff       (20)     3831 2024-04-17 21:46:52.000000 algorin-cli-0.1/algorin_cli.egg-info/requires.txt
+-rw-r--r--   0 1064331    (502) staff       (20)       18 2024-04-17 21:46:52.000000 algorin-cli-0.1/algorin_cli.egg-info/top_level.txt
+-rw-r--r--   0 1064331    (502) staff       (20)       38 2024-04-17 21:46:52.948799 algorin-cli-0.1/setup.cfg
+-rw-r--r--   0 1064331    (502) staff       (20)      703 2024-04-17 21:46:28.000000 algorin-cli-0.1/setup.py
+drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:46:52.939440 algorin-cli-0.1/tests/
+-rw-r--r--   0 1064331    (502) staff       (20)      178 2024-04-17 20:21:38.000000 algorin-cli-0.1/tests/__init__.py
+-rw-r--r--   0 1064331    (502) staff       (20)      546 2024-04-17 20:22:40.000000 algorin-cli-0.1/tests/test_chatbot.py
+-rw-r--r--   0 1064331    (502) staff       (20)      769 2024-04-17 20:22:47.000000 algorin-cli-0.1/tests/test_file_extractor.py
+-rw-r--r--   0 1064331    (502) staff       (20)      631 2024-04-17 20:22:52.000000 algorin-cli-0.1/tests/test_main.py
```

### Comparing `algorin_cli-0.0.1/PKG-INFO` & `algorin-cli-0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: algorin_cli
-Version: 0.0.1
+Name: algorin-cli
+Version: 0.1
 Summary: Acceso a GPT-3 y procesamiento de documentos desde la línea de comandos.
 Home-page: https://github.com/Jorge-Polanco-Roque/bot_cli
 Author: JP
 Author-email: jorge.polanco@itesm.mx
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `algorin_cli-0.0.1/algorin/chatbot.py` & `algorin-cli-0.1/algorin-cli/chatbot.py`

 * *Files identical despite different names*

### Comparing `algorin_cli-0.0.1/algorin/file_extractor.py` & `algorin-cli-0.1/algorin-cli/file_extractor.py`

 * *Files identical despite different names*

### Comparing `algorin_cli-0.0.1/algorin/main.py` & `algorin-cli-0.1/algorin-cli/main.py`

 * *Files identical despite different names*

### Comparing `algorin_cli-0.0.1/algorin_cli.egg-info/PKG-INFO` & `algorin-cli-0.1/algorin_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algorin-cli
-Version: 0.0.1
+Version: 0.1
 Summary: Acceso a GPT-3 y procesamiento de documentos desde la línea de comandos.
 Home-page: https://github.com/Jorge-Polanco-Roque/bot_cli
 Author: JP
 Author-email: jorge.polanco@itesm.mx
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `algorin_cli-0.0.1/algorin_cli.egg-info/requires.txt` & `algorin-cli-0.1/algorin_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `algorin_cli-0.0.1/setup.py` & `algorin-cli-0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='algorin_cli',
-    version='0.0.1',
+    name='algorin-cli',
+    version='0.1',
     author='JP',
     author_email='jorge.polanco@itesm.mx',
     packages=find_packages(),
     install_requires=[line.strip() for line in open("requirements.txt", "r")],
     description='Acceso a GPT-3 y procesamiento de documentos desde la línea de comandos.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `algorin_cli-0.0.1/tests/test_chatbot.py` & `algorin-cli-0.1/tests/test_chatbot.py`

 * *Files identical despite different names*

### Comparing `algorin_cli-0.0.1/tests/test_file_extractor.py` & `algorin-cli-0.1/tests/test_file_extractor.py`

 * *Files identical despite different names*

### Comparing `algorin_cli-0.0.1/tests/test_main.py` & `algorin-cli-0.1/tests/test_main.py`

 * *Files identical despite different names*

