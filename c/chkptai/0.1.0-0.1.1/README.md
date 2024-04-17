# Comparing `tmp/chkptai-0.1.0.tar.gz` & `tmp/chkptai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chkptai-0.1.0.tar", last modified: Wed Apr 17 16:47:19 2024, max compression
+gzip compressed data, was "chkptai-0.1.1.tar", last modified: Wed Apr 17 17:04:53 2024, max compression
```

## Comparing `chkptai-0.1.0.tar` & `chkptai-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 16:47:19.996343 chkptai-0.1.0/
--rw-r--r--   0 jp         (501) staff       (20)       97 2024-04-11 22:46:48.000000 chkptai-0.1.0/MANIFEST.in
--rw-r--r--   0 jp         (501) staff       (20)      584 2024-04-17 16:47:19.996161 chkptai-0.1.0/PKG-INFO
--rw-r--r--   0 jp         (501) staff       (20)      103 2024-04-16 18:49:54.000000 chkptai-0.1.0/README.md
--rw-r--r--   0 jp         (501) staff       (20)      704 2024-04-17 03:53:47.000000 chkptai-0.1.0/pyproject.toml
--rw-r--r--   0 jp         (501) staff       (20)       38 2024-04-17 16:47:19.996388 chkptai-0.1.0/setup.cfg
--rw-r--r--   0 jp         (501) staff       (20)      240 2024-04-17 16:46:44.000000 chkptai-0.1.0/setup.py
-drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 16:47:19.993578 chkptai-0.1.0/src/
-drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 16:47:19.994473 chkptai-0.1.0/src/chkptai/
--rw-r--r--   0 jp         (501) staff       (20)     6255 2024-04-17 03:21:01.000000 chkptai-0.1.0/src/chkptai/ChkptAI.py
--rw-r--r--   0 jp         (501) staff       (20)       92 2024-04-17 16:46:59.000000 chkptai-0.1.0/src/chkptai/__init__.py
--rw-r--r--   0 jp         (501) staff       (20)     4719 2024-04-13 21:24:58.000000 chkptai-0.1.0/src/chkptai/chkpt_types.py
-drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 16:47:19.995732 chkptai-0.1.0/src/chkptai.egg-info/
--rw-r--r--   0 jp         (501) staff       (20)      584 2024-04-17 16:47:19.000000 chkptai-0.1.0/src/chkptai.egg-info/PKG-INFO
--rw-r--r--   0 jp         (501) staff       (20)      364 2024-04-17 16:47:19.000000 chkptai-0.1.0/src/chkptai.egg-info/SOURCES.txt
--rw-r--r--   0 jp         (501) staff       (20)        1 2024-04-17 16:47:19.000000 chkptai-0.1.0/src/chkptai.egg-info/dependency_links.txt
--rw-r--r--   0 jp         (501) staff       (20)        1 2024-04-12 22:51:28.000000 chkptai-0.1.0/src/chkptai.egg-info/not-zip-safe
--rw-r--r--   0 jp         (501) staff       (20)       39 2024-04-17 16:47:19.000000 chkptai-0.1.0/src/chkptai.egg-info/requires.txt
--rw-r--r--   0 jp         (501) staff       (20)        8 2024-04-17 16:47:19.000000 chkptai-0.1.0/src/chkptai.egg-info/top_level.txt
-drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 16:47:19.995543 chkptai-0.1.0/tests/
--rw-r--r--   0 jp         (501) staff       (20)     5063 2024-04-15 21:30:22.000000 chkptai-0.1.0/tests/test_chkptai.py
--rw-r--r--   0 jp         (501) staff       (20)      440 2024-04-15 21:28:38.000000 chkptai-0.1.0/tests/tests.py
+drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 17:04:53.978734 chkptai-0.1.1/
+-rw-r--r--   0 jp         (501) staff       (20)       97 2024-04-11 22:46:48.000000 chkptai-0.1.1/MANIFEST.in
+-rw-r--r--   0 jp         (501) staff       (20)      639 2024-04-17 17:04:53.978532 chkptai-0.1.1/PKG-INFO
+-rw-r--r--   0 jp         (501) staff       (20)      103 2024-04-16 18:49:54.000000 chkptai-0.1.1/README.md
+-rw-r--r--   0 jp         (501) staff       (20)      733 2024-04-17 16:58:22.000000 chkptai-0.1.1/pyproject.toml
+-rw-r--r--   0 jp         (501) staff       (20)       38 2024-04-17 17:04:53.978778 chkptai-0.1.1/setup.cfg
+-rw-r--r--   0 jp         (501) staff       (20)      164 2024-04-17 16:59:08.000000 chkptai-0.1.1/setup.py
+drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 17:04:53.976007 chkptai-0.1.1/src/
+drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 17:04:53.976913 chkptai-0.1.1/src/chkptai/
+-rw-r--r--   0 jp         (501) staff       (20)     6255 2024-04-17 03:21:01.000000 chkptai-0.1.1/src/chkptai/ChkptAI.py
+-rw-r--r--   0 jp         (501) staff       (20)       92 2024-04-17 16:53:34.000000 chkptai-0.1.1/src/chkptai/__init__.py
+-rw-r--r--   0 jp         (501) staff       (20)     4719 2024-04-13 21:24:58.000000 chkptai-0.1.1/src/chkptai/chkpt_types.py
+drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 17:04:53.978125 chkptai-0.1.1/src/chkptai.egg-info/
+-rw-r--r--   0 jp         (501) staff       (20)      639 2024-04-17 17:04:53.000000 chkptai-0.1.1/src/chkptai.egg-info/PKG-INFO
+-rw-r--r--   0 jp         (501) staff       (20)      364 2024-04-17 17:04:53.000000 chkptai-0.1.1/src/chkptai.egg-info/SOURCES.txt
+-rw-r--r--   0 jp         (501) staff       (20)        1 2024-04-17 17:04:53.000000 chkptai-0.1.1/src/chkptai.egg-info/dependency_links.txt
+-rw-r--r--   0 jp         (501) staff       (20)        1 2024-04-12 22:51:28.000000 chkptai-0.1.1/src/chkptai.egg-info/not-zip-safe
+-rw-r--r--   0 jp         (501) staff       (20)       64 2024-04-17 17:04:53.000000 chkptai-0.1.1/src/chkptai.egg-info/requires.txt
+-rw-r--r--   0 jp         (501) staff       (20)        8 2024-04-17 17:04:53.000000 chkptai-0.1.1/src/chkptai.egg-info/top_level.txt
+drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 17:04:53.977897 chkptai-0.1.1/tests/
+-rw-r--r--   0 jp         (501) staff       (20)     5063 2024-04-15 21:30:22.000000 chkptai-0.1.1/tests/test_chkptai.py
+-rw-r--r--   0 jp         (501) staff       (20)      440 2024-04-15 21:28:38.000000 chkptai-0.1.1/tests/tests.py
```

### Comparing `chkptai-0.1.0/PKG-INFO` & `chkptai-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: chkptai
-Version: 0.1.0
+Version: 0.1.1
 Summary: Checkpoint-AI Python SDK
 Author-email: Checkpoint-AI <mail@checkpoint-ai.com>
 License: proprietary
 Project-URL: homepage, https://checkpoint-ai.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: openai
+Requires-Dist: typing_extensions
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
```

### Comparing `chkptai-0.1.0/pyproject.toml` & `chkptai-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 authors = [{ name = "Checkpoint-AI", email = "mail@checkpoint-ai.com" }]
 
 dynamic = ["version"]
 keywords = []
 description = "Checkpoint-AI Python SDK"
 requires-python = ">=3.10"
 readme = "README.md"
-dependencies = []
+dependencies = ["openai", "typing_extensions"]
 license = { text = "proprietary" }
 
 [project.optional-dependencies]
 dev = ["mypy", "flake8", "pytest", "black", "pylint"]
 [project.urls]
 
 homepage = "https://checkpoint-ai.com"
```

### Comparing `chkptai-0.1.0/src/chkptai/ChkptAI.py` & `chkptai-0.1.1/src/chkptai/ChkptAI.py`

 * *Files identical despite different names*

### Comparing `chkptai-0.1.0/src/chkptai/chkpt_types.py` & `chkptai-0.1.1/src/chkptai/chkpt_types.py`

 * *Files identical despite different names*

### Comparing `chkptai-0.1.0/src/chkptai.egg-info/PKG-INFO` & `chkptai-0.1.1/src/chkptai.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: chkptai
-Version: 0.1.0
+Version: 0.1.1
 Summary: Checkpoint-AI Python SDK
 Author-email: Checkpoint-AI <mail@checkpoint-ai.com>
 License: proprietary
 Project-URL: homepage, https://checkpoint-ai.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: openai
+Requires-Dist: typing_extensions
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
```

### Comparing `chkptai-0.1.0/tests/test_chkptai.py` & `chkptai-0.1.1/tests/test_chkptai.py`

 * *Files identical despite different names*

