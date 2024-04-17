# Comparing `tmp/algorin-cli-0.1.tar.gz` & `tmp/algorin-cli-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algorin-cli-0.1.tar", last modified: Wed Apr 17 21:46:52 2024, max compression
+gzip compressed data, was "algorin-cli-0.11.tar", last modified: Wed Apr 17 21:53:56 2024, max compression
```

## Comparing `algorin-cli-0.1.tar` & `algorin-cli-0.11.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:46:52.948705 algorin-cli-0.1/
--rw-r--r--   0 1064331    (502) staff       (20)     7651 2024-04-17 21:46:52.948022 algorin-cli-0.1/PKG-INFO
--rw-r--r--   0 1064331    (502) staff       (20)       33 2024-04-17 19:58:47.000000 algorin-cli-0.1/README.md
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:46:52.927391 algorin-cli-0.1/algorin-cli/
--rw-r--r--   0 1064331    (502) staff       (20)      425 2024-04-17 20:22:58.000000 algorin-cli-0.1/algorin-cli/__init__.py
--rw-r--r--   0 1064331    (502) staff       (20)     1021 2024-04-17 18:41:07.000000 algorin-cli-0.1/algorin-cli/chatbot.py
--rw-r--r--   0 1064331    (502) staff       (20)     1021 2024-04-17 18:41:17.000000 algorin-cli-0.1/algorin-cli/file_extractor.py
--rw-r--r--   0 1064331    (502) staff       (20)     1834 2024-04-17 18:41:13.000000 algorin-cli-0.1/algorin-cli/main.py
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:46:52.931923 algorin-cli-0.1/algorin_cli.egg-info/
--rw-r--r--   0 1064331    (502) staff       (20)     7651 2024-04-17 21:46:52.000000 algorin-cli-0.1/algorin_cli.egg-info/PKG-INFO
--rw-r--r--   0 1064331    (502) staff       (20)      377 2024-04-17 21:46:52.000000 algorin-cli-0.1/algorin_cli.egg-info/SOURCES.txt
--rw-r--r--   0 1064331    (502) staff       (20)        1 2024-04-17 21:46:52.000000 algorin-cli-0.1/algorin_cli.egg-info/dependency_links.txt
--rw-r--r--   0 1064331    (502) staff       (20)     3831 2024-04-17 21:46:52.000000 algorin-cli-0.1/algorin_cli.egg-info/requires.txt
--rw-r--r--   0 1064331    (502) staff       (20)       18 2024-04-17 21:46:52.000000 algorin-cli-0.1/algorin_cli.egg-info/top_level.txt
--rw-r--r--   0 1064331    (502) staff       (20)       38 2024-04-17 21:46:52.948799 algorin-cli-0.1/setup.cfg
--rw-r--r--   0 1064331    (502) staff       (20)      703 2024-04-17 21:46:28.000000 algorin-cli-0.1/setup.py
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:46:52.939440 algorin-cli-0.1/tests/
--rw-r--r--   0 1064331    (502) staff       (20)      178 2024-04-17 20:21:38.000000 algorin-cli-0.1/tests/__init__.py
--rw-r--r--   0 1064331    (502) staff       (20)      546 2024-04-17 20:22:40.000000 algorin-cli-0.1/tests/test_chatbot.py
--rw-r--r--   0 1064331    (502) staff       (20)      769 2024-04-17 20:22:47.000000 algorin-cli-0.1/tests/test_file_extractor.py
--rw-r--r--   0 1064331    (502) staff       (20)      631 2024-04-17 20:22:52.000000 algorin-cli-0.1/tests/test_main.py
+drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:53:56.911582 algorin-cli-0.11/
+-rw-r--r--   0 1064331    (502) staff       (20)     7652 2024-04-17 21:53:56.910498 algorin-cli-0.11/PKG-INFO
+-rw-r--r--   0 1064331    (502) staff       (20)       33 2024-04-17 19:58:47.000000 algorin-cli-0.11/README.md
+drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:53:56.884886 algorin-cli-0.11/algorin-cli/
+-rw-r--r--   0 1064331    (502) staff       (20)      425 2024-04-17 20:22:58.000000 algorin-cli-0.11/algorin-cli/__init__.py
+-rw-r--r--   0 1064331    (502) staff       (20)     1021 2024-04-17 18:41:07.000000 algorin-cli-0.11/algorin-cli/chatbot.py
+-rw-r--r--   0 1064331    (502) staff       (20)     1021 2024-04-17 18:41:17.000000 algorin-cli-0.11/algorin-cli/file_extractor.py
+-rw-r--r--   0 1064331    (502) staff       (20)     1834 2024-04-17 18:41:13.000000 algorin-cli-0.11/algorin-cli/main.py
+drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:53:56.896958 algorin-cli-0.11/algorin_cli.egg-info/
+-rw-r--r--   0 1064331    (502) staff       (20)     7652 2024-04-17 21:53:56.000000 algorin-cli-0.11/algorin_cli.egg-info/PKG-INFO
+-rw-r--r--   0 1064331    (502) staff       (20)      415 2024-04-17 21:53:56.000000 algorin-cli-0.11/algorin_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 1064331    (502) staff       (20)        1 2024-04-17 21:53:56.000000 algorin-cli-0.11/algorin_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 1064331    (502) staff       (20)       58 2024-04-17 21:53:56.000000 algorin-cli-0.11/algorin_cli.egg-info/entry_points.txt
+-rw-r--r--   0 1064331    (502) staff       (20)     3831 2024-04-17 21:53:56.000000 algorin-cli-0.11/algorin_cli.egg-info/requires.txt
+-rw-r--r--   0 1064331    (502) staff       (20)       18 2024-04-17 21:53:56.000000 algorin-cli-0.11/algorin_cli.egg-info/top_level.txt
+-rw-r--r--   0 1064331    (502) staff       (20)       38 2024-04-17 21:53:56.911679 algorin-cli-0.11/setup.cfg
+-rw-r--r--   0 1064331    (502) staff       (20)      882 2024-04-17 21:53:44.000000 algorin-cli-0.11/setup.py
+drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:53:56.902253 algorin-cli-0.11/tests/
+-rw-r--r--   0 1064331    (502) staff       (20)      178 2024-04-17 20:21:38.000000 algorin-cli-0.11/tests/__init__.py
+-rw-r--r--   0 1064331    (502) staff       (20)      546 2024-04-17 20:22:40.000000 algorin-cli-0.11/tests/test_chatbot.py
+-rw-r--r--   0 1064331    (502) staff       (20)      769 2024-04-17 20:22:47.000000 algorin-cli-0.11/tests/test_file_extractor.py
+-rw-r--r--   0 1064331    (502) staff       (20)      631 2024-04-17 20:22:52.000000 algorin-cli-0.11/tests/test_main.py
```

### Comparing `algorin-cli-0.1/PKG-INFO` & `algorin-cli-0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algorin-cli
-Version: 0.1
+Version: 0.11
 Summary: Acceso a GPT-3 y procesamiento de documentos desde la línea de comandos.
 Home-page: https://github.com/Jorge-Polanco-Roque/bot_cli
 Author: JP
 Author-email: jorge.polanco@itesm.mx
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `algorin-cli-0.1/algorin-cli/chatbot.py` & `algorin-cli-0.11/algorin-cli/chatbot.py`

 * *Files identical despite different names*

### Comparing `algorin-cli-0.1/algorin-cli/file_extractor.py` & `algorin-cli-0.11/algorin-cli/file_extractor.py`

 * *Files identical despite different names*

### Comparing `algorin-cli-0.1/algorin-cli/main.py` & `algorin-cli-0.11/algorin-cli/main.py`

 * *Files identical despite different names*

### Comparing `algorin-cli-0.1/algorin_cli.egg-info/PKG-INFO` & `algorin-cli-0.11/algorin_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algorin-cli
-Version: 0.1
+Version: 0.11
 Summary: Acceso a GPT-3 y procesamiento de documentos desde la línea de comandos.
 Home-page: https://github.com/Jorge-Polanco-Roque/bot_cli
 Author: JP
 Author-email: jorge.polanco@itesm.mx
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `algorin-cli-0.1/algorin_cli.egg-info/requires.txt` & `algorin-cli-0.11/algorin_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `algorin-cli-0.1/setup.py` & `algorin-cli-0.11/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='algorin-cli',
-    version='0.1',
+    version='0.11',
     author='JP',
     author_email='jorge.polanco@itesm.mx',
     packages=find_packages(),
-    install_requires=[line.strip() for line in open("requirements.txt", "r")],
+    install_requires=[line.strip() for line in open("requirements.txt", "r").readlines()],
     description='Acceso a GPT-3 y procesamiento de documentos desde la línea de comandos.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown', 
     url='https://github.com/Jorge-Polanco-Roque/bot_cli',
     license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    entry_points={
+        'console_scripts': [
+            'algorin-cli=algorincli.main:main_menu',  # Asegúrate de que el path aquí es correcto
+        ],
+    },
 )
```

### Comparing `algorin-cli-0.1/tests/test_chatbot.py` & `algorin-cli-0.11/tests/test_chatbot.py`

 * *Files identical despite different names*

### Comparing `algorin-cli-0.1/tests/test_file_extractor.py` & `algorin-cli-0.11/tests/test_file_extractor.py`

 * *Files identical despite different names*

### Comparing `algorin-cli-0.1/tests/test_main.py` & `algorin-cli-0.11/tests/test_main.py`

 * *Files identical despite different names*

