# Comparing `tmp/suvvyapi-2.0a8.tar.gz` & `tmp/suvvyapi-2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suvvyapi-2.0a8.tar", max compression
+gzip compressed data, was "suvvyapi-2.0a9.tar", max compression
```

## Comparing `suvvyapi-2.0a8.tar` & `suvvyapi-2.0a9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1088 2023-12-22 15:10:17.631455 suvvyapi-2.0a8/LICENSE
--rw-r--r--   0        0        0     1872 2024-02-26 15:26:08.263285 suvvyapi-2.0a8/README.md
--rw-r--r--   0        0        0     1455 2024-03-14 21:58:59.891807 suvvyapi-2.0a8/pyproject.toml
--rw-r--r--   0        0        0      262 2024-02-26 15:16:47.199764 suvvyapi-2.0a8/suvvyapi/__init__.py
--rw-r--r--   0        0        0      190 2023-12-25 18:31:44.995359 suvvyapi-2.0a8/suvvyapi/_utils.py
--rw-r--r--   0        0        0        0 2023-12-24 16:00:32.146606 suvvyapi-2.0a8/suvvyapi/exceptions/__init__.py
--rw-r--r--   0        0        0     1480 2023-12-26 16:31:02.473980 suvvyapi-2.0a8/suvvyapi/exceptions/api.py
--rw-r--r--   0        0        0     2867 2024-02-26 15:25:40.206896 suvvyapi-2.0a8/suvvyapi/history/__init__.py
--rw-r--r--   0        0        0        0 2023-12-24 16:00:32.147098 suvvyapi-2.0a8/suvvyapi/models/__init__.py
--rw-r--r--   0        0        0      925 2024-02-26 15:05:04.314906 suvvyapi-2.0a8/suvvyapi/models/dialogue.py
--rw-r--r--   0        0        0      277 2024-02-26 14:59:57.099818 suvvyapi-2.0a8/suvvyapi/models/enums/__init__.py
--rw-r--r--   0        0        0      285 2024-02-26 14:57:58.202549 suvvyapi-2.0a8/suvvyapi/models/enums/channel.py
--rw-r--r--   0        0        0      841 2024-03-14 07:32:58.095728 suvvyapi-2.0a8/suvvyapi/models/enums/content_type.py
--rw-r--r--   0        0        0      249 2024-03-14 07:34:22.795083 suvvyapi-2.0a8/suvvyapi/models/enums/event.py
--rw-r--r--   0        0        0      604 2024-02-26 14:59:57.093809 suvvyapi-2.0a8/suvvyapi/models/enums/reason.py
--rw-r--r--   0        0        0      663 2024-02-26 14:27:49.455263 suvvyapi-2.0a8/suvvyapi/models/enums/role.py
--rw-r--r--   0        0        0       76 2024-03-14 07:43:10.470635 suvvyapi-2.0a8/suvvyapi/models/files/__init__.py
--rw-r--r--   0        0        0     1921 2024-03-14 07:43:10.464372 suvvyapi-2.0a8/suvvyapi/models/files/file.py
--rw-r--r--   0        0        0     1469 2024-03-14 07:39:06.378944 suvvyapi-2.0a8/suvvyapi/models/message.py
--rw-r--r--   0        0        0        0 2024-03-06 17:48:36.419681 suvvyapi-2.0a8/suvvyapi/models/messages/__init__.py
--rw-r--r--   0        0        0        0 2024-03-06 17:48:36.420328 suvvyapi-2.0a8/suvvyapi/models/messages/content/__init__.py
--rw-r--r--   0        0        0      517 2024-03-14 07:41:27.048008 suvvyapi-2.0a8/suvvyapi/models/messages/content/audio.py
--rw-r--r--   0        0        0      181 2024-03-14 07:37:53.689293 suvvyapi-2.0a8/suvvyapi/models/messages/content/base.py
--rw-r--r--   0        0        0      811 2024-03-14 07:37:53.724118 suvvyapi-2.0a8/suvvyapi/models/messages/content/event.py
--rw-r--r--   0        0        0      516 2024-03-14 07:41:27.054621 suvvyapi-2.0a8/suvvyapi/models/messages/content/image.py
--rw-r--r--   0        0        0      259 2024-03-14 07:37:53.698255 suvvyapi-2.0a8/suvvyapi/models/messages/content/text.py
--rw-r--r--   0        0        0      610 2024-03-14 07:37:53.694196 suvvyapi-2.0a8/suvvyapi/models/messages/content/tool_call.py
--rw-r--r--   0        0        0      485 2024-03-14 07:37:53.714231 suvvyapi-2.0a8/suvvyapi/models/messages/content/tool_response.py
--rw-r--r--   0        0        0      472 2024-02-26 17:46:41.576453 suvvyapi-2.0a8/suvvyapi/models/token_usage.py
--rw-r--r--   0        0        0    11270 2024-03-14 21:58:59.898770 suvvyapi-2.0a8/suvvyapi/wrapper/__init__.py
--rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 suvvyapi-2.0a8/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-04-17 13:19:15.382727 suvvyapi-2.0a9/LICENSE
+-rw-r--r--   0        0        0     1872 2024-04-17 13:19:38.005207 suvvyapi-2.0a9/README.md
+-rw-r--r--   0        0        0     1455 2024-04-17 13:21:24.182339 suvvyapi-2.0a9/pyproject.toml
+-rw-r--r--   0        0        0      262 2024-04-17 13:19:38.005460 suvvyapi-2.0a9/suvvyapi/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-17 13:19:15.383418 suvvyapi-2.0a9/suvvyapi/_utils.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:19:15.383668 suvvyapi-2.0a9/suvvyapi/exceptions/__init__.py
+-rw-r--r--   0        0        0     1480 2024-04-17 13:19:15.383727 suvvyapi-2.0a9/suvvyapi/exceptions/api.py
+-rw-r--r--   0        0        0     2867 2024-04-17 13:19:38.005572 suvvyapi-2.0a9/suvvyapi/history/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:19:15.383855 suvvyapi-2.0a9/suvvyapi/models/__init__.py
+-rw-r--r--   0        0        0      925 2024-04-17 13:19:38.005647 suvvyapi-2.0a9/suvvyapi/models/dialogue.py
+-rw-r--r--   0        0        0      277 2024-04-17 13:19:38.005723 suvvyapi-2.0a9/suvvyapi/models/enums/__init__.py
+-rw-r--r--   0        0        0      285 2024-04-17 13:19:38.005776 suvvyapi-2.0a9/suvvyapi/models/enums/channel.py
+-rw-r--r--   0        0        0      841 2024-04-17 13:19:38.005831 suvvyapi-2.0a9/suvvyapi/models/enums/content_type.py
+-rw-r--r--   0        0        0      249 2024-04-17 13:19:38.005882 suvvyapi-2.0a9/suvvyapi/models/enums/event.py
+-rw-r--r--   0        0        0      604 2024-04-17 13:19:38.005933 suvvyapi-2.0a9/suvvyapi/models/enums/reason.py
+-rw-r--r--   0        0        0      663 2024-04-17 13:19:38.005983 suvvyapi-2.0a9/suvvyapi/models/enums/role.py
+-rw-r--r--   0        0        0       76 2024-04-17 13:19:38.006055 suvvyapi-2.0a9/suvvyapi/models/files/__init__.py
+-rw-r--r--   0        0        0     1921 2024-04-17 13:19:38.006107 suvvyapi-2.0a9/suvvyapi/models/files/file.py
+-rw-r--r--   0        0        0     1476 2024-04-17 13:21:08.863906 suvvyapi-2.0a9/suvvyapi/models/message.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:19:38.006203 suvvyapi-2.0a9/suvvyapi/models/messages/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:19:38.006259 suvvyapi-2.0a9/suvvyapi/models/messages/content/__init__.py
+-rw-r--r--   0        0        0      517 2024-04-17 13:19:38.006317 suvvyapi-2.0a9/suvvyapi/models/messages/content/audio.py
+-rw-r--r--   0        0        0      181 2024-04-17 13:19:38.006361 suvvyapi-2.0a9/suvvyapi/models/messages/content/base.py
+-rw-r--r--   0        0        0      811 2024-04-17 13:19:38.006406 suvvyapi-2.0a9/suvvyapi/models/messages/content/event.py
+-rw-r--r--   0        0        0      516 2024-04-17 13:19:38.006456 suvvyapi-2.0a9/suvvyapi/models/messages/content/image.py
+-rw-r--r--   0        0        0      259 2024-04-17 13:19:38.006505 suvvyapi-2.0a9/suvvyapi/models/messages/content/text.py
+-rw-r--r--   0        0        0      610 2024-04-17 13:19:38.006562 suvvyapi-2.0a9/suvvyapi/models/messages/content/tool_call.py
+-rw-r--r--   0        0        0      485 2024-04-17 13:19:38.006634 suvvyapi-2.0a9/suvvyapi/models/messages/content/tool_response.py
+-rw-r--r--   0        0        0      472 2024-04-17 13:19:38.006694 suvvyapi-2.0a9/suvvyapi/models/token_usage.py
+-rw-r--r--   0        0        0    11270 2024-04-17 13:19:38.007221 suvvyapi-2.0a9/suvvyapi/wrapper/__init__.py
+-rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 suvvyapi-2.0a9/PKG-INFO
```

### Comparing `suvvyapi-2.0a8/LICENSE` & `suvvyapi-2.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/README.md` & `suvvyapi-2.0a9/README.md`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/pyproject.toml` & `suvvyapi-2.0a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "suvvyapi"
-version = "2.0a8"
+version = "2.0a9"
 description = "A Python API wrapper for Suvvy AI API"
 authors = ["Roman Poltorabatko <barabum@duck.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["python", "wrapper", "chatgpt", "suvvy", "ai", "suvvyai"]
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `suvvyapi-2.0a8/suvvyapi/exceptions/api.py` & `suvvyapi-2.0a9/suvvyapi/exceptions/api.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/suvvyapi/history/__init__.py` & `suvvyapi-2.0a9/suvvyapi/history/__init__.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/suvvyapi/models/dialogue.py` & `suvvyapi-2.0a9/suvvyapi/models/dialogue.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/suvvyapi/models/enums/content_type.py` & `suvvyapi-2.0a9/suvvyapi/models/enums/content_type.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/suvvyapi/models/enums/reason.py` & `suvvyapi-2.0a9/suvvyapi/models/enums/reason.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/suvvyapi/models/enums/role.py` & `suvvyapi-2.0a9/suvvyapi/models/enums/role.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/suvvyapi/models/files/file.py` & `suvvyapi-2.0a9/suvvyapi/models/files/file.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/suvvyapi/models/message.py` & `suvvyapi-2.0a9/suvvyapi/models/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,12 +32,12 @@
 
 class RequestMessage(Message):
     message_sender: Literal[SenderRole.CUSTOMER, SenderRole.EMPLOYEE]
 
 
 class DialogueMessage(Message):
     message_id: UUID4 = Field(frozen=True)
-    tokens: int = Field(frozen=True)
+    tokens: int | None = Field(frozen=True)
     created_at: datetime = Field(frozen=True)
 
     message_sender: SenderRole = Field(frozen=True)
     message_data: MessageDataUnion = Field(frozen=True)
```

### Comparing `suvvyapi-2.0a8/suvvyapi/models/messages/content/audio.py` & `suvvyapi-2.0a9/suvvyapi/models/messages/content/audio.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/suvvyapi/models/messages/content/event.py` & `suvvyapi-2.0a9/suvvyapi/models/messages/content/event.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/suvvyapi/models/messages/content/image.py` & `suvvyapi-2.0a9/suvvyapi/models/messages/content/image.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/suvvyapi/models/messages/content/tool_call.py` & `suvvyapi-2.0a9/suvvyapi/models/messages/content/tool_call.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/suvvyapi/wrapper/__init__.py` & `suvvyapi-2.0a9/suvvyapi/wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-2.0a8/PKG-INFO` & `suvvyapi-2.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suvvyapi
-Version: 2.0a8
+Version: 2.0a9
 Summary: A Python API wrapper for Suvvy AI API
 Home-page: https://github.com/suvvyai/suvvyapi
 License: MIT
 Keywords: python,wrapper,chatgpt,suvvy,ai,suvvyai
 Author: Roman Poltorabatko
 Author-email: barabum@duck.com
 Requires-Python: >=3.10
```

