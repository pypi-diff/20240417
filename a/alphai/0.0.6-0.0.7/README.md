# Comparing `tmp/alphai-0.0.6.tar.gz` & `tmp/alphai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphai-0.0.6.tar", max compression
+gzip compressed data, was "alphai-0.0.7.tar", max compression
```

## Comparing `alphai-0.0.6.tar` & `alphai-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     3380 2024-03-14 04:19:08.357857 alphai-0.0.6/README.md
--rw-r--r--   0        0        0     1241 2024-03-14 04:19:08.369857 alphai-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       63 2024-03-14 04:19:08.369857 alphai-0.0.6/src/alphai/__init__.py
--rw-r--r--   0        0        0    30032 2024-03-14 04:19:08.369857 alphai-0.0.6/src/alphai/alphai.py
--rw-r--r--   0        0        0        0 2024-03-14 04:19:08.369857 alphai-0.0.6/src/alphai/api/client.py
--rw-r--r--   0        0        0     1050 2024-03-14 04:19:08.369857 alphai-0.0.6/src/alphai/benchmarking/benchmarker.py
--rw-r--r--   0        0        0        0 2024-03-14 04:19:08.369857 alphai-0.0.6/src/alphai/client/__init__.py
--rw-r--r--   0        0        0    12139 2024-03-14 04:19:08.369857 alphai-0.0.6/src/alphai/client/client.py
--rw-r--r--   0        0        0        0 2024-03-14 04:19:08.369857 alphai-0.0.6/src/alphai/profilers/__init__.py
--rw-r--r--   0        0        0      145 2024-03-14 04:19:08.369857 alphai-0.0.6/src/alphai/profilers/configs_base.py
--rw-r--r--   0        0        0     1165 2024-03-14 04:19:08.369857 alphai-0.0.6/src/alphai/profilers/jax.py
--rw-r--r--   0        0        0     2722 2024-03-14 04:19:08.369857 alphai-0.0.6/src/alphai/profilers/pytorch.py
--rw-r--r--   0        0        0    13868 2024-03-14 04:19:08.369857 alphai-0.0.6/src/alphai/profilers/pytorch_utils.py
--rw-r--r--   0        0        0      465 2024-03-14 04:19:08.369857 alphai-0.0.6/src/alphai/util.py
--rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 alphai-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-16 22:18:31.948565 alphai-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3380 2024-04-16 22:18:31.948565 alphai-0.0.7/README.md
+-rw-r--r--   0        0        0     1241 2024-04-16 22:18:31.960565 alphai-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       63 2024-04-16 22:18:31.960565 alphai-0.0.7/src/alphai/__init__.py
+-rw-r--r--   0        0        0    30965 2024-04-16 22:18:31.960565 alphai-0.0.7/src/alphai/alphai.py
+-rw-r--r--   0        0        0        0 2024-04-16 22:18:31.960565 alphai-0.0.7/src/alphai/api/client.py
+-rw-r--r--   0        0        0     1050 2024-04-16 22:18:31.960565 alphai-0.0.7/src/alphai/benchmarking/benchmarker.py
+-rw-r--r--   0        0        0        0 2024-04-16 22:18:31.960565 alphai-0.0.7/src/alphai/client/__init__.py
+-rw-r--r--   0        0        0    12630 2024-04-16 22:18:31.960565 alphai-0.0.7/src/alphai/client/client.py
+-rw-r--r--   0        0        0        0 2024-04-16 22:18:31.960565 alphai-0.0.7/src/alphai/profilers/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-16 22:18:31.960565 alphai-0.0.7/src/alphai/profilers/configs_base.py
+-rw-r--r--   0        0        0     1165 2024-04-16 22:18:31.960565 alphai-0.0.7/src/alphai/profilers/jax.py
+-rw-r--r--   0        0        0     2722 2024-04-16 22:18:31.960565 alphai-0.0.7/src/alphai/profilers/pytorch.py
+-rw-r--r--   0        0        0    13868 2024-04-16 22:18:31.960565 alphai-0.0.7/src/alphai/profilers/pytorch_utils.py
+-rw-r--r--   0        0        0      465 2024-04-16 22:18:31.960565 alphai-0.0.7/src/alphai/util.py
+-rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 alphai-0.0.7/PKG-INFO
```

### Comparing `alphai-0.0.6/README.md` & `alphai-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alphai-0.0.6/pyproject.toml` & `alphai-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alphai"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["Andrew Chang"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.12"
 jh-client = "^1.3.0"
```

### Comparing `alphai-0.0.6/src/alphai/alphai.py` & `alphai-0.0.7/src/alphai/alphai.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,30 +208,35 @@
         Returns:
             A list of servers if successful, or raises an exception if the user is not authenticated.
         """
         if not self.api_key:
             raise ValueError("Requires user authentication with an API Key")
         return self.client.get_servers()
 
-    def start_server(self, server_name: str = None):
+    def start_server(
+            self,
+            server_name: str = None,
+            environment: str = "ai",
+            server_request: str = "medium-cpu",
+        ):
         """
         Starts a server with the given name.
 
         Args:
             server_name (str): The name of the server to start. If None, uses the server name set in the instance.
 
         Returns:
             Response from the server start request.
         """
         if not self.api_key:
             raise ValueError("Requires user authentication with an API Key")
         # Use set self.server_name if not provided
         if server_name is None:
             server_name = self.server_name
-        return self.client.start_server(server_name=server_name)
+        return self.client.start_server(server_name=server_name, environment=environment, server_request=server_request)
 
     def stop_server(self, server_name: str = None):
         """
         Stops a server with the given name.
 
         Args:
             server_name (str): The name of the server to stop. If None, uses the server name set in the instance.
@@ -242,14 +247,36 @@
         if not self.api_key:
             raise ValueError("Requires user authentication with an API Key")
         # Use set self.server_name if not provided
         if server_name is None:
             server_name = self.server_name
         return self.client.stop_server(server_name=server_name)
 
+    def alph(
+            self,
+            server_name: str = None,
+            messages: str = "ls",
+            engine: str = "gpt3",
+        ):
+        """
+        Gives alph commands to help you and run on the server.
+
+        Args:
+            server_name (str): The name of the server to stop. If None, uses the server name set in the instance.
+
+        Returns:
+            Response from the server stop request.
+        """
+        if not self.api_key:
+            raise ValueError("Requires user authentication with an API Key")
+        # Use set self.server_name if not provided
+        if server_name is None:
+            server_name = self.server_name
+        return self.client.alph(server_name=server_name, messages=messages, engine=engine)
+
     def upload(self, server_name: str = None, file_path: str = "", remote_path=""):
         """
         Uploads a file to a remote server.
 
         Args:
             server_name (str): The name of the server to which the file will be uploaded. If None, uses the server name set in the instance.
             file_path (str): The local path to the file.
```

### Comparing `alphai-0.0.6/src/alphai/benchmarking/benchmarker.py` & `alphai-0.0.7/src/alphai/benchmarking/benchmarker.py`

 * *Files identical despite different names*

### Comparing `alphai-0.0.6/src/alphai/client/client.py` & `alphai-0.0.7/src/alphai/client/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 from pprint import pprint
 
 
 class Client:
     def __init__(
         self,
         host: str = "https://lab.amdatascience.com",
+        dashboard_url: str = "https://dashboard.amdatascience.com",
         access_token=None,
     ):
         self.host = host
+        self.dashboard_url = dashboard_url
         self.access_token = access_token
         self.configuration = jh_client.Configuration(host=f"{host}/hub/api")
         self.configuration.access_token = access_token
 
         # Enter a context with an instance of the API client
         self.api_client = jh_client.ApiClient(self.configuration)
         # Create an instance of the API class
@@ -69,61 +71,130 @@
                 "ready": v["ready"],
                 "url": v["url"],
                 "last_activity": v["last_activity"],
             }
             for k, v in servers.items()
         }
 
-    # JH Client
-    def start_server(self, server_name: str = "", options: dict = None):
+    # Dashboard Client
+    def start_server(
+            self,
+            server_name: str = "",
+            environment: str = "ai",
+            server_request: str = "medium-cpu",
+        ):
+
         # Start Server given name
-        # str | name given to a named-server.  Note that depending on your JupyterHub infrastructure there are chracterter size limitation to `server_name`. Default spawner with K8s pod will not allow Jupyter Notebooks to be spawned with a name that contains more than 253 characters (keep in mind that the pod will be spawned with extra characters to identify the user and hub).
-        # object | Spawn options can be passed as a JSON body when spawning via the API instead of spawn form. The structure of the options will depend on the Spawner's configuration.  (optional)
-        server_url = (
-            f"{self.host}/user/{self.user_name}/{urllib.parse.quote(server_name)}"
-        )
-        server_pending_url = f"{self.host}/hub/spawn-pending/{self.user_name}/{urllib.parse.quote(server_name)}"
-        server_pending_url = (
-            server_pending_url[:-1]
-            if server_pending_url[-1] == "/"
-            else server_pending_url
+        # Data to be sent in POST request
+        data = {
+            "server_name": server_name,
+            "environment": environment,
+            "server_request": server_request,
+            "port": 5000,
+        }
+
+        url = f"{self.dashboard_url}/api/server"
+        headers = {
+            "apikey": f"{self.access_token}",
+            'Accept': 'application/json'
+        }
+
+        response = requests.post(
+            url,
+            json=data,
+            headers=headers,
         )
+
+        # If the response is JSON
         try:
-            # Start a user's single-user named-server notebook server
-            resp_start_server = self.api_instance.users_name_servers_server_name_post(
-                self.user_name, server_name, options=options
-            )
-            print(f"Jupyter Lab Server Starting! Link-> {server_pending_url}")
-        except Exception as e:
-            print(
-                "Exception when calling DefaultApi->users_name_servers_server_name_post: %s\n"
-                % e
-            )
-            return
+            response_data = response.json()
+            return response_data
+        except ValueError:
+            print("Response is not in JSON format")
 
-        return resp_start_server
 
     def stop_server(self, server_name: str = ""):
-        # Start Server given name
-        # str | name given to a named-server.  Note that depending on your JupyterHub infrastructure there are chracterter size limitation to `server_name`. Default spawner with K8s pod will not allow Jupyter Notebooks to be spawned with a name that contains more than 253 characters (keep in mind that the pod will be spawned with extra characters to identify the user and hub).
-        # object | Spawn options can be passed as a JSON body when spawning via the API instead of spawn form. The structure of the options will depend on the Spawner's configuration.  (optional)
+        # Stop Server given name
+        # Data to be sent in POST request
+        if not server_name:
+            server_name = "default"
+        data = {
+            "stop": True,
+        }
+
+        url = f"{self.dashboard_url}/api/server/{server_name}"
+        headers = {
+            "apikey": f"{self.access_token}",
+            'Accept': 'application/json'
+            }
 
+        response = requests.post(
+            url,
+            json=data,
+            headers=headers,
+        )
+
+        # If the response is JSON
         try:
-            # Start a user's single-user named-server notebook server
-            resp_start_server = self.api_instance.users_name_servers_server_name_delete(
-                self.user_name, server_name
-            )
-        except Exception as e:
-            print(
-                "Exception when calling DefaultApi->users_name_servers_server_name_delete: %s\n"
-                % e
-            )
-            return
+            response_data = response.json()
+            return response_data
+        except ValueError:
+            print("Response is not in JSON format")
+
+    def alph(
+            self,
+            server_name: str = "",
+            messages: str | list = "Hi Alph.",
+            engine: str = "gpt3",
+        ):
+
+        # Agent Alph call
+        # Data to be sent in POST request
+        if isinstance(messages, str):
+            data = {
+                "messages": [
+                    {"role": "user", "content": messages}
+                ],
+            }
+        else:
+            data = {
+                "messages": messages
+            }
 
-        return resp_start_server
+        url = f"{self.dashboard_url}/api/alph/{server_name}/{engine}"
+        headers = {
+            "apikey": f"{self.access_token}",
+            'Accept': 'application/json'
+        }
+
+        response = requests.post(
+            url,
+            json=data,
+            headers=headers,
+            stream=True
+        )
+
+        # If the response is JSON
+        #try:
+        if response.encoding is None:
+            response.encoding = 'utf-8'
+
+        full_output = []
+        try:
+            for line in response.iter_lines(decode_unicode=True):
+                if line:
+                    #import pdb; pdb.set_trace()
+                    split_line = line.split(':')
+                    cleaned_line = split_line[1].replace('"', '')
+                    print(cleaned_line, end="")
+                    full_output.append(cleaned_line)
+        except ValueError:
+            print("Response encoded incorrectly.")
+        
+        return "".join(full_output)
 
     # NB server client
     def get_contents(self, server_name: str = ""):
         if server_name != self.server_name:
             self.initialize_server(server_name=server_name)
         path = ""  # str | file path
         type = None  # str | File type ('file', 'directory') (optional)
```

### Comparing `alphai-0.0.6/src/alphai/profilers/jax.py` & `alphai-0.0.7/src/alphai/profilers/jax.py`

 * *Files identical despite different names*

### Comparing `alphai-0.0.6/src/alphai/profilers/pytorch.py` & `alphai-0.0.7/src/alphai/profilers/pytorch.py`

 * *Files identical despite different names*

### Comparing `alphai-0.0.6/src/alphai/profilers/pytorch_utils.py` & `alphai-0.0.7/src/alphai/profilers/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `alphai-0.0.6/PKG-INFO` & `alphai-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphai
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: Andrew Chang
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

