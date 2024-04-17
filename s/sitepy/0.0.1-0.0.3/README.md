# Comparing `tmp/sitepy-0.0.1.tar.gz` & `tmp/sitepy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitepy-0.0.1.tar", last modified: Wed Apr 17 17:48:28 2024, max compression
+gzip compressed data, was "sitepy-0.0.3.tar", last modified: Wed Apr 17 17:57:48 2024, max compression
```

## Comparing `sitepy-0.0.1.tar` & `sitepy-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 17:48:28.248852 sitepy-0.0.1/
--rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 17:48:28.248110 sitepy-0.0.1/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-17 17:48:28.249079 sitepy-0.0.1/setup.cfg
--rw-r--r--   0 lewis-family   (501) staff       (20)     1028 2024-04-17 17:48:22.000000 sitepy-0.0.1/setup.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 17:48:28.244937 sitepy-0.0.1/sitepy/
--rw-r--r--   0 lewis-family   (501) staff       (20)       13 2024-04-17 17:33:26.000000 sitepy-0.0.1/sitepy/__init__.py
--rw-r--r--   0 lewis-family   (501) staff       (20)     2923 2024-04-17 17:28:06.000000 sitepy-0.0.1/sitepy/sitepy.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 17:48:28.247485 sitepy-0.0.1/sitepy.egg-info/
--rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 17:48:28.000000 sitepy-0.0.1/sitepy.egg-info/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      164 2024-04-17 17:48:28.000000 sitepy-0.0.1/sitepy.egg-info/SOURCES.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-17 17:48:28.000000 sitepy-0.0.1/sitepy.egg-info/dependency_links.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-04-17 17:48:28.000000 sitepy-0.0.1/sitepy.egg-info/top_level.txt
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 17:57:48.517286 sitepy-0.0.3/
+-rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 17:57:48.516367 sitepy-0.0.3/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-17 17:57:48.517599 sitepy-0.0.3/setup.cfg
+-rw-r--r--   0 lewis-family   (501) staff       (20)     1028 2024-04-17 17:56:39.000000 sitepy-0.0.3/setup.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 17:57:48.513395 sitepy-0.0.3/sitepy/
+-rw-r--r--   0 lewis-family   (501) staff       (20)       18 2024-04-17 17:54:48.000000 sitepy-0.0.3/sitepy/__init__.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2784 2024-04-17 17:53:10.000000 sitepy-0.0.3/sitepy/sitepy0_0_2.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 17:57:48.515815 sitepy-0.0.3/sitepy.egg-info/
+-rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 17:57:48.000000 sitepy-0.0.3/sitepy.egg-info/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      169 2024-04-17 17:57:48.000000 sitepy-0.0.3/sitepy.egg-info/SOURCES.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-17 17:57:48.000000 sitepy-0.0.3/sitepy.egg-info/dependency_links.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-04-17 17:57:48.000000 sitepy-0.0.3/sitepy.egg-info/top_level.txt
```

### Comparing `sitepy-0.0.1/PKG-INFO` & `sitepy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.0.1
+Version: 0.0.3
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sitepy-0.0.1/setup.py` & `sitepy-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sitepy',
-    version='0.0.1',
+    version='0.0.3',
     description='A simple web framework.',
     author='WolfTheDev',
     author_email='wolfthedev@gmail.com',
     url='https://github.com/WolfTheDeveloper/sitepy',
     packages=find_packages(),
     long_description=open('sitepy/README.md').read(),
     long_description_content_type='text/markdown',  # Add this line
```

### Comparing `sitepy-0.0.1/sitepy/sitepy.py` & `sitepy-0.0.3/sitepy/sitepy0_0_2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from urllib.parse import parse_qs
 from wsgiref.simple_server import make_server
 import inspect
 
-class sitepy:
+class SitePy:
     def __init__(self, static_dir='static'):
         self.routes = {}
         self.middleware = [self.logger_middleware]
         self.static_dir = static_dir
 
     def route(self, path, methods=['GET']):
         def wrapper(handler):
@@ -67,16 +67,7 @@
         try:
             server = make_server(host, port, self)
             print(f'Serving on {host}:{port}')
             server.serve_forever()
         except KeyboardInterrupt:
             print('\nServer shutting down...')
             server.server_close()
-
-app = sitepy()
-
-@app.route("/", methods=['GET', 'POST'])
-def index():
-    return "Hello, World!"
-
-if __name__ == "__main__":
-    app.run()
```

### Comparing `sitepy-0.0.1/sitepy.egg-info/PKG-INFO` & `sitepy-0.0.3/sitepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.0.1
+Version: 0.0.3
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

