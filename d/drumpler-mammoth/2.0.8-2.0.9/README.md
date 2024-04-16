# Comparing `tmp/drumpler_mammoth-2.0.8.tar.gz` & `tmp/drumpler_mammoth-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler_mammoth-2.0.8.tar", last modified: Tue Apr 16 21:06:12 2024, max compression
+gzip compressed data, was "drumpler_mammoth-2.0.9.tar", last modified: Tue Apr 16 21:48:17 2024, max compression
```

## Comparing `drumpler_mammoth-2.0.8.tar` & `drumpler_mammoth-2.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:06:12.744154 drumpler_mammoth-2.0.8/
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler_mammoth-2.0.8/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 21:06:12.743312 drumpler_mammoth-2.0.8/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler_mammoth-2.0.8/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:06:12.739792 drumpler_mammoth-2.0.8/drumpler_mammoth/
--rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-16 20:58:49.000000 drumpler_mammoth-2.0.8/drumpler_mammoth/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      301 2024-04-16 20:08:33.000000 drumpler_mammoth-2.0.8/drumpler_mammoth/config.py
--rw-r--r--   0 Karel      (503) staff       (20)     3133 2024-04-16 20:51:21.000000 drumpler_mammoth-2.0.8/drumpler_mammoth/http_request.py
--rw-r--r--   0 Karel      (503) staff       (20)     3427 2024-04-16 20:09:39.000000 drumpler_mammoth-2.0.8/drumpler_mammoth/mammoth.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:06:12.742636 drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 21:06:12.000000 drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      342 2024-04-16 21:06:12.000000 drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 21:06:12.000000 drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 21:06:12.000000 drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-16 21:06:12.000000 drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 21:06:12.744328 drumpler_mammoth-2.0.8/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      700 2024-04-16 21:06:07.000000 drumpler_mammoth-2.0.8/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:48:17.673203 drumpler_mammoth-2.0.9/
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler_mammoth-2.0.9/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4083 2024-04-16 21:48:17.672373 drumpler_mammoth-2.0.9/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler_mammoth-2.0.9/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:48:17.668833 drumpler_mammoth-2.0.9/drumpler_mammoth/
+-rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-16 20:58:49.000000 drumpler_mammoth-2.0.9/drumpler_mammoth/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      301 2024-04-16 21:10:49.000000 drumpler_mammoth-2.0.9/drumpler_mammoth/config.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3133 2024-04-16 21:47:28.000000 drumpler_mammoth-2.0.9/drumpler_mammoth/http_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)     4368 2024-04-16 21:48:01.000000 drumpler_mammoth-2.0.9/drumpler_mammoth/mammoth.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:48:17.671566 drumpler_mammoth-2.0.9/drumpler_mammoth.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4083 2024-04-16 21:48:17.000000 drumpler_mammoth-2.0.9/drumpler_mammoth.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      342 2024-04-16 21:48:17.000000 drumpler_mammoth-2.0.9/drumpler_mammoth.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 21:48:17.000000 drumpler_mammoth-2.0.9/drumpler_mammoth.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       23 2024-04-16 21:48:17.000000 drumpler_mammoth-2.0.9/drumpler_mammoth.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-16 21:48:17.000000 drumpler_mammoth-2.0.9/drumpler_mammoth.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 21:48:17.673373 drumpler_mammoth-2.0.9/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      725 2024-04-16 21:48:06.000000 drumpler_mammoth-2.0.9/setup.py
```

### Comparing `drumpler_mammoth-2.0.8/LICENSE` & `drumpler_mammoth-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.8/PKG-INFO` & `drumpler_mammoth-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drumpler_mammoth
-Version: 2.0.8
+Version: 2.0.9
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler-Mammoth
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: python-dotenv
 
 
 # `Drumpler`
 
 `Drumpler` is a general-purpose application designed to facilitate efficient workflow automation through RESTful API interactions and job processing. Built on Flask and SQLAlchemy, this application serves as a robust backend for capturing, storing, and processing HTTP requests in a scalable manner. The application is split into two main components: `drumpler.py` for handling RESTful API requests and `mammoth.py` for querying the API and processing jobs asynchronously.
 
 # High Level Overview
```

### Comparing `drumpler_mammoth-2.0.8/README.md` & `drumpler_mammoth-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.8/drumpler_mammoth/http_request.py` & `drumpler_mammoth-2.0.9/drumpler_mammoth/http_request.py`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.8/drumpler_mammoth/mammoth.py` & `drumpler_mammoth-2.0.9/drumpler_mammoth/mammoth.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,36 +11,59 @@
         self.drumpler_url = drumpler_url
         self.auth_key = Config.AUTHORIZATION_KEY  # Default value if not set
         self.workers = workers if workers is not None else multiprocessing.cpu_count()
         self.stop_signal = threading.Event()  # Use an event to signal workers to stop
         self.user_process_request_data = process_request_data
         self.custom_value = custom_value
 
-    def fetch_next_unhandled_request(self):
+    def fetch_next_pending_job(self):
         headers = {"Authorization": f"Bearer {self.auth_key}"}
         params = {'custom_value': self.custom_value} if self.custom_value else {}
-        response = requests.get(f"{self.drumpler_url}/request/next-unhandled", headers=headers, params=params)
+        response = requests.get(f"{self.drumpler_url}/jobs/next-pending", headers=headers, params=params)
 
         if response.status_code == 200:
             data = response.json()
             return HttpRequest(
-                id=data['id'],
-                timestamp=data['timestamp'],
+                id=data['request_id'],
+                job_id=data['job_id'],
                 source_ip=data['source_ip'],
                 user_agent=data['user_agent'],
                 method=data['method'],
                 request_url=data['request_url'],
-                request_raw=json.dumps(data['request_raw']),
-                custom_value=data['custom_value'],
-                is_handled=data['is_handled']
+                request_raw=json.loads(data['request_raw']),
+                custom_value=data['custom_value']
             )
         else:
-            print(f"Failed to fetch unhandled request: {response.status_code}")
+            print(f"Failed to fetch next pending job: {response.status_code}")
             return None
 
+
+    # deprecated
+    #def fetch_next_unhandled_request(self):
+    #    headers = {"Authorization": f"Bearer {self.auth_key}"}
+    #    params = {'custom_value': self.custom_value} if self.custom_value else {}
+    #    response = requests.get(f"{self.drumpler_url}/request/next-unhandled", headers=headers, params=params)
+#
+    #    if response.status_code == 200:
+    #        data = response.json()
+    #        return HttpRequest(
+    #            id=data['id'],
+    #            timestamp=data['timestamp'],
+    #            source_ip=data['source_ip'],
+    #            user_agent=data['user_agent'],
+    #            method=data['method'],
+    #            request_url=data['request_url'],
+    #            request_raw=json.dumps(data['request_raw']),
+    #            custom_value=data['custom_value'],
+    #            is_handled=data['is_handled']
+    #        )
+    #    else:
+    #        print(f"Failed to fetch unhandled request: {response.status_code}")
+    #        return None
+
     def insert_event(self, job_id, message):
         headers = {"Authorization": f"Bearer {self.auth_key}"}
         event_data = {
             "job_id": job_id,
             "message": message
         }
         response = requests.post(f"{self.drumpler_url}/events", json=event_data, headers=headers)
@@ -51,17 +74,17 @@
 
     def run(self):
         with ThreadPoolExecutor(max_workers=self.workers) as executor:
             executor.submit(self.worker_task)
 
     def worker_task(self):
         while not self.stop_signal.is_set():
-            request = self.fetch_next_unhandled_request()
+            request = self.fetch_next_pending_job()
             if request:
-                print(f"Processing request {request.id}")
+                print(f"Fetched next pending job {request.job_id}")
                 if self.user_process_request_data(request):
                     result = request.mark_as_handled()
                     print(result)
                     self.insert_event(request.id, "Request processed successfully")
                 else:
                     self.insert_event(request.id, "Failed to process request")
```

### Comparing `drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/PKG-INFO` & `drumpler_mammoth-2.0.9/drumpler_mammoth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drumpler_mammoth
-Version: 2.0.8
+Version: 2.0.9
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler-Mammoth
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: python-dotenv
 
 
 # `Drumpler`
 
 `Drumpler` is a general-purpose application designed to facilitate efficient workflow automation through RESTful API interactions and job processing. Built on Flask and SQLAlchemy, this application serves as a robust backend for capturing, storing, and processing HTTP requests in a scalable manner. The application is split into two main components: `drumpler.py` for handling RESTful API requests and `mammoth.py` for querying the API and processing jobs asynchronously.
 
 # High Level Overview
```

### Comparing `drumpler_mammoth-2.0.8/setup.py` & `drumpler_mammoth-2.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='drumpler_mammoth',
-    version='2.0.8',
+    version='2.0.9',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler-Mammoth',
     packages=find_packages(),
@@ -14,9 +14,10 @@
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
     install_requires=[
         'requests',
+        'python-dotenv',
     ],
 )
```

