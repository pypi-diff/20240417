# Comparing `tmp/drumpler-2.2.0.tar.gz` & `tmp/drumpler-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler-2.2.0.tar", last modified: Tue Apr 16 21:45:17 2024, max compression
+gzip compressed data, was "drumpler-2.2.1.tar", last modified: Tue Apr 16 23:34:23 2024, max compression
```

## Comparing `drumpler-2.2.0.tar` & `drumpler-2.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:45:17.645516 drumpler-2.2.0/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:45:17.643841 drumpler-2.2.0/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4153 2024-04-16 21:45:17.000000 drumpler-2.2.0/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      355 2024-04-16 21:45:17.000000 drumpler-2.2.0/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 21:45:17.000000 drumpler-2.2.0/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       64 2024-04-16 21:45:17.000000 drumpler-2.2.0/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 21:45:17.000000 drumpler-2.2.0/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.0/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4153 2024-04-16 21:45:17.644816 drumpler-2.2.0/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.0/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:45:17.642430 drumpler-2.2.0/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-16 18:54:33.000000 drumpler-2.2.0/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      738 2024-04-16 19:59:55.000000 drumpler-2.2.0/drumpler/config.py
--rw-r--r--   0 Karel      (503) staff       (20)    10073 2024-04-16 21:44:39.000000 drumpler-2.2.0/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)       69 2024-04-16 18:54:36.000000 drumpler-2.2.0/drumpler/sql_base.py
--rw-r--r--   0 Karel      (503) staff       (20)      497 2024-04-16 18:54:38.000000 drumpler-2.2.0/drumpler/sql_event.py
--rw-r--r--   0 Karel      (503) staff       (20)      710 2024-04-16 18:54:37.000000 drumpler-2.2.0/drumpler/sql_job.py
--rw-r--r--   0 Karel      (503) staff       (20)      579 2024-04-16 21:42:49.000000 drumpler-2.2.0/drumpler/sql_request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 21:45:17.645667 drumpler-2.2.0/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      783 2024-04-16 21:44:53.000000 drumpler-2.2.0/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:45:17.643033 drumpler-2.2.0/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.0/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 23:34:23.294312 drumpler-2.2.1/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 23:34:23.293088 drumpler-2.2.1/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4153 2024-04-16 23:34:23.000000 drumpler-2.2.1/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      355 2024-04-16 23:34:23.000000 drumpler-2.2.1/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 23:34:23.000000 drumpler-2.2.1/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       64 2024-04-16 23:34:23.000000 drumpler-2.2.1/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 23:34:23.000000 drumpler-2.2.1/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.1/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4153 2024-04-16 23:34:23.293718 drumpler-2.2.1/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.1/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 23:34:23.291541 drumpler-2.2.1/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-16 18:54:33.000000 drumpler-2.2.1/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      738 2024-04-16 19:59:55.000000 drumpler-2.2.1/drumpler/config.py
+-rw-r--r--   0 Karel      (503) staff       (20)    10073 2024-04-16 23:34:04.000000 drumpler-2.2.1/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)       69 2024-04-16 18:54:36.000000 drumpler-2.2.1/drumpler/sql_base.py
+-rw-r--r--   0 Karel      (503) staff       (20)      497 2024-04-16 18:54:38.000000 drumpler-2.2.1/drumpler/sql_event.py
+-rw-r--r--   0 Karel      (503) staff       (20)      710 2024-04-16 18:54:37.000000 drumpler-2.2.1/drumpler/sql_job.py
+-rw-r--r--   0 Karel      (503) staff       (20)      579 2024-04-16 21:42:49.000000 drumpler-2.2.1/drumpler/sql_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 23:34:23.294425 drumpler-2.2.1/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      783 2024-04-16 23:34:10.000000 drumpler-2.2.1/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 23:34:23.292361 drumpler-2.2.1/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.1/test/test_drumpler.py
```

### Comparing `drumpler-2.2.0/Drumpler.egg-info/PKG-INFO` & `drumpler-2.2.1/Drumpler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.0
+Version: 2.2.1
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.0/LICENSE` & `drumpler-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.0/PKG-INFO` & `drumpler-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.0
+Version: 2.2.1
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.0/README.md` & `drumpler-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.0/drumpler/config.py` & `drumpler-2.2.1/drumpler/config.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.0/drumpler/drumpler.py` & `drumpler-2.2.1/drumpler/drumpler.py`

 * *Files 26% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         self.app.add_url_rule('/', view_func=self.hello_world, methods=['GET'])
         self.app.add_url_rule('/request', view_func=self.__process_request, methods=['POST'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__get_request, methods=['GET'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__update_request, methods=['PUT'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__delete_request, methods=['DELETE'])
         self.app.add_url_rule('/jobs/next-pending', view_func=self.__get_next_pending_job, methods=['GET'])
         self.app.add_url_rule('/jobs/<int:job_id>', view_func=self.__update_job, methods=['PUT'])
+        self.app.add_url_rule('/jobs/<int:job_id>/update-status', view_func=self.__update_job_status, methods=['PUT'])
+        self.app.add_url_rule('/jobs/<int:job_id>/mark-handled', view_func=self.__mark_request_as_handled, methods=['PUT'])
         self.app.add_url_rule('/events', view_func=self.__create_event, methods=['POST'])
 
     def __init_env(self):
         if not os.path.exists(".env"):
             sys.exit("ERROR! You must create a .env file that contains a single line 'AUTHORIZATION_KEY=YourAuthorizationKeyHere'")
 
     def __authorize_request(self):
@@ -86,70 +88,67 @@
             db.session.add(new_job)
             db.session.commit()
             return jsonify({"message": "Request processed successfully", "id": new_request.id, "job_id": new_job.id}), 200
         else:
             db.session.commit()
             return jsonify({"message": "Request processed successfully", "id": new_request.id}), 200
 
-    @app.route('/jobs/next-pending', methods=['GET'])
-    def __get_next_pending_job():
+    def __get_next_pending_job(self):
         custom_value = request.args.get('custom_value', None)
-        with db.session.begin():
-            job = db.session.query(SqlJob, SqlRequest).join(SqlRequest).filter(
-                SqlJob.status == 'Pending',
-                SqlRequest.custom_value == custom_value,
-                SqlRequest.is_handled == False
-            ).order_by(SqlJob.created_date).first()
+        try:
+            job = db.session.query(SqlJob, SqlRequest)\
+                .join(SqlRequest, SqlJob.request_id == SqlRequest.id)\
+                .filter(
+                    SqlJob.status == 'Pending',
+                    SqlRequest.custom_value == custom_value,
+                    SqlRequest.is_handled == 0
+                ).order_by(SqlJob.created_date).first()
 
             if job:
                 job_data, request_data = job
-                job_data.is_being_processed = True  # Mark job as being processed
-                db.session.commit()
+                # Mark job as being processed
+                job_data.is_being_processed = True  
+                db.session.commit()  # Commit changes explicitly
                 return jsonify({
                     "job_id": job_data.id,
                     "request_id": request_data.id,
                     "source_ip": request_data.source_ip,
                     "user_agent": request_data.user_agent,
                     "method": request_data.method,
                     "request_url": request_data.request_url,
                     "request_raw": request_data.request_raw,
                     "custom_value": request_data.custom_value
                 }), 200
             else:
+                db.session.rollback()  # Rollback explicitly if nothing found
                 return jsonify({"message": "No pending jobs found."}), 404
 
+        except Exception as e:
+            db.session.rollback()  # Ensure rollback on exception
+            print(f"Exception occurred: {str(e)}")
+            return jsonify({"message": "Error occurred."}), 500
+        
+    def __update_job_status(self, job_id):
+        with self.app.app_context():  # Ensure the application context is being used
+            job = db.session.query(SqlJob).get(job_id)  # Use db.session.query
+            if job:
+                job.status = request.json.get('status', job.status)
+                db.session.commit()
+                return jsonify({"message": "Job status updated successfully"}), 200
+            else:
+                return jsonify({"message": "Job not found"}), 404
 
-    # deprecated
-    #def __get_next_unhandled_request(self):
-    #    with db.session.begin():
-    #        query = db.session.query(SqlRequest)\
-    #            .filter(SqlRequest.is_handled == 0, 
-    #                    SqlRequest.is_being_processed == False)
-    #        custom_value = request.args.get('custom_value', None)
-    #        if custom_value is not None:
-    #            query = query.filter(SqlRequest.custom_value == custom_value)
-    #        unhandled_request = query.order_by(SqlRequest.id)\
-    #            .with_for_update(skip_locked=True).first()
-    #        if unhandled_request:
-    #            unhandled_request.is_being_processed = True
-    #            request_data = {
-    #                "id": unhandled_request.id,
-    #                "timestamp": unhandled_request.timestamp.isoformat(),
-    #                "source_ip": unhandled_request.source_ip,
-    #                "user_agent": unhandled_request.user_agent,
-    #                "method": unhandled_request.method,
-    #                "request_url": unhandled_request.request_url,
-    #                "request_raw": unhandled_request.request_raw,
-    #                "custom_value": unhandled_request.custom_value,
-    #                "is_handled": unhandled_request.is_handled
-    #            }
-    #    if unhandled_request:
-    #        return jsonify(request_data), 200
-    #    else:
-    #        return jsonify({"message": "No unhandled requests found."}), 404
+    def __mark_request_as_handled(self, job_id):
+        job = SqlJob.query.get(job_id)
+        if job:
+            request = SqlRequest.query.get(job.request_id)
+            request.is_handled = 1
+            db.session.commit()
+            return jsonify({"message": "Request marked as handled"}), 200
+        return jsonify({"message": "Job or request not found"}), 404
 
     def __get_request(self, request_id):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
         request_entry = SqlRequest.query.get(request_id)
         if request_entry:
             return jsonify({
```

### Comparing `drumpler-2.2.0/drumpler/sql_job.py` & `drumpler-2.2.1/drumpler/sql_job.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.0/drumpler/sql_request.py` & `drumpler-2.2.1/drumpler/sql_request.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.0/setup.py` & `drumpler-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='2.2.0',
+    version='2.2.1',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `drumpler-2.2.0/test/test_drumpler.py` & `drumpler-2.2.1/test/test_drumpler.py`

 * *Files identical despite different names*

