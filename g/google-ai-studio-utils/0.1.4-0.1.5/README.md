# Comparing `tmp/google_ai_studio_utils-0.1.4.tar.gz` & `tmp/google_ai_studio_utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_ai_studio_utils-0.1.4.tar", max compression
+gzip compressed data, was "google_ai_studio_utils-0.1.5.tar", max compression
```

## Comparing `google_ai_studio_utils-0.1.4.tar` & `google_ai_studio_utils-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       24 2024-04-15 15:56:31.370705 google_ai_studio_utils-0.1.4/README.md
--rw-r--r--   0        0        0      214 2024-04-15 16:21:49.454447 google_ai_studio_utils-0.1.4/google_ai_studio_utils/config.py
--rwxr-xr-x   0        0        0     2916 2024-04-15 17:01:31.595230 google_ai_studio_utils-0.1.4/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py
--rw-r--r--   0        0        0     1711 2024-04-15 17:00:10.849470 google_ai_studio_utils-0.1.4/google_ai_studio_utils/utils.py
--rw-r--r--   0        0        0      827 2024-04-15 17:02:13.303922 google_ai_studio_utils-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 google_ai_studio_utils-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       24 2024-04-15 15:56:31.370705 google_ai_studio_utils-0.1.5/README.md
+-rw-r--r--   0        0        0      188 2024-04-17 01:59:04.520871 google_ai_studio_utils-0.1.5/google_ai_studio_utils/config.py
+-rwxr-xr-x   0        0        0     2916 2024-04-15 17:01:31.595230 google_ai_studio_utils-0.1.5/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py
+-rw-r--r--   0        0        0     1711 2024-04-15 17:00:10.849470 google_ai_studio_utils-0.1.5/google_ai_studio_utils/utils.py
+-rw-r--r--   0        0        0      827 2024-04-17 01:59:20.751424 google_ai_studio_utils-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 google_ai_studio_utils-0.1.5/PKG-INFO
```

### Comparing `google_ai_studio_utils-0.1.4/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py` & `google_ai_studio_utils-0.1.5/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py`

 * *Files identical despite different names*

### Comparing `google_ai_studio_utils-0.1.4/google_ai_studio_utils/utils.py` & `google_ai_studio_utils-0.1.5/google_ai_studio_utils/utils.py`

 * *Files identical despite different names*

### Comparing `google_ai_studio_utils-0.1.4/pyproject.toml` & `google_ai_studio_utils-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "google-ai-studio-utils"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tddschn/google-ai-studio-utils"
 repository = "https://github.com/tddschn/google-ai-studio-utils"
 classifiers = ["Topic :: Utilities"]
```

### Comparing `google_ai_studio_utils-0.1.4/PKG-INFO` & `google_ai_studio_utils-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ai-studio-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Home-page: https://github.com/tddschn/google-ai-studio-utils
 License: MIT
 Keywords: chatgpt
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

