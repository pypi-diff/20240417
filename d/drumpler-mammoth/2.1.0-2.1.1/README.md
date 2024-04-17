# Comparing `tmp/drumpler_mammoth-2.1.0.tar.gz` & `tmp/drumpler_mammoth-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler_mammoth-2.1.0.tar", last modified: Tue Apr 16 23:35:14 2024, max compression
+gzip compressed data, was "drumpler_mammoth-2.1.1.tar", last modified: Wed Apr 17 17:53:18 2024, max compression
```

## Comparing `drumpler_mammoth-2.1.0.tar` & `drumpler_mammoth-2.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 23:35:14.538106 drumpler_mammoth-2.1.0/
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler_mammoth-2.1.0/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4083 2024-04-16 23:35:14.537500 drumpler_mammoth-2.1.0/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler_mammoth-2.1.0/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 23:35:14.534035 drumpler_mammoth-2.1.0/drumpler_mammoth/
--rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-16 20:58:49.000000 drumpler_mammoth-2.1.0/drumpler_mammoth/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      301 2024-04-16 21:10:49.000000 drumpler_mammoth-2.1.0/drumpler_mammoth/config.py
--rw-r--r--   0 Karel      (503) staff       (20)     3132 2024-04-16 23:32:45.000000 drumpler_mammoth-2.1.0/drumpler_mammoth/http_request.py
--rw-r--r--   0 Karel      (503) staff       (20)     5121 2024-04-16 23:31:51.000000 drumpler_mammoth-2.1.0/drumpler_mammoth/mammoth.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 23:35:14.536789 drumpler_mammoth-2.1.0/drumpler_mammoth.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4083 2024-04-16 23:35:14.000000 drumpler_mammoth-2.1.0/drumpler_mammoth.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      342 2024-04-16 23:35:14.000000 drumpler_mammoth-2.1.0/drumpler_mammoth.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 23:35:14.000000 drumpler_mammoth-2.1.0/drumpler_mammoth.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       23 2024-04-16 23:35:14.000000 drumpler_mammoth-2.1.0/drumpler_mammoth.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-16 23:35:14.000000 drumpler_mammoth-2.1.0/drumpler_mammoth.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 23:35:14.538250 drumpler_mammoth-2.1.0/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      725 2024-04-16 23:35:00.000000 drumpler_mammoth-2.1.0/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:53:18.873572 drumpler_mammoth-2.1.1/
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler_mammoth-2.1.1/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4083 2024-04-17 17:53:18.872629 drumpler_mammoth-2.1.1/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler_mammoth-2.1.1/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:53:18.868033 drumpler_mammoth-2.1.1/drumpler_mammoth/
+-rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-16 20:58:49.000000 drumpler_mammoth-2.1.1/drumpler_mammoth/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      301 2024-04-16 21:10:49.000000 drumpler_mammoth-2.1.1/drumpler_mammoth/config.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3132 2024-04-16 23:32:45.000000 drumpler_mammoth-2.1.1/drumpler_mammoth/http_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6039 2024-04-17 17:49:15.000000 drumpler_mammoth-2.1.1/drumpler_mammoth/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)      938 2024-04-17 16:38:09.000000 drumpler_mammoth-2.1.1/drumpler_mammoth/mylogger.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:53:18.871715 drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4083 2024-04-17 17:53:18.000000 drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      371 2024-04-17 17:53:18.000000 drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-17 17:53:18.000000 drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       23 2024-04-17 17:53:18.000000 drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-17 17:53:18.000000 drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-17 17:53:18.873768 drumpler_mammoth-2.1.1/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      725 2024-04-17 17:53:06.000000 drumpler_mammoth-2.1.1/setup.py
```

### Comparing `drumpler_mammoth-2.1.0/LICENSE` & `drumpler_mammoth-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.1.0/PKG-INFO` & `drumpler_mammoth-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drumpler_mammoth
-Version: 2.1.0
+Version: 2.1.1
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler-Mammoth
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler_mammoth-2.1.0/README.md` & `drumpler_mammoth-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.1.0/drumpler_mammoth/http_request.py` & `drumpler_mammoth-2.1.1/drumpler_mammoth/http_request.py`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.1.0/drumpler_mammoth/mammoth.py` & `drumpler_mammoth-2.1.1/drumpler_mammoth/mammoth.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,119 +1,140 @@
 import requests
 import json
+import signal
 import threading
-from concurrent.futures import ThreadPoolExecutor
 import multiprocessing
 from .http_request import HttpRequest  # Make sure to import your HttpRequest class
 from .config import Config
-import traceback
+from .mylogger import MyLogger
+
 
 class Mammoth:
-    def __init__(self, process_request_data, drumpler_url=Config.DRUMPLER_URL, workers=1, custom_value=None):
+    def __init__(self, process_request_data, drumpler_url=Config.DRUMPLER_URL, num_workers=1, custom_value=None):
         self.drumpler_url = drumpler_url
-        self.auth_key = Config.AUTHORIZATION_KEY  # Default value if not set
-        self.workers = workers if workers is not None else multiprocessing.cpu_count()
-        self.stop_signal = threading.Event()  # Use an event to signal workers to stop
         self.user_process_request_data = process_request_data
+        self.auth_key = Config.AUTHORIZATION_KEY  # Default value if not set
         self.custom_value = custom_value
+        
+        # Initialize custom logger
+        self.logger = MyLogger.get_logger()
+        
+        self.num_workers = num_workers if num_workers is not None else multiprocessing.cpu_count()
+        
+        # Signal handling to gracefully shutdown on SIGINT (CTRL+C)
+        self.stop_signal = threading.Event()  # Use an event to signal workers to stop
+        signal.signal(signal.SIGINT, self.signal_handler)
 
-    def fetch_next_pending_job(self):
-        headers = {"Authorization": f"Bearer {self.auth_key}"}
-        params = {'custom_value': self.custom_value} if self.custom_value else {}
-        response = requests.get(f"{self.drumpler_url}/jobs/next-pending", headers=headers, params=params)
+        # Simplified run method using threads directly
+        self.worker_threads = []
 
-        if response.status_code == 200:
-            data = response.json()
-            # Ensure request_raw is parsed from JSON only if it's a string
-            request_raw = data['request_raw']
-            if isinstance(request_raw, str):
-                request_raw = json.loads(request_raw)
-
-            return HttpRequest(
-                id=data['request_id'],
-                job_id=data['job_id'],
-                source_ip=data['source_ip'],
-                user_agent=data['user_agent'],
-                method=data['method'],
-                request_url=data['request_url'],
-                request_raw=request_raw,
-                custom_value=data['custom_value']
-            )
-        else:
-            print(f"Failed to fetch next pending job: {response.status_code}")
+    def get_logger(self):
+        return self.logger
+
+    def signal_handler(self, signum, frame):
+        print("Shutdown signal received, stopping workers...")
+        self.stop_signal.set()  # Signal all threads to stop
+
+    def fetch_next_pending_job(self):
+        try:
+            headers = {"Authorization": f"Bearer {self.auth_key}"}
+            params = {'custom_value': self.custom_value} if self.custom_value else {}
+            response = requests.get(f"{self.drumpler_url}/jobs/next-pending", headers=headers, params=params)
+            if response.status_code == 200:
+                data = response.json()
+                return HttpRequest(
+                    id=data['request_id'],
+                    job_id=data['job_id'],
+                    source_ip=data['source_ip'],
+                    user_agent=data['user_agent'],
+                    method=data['method'],
+                    request_url=data['request_url'],
+                    request_raw=json.loads(data['request_raw']),
+                    custom_value=data['custom_value']
+                )
+            else:
+                self.logger.error(f"Failed to fetch next pending job: {response.status_code} - {response.text}")
+                return None
+        except requests.ConnectionError as e:
+            self.logger.error(f"Network problem occurred: {str(e)}")
+            return None
+        except requests.Timeout as e:
+            self.logger.error(f"Request timed out: {str(e)}")
+            return None
+        except requests.RequestException as e:
+            self.logger.error(f"HTTP request failed: {str(e)}")
             return None
         
     def insert_event(self, job_id, message):
         headers = {"Authorization": f"Bearer {self.auth_key}"}
         event_data = {
             "job_id": job_id,
             "message": message
         }
         response = requests.post(f"{self.drumpler_url}/events", json=event_data, headers=headers)
         if response.status_code == 201:
             print(f"Event logged successfully for job {job_id}")
         else:
             print(f"Failed to log event for job {job_id}: {response.status_code}")
 
-    def update_status(self, job_id, new_status):
-        """
-        Update the status of a job in Drumpler.
-        """
-        headers = {"Authorization": f"Bearer {self.auth_key}"}
-        data = {
-            "status": new_status
-        }
-        response = requests.put(f"{self.drumpler_url}/jobs/{job_id}/update-status", json=data, headers=headers)
-        if response.status_code == 200:
-            print(f"Status updated to {new_status} for job {job_id}")
-            if new_status == "Completed":
-                self.mark_request_as_handled(job_id)
-        else:
-            print(f"Failed to update status for job {job_id}: {response.status_code}")
-
     def mark_request_as_handled(self, job_id):
         """
         Mark the request as handled when the job is completed.
         """
         headers = {"Authorization": f"Bearer {self.auth_key}"}
         response = requests.put(f"{self.drumpler_url}/jobs/{job_id}/mark-handled", headers=headers)
         if response.status_code == 200:
             print(f"Request marked as handled for job {job_id}")
         else:
             print(f"Failed to mark request as handled for job {job_id}: {response.status_code}")
-
-    def run(self):
-        with ThreadPoolExecutor(max_workers=self.workers) as executor:
-            future = executor.submit(self.worker_task)
-            try:
-                future.result()  # This will wait until the callable completes
-            except Exception as e:
-                traceback.print_exc()
-                print(f"Worker task raised an exception: {e}")
+        
+    def update_status(self, job_id, new_status):
+        headers = {"Authorization": f"Bearer {self.auth_key}"}
+        data = {"status": new_status}
+        try:
+            response = requests.put(f"{self.drumpler_url}/jobs/{job_id}/update-status", json=data, headers=headers)
+            if response.status_code == 200:
+                self.logger.info(f"Status updated to {new_status} for job {job_id}")
+                if new_status == "Completed":
+                    self.mark_request_as_handled(job_id)
+            else:
+                self.logger.error(f"Failed to update status for job {job_id}: {response.status_code} - {response.text}")
+        except requests.RequestException as e:
+            self.logger.error(f"Failed to update status due to HTTP error: {str(e)}")
 
     def worker_task(self):
         while not self.stop_signal.is_set():
             request = self.fetch_next_pending_job()
             if request:
-                print(f"Fetched next pending job {request.job_id}")
-                print(f"Updating status to 'In Progress'")
-                self.update_status(request.job_id, "In Progress")
                 if self.user_process_request_data(request):
                     self.insert_event(request.job_id, "Request processed successfully")
                     self.update_status(request.job_id, "Completed")
+                    self.logger.info(f"Request processed successfully for job {request.job_id}")
                 else:
                     self.insert_event(request.job_id, "Failed to process request")
                     self.update_status(request.job_id, "Error")
+                    self.logger.error(f"Failed to process request for job {request.job_id}")
+            if self.stop_signal.wait(timeout=0.1):
+                break
 
     def stop(self):
         self.stop_signal.set()
+        for thread in self.worker_threads:
+            thread.join()
+
+    def run(self):
+        self.worker_threads = [threading.Thread(target=self.worker_task) for _ in range(self.num_workers)]
+        for thread in self.worker_threads:
+            thread.start()
+        for thread in self.worker_threads:
+            thread.join()
+    
 
-# Setup signal handling to gracefully handle shutdowns
 if __name__ == "__main__":
-    mammoth = Mammoth(process_request_data=lambda req: True)  # Sample process_request_data function
+    mammoth = Mammoth(process_request_data=lambda req: True)
     print("Starting Mammoth application...")
     try:
         mammoth.run()
     except KeyboardInterrupt:
         print("Shutdown signal received")
         mammoth.stop()
-        print("Mammoth application stopped gracefully")
+        print("Mammoth application stopped gracefully")
```

### Comparing `drumpler_mammoth-2.1.0/drumpler_mammoth.egg-info/PKG-INFO` & `drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drumpler_mammoth
-Version: 2.1.0
+Version: 2.1.1
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler-Mammoth
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler_mammoth-2.1.0/setup.py` & `drumpler_mammoth-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='drumpler_mammoth',
-    version='2.1.0',
+    version='2.1.1',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler-Mammoth',
     packages=find_packages(),
```

