# Comparing `tmp/drumpler-2.2.3.tar.gz` & `tmp/drumpler-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler-2.2.3.tar", last modified: Wed Apr 17 17:13:33 2024, max compression
+gzip compressed data, was "drumpler-2.2.4.tar", last modified: Wed Apr 17 18:47:10 2024, max compression
```

## Comparing `drumpler-2.2.3.tar` & `drumpler-2.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:13:33.399368 drumpler-2.2.3/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:13:33.398133 drumpler-2.2.3/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-17 17:13:33.000000 drumpler-2.2.3/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      355 2024-04-17 17:13:33.000000 drumpler-2.2.3/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-17 17:13:33.000000 drumpler-2.2.3/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       71 2024-04-17 17:13:33.000000 drumpler-2.2.3/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-17 17:13:33.000000 drumpler-2.2.3/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.3/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-17 17:13:33.398803 drumpler-2.2.3/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.3/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:13:33.396296 drumpler-2.2.3/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-16 18:54:33.000000 drumpler-2.2.3/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      738 2024-04-16 19:59:55.000000 drumpler-2.2.3/drumpler/config.py
--rw-r--r--   0 Karel      (503) staff       (20)    10582 2024-04-17 17:12:50.000000 drumpler-2.2.3/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)      100 2024-04-17 16:55:13.000000 drumpler-2.2.3/drumpler/sql_base.py
--rw-r--r--   0 Karel      (503) staff       (20)      331 2024-04-17 16:56:03.000000 drumpler-2.2.3/drumpler/sql_event.py
--rw-r--r--   0 Karel      (503) staff       (20)      602 2024-04-17 16:55:48.000000 drumpler-2.2.3/drumpler/sql_job.py
--rw-r--r--   0 Karel      (503) staff       (20)      508 2024-04-17 16:55:19.000000 drumpler-2.2.3/drumpler/sql_request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-17 17:13:33.399483 drumpler-2.2.3/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      800 2024-04-17 17:13:13.000000 drumpler-2.2.3/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:13:33.397303 drumpler-2.2.3/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.3/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 18:47:10.569818 drumpler-2.2.4/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 18:47:10.567684 drumpler-2.2.4/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-17 18:47:10.000000 drumpler-2.2.4/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      355 2024-04-17 18:47:10.000000 drumpler-2.2.4/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-17 18:47:10.000000 drumpler-2.2.4/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       71 2024-04-17 18:47:10.000000 drumpler-2.2.4/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-17 18:47:10.000000 drumpler-2.2.4/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.4/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-17 18:47:10.568738 drumpler-2.2.4/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.4/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 18:47:10.566115 drumpler-2.2.4/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-16 18:54:33.000000 drumpler-2.2.4/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      738 2024-04-16 19:59:55.000000 drumpler-2.2.4/drumpler/config.py
+-rw-r--r--   0 Karel      (503) staff       (20)    10588 2024-04-17 18:46:46.000000 drumpler-2.2.4/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)      100 2024-04-17 16:55:13.000000 drumpler-2.2.4/drumpler/sql_base.py
+-rw-r--r--   0 Karel      (503) staff       (20)      331 2024-04-17 16:56:03.000000 drumpler-2.2.4/drumpler/sql_event.py
+-rw-r--r--   0 Karel      (503) staff       (20)      602 2024-04-17 16:55:48.000000 drumpler-2.2.4/drumpler/sql_job.py
+-rw-r--r--   0 Karel      (503) staff       (20)      508 2024-04-17 16:55:19.000000 drumpler-2.2.4/drumpler/sql_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-17 18:47:10.570003 drumpler-2.2.4/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      800 2024-04-17 18:46:58.000000 drumpler-2.2.4/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 18:47:10.566711 drumpler-2.2.4/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.4/test/test_drumpler.py
```

### Comparing `drumpler-2.2.3/Drumpler.egg-info/PKG-INFO` & `drumpler-2.2.4/Drumpler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.3
+Version: 2.2.4
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.3/LICENSE` & `drumpler-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.3/PKG-INFO` & `drumpler-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.3
+Version: 2.2.4
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.3/README.md` & `drumpler-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.3/drumpler/config.py` & `drumpler-2.2.4/drumpler/config.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.3/drumpler/drumpler.py` & `drumpler-2.2.4/drumpler/drumpler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import json
 import sys
 import psutil
+from datetime import datetime, timezone
 from flask import Flask, request, jsonify
 from .config import Config
 from .sql_base import db, init_app  # Import db and the initialization function
 from .sql_request import SqlRequest
 from .sql_job import SqlJob
 from .sql_event import SqlEvent
 
@@ -135,15 +136,21 @@
             print(f"Exception occurred: {str(e)}")
             return jsonify({"message": "Error occurred."}), 500
         
     def __update_job_status(self, job_id):
         with self.app.app_context():  # Ensure the application context is being used
             job = db.session.query(SqlJob).get(job_id)  # Use db.session.query
             if job:
-                job.status = request.json.get('status', job.status)
+                new_status = request.json.get('status')
+                job.status = new_status if new_status else job.status
+                job.modified_date = datetime.now(timezone.utc)  # Update the modified date to current timestamp
+
+                if job.status == "Completed":
+                    job.finished_date = datetime.now(timezone.utc)  # Set finished date if job is completed
+
                 db.session.commit()
                 return jsonify({"message": "Job status updated successfully"}), 200
             else:
                 return jsonify({"message": "Job not found"}), 404
 
     def __mark_request_as_handled(self, job_id):
         with self.app.app_context():  # Ensure the application context is being used
@@ -193,23 +200,14 @@
         if request_entry:
             db.session.delete(request_entry)
             db.session.commit()
             return jsonify({"message": "Request deleted successfully"}), 200
         else:
             return jsonify({"message": "Request not found"}), 404
 
-    def __create_job(self):
-        if not self.__authorize_request():
-            return jsonify({"message": "Unauthorized access"}), 401
-        data = request.get_json()
-        new_job = SqlJob(request_id=data['request_id'], status='Pending')
-        db.session.add(new_job)
-        db.session.commit()
-        return jsonify({'job_id': new_job.id}), 201
-
     def __update_job(self, job_id):
         if not self.__authorize_request():
             return jsonify({"message": "Unauthorized access"}), 401
         data = request.get_json()
         job = SqlJob.query.get(job_id)
         if job:
             job.status = data.get('status', job.status)
```

### Comparing `drumpler-2.2.3/drumpler/sql_job.py` & `drumpler-2.2.4/drumpler/sql_job.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.3/setup.py` & `drumpler-2.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='2.2.3',
+    version='2.2.4',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `drumpler-2.2.3/test/test_drumpler.py` & `drumpler-2.2.4/test/test_drumpler.py`

 * *Files identical despite different names*

