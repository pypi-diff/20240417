# Comparing `tmp/paquetes_franaser1985-5.0.tar.gz` & `tmp/paquetes_franaser1985-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paquetes_franaser1985-5.0.tar", last modified: Wed Apr 17 15:48:39 2024, max compression
+gzip compressed data, was "paquetes_franaser1985-6.0.tar", last modified: Wed Apr 17 16:02:28 2024, max compression
```

## Comparing `paquetes_franaser1985-5.0.tar` & `paquetes_franaser1985-6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-17 15:48:39.550716 paquetes_franaser1985-5.0/
--rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)     1082 2024-04-17 15:08:11.000000 paquetes_franaser1985-5.0/LICENSE
--rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)       58 2024-04-17 15:08:37.000000 paquetes_franaser1985-5.0/MANIFEST.in
--rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)     1096 2024-04-17 15:48:39.547793 paquetes_franaser1985-5.0/PKG-INFO
-drwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-17 15:48:39.512997 paquetes_franaser1985-5.0/Paquetes/
-drwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-17 15:48:39.520578 paquetes_franaser1985-5.0/Paquetes/Adios/
--rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)      151 2024-03-04 21:44:51.000000 paquetes_franaser1985-5.0/Paquetes/Adios/__init__.py
--rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)      187 2024-03-04 21:47:07.000000 paquetes_franaser1985-5.0/Paquetes/Adios/despedidas.py
-drwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-17 15:48:39.524073 paquetes_franaser1985-5.0/Paquetes/Hola/
--rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)      150 2024-03-04 21:43:53.000000 paquetes_franaser1985-5.0/Paquetes/Hola/__init__.py
--rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)      740 2024-04-16 22:45:56.000000 paquetes_franaser1985-5.0/Paquetes/Hola/test3.py
--rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)      151 2024-03-04 21:41:52.000000 paquetes_franaser1985-5.0/Paquetes/__init__.py
-drwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-17 15:48:39.542903 paquetes_franaser1985-5.0/Paquetes_franaser1985.egg-info/
--rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)     1096 2024-04-17 15:48:39.000000 paquetes_franaser1985-5.0/Paquetes_franaser1985.egg-info/PKG-INFO
--rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)      462 2024-04-17 15:48:39.000000 paquetes_franaser1985-5.0/Paquetes_franaser1985.egg-info/SOURCES.txt
--rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)        1 2024-04-17 15:48:39.000000 paquetes_franaser1985-5.0/Paquetes_franaser1985.egg-info/dependency_links.txt
--rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)       14 2024-04-17 15:48:39.000000 paquetes_franaser1985-5.0/Paquetes_franaser1985.egg-info/requires.txt
--rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)       15 2024-04-17 15:48:39.000000 paquetes_franaser1985-5.0/Paquetes_franaser1985.egg-info/top_level.txt
--rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)       81 2024-04-17 15:02:34.000000 paquetes_franaser1985-5.0/README.md
--rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)       13 2024-04-16 22:36:43.000000 paquetes_franaser1985-5.0/requirements.txt
--rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)       38 2024-04-17 15:48:39.551120 paquetes_franaser1985-5.0/setup.cfg
--rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)     1693 2024-04-17 15:48:29.000000 paquetes_franaser1985-5.0/setup.py
-drwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-17 15:48:39.539652 paquetes_franaser1985-5.0/tests/
--rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-16 22:56:23.000000 paquetes_franaser1985-5.0/tests/__init__.py
--rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-16 22:49:58.000000 paquetes_franaser1985-5.0/tests/test_adios.py
--rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)      285 2024-04-16 22:57:49.000000 paquetes_franaser1985-5.0/tests/test_hola.py
+drwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-17 16:02:28.026841 paquetes_franaser1985-6.0/
+-rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)     1082 2024-04-17 15:08:11.000000 paquetes_franaser1985-6.0/LICENSE
+-rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)       58 2024-04-17 15:08:37.000000 paquetes_franaser1985-6.0/MANIFEST.in
+-rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)     1096 2024-04-17 16:02:28.025225 paquetes_franaser1985-6.0/PKG-INFO
+drwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-17 16:02:27.995021 paquetes_franaser1985-6.0/Paquetes/
+drwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-17 16:02:27.997537 paquetes_franaser1985-6.0/Paquetes/Adios/
+-rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)      151 2024-03-04 21:44:51.000000 paquetes_franaser1985-6.0/Paquetes/Adios/__init__.py
+-rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)      187 2024-03-04 21:47:07.000000 paquetes_franaser1985-6.0/Paquetes/Adios/despedidas.py
+drwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-17 16:02:28.002639 paquetes_franaser1985-6.0/Paquetes/Hola/
+-rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)      150 2024-03-04 21:43:53.000000 paquetes_franaser1985-6.0/Paquetes/Hola/__init__.py
+-rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)      750 2024-04-17 16:01:22.000000 paquetes_franaser1985-6.0/Paquetes/Hola/test3.py
+-rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)      151 2024-03-04 21:41:52.000000 paquetes_franaser1985-6.0/Paquetes/__init__.py
+drwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-17 16:02:28.021512 paquetes_franaser1985-6.0/Paquetes_franaser1985.egg-info/
+-rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)     1096 2024-04-17 16:02:27.000000 paquetes_franaser1985-6.0/Paquetes_franaser1985.egg-info/PKG-INFO
+-rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)      462 2024-04-17 16:02:27.000000 paquetes_franaser1985-6.0/Paquetes_franaser1985.egg-info/SOURCES.txt
+-rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)        1 2024-04-17 16:02:27.000000 paquetes_franaser1985-6.0/Paquetes_franaser1985.egg-info/dependency_links.txt
+-rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)       14 2024-04-17 16:02:27.000000 paquetes_franaser1985-6.0/Paquetes_franaser1985.egg-info/requires.txt
+-rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)       15 2024-04-17 16:02:27.000000 paquetes_franaser1985-6.0/Paquetes_franaser1985.egg-info/top_level.txt
+-rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)       81 2024-04-17 15:02:34.000000 paquetes_franaser1985-6.0/README.md
+-rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)       13 2024-04-16 22:36:43.000000 paquetes_franaser1985-6.0/requirements.txt
+-rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)       38 2024-04-17 16:02:28.027111 paquetes_franaser1985-6.0/setup.cfg
+-rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)     1693 2024-04-17 16:01:28.000000 paquetes_franaser1985-6.0/setup.py
+drwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-17 16:02:28.015211 paquetes_franaser1985-6.0/tests/
+-rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-16 22:56:23.000000 paquetes_franaser1985-6.0/tests/__init__.py
+-rw-r--r--   0 franchesconaranjoserrano   (501) staff       (20)        0 2024-04-16 22:49:58.000000 paquetes_franaser1985-6.0/tests/test_adios.py
+-rwxr-xr-x   0 franchesconaranjoserrano   (501) staff       (20)      285 2024-04-16 22:57:49.000000 paquetes_franaser1985-6.0/tests/test_hola.py
```

### Comparing `paquetes_franaser1985-5.0/LICENSE` & `paquetes_franaser1985-6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paquetes_franaser1985-5.0/PKG-INFO` & `paquetes_franaser1985-6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Paquetes-franaser1985
-Version: 5.0
+Version: 6.0
 Summary: Un paquete para hola y adios
 Home-page: https://www.hektor.dev
 Author: Franchesco Naranjo Serrano
 Author-email: franchesco.naranjoserrano@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paquetes_franaser1985-5.0/Paquetes/Hola/test3.py` & `paquetes_franaser1985-6.0/Paquetes/Hola/test3.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 
 def saludar():
     print("Hola, te saludo desde saludos.saludar()")
 
 def prueba():
-    print("Esto es una prueba de la nueva version")
+    print("Esto es una nueva prueba de la nueva version 6.0")
 
 def generar_arrray(numeros):
     return np.arange(numeros)
 
 #print(__name__)
 class Saludo():
```

### Comparing `paquetes_franaser1985-5.0/Paquetes_franaser1985.egg-info/PKG-INFO` & `paquetes_franaser1985-6.0/Paquetes_franaser1985.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Paquetes-franaser1985
-Version: 5.0
+Version: 6.0
 Summary: Un paquete para hola y adios
 Home-page: https://www.hektor.dev
 Author: Franchesco Naranjo Serrano
 Author-email: franchesco.naranjoserrano@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paquetes_franaser1985-5.0/setup.py` & `paquetes_franaser1985-6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 setup(
       #nombre_del_paquete
       name='Paquetes-franaser1985',
       #versión_del_paquete
-      version='5.0',
+      version='6.0',
       #breve descripción
       description='Un paquete para hola y adios',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       author='Franchesco Naranjo Serrano',
       author_email='franchesco.naranjoserrano@gmail.com',
       url='https://www.hektor.dev',
```

