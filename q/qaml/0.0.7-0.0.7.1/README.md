# Comparing `tmp/qaml-0.0.7.tar.gz` & `tmp/qaml-0.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.7.tar", last modified: Thu Apr 11 17:20:48 2024, max compression
+gzip compressed data, was "qaml-0.0.7.1.tar", last modified: Wed Apr 17 15:45:16 2024, max compression
```

## Comparing `qaml-0.0.7.tar` & `qaml-0.0.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-11 17:20:48.205490 qaml-0.0.7/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1561 2024-04-11 17:20:48.205352 qaml-0.0.7/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      733 2024-04-11 17:16:45.000000 qaml-0.0.7/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-11 17:20:48.204455 qaml-0.0.7/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      948 2024-04-11 17:16:45.000000 qaml-0.0.7/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)    10256 2024-04-11 17:19:58.000000 qaml-0.0.7/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-11 17:20:48.205193 qaml-0.0.7/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1561 2024-04-11 17:20:48.000000 qaml-0.0.7/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-11 17:20:48.000000 qaml-0.0.7/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-11 17:20:48.000000 qaml-0.0.7/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-11 17:20:48.000000 qaml-0.0.7/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-11 17:20:48.000000 qaml-0.0.7/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-11 17:20:48.000000 qaml-0.0.7/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-11 17:20:48.205527 qaml-0.0.7/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 15:45:16.229779 qaml-0.0.7.1/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.1/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 15:45:16.229519 qaml-0.0.7.1/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.1/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-17 15:45:13.000000 qaml-0.0.7.1/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 15:45:16.228373 qaml-0.0.7.1/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.1/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1113 2024-04-11 18:51:32.000000 qaml-0.0.7.1/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    10610 2024-04-17 15:43:09.000000 qaml-0.0.7.1/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 15:45:16.229176 qaml-0.0.7.1/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 15:45:16.000000 qaml-0.0.7.1/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-17 15:45:16.000000 qaml-0.0.7.1/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-17 15:45:16.000000 qaml-0.0.7.1/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-17 15:45:16.000000 qaml-0.0.7.1/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-17 15:45:16.000000 qaml-0.0.7.1/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-17 15:45:16.000000 qaml-0.0.7.1/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-17 15:45:16.229830 qaml-0.0.7.1/setup.cfg
```

### Comparing `qaml-0.0.7/LICENSE` & `qaml-0.0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7/PKG-INFO` & `qaml-0.0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.7/README.md` & `qaml-0.0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7/pyproject.toml` & `qaml-0.0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.7"
+version = "0.0.7.1"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.7/qaml/__main__.py` & `qaml-0.0.7.1/qaml/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,21 @@
     api_key = os.environ.get("QAML_API_KEY")
     use_mjpeg = os.environ.get("QAML_USE_MJPEG", "true").lower() == "true"
     if api_key is None:
         print("Please set the QAML_API_KEY environment variable")
         sys.exit(1)
     print("Initializing device driver...")
     client = qaml.Client(api_key=api_key, use_mjpeg=use_mjpeg)
+    print(dir(qaml))
+    print(qaml.__file__)
+    print(qaml.__name__)
+    print(qaml.__package__)
+    print(qaml.__path__)
+    print(qaml.__spec__)
+    print(qaml)
     # if no args, start repl
     if len(sys.argv) == 1:
         while True:
             try:
                 command = input("Enter a command: ")
                 client.execute(command)
             except EOFError:
```

### Comparing `qaml-0.0.7/qaml/client.py` & `qaml-0.0.7.1/qaml/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,18 +82,27 @@
         }
         for action in actions:
             function = available_functions[action["name"]]
             arguments = json.loads(action["arguments"])
             function(**arguments)
 
     def agent(self, task):
-        screenshot = self.get_screenshot()
-        payload = {"task": task, "platform": self.platform, "screenshot": screenshot}
-        response = self.req_session.post("https://api.camelqa.com/v1/agent", json=payload)
-        print(response.text)
+        progress = []
+        while True:
+            screenshot = self.get_screenshot()
+            payload = {"task": task, "progress": progress, "platform": self.platform, "screenshot": screenshot}
+            response = self.req_session.post("https://api.camelqa.com/v1/agent", json=payload)
+            response_json = response.json()
+            status = response_json["status"]
+            progress += response_json["progress"]
+            actions = response_json["actions"]
+            if status != "in_progress":
+                return status, progress
+            for action in actions:
+                self.execute(action)
 
 class AndroidClient(BaseClient):
     def __init__(self, api_key, driver=None):
         super().__init__(api_key)
         self.platform = "Android"
         if driver:
             self.driver = driver
@@ -233,15 +242,15 @@
             devices = result.stdout.splitlines()[1:]  # Skip the first line, which is a header
             connected_devices = [line.split('\t')[0] for line in devices if "device" in line]
             return connected_devices
         except:
             return []
 
     if driver is not None:
-            platform_name = driver.desired_capabilities.get('platformName', '').lower()
+            platform_name = driver.platform_name.lower()
             if platform_name == 'android':
                 print("Using the provided Appium driver for Android.")
                 return AndroidClient(api_key, driver=driver)
             elif platform_name == 'ios':
                 print("Using the provided Appium driver for iOS.")
                 return IOSClient(api_key, driver=driver)
             else:
```

### Comparing `qaml-0.0.7/qaml.egg-info/PKG-INFO` & `qaml-0.0.7.1/qaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

