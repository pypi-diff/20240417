# Comparing `tmp/socktalk-0.2.0.tar.gz` & `tmp/socktalk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socktalk-0.2.0.tar", last modified: Tue Apr 16 19:50:52 2024, max compression
+gzip compressed data, was "socktalk-0.2.1.tar", last modified: Tue Apr 16 23:01:48 2024, max compression
```

## Comparing `socktalk-0.2.0.tar` & `socktalk-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-16 19:50:52.986607 socktalk-0.2.0/
--rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.2.0/LICENSE
--rw-r--r--   0 mike      (1000) mike      (1000)     5014 2024-04-16 19:50:52.986607 socktalk-0.2.0/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     4015 2024-04-16 19:48:25.000000 socktalk-0.2.0/README.md
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-16 19:50:52.986607 socktalk-0.2.0/server_client/
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.2.0/server_client/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     5489 2024-04-16 17:07:47.000000 socktalk-0.2.0/server_client/ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.2.0/server_client/client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      614 2024-04-16 16:42:54.000000 socktalk-0.2.0/server_client/main.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2832 2024-04-16 19:45:03.000000 socktalk-0.2.0/server_client/new_main.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4739 2024-04-16 17:05:12.000000 socktalk-0.2.0/server_client/server.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3456 2024-04-11 11:27:09.000000 socktalk-0.2.0/server_client/start_server_with_ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2779 2024-04-16 18:48:07.000000 socktalk-0.2.0/server_client/terminal_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-16 19:50:52.986607 socktalk-0.2.0/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     1320 2024-04-11 17:50:39.000000 socktalk-0.2.0/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-16 19:50:52.986607 socktalk-0.2.0/socktalk.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)     5014 2024-04-16 19:50:52.000000 socktalk-0.2.0/socktalk.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      447 2024-04-16 19:50:52.000000 socktalk-0.2.0/socktalk.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-16 19:50:52.000000 socktalk-0.2.0/socktalk.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       53 2024-04-16 19:50:52.000000 socktalk-0.2.0/socktalk.egg-info/entry_points.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      301 2024-04-16 19:50:52.000000 socktalk-0.2.0/socktalk.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-16 19:50:52.000000 socktalk-0.2.0/socktalk.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-16 23:01:48.714338 socktalk-0.2.1/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.2.1/LICENSE
+-rw-r--r--   0 mike      (1000) mike      (1000)     4459 2024-04-16 23:01:48.714338 socktalk-0.2.1/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3297 2024-04-16 23:01:16.000000 socktalk-0.2.1/README.md
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-16 23:01:48.714338 socktalk-0.2.1/server_client/
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.2.1/server_client/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5489 2024-04-16 17:07:47.000000 socktalk-0.2.1/server_client/ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.2.1/server_client/client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4428 2024-04-16 22:38:18.000000 socktalk-0.2.1/server_client/main.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4739 2024-04-16 17:05:12.000000 socktalk-0.2.1/server_client/server.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2343 2024-04-16 22:03:43.000000 socktalk-0.2.1/server_client/start_server_with_ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2779 2024-04-16 18:48:07.000000 socktalk-0.2.1/server_client/terminal_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-16 23:01:48.714338 socktalk-0.2.1/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1514 2024-04-16 20:51:36.000000 socktalk-0.2.1/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-16 23:01:48.714338 socktalk-0.2.1/socktalk.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)     4459 2024-04-16 23:01:48.000000 socktalk-0.2.1/socktalk.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      421 2024-04-16 23:01:48.000000 socktalk-0.2.1/socktalk.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-16 23:01:48.000000 socktalk-0.2.1/socktalk.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       53 2024-04-16 23:01:48.000000 socktalk-0.2.1/socktalk.egg-info/entry_points.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      301 2024-04-16 23:01:48.000000 socktalk-0.2.1/socktalk.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-16 23:01:48.000000 socktalk-0.2.1/socktalk.egg-info/top_level.txt
```

### Comparing `socktalk-0.2.0/LICENSE` & `socktalk-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `socktalk-0.2.0/server_client/ai_client.py` & `socktalk-0.2.1/server_client/ai_client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.2.0/server_client/client.py` & `socktalk-0.2.1/server_client/client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.2.0/server_client/server.py` & `socktalk-0.2.1/server_client/server.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.2.0/server_client/start_server_with_ai_client.py` & `socktalk-0.2.1/server_client/start_server_with_ai_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,24 @@
 import threading
 import time
 import os
 from server_client.server import ChatServer
 from server_client.ai_client import AIChatClient
 
 
-def load_env_variables(filename='.env'):
-    try:
-        with open(filename) as f:
-            for line in f:
-                if line.strip() and not line.startswith('#'):
-                    key, value = line.strip().split('=', 1)
-                    os.environ[key] = value
-    except FileNotFoundError:
-        pass
-
-
 def start_server(ip, port):
     server = ChatServer(ip, port)
     server.run()
 
 
 def main(server_ip_address="127.0.0.1", server_port=1234, send_full_chat_history=True, ai_mode1_active=True,
          ai_mode1_interval=1, ai_mode1_model="gpt-3.5-turbo", ai_mode2_active=True, ai_mode2_interval=60,
          ai_mode2_model="gpt-3.5-turbo", ai_mode2_content="Say something interesting from a random Wikipedia page and"
                                                        " start your response with 'Did you know', but don't mention the"
                                                        " source."):
-    load_env_variables()
-
-    server_ip_address = os.getenv("SERVER_IP_ADDRESS", server_ip_address)
-    server_port = int(os.getenv("SERVER_PORT", server_port))
-    send_full_chat_history = os.getenv("SEND_FULL_CHAT_HISTORY", str(send_full_chat_history)) == "True"
-    ai_mode1_active = os.getenv("AI_MODE1_ACTIVE", str(ai_mode1_active)) == "True"
-    ai_mode1_interval = int(os.getenv("AI_MODE1_INTERVAL", ai_mode1_interval))
-    ai_mode1_model = os.getenv("AI_MODE1_MODEL", ai_mode1_model)
-    ai_mode2_active = os.getenv("AI_MODE2_ACTIVE", str(ai_mode2_active)) == "True"
-    ai_mode2_interval = int(os.getenv("AI_MODE2_INTERVAL", ai_mode2_interval))
-    ai_mode2_model = os.getenv("AI_MODE2_MODEL", ai_mode2_model)
-    ai_mode2_content = os.getenv("AI_MODE2_CONTENT", ai_mode2_content)
 
     server = ChatServer(server_ip_address, server_port)
     server_thread = threading.Thread(target=server.run)
     server_thread.start()
     print("AI chat server is running...")
     time.sleep(1)
 
@@ -74,8 +51,8 @@
     ai_mode2_active = True
     ai_mode2_interval = 60
     ai_mode2_model = "gpt-3.5-turbo"
     ai_mode2_content= ("Say something interesting from a random Wikipedia page and start your response with"
                        " 'Did you know', but don't mention the source.")
 
     main(server_ip_address, server_port, send_full_chat_history, ai_mode1_active, ai_mode1_interval, ai_mode1_model,
-         ai_mode2_active, ai_mode2_interval, ai_mode2_model, ai_mode2_content)
+         ai_mode2_active, ai_mode2_interval, ai_mode2_model, ai_mode2_content)
```

### Comparing `socktalk-0.2.0/server_client/terminal_client.py` & `socktalk-0.2.1/server_client/terminal_client.py`

 * *Files identical despite different names*

