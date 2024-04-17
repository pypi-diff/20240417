# Comparing `tmp/maitai-sdk-python-0.423.tar.gz` & `tmp/maitai-sdk-python-0.424.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maitai-sdk-python-0.423.tar", last modified: Mon Apr 15 21:15:08 2024, max compression
+gzip compressed data, was "maitai-sdk-python-0.424.tar", last modified: Wed Apr 17 19:15:17 2024, max compression
```

## Comparing `maitai-sdk-python-0.423.tar` & `maitai-sdk-python-0.424.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 21:15:08.862220 maitai-sdk-python-0.423/
--rw-rw-rw-   0        0        0      380 2024-04-15 21:15:08.861220 maitai-sdk-python-0.423/PKG-INFO
--rw-rw-rw-   0        0        0     5332 2024-04-15 21:14:54.000000 maitai-sdk-python-0.423/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 21:15:08.832266 maitai-sdk-python-0.423/maitai/
--rw-rw-rw-   0        0        0      327 2024-04-13 18:48:05.000000 maitai-sdk-python-0.423/maitai/__init__.py
--rw-rw-rw-   0        0        0      413 2024-04-13 18:48:23.000000 maitai-sdk-python-0.423/maitai/_config.py
--rw-rw-rw-   0        0        0      594 2024-04-09 05:13:35.000000 maitai-sdk-python-0.423/maitai/_eval_request.py
--rw-rw-rw-   0        0        0     9658 2024-04-15 21:11:56.000000 maitai-sdk-python-0.423/maitai/_evaluator.py
--rw-rw-rw-   0        0        0     1171 2022-12-02 23:23:26.000000 maitai-sdk-python-0.423/maitai/_loadable.py
--rw-rw-rw-   0        0        0      206 2024-04-13 18:48:42.000000 maitai-sdk-python-0.423/maitai/_maitai_object.py
-drwxrwxrwx   0        0        0        0 2024-04-15 21:15:08.859219 maitai-sdk-python-0.423/maitai_sdk_python.egg-info/
--rw-rw-rw-   0        0        0      380 2024-04-15 21:15:08.000000 maitai-sdk-python-0.423/maitai_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-04-15 21:15:08.000000 maitai-sdk-python-0.423/maitai_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 21:15:08.000000 maitai-sdk-python-0.423/maitai_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-15 21:15:08.000000 maitai-sdk-python-0.423/maitai_sdk_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-15 21:15:08.000000 maitai-sdk-python-0.423/maitai_sdk_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 21:15:08.862220 maitai-sdk-python-0.423/setup.cfg
--rw-rw-rw-   0        0        0      573 2024-04-15 21:11:56.000000 maitai-sdk-python-0.423/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 19:15:17.023124 maitai-sdk-python-0.424/
+-rw-rw-rw-   0        0        0      380 2024-04-17 19:15:17.022124 maitai-sdk-python-0.424/PKG-INFO
+-rw-rw-rw-   0        0        0     5332 2024-04-15 21:14:54.000000 maitai-sdk-python-0.424/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 19:15:16.985497 maitai-sdk-python-0.424/maitai/
+-rw-rw-rw-   0        0        0      327 2024-04-13 18:48:05.000000 maitai-sdk-python-0.424/maitai/__init__.py
+-rw-rw-rw-   0        0        0      413 2024-04-13 18:48:23.000000 maitai-sdk-python-0.424/maitai/_config.py
+-rw-rw-rw-   0        0        0      636 2024-04-17 19:09:29.000000 maitai-sdk-python-0.424/maitai/_eval_request.py
+-rw-rw-rw-   0        0        0    10965 2024-04-17 19:13:10.000000 maitai-sdk-python-0.424/maitai/_evaluator.py
+-rw-rw-rw-   0        0        0     1171 2022-12-02 23:23:26.000000 maitai-sdk-python-0.424/maitai/_loadable.py
+-rw-rw-rw-   0        0        0      206 2024-04-13 18:48:42.000000 maitai-sdk-python-0.424/maitai/_maitai_object.py
+drwxrwxrwx   0        0        0        0 2024-04-17 19:15:17.021126 maitai-sdk-python-0.424/maitai_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0      380 2024-04-17 19:15:16.000000 maitai-sdk-python-0.424/maitai_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-04-17 19:15:16.000000 maitai-sdk-python-0.424/maitai_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 19:15:16.000000 maitai-sdk-python-0.424/maitai_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-17 19:15:16.000000 maitai-sdk-python-0.424/maitai_sdk_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-17 19:15:16.000000 maitai-sdk-python-0.424/maitai_sdk_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 19:15:17.024129 maitai-sdk-python-0.424/setup.cfg
+-rw-rw-rw-   0        0        0      573 2024-04-17 19:13:29.000000 maitai-sdk-python-0.424/setup.py
```

### Comparing `maitai-sdk-python-0.423/README.md` & `maitai-sdk-python-0.424/README.md`

 * *Files identical despite different names*

### Comparing `maitai-sdk-python-0.423/maitai/_eval_request.py` & `maitai-sdk-python-0.424/maitai/_eval_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 class EvalRequest(Loadable):
 
     def __init__(self):
         super().__init__()
         self.id = -1
         self.date_created = -1
         self.application_id = -1
+        self.application_ref_name = None
         self.session_id = None
         self.reference_id = None
         self.evaluation_content_type = ''
         self.evaluation_content = ''
         self.action_type = ''
```

### Comparing `maitai-sdk-python-0.423/maitai/_evaluator.py` & `maitai-sdk-python-0.424/maitai/_evaluator.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,69 +12,84 @@
 
     MAITAI_HOST = 'https://maitai.ai.yewpay.com'
 
     def __init__(self):
         super().__init__()
 
     @classmethod
-    def evaluate(cls, application_id, session_id, reference_id, action_type, content):
-        eval_request: EvalRequest = cls.create_eval_request(application_id, session_id, reference_id, action_type, content)
+    def evaluate(cls, session_id, reference_id, action_type, content, application_id=None, application_ref_name=None):
+        if application_id is None and application_ref_name is None:
+            raise Exception('application_id or application_ref_name must be provided')
+        eval_request: EvalRequest = cls.create_eval_request(application_id, application_ref_name, session_id, reference_id, action_type, content)
         cls.run_async(cls.send_evaluation_request(eval_request))
 
     @classmethod
-    def create_eval_request(cls, application_id, session_id, reference_id, action_type, content):
+    def create_eval_request(cls, application_id, application_ref_name, session_id, reference_id, action_type, content):
         if type(content) != str:
             raise Exception('Content must be a string')
         eval_request: EvalRequest = EvalRequest()
         eval_request.application_id = application_id
+        eval_request.application_ref_name = application_ref_name
         eval_request.session_id = session_id
         eval_request.reference_id = reference_id
         eval_request.action_type = action_type
         eval_request.evaluation_content = content
         eval_request.evaluation_content_type = 'text'
         return eval_request
 
     @classmethod
-    def update_session_context(cls, application_id, session_id, context):
+    def update_session_context(cls, session_id, context, application_id = None, application_ref_name = None):
         if type(context) != dict:
             raise Exception('Context must be a dictionary')
+        if application_id is None and application_ref_name is None:
+            raise Exception('application_id or application_ref_name must be provided')
         session_context = {
             'application_id': application_id,
+            'application_ref_name': application_ref_name,
             'session_id': session_id,
             'context': context
         }
         cls.run_async(cls.send_session_context_update(session_context))
 
     @classmethod
-    def append_session_context(cls, application_id, session_id, context):
+    def append_session_context(cls, session_id, context, application_id = None, application_ref_name = None):
         if type(context) != dict:
             raise Exception('Context must be a dictionary')
+        if application_id is None and application_ref_name is None:
+            raise Exception('application_id or application_ref_name must be provided')
         session_context = {
             'application_id': application_id,
+            'application_ref_name': application_ref_name,
             'session_id': session_id,
             'context': context
         }
         cls.run_async(cls.send_session_context_append(session_context))
 
     @classmethod
-    def update_application_context(cls, application_id, context):
+    def update_application_context(cls, context, application_id = None, application_ref_name = None):
         if type(context) != dict:
             raise Exception('Context must be a dictionary')
+        if application_id is None and application_ref_name is None:
+            raise Exception('application_id or application_ref_name must be provided')
         application_context = {
             'application_id': application_id,
+            'application_ref_name': application_ref_name,
             'context': context
         }
         cls.run_async(cls.send_application_context_update(application_context))
 
     @classmethod
-    def append_application_context(cls, application_id, context):
+    def append_application_context(cls, context, application_id = None, application_ref_name = None):
         if type(context) != dict:
             raise Exception('Context must be a dictionary')
+        if application_id is None and application_ref_name is None:
+            raise Exception('application_id or application_ref_name must be provided')
         application_context = {
             'application_id': application_id,
+            'application_ref_name': application_ref_name,
             'context': context
         }
         cls.run_async(cls.send_application_context_append(application_context))
 
     @classmethod
     async def send_evaluation_request(cls, eval_request):
         async def send_request():
```

### Comparing `maitai-sdk-python-0.423/maitai/_loadable.py` & `maitai-sdk-python-0.424/maitai/_loadable.py`

 * *Files identical despite different names*

### Comparing `maitai-sdk-python-0.423/setup.py` & `maitai-sdk-python-0.424/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='maitai-sdk-python',
-    version='0.423',
+    version='0.424',
     packages=find_packages(),
     install_requires=[
         'requests',
         'aiohttp'
     ],
     # Optional metadata
     author='Christian DalSanto',
```

