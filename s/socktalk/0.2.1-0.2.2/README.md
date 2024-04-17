# Comparing `tmp/socktalk-0.2.1.tar.gz` & `tmp/socktalk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socktalk-0.2.1.tar", last modified: Tue Apr 16 23:01:48 2024, max compression
+gzip compressed data, was "socktalk-0.2.2.tar", last modified: Wed Apr 17 11:13:16 2024, max compression
```

## Comparing `socktalk-0.2.1.tar` & `socktalk-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-16 23:01:48.714338 socktalk-0.2.1/
--rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.2.1/LICENSE
--rw-r--r--   0 mike      (1000) mike      (1000)     4459 2024-04-16 23:01:48.714338 socktalk-0.2.1/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     3297 2024-04-16 23:01:16.000000 socktalk-0.2.1/README.md
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-16 23:01:48.714338 socktalk-0.2.1/server_client/
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.2.1/server_client/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     5489 2024-04-16 17:07:47.000000 socktalk-0.2.1/server_client/ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.2.1/server_client/client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4428 2024-04-16 22:38:18.000000 socktalk-0.2.1/server_client/main.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4739 2024-04-16 17:05:12.000000 socktalk-0.2.1/server_client/server.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2343 2024-04-16 22:03:43.000000 socktalk-0.2.1/server_client/start_server_with_ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2779 2024-04-16 18:48:07.000000 socktalk-0.2.1/server_client/terminal_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-16 23:01:48.714338 socktalk-0.2.1/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     1514 2024-04-16 20:51:36.000000 socktalk-0.2.1/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-16 23:01:48.714338 socktalk-0.2.1/socktalk.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)     4459 2024-04-16 23:01:48.000000 socktalk-0.2.1/socktalk.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      421 2024-04-16 23:01:48.000000 socktalk-0.2.1/socktalk.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-16 23:01:48.000000 socktalk-0.2.1/socktalk.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       53 2024-04-16 23:01:48.000000 socktalk-0.2.1/socktalk.egg-info/entry_points.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      301 2024-04-16 23:01:48.000000 socktalk-0.2.1/socktalk.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-16 23:01:48.000000 socktalk-0.2.1/socktalk.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-17 11:13:16.392234 socktalk-0.2.2/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.2.2/LICENSE
+-rw-r--r--   0 mike      (1000) mike      (1000)     4695 2024-04-17 11:13:16.392234 socktalk-0.2.2/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3533 2024-04-17 11:12:11.000000 socktalk-0.2.2/README.md
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-17 11:13:16.392234 socktalk-0.2.2/server_client/
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.2.2/server_client/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5489 2024-04-16 17:07:47.000000 socktalk-0.2.2/server_client/ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5973 2024-04-17 10:50:20.000000 socktalk-0.2.2/server_client/client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4627 2024-04-17 10:48:45.000000 socktalk-0.2.2/server_client/main.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4577 2024-04-17 10:50:45.000000 socktalk-0.2.2/server_client/server.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2303 2024-04-17 10:49:28.000000 socktalk-0.2.2/server_client/start_server_with_ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2791 2024-04-17 10:51:24.000000 socktalk-0.2.2/server_client/terminal_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-17 11:13:16.392234 socktalk-0.2.2/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1514 2024-04-17 10:24:13.000000 socktalk-0.2.2/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-17 11:13:16.392234 socktalk-0.2.2/socktalk.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)     4695 2024-04-17 11:13:16.000000 socktalk-0.2.2/socktalk.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      421 2024-04-17 11:13:16.000000 socktalk-0.2.2/socktalk.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-17 11:13:16.000000 socktalk-0.2.2/socktalk.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       53 2024-04-17 11:13:16.000000 socktalk-0.2.2/socktalk.egg-info/entry_points.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      301 2024-04-17 11:13:16.000000 socktalk-0.2.2/socktalk.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-17 11:13:16.000000 socktalk-0.2.2/socktalk.egg-info/top_level.txt
```

### Comparing `socktalk-0.2.1/LICENSE` & `socktalk-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `socktalk-0.2.1/PKG-INFO` & `socktalk-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socktalk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Socket-based AI chat server and multi-user chat client
 Project-URL: Source, https://github.com/mdkmk/socktalk
 Keywords: chat server,chat client,AI chatbot,chatGPT,OPENAI API,socket programming,select.select(),multi-user chat,real-time communication,Python chat application
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -27,20 +27,20 @@
 Requires-Dist: PyQt5-sip==12.13.0
 Requires-Dist: sniffio==1.3.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: typing_extensions==4.11.0
 
 # socktalk - A Robust Socket-based AI Chat Server and Multi-user Chat Client
 
-**socktalk** is a sophisticated chat server framework developed using Python's socket programming. It facilitates real-time, multi-user interactions and integrates with OpenAI's GPT models to offer an AI-driven chatting experience. This makes it suitable for both educational purposes and practical applications.
+**socktalk** is a chat server and client developed using Python's socket programming. It affords real-time, multi-user interactions and integrates with OpenAI's GPT models to offer an AI-driven chatting experience.
 
 ## Features
-- **Multi-User Support**: Manages multiple connections simultaneously to support extensive user interactions.
-- **Efficient Message Handling**: Utilizes non-blocking sockets and `select.select()` for real-time, concurrent message processing.
-- **AI Integration**: Enhances chat functionalities with AI-driven responses, configurable for different operational modes.
+- **Multi-User Support**: Manages multiple connections simultaneously to support multi-user interactions.
+- **Efficient Message Handling**: Uses non-blocking sockets and `select.select()` for real-time, concurrent message processing.
+- **AI Integration**: Augments multi-user chat with AI-driven responses, configurable for different operational modes.
 - **Standardized Protocol**: Implements a simple message protocol with fixed-length headers to streamline communication.
 - **Versatile Client Options**: Offers both a sophisticated graphical user interface and a lightweight terminal-based client.
 
 For further details, visit the [GitHub repository for socktalk](https://github.com/mdkmk/socktalk/tree/main).
 ## Installation
 
 ### From GitHub
@@ -55,33 +55,52 @@
 
 ### Using pip
 - To install using pip directly from PyPI:
     ```bash
     pip install socktalk
 
 ## Usage - Run different components of "socktalk" using the following commands:
-- AI-enhanced chat server:  
-Set up the .env file in your working directory to configure AI behaviors and server settings.
-    ```bash
-    socktalk --ai
-    ```
-    Alternatively, override .env settings using command-line flags:
-    ```bash
-    socktalk --ai --openai_api_key=YOUR_OPENAI_API_KEY_HERE --ai_mode2_active=False --ai_mode1_interval=3
-    ```
-- Chat server without AI integration:
-     ```bash
-    socktalk --server
-- GUI-enabled multi-user chat client:
-     ```bash
-    socktalk --client
-- Terminal-based chat client:
-    ```bash
-    socktalk --terminal
-   
+Set up the .env file in your working directory to configure AI behaviors and server/client settings without using command-line flags.
+Alternatively, you can use command-line flags to override .env or default settings.
+### **AI-enhanced chat server:**
+```bash
+socktalk --ai
+```
+With flag override:
+```bash
+socktalk --ai --openai_api_key=YOUR_OPENAI_API_KEY_HERE --ai_mode2_active=False --ai_mode1_interval=3
+```
+---
+### **Chat server without AI integration:**
+```bash
+socktalk --server
+```
+With flag override:
+```bash
+socktalk --server --server_ip=127.0.0.1 --server_port=1234
+```
+---
+### **GUI-enabled multi-user chat client:**
+```bash
+socktalk --client
+```
+With flag override:
+```bash
+socktalk --client --server_ip=127.0.0.1 --server_port=1234
+```
+---
+### **Terminal-based chat client:**
+```bash
+socktalk --terminal
+```
+With flag override:
+```bash
+socktalk --terminal --server_ip=127.0.0.1 --server_port=1234
+```
+---
 ## AI Chatbot Configuration
 ### AI Client Modes:
 1. Respond every N lines: The AI reads the conversation and responds after every N lines.
 2. Respond every N seconds: The AI generates new content at specified intervals.
 
 ### Example .env File Configuration
  Below is an example .env file. Update the OpenAI chatgpt API key and ensure you have at least $5 credit on your OpenAI account.
```

### Comparing `socktalk-0.2.1/README.md` & `socktalk-0.2.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # socktalk - A Robust Socket-based AI Chat Server and Multi-user Chat Client
 
-**socktalk** is a sophisticated chat server framework developed using Python's socket programming. It facilitates real-time, multi-user interactions and integrates with OpenAI's GPT models to offer an AI-driven chatting experience. This makes it suitable for both educational purposes and practical applications.
+**socktalk** is a chat server and client developed using Python's socket programming. It affords real-time, multi-user interactions and integrates with OpenAI's GPT models to offer an AI-driven chatting experience.
 
 ## Features
-- **Multi-User Support**: Manages multiple connections simultaneously to support extensive user interactions.
-- **Efficient Message Handling**: Utilizes non-blocking sockets and `select.select()` for real-time, concurrent message processing.
-- **AI Integration**: Enhances chat functionalities with AI-driven responses, configurable for different operational modes.
+- **Multi-User Support**: Manages multiple connections simultaneously to support multi-user interactions.
+- **Efficient Message Handling**: Uses non-blocking sockets and `select.select()` for real-time, concurrent message processing.
+- **AI Integration**: Augments multi-user chat with AI-driven responses, configurable for different operational modes.
 - **Standardized Protocol**: Implements a simple message protocol with fixed-length headers to streamline communication.
 - **Versatile Client Options**: Offers both a sophisticated graphical user interface and a lightweight terminal-based client.
 
 For further details, visit the [GitHub repository for socktalk](https://github.com/mdkmk/socktalk/tree/main).
 ## Installation
 
 ### From GitHub
@@ -24,33 +24,52 @@
 
 ### Using pip
 - To install using pip directly from PyPI:
     ```bash
     pip install socktalk
 
 ## Usage - Run different components of "socktalk" using the following commands:
-- AI-enhanced chat server:  
-Set up the .env file in your working directory to configure AI behaviors and server settings.
-    ```bash
-    socktalk --ai
-    ```
-    Alternatively, override .env settings using command-line flags:
-    ```bash
-    socktalk --ai --openai_api_key=YOUR_OPENAI_API_KEY_HERE --ai_mode2_active=False --ai_mode1_interval=3
-    ```
-- Chat server without AI integration:
-     ```bash
-    socktalk --server
-- GUI-enabled multi-user chat client:
-     ```bash
-    socktalk --client
-- Terminal-based chat client:
-    ```bash
-    socktalk --terminal
-   
+Set up the .env file in your working directory to configure AI behaviors and server/client settings without using command-line flags.
+Alternatively, you can use command-line flags to override .env or default settings.
+### **AI-enhanced chat server:**
+```bash
+socktalk --ai
+```
+With flag override:
+```bash
+socktalk --ai --openai_api_key=YOUR_OPENAI_API_KEY_HERE --ai_mode2_active=False --ai_mode1_interval=3
+```
+---
+### **Chat server without AI integration:**
+```bash
+socktalk --server
+```
+With flag override:
+```bash
+socktalk --server --server_ip=127.0.0.1 --server_port=1234
+```
+---
+### **GUI-enabled multi-user chat client:**
+```bash
+socktalk --client
+```
+With flag override:
+```bash
+socktalk --client --server_ip=127.0.0.1 --server_port=1234
+```
+---
+### **Terminal-based chat client:**
+```bash
+socktalk --terminal
+```
+With flag override:
+```bash
+socktalk --terminal --server_ip=127.0.0.1 --server_port=1234
+```
+---
 ## AI Chatbot Configuration
 ### AI Client Modes:
 1. Respond every N lines: The AI reads the conversation and responds after every N lines.
 2. Respond every N seconds: The AI generates new content at specified intervals.
 
 ### Example .env File Configuration
  Below is an example .env file. Update the OpenAI chatgpt API key and ensure you have at least $5 credit on your OpenAI account.
```

### Comparing `socktalk-0.2.1/server_client/ai_client.py` & `socktalk-0.2.2/server_client/ai_client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.2.1/server_client/client.py` & `socktalk-0.2.2/server_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,24 +137,24 @@
 
     def closeEvent(self, event):
         if self.receiver_thread.isRunning():
             self.receiver_thread.stop()
             self.client_socket.close()
         event.accept()
 
-def main():
+
+def main(server_ip, server_port):
     app = QApplication(sys.argv)
     username = input("Enter your username: ")
-    server_ip = input("Enter server IP (for default 127.0.0.1, press enter): ") or "127.0.0.1"
-    server_port = input("Enter server port (for default 1234, press enter): ") or "1234"
     server_port = int(server_port)
     client = ChatClient(server_ip, server_port, username)
     print("Chat client is running...")
     client.show()
     sys.exit(app.exec_())
 
+
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     username = input("Enter your username: ")
     client = ChatClient("127.0.0.1", 1234, username)
     client.show()
     sys.exit(app.exec_())
```

### Comparing `socktalk-0.2.1/server_client/main.py` & `socktalk-0.2.2/server_client/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     parser = argparse.ArgumentParser(description='Run different parts of the chat application.')
     parser.add_argument('--ai', action='store_true', help='Run the AI server.')
     parser.add_argument('--server', action='store_true', help='Run the server.')
     parser.add_argument('--client', action='store_true', help='Run the client.')
     parser.add_argument('--terminal', action='store_true', help='Run the terminal client.')
 
     # Optional settings for the AI server
-    parser.add_argument('--server_ip_address', type=str, default=os.getenv("SERVER_IP_ADDRESS", "127.0.0.1"),
+    parser.add_argument('--server_ip', type=str, default=os.getenv("SERVER_IP", "127.0.0.1"),
                         help='IP address of the server')
     parser.add_argument('--server_port', type=int, default=int(os.getenv("SERVER_PORT", 1234)),
                         help='Port number of the server')
     parser.add_argument('--send_full_chat_history', type=lambda x: (str(x).lower() in ['true', '1', 't']),
                         default=os.getenv("SEND_FULL_CHAT_HISTORY", "True") == "True",
                         help='Whether to send full chat history')
     parser.add_argument('--ai_mode1_active', type=lambda x: (str(x).lower() in ['true', '1', 't']),
@@ -56,29 +56,32 @@
 
     args = parser.parse_args()
 
     if args.ai:
         if args.openai_api_key:
             os.environ['OPENAI_API_KEY'] = args.openai_api_key
 
-        ai_server_main(server_ip_address=args.server_ip_address,
+        ai_server_main(server_ip=args.server_ip,
                        server_port=args.server_port,
                        send_full_chat_history=args.send_full_chat_history,
                        ai_mode1_active=args.ai_mode1_active,
                        ai_mode1_interval=args.ai_mode1_interval,
                        ai_mode1_model=args.ai_mode1_model,
                        ai_mode2_active=args.ai_mode2_active,
                        ai_mode2_interval=args.ai_mode2_interval,
                        ai_mode2_model=args.ai_mode2_model,
                        ai_mode2_content=args.ai_mode2_content)
     elif args.server:
-        server_main()
+        server_main(server_ip=args.server_ip,
+                       server_port=args.server_port)
     elif args.client:
-        client_main()
+        client_main(server_ip=args.server_ip,
+                       server_port=args.server_port)
     elif args.terminal:
-        terminal_client_main()
+        terminal_client_main(server_ip=args.server_ip,
+                       server_port=args.server_port)
     else:
         parser.print_help()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `socktalk-0.2.1/server_client/server.py` & `socktalk-0.2.2/server_client/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,15 @@
                 client_socket.send(message_header + message_encoded)
 
     def shutdown(self):
         self.running = False
         self.server_socket.close()
 
 
-def main():
-    server_ip = input("Enter server IP (for default 127.0.0.1, press enter): ") or "127.0.0.1"
-    server_port = input("Enter server port (for default 1234, press enter): ") or "1234"
+def main(server_ip, server_port):
     server_port = int(server_port)
     server = ChatServer(server_ip, server_port)
 
     try:
         print("Chat server is running...")
         server.run()
     except KeyboardInterrupt:
```

### Comparing `socktalk-0.2.1/server_client/start_server_with_ai_client.py` & `socktalk-0.2.2/server_client/start_server_with_ai_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def start_server(ip, port):
     server = ChatServer(ip, port)
     server.run()
 
 
-def main(server_ip_address="127.0.0.1", server_port=1234, send_full_chat_history=True, ai_mode1_active=True,
+def main(server_ip="127.0.0.1", server_port=1234, send_full_chat_history=True, ai_mode1_active=True,
          ai_mode1_interval=1, ai_mode1_model="gpt-3.5-turbo", ai_mode2_active=True, ai_mode2_interval=60,
          ai_mode2_model="gpt-3.5-turbo", ai_mode2_content="Say something interesting from a random Wikipedia page and"
                                                        " start your response with 'Did you know', but don't mention the"
                                                        " source."):
 
-    server = ChatServer(server_ip_address, server_port)
+    server = ChatServer(server_ip, server_port)
     server_thread = threading.Thread(target=server.run)
     server_thread.start()
     print("AI chat server is running...")
     time.sleep(1)
 
     if ai_mode1_active or ai_mode2_active:
         username = "AI"
-        ai_client = AIChatClient(server, server_ip_address, server_port, username, ai_mode1_active, ai_mode1_interval,
+        ai_client = AIChatClient(server, server_ip, server_port, username, ai_mode1_active, ai_mode1_interval,
                                  ai_mode1_model, ai_mode2_active, ai_mode2_interval, ai_mode2_model,
                                  send_full_chat_history, ai_mode2_content)
         threading.Thread(target=ai_client.receive_message).start()
 
     try:
         server_thread.join()
     except KeyboardInterrupt:
@@ -36,23 +36,23 @@
         server.shutdown()
         if ai_client:
             ai_client.shutdown()
         server_thread.join()
 
 
 if __name__ == '__main__':
-    server_ip_address = "127.0.0.1"
+    server_ip = "127.0.0.1"
     server_port = 1234
 
     os.environ['OPENAI_API_KEY'] = "<OPENAI_API_KEY_HERE>"
     send_full_chat_history = True
     ai_mode1_active = True
     ai_mode1_interval = 1
     ai_mode1_model = "gpt-3.5-turbo"
     ai_mode2_active = True
     ai_mode2_interval = 60
     ai_mode2_model = "gpt-3.5-turbo"
     ai_mode2_content= ("Say something interesting from a random Wikipedia page and start your response with"
                        " 'Did you know', but don't mention the source.")
 
-    main(server_ip_address, server_port, send_full_chat_history, ai_mode1_active, ai_mode1_interval, ai_mode1_model,
+    main(server_ip, server_port, send_full_chat_history, ai_mode1_active, ai_mode1_interval, ai_mode1_model,
          ai_mode2_active, ai_mode2_interval, ai_mode2_model, ai_mode2_content)
```

### Comparing `socktalk-0.2.1/server_client/terminal_client.py` & `socktalk-0.2.2/server_client/terminal_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import socket
 import sys
 import threading
 import errno
 
 class ReceiverThread(threading.Thread):
-    def __init__(self, client_socket, header_length):
+    def __init__(self, client_socket, header_length, username):
         super().__init__()
         self.client_socket = client_socket
         self.header_length = header_length
+        self.username = username
         self.running = True
 
     def run(self):
         while self.running:
             try:
                 while True:
                     message_header = self.client_socket.recv(self.header_length)
                     if not len(message_header):
                         if self.running:
                             print("\nConnection closed by the server")
                         self.running = False
                         return
                     message_length = int(message_header.decode("utf-8").strip())
                     message = self.client_socket.recv(message_length).decode("utf-8")
-                    current_username, _, _ = message.partition(' > ')
-                    print("\r" + message + f"\n{username} > ", end="")
+                    print("\r" + message + f"\n{self.username} > ", end="")
                     sys.stdout.flush()
             except IOError as e:
                 if e.errno != errno.EAGAIN and e.errno != errno.EWOULDBLOCK:
                     print("\nReading error", str(e))
                     self.running = False
                     return
                 continue
@@ -36,40 +36,39 @@
                 self.running = False
                 return
 
     def stop(self):
         self.running = False
         self.join()
 
-def main():
-    global username
+def main(server_ip, server_port):
     HEADER_LENGTH = 10
     username = input("Enter your username: ")
-    server_ip = input("Enter server IP (for default 127.0.0.1, press enter): ") or "127.0.0.1"
-    server_port = input("Enter server port (for default 1234, press enter): ") or "1234"
     server_port = int(server_port)
     print("Chat client is running...")
 
     client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     client_socket.connect((server_ip, server_port))
     client_socket.setblocking(False)
 
     username_encoded = username.encode("utf-8")
     username_header = f"{len(username_encoded):<{HEADER_LENGTH}}".encode("utf-8")
     client_socket.send(username_header + username_encoded)
 
-    receiver_thread = ReceiverThread(client_socket, HEADER_LENGTH)
+    receiver_thread = ReceiverThread(client_socket, HEADER_LENGTH, username)
     receiver_thread.start()
 
     try:
         while True:
             message = input(f"{username} > ")
             if message:
                 message_encoded = message.encode("utf-8")
                 message_header = f"{len(message_encoded):<{HEADER_LENGTH}}".encode("utf-8")
                 client_socket.send(message_header + message_encoded)
     except KeyboardInterrupt:
         print("\nShutting down...")
         receiver_thread.stop()
 
 if __name__ == '__main__':
-    main()
+    server_ip = input("Enter server IP (for default 127.0.0.1, press enter): ") or "127.0.0.1"
+    server_port = input("Enter server port (for default 1234, press enter): ") or "1234"
+    main(server_ip, server_port)
```

### Comparing `socktalk-0.2.1/setup.py` & `socktalk-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='socktalk',
-    version='0.2.1',
+    version='0.2.2',
     packages=find_packages(),
     project_urls={
         'Source': 'https://github.com/mdkmk/socktalk'
     },
     install_requires=[
         'annotated-types==0.6.0',
         'anyio==4.3.0',
```

### Comparing `socktalk-0.2.1/socktalk.egg-info/PKG-INFO` & `socktalk-0.2.2/socktalk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socktalk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Socket-based AI chat server and multi-user chat client
 Project-URL: Source, https://github.com/mdkmk/socktalk
 Keywords: chat server,chat client,AI chatbot,chatGPT,OPENAI API,socket programming,select.select(),multi-user chat,real-time communication,Python chat application
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -27,20 +27,20 @@
 Requires-Dist: PyQt5-sip==12.13.0
 Requires-Dist: sniffio==1.3.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: typing_extensions==4.11.0
 
 # socktalk - A Robust Socket-based AI Chat Server and Multi-user Chat Client
 
-**socktalk** is a sophisticated chat server framework developed using Python's socket programming. It facilitates real-time, multi-user interactions and integrates with OpenAI's GPT models to offer an AI-driven chatting experience. This makes it suitable for both educational purposes and practical applications.
+**socktalk** is a chat server and client developed using Python's socket programming. It affords real-time, multi-user interactions and integrates with OpenAI's GPT models to offer an AI-driven chatting experience.
 
 ## Features
-- **Multi-User Support**: Manages multiple connections simultaneously to support extensive user interactions.
-- **Efficient Message Handling**: Utilizes non-blocking sockets and `select.select()` for real-time, concurrent message processing.
-- **AI Integration**: Enhances chat functionalities with AI-driven responses, configurable for different operational modes.
+- **Multi-User Support**: Manages multiple connections simultaneously to support multi-user interactions.
+- **Efficient Message Handling**: Uses non-blocking sockets and `select.select()` for real-time, concurrent message processing.
+- **AI Integration**: Augments multi-user chat with AI-driven responses, configurable for different operational modes.
 - **Standardized Protocol**: Implements a simple message protocol with fixed-length headers to streamline communication.
 - **Versatile Client Options**: Offers both a sophisticated graphical user interface and a lightweight terminal-based client.
 
 For further details, visit the [GitHub repository for socktalk](https://github.com/mdkmk/socktalk/tree/main).
 ## Installation
 
 ### From GitHub
@@ -55,33 +55,52 @@
 
 ### Using pip
 - To install using pip directly from PyPI:
     ```bash
     pip install socktalk
 
 ## Usage - Run different components of "socktalk" using the following commands:
-- AI-enhanced chat server:  
-Set up the .env file in your working directory to configure AI behaviors and server settings.
-    ```bash
-    socktalk --ai
-    ```
-    Alternatively, override .env settings using command-line flags:
-    ```bash
-    socktalk --ai --openai_api_key=YOUR_OPENAI_API_KEY_HERE --ai_mode2_active=False --ai_mode1_interval=3
-    ```
-- Chat server without AI integration:
-     ```bash
-    socktalk --server
-- GUI-enabled multi-user chat client:
-     ```bash
-    socktalk --client
-- Terminal-based chat client:
-    ```bash
-    socktalk --terminal
-   
+Set up the .env file in your working directory to configure AI behaviors and server/client settings without using command-line flags.
+Alternatively, you can use command-line flags to override .env or default settings.
+### **AI-enhanced chat server:**
+```bash
+socktalk --ai
+```
+With flag override:
+```bash
+socktalk --ai --openai_api_key=YOUR_OPENAI_API_KEY_HERE --ai_mode2_active=False --ai_mode1_interval=3
+```
+---
+### **Chat server without AI integration:**
+```bash
+socktalk --server
+```
+With flag override:
+```bash
+socktalk --server --server_ip=127.0.0.1 --server_port=1234
+```
+---
+### **GUI-enabled multi-user chat client:**
+```bash
+socktalk --client
+```
+With flag override:
+```bash
+socktalk --client --server_ip=127.0.0.1 --server_port=1234
+```
+---
+### **Terminal-based chat client:**
+```bash
+socktalk --terminal
+```
+With flag override:
+```bash
+socktalk --terminal --server_ip=127.0.0.1 --server_port=1234
+```
+---
 ## AI Chatbot Configuration
 ### AI Client Modes:
 1. Respond every N lines: The AI reads the conversation and responds after every N lines.
 2. Respond every N seconds: The AI generates new content at specified intervals.
 
 ### Example .env File Configuration
  Below is an example .env file. Update the OpenAI chatgpt API key and ensure you have at least $5 credit on your OpenAI account.
```

