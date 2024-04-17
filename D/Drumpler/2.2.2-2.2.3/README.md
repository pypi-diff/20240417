# Comparing `tmp/drumpler-2.2.2.tar.gz` & `tmp/drumpler-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler-2.2.2.tar", last modified: Tue Apr 16 23:55:38 2024, max compression
+gzip compressed data, was "drumpler-2.2.3.tar", last modified: Wed Apr 17 17:13:33 2024, max compression
```

## Comparing `drumpler-2.2.2.tar` & `drumpler-2.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 23:55:38.131598 drumpler-2.2.2/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 23:55:38.130297 drumpler-2.2.2/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4153 2024-04-16 23:55:38.000000 drumpler-2.2.2/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      355 2024-04-16 23:55:38.000000 drumpler-2.2.2/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 23:55:38.000000 drumpler-2.2.2/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       64 2024-04-16 23:55:38.000000 drumpler-2.2.2/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 23:55:38.000000 drumpler-2.2.2/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.2/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4153 2024-04-16 23:55:38.131018 drumpler-2.2.2/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.2/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 23:55:38.128574 drumpler-2.2.2/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-16 18:54:33.000000 drumpler-2.2.2/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      738 2024-04-16 19:59:55.000000 drumpler-2.2.2/drumpler/config.py
--rw-r--r--   0 Karel      (503) staff       (20)    10186 2024-04-16 23:55:11.000000 drumpler-2.2.2/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)       69 2024-04-16 18:54:36.000000 drumpler-2.2.2/drumpler/sql_base.py
--rw-r--r--   0 Karel      (503) staff       (20)      497 2024-04-16 18:54:38.000000 drumpler-2.2.2/drumpler/sql_event.py
--rw-r--r--   0 Karel      (503) staff       (20)      710 2024-04-16 18:54:37.000000 drumpler-2.2.2/drumpler/sql_job.py
--rw-r--r--   0 Karel      (503) staff       (20)      579 2024-04-16 21:42:49.000000 drumpler-2.2.2/drumpler/sql_request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 23:55:38.131709 drumpler-2.2.2/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      783 2024-04-16 23:55:25.000000 drumpler-2.2.2/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 23:55:38.129469 drumpler-2.2.2/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.2/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:13:33.399368 drumpler-2.2.3/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:13:33.398133 drumpler-2.2.3/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-17 17:13:33.000000 drumpler-2.2.3/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      355 2024-04-17 17:13:33.000000 drumpler-2.2.3/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-17 17:13:33.000000 drumpler-2.2.3/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       71 2024-04-17 17:13:33.000000 drumpler-2.2.3/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-17 17:13:33.000000 drumpler-2.2.3/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.3/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-17 17:13:33.398803 drumpler-2.2.3/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.3/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:13:33.396296 drumpler-2.2.3/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-16 18:54:33.000000 drumpler-2.2.3/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      738 2024-04-16 19:59:55.000000 drumpler-2.2.3/drumpler/config.py
+-rw-r--r--   0 Karel      (503) staff       (20)    10582 2024-04-17 17:12:50.000000 drumpler-2.2.3/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)      100 2024-04-17 16:55:13.000000 drumpler-2.2.3/drumpler/sql_base.py
+-rw-r--r--   0 Karel      (503) staff       (20)      331 2024-04-17 16:56:03.000000 drumpler-2.2.3/drumpler/sql_event.py
+-rw-r--r--   0 Karel      (503) staff       (20)      602 2024-04-17 16:55:48.000000 drumpler-2.2.3/drumpler/sql_job.py
+-rw-r--r--   0 Karel      (503) staff       (20)      508 2024-04-17 16:55:19.000000 drumpler-2.2.3/drumpler/sql_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-17 17:13:33.399483 drumpler-2.2.3/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      800 2024-04-17 17:13:13.000000 drumpler-2.2.3/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:13:33.397303 drumpler-2.2.3/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.3/test/test_drumpler.py
```

### Comparing `drumpler-2.2.2/Drumpler.egg-info/PKG-INFO` & `drumpler-2.2.3/Drumpler.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.2
+Version: 2.2.3
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask
 Requires-Dist: python-dotenv
 Requires-Dist: SQLAlchemy
 Requires-Dist: Flask_SQLAlchemy
 Requires-Dist: psycopg2-binary
+Requires-Dist: psutil
 
 
 # `Drumpler`
 
 `Drumpler` is a general-purpose application designed to facilitate efficient workflow automation through RESTful API interactions and job processing. Built on Flask and SQLAlchemy, this application serves as a robust backend for capturing, storing, and processing HTTP requests in a scalable manner. The application is split into two main components: `drumpler.py` for handling RESTful API requests and `mammoth.py` for querying the API and processing jobs asynchronously.
 
 # High Level Overview
```

### Comparing `drumpler-2.2.2/LICENSE` & `drumpler-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.2/PKG-INFO` & `drumpler-2.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.2
+Version: 2.2.3
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask
 Requires-Dist: python-dotenv
 Requires-Dist: SQLAlchemy
 Requires-Dist: Flask_SQLAlchemy
 Requires-Dist: psycopg2-binary
+Requires-Dist: psutil
 
 
 # `Drumpler`
 
 `Drumpler` is a general-purpose application designed to facilitate efficient workflow automation through RESTful API interactions and job processing. Built on Flask and SQLAlchemy, this application serves as a robust backend for capturing, storing, and processing HTTP requests in a scalable manner. The application is split into two main components: `drumpler.py` for handling RESTful API requests and `mammoth.py` for querying the API and processing jobs asynchronously.
 
 # High Level Overview
```

### Comparing `drumpler-2.2.2/README.md` & `drumpler-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.2/drumpler/config.py` & `drumpler-2.2.3/drumpler/config.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.2/drumpler/drumpler.py` & `drumpler-2.2.3/drumpler/drumpler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,54 @@
-# drumpler.py
 import os
 import json
 import sys
+import psutil
 from flask import Flask, request, jsonify
-from flask_sqlalchemy import SQLAlchemy
 from .config import Config
-from .sql_base import Base  # Import the Base declarative class directly
+from .sql_base import db, init_app  # Import db and the initialization function
 from .sql_request import SqlRequest
 from .sql_job import SqlJob
 from .sql_event import SqlEvent
 
 app = Flask(__name__)
-db = SQLAlchemy()
+app.config['SQLALCHEMY_DATABASE_URI'] = Config.DATABASE_URI
+app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
+init_app(app)  # Initialize SQLAlchemy with the Flask app
 
 class Drumpler:
     def __init__(self):
         self.app = app  # Use the global app instance
         self.__init_env()
         self.__init_config()
         self.__init_db()
         self.__setup_routes()
 
     def __init_config(self):
-        self.app.config['SQLALCHEMY_DATABASE_URI'] = Config.DATABASE_URI
-        self.app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
-        self.app.config['SQLALCHEMY_POOL_SIZE'] = 10
-        self.app.config['SQLALCHEMY_MAX_OVERFLOW'] = 5
-        self.app.config['SQLALCHEMY_POOL_TIMEOUT'] = 30
-        self.app.config['SQLALCHEMY_POOL_RECYCLE'] = 1800
+        cpu_cores = psutil.cpu_count()
+        total_memory_gb = psutil.virtual_memory().total / (1024 ** 3)
+
+        # Example dynamic settings based on system resources
+        pool_size = max(10, cpu_cores * 2)  # Starting at 10, increasing with more cores
+        max_overflow = max(5, int(pool_size * 0.5))  # 50% of pool_size
+        pool_timeout = 30  # Static setting, can adjust if needed
+        pool_recycle = 1800  # Static setting, can adjust if needed
+
+        self.app.config['SQLALCHEMY_POOL_SIZE'] = pool_size
+        self.app.config['SQLALCHEMY_MAX_OVERFLOW'] = max_overflow
+        self.app.config['SQLALCHEMY_POOL_TIMEOUT'] = pool_timeout
+        self.app.config['SQLALCHEMY_POOL_RECYCLE'] = pool_recycle
+
         self.AUTHORIZATION_KEY = Config.AUTHORIZATION_KEY
         self.host = Config.DRUMPLER_HOST
         self.port = Config.DRUMPLER_PORT
         self.debug = Config.DRUMPLER_DEBUG
 
     def __init_db(self):
-        db.init_app(self.app)  # Initialize SQLAlchemy with app
         with self.app.app_context():
-            Base.metadata.create_all(db.engine)  # Create tables from the same Base used in model definitions
+            db.create_all()  # Create tables based on the models if they don't exist
 
     def __setup_routes(self):
         self.app.add_url_rule('/', view_func=self.hello_world, methods=['GET'])
         self.app.add_url_rule('/request', view_func=self.__process_request, methods=['POST'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__get_request, methods=['GET'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__update_request, methods=['PUT'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__delete_request, methods=['DELETE'])
```

### Comparing `drumpler-2.2.2/setup.py` & `drumpler-2.2.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='2.2.2',
+    version='2.2.3',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
@@ -18,9 +18,10 @@
     python_requires='>=3.6',
     install_requires=[
         'Flask',
         'python-dotenv',
         'SQLAlchemy',
         'Flask_SQLAlchemy',
         'psycopg2-binary',
+        'psutil'
     ],
 )
```

### Comparing `drumpler-2.2.2/test/test_drumpler.py` & `drumpler-2.2.3/test/test_drumpler.py`

 * *Files identical despite different names*

