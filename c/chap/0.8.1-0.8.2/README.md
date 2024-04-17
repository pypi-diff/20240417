# Comparing `tmp/chap-0.8.1.tar.gz` & `tmp/chap-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chap-0.8.1.tar", last modified: Fri Mar  8 20:27:48 2024, max compression
+gzip compressed data, was "chap-0.8.2.tar", last modified: Wed Apr 17 15:49:09 2024, max compression
```

## Comparing `chap-0.8.1.tar` & `chap-0.8.2.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:27:48.561638 chap-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:27:48.549638 chap-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:27:48.553638 chap-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-08 20:27:39.000000 chap-0.8.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-08 20:27:39.000000 chap-0.8.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-08 20:27:39.000000 chap-0.8.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-08 20:27:39.000000 chap-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-08 20:27:39.000000 chap-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-03-08 20:27:39.000000 chap-0.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-03-08 20:27:39.000000 chap-0.8.1/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:27:48.553638 chap-0.8.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    17023 2024-03-08 20:27:39.000000 chap-0.8.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-03-08 20:27:39.000000 chap-0.8.1/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-08 20:27:39.000000 chap-0.8.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-08 20:27:39.000000 chap-0.8.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-08 20:27:39.000000 chap-0.8.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-03-08 20:27:48.561638 chap-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-03-08 20:27:39.000000 chap-0.8.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      574 2024-03-08 20:27:39.000000 chap-0.8.1/chap-dev.py
--rw-r--r--   0 runner    (1001) docker     (127)   336717 2024-03-08 20:27:39.000000 chap-0.8.1/chap.gif
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-08 20:27:39.000000 chap-0.8.1/chap.gif.license
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-08 20:27:39.000000 chap-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-08 20:27:39.000000 chap-0.8.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-08 20:27:39.000000 chap-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 20:27:48.561638 chap-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:27:48.553638 chap-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:27:48.557638 chap-0.8.1/src/chap/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-08 20:27:48.000000 chap-0.8.1/src/chap/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:27:48.557638 chap-0.8.1/src/chap/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/backends/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/backends/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/backends/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/backends/lorem.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/backends/openai_chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/backends/textgen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:27:48.557638 chap-0.8.1/src/chap/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/commands/ask.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/commands/cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/commands/grep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/commands/import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/commands/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/commands/tui.css
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/commands/tui.py
--rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/key.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-08 20:27:39.000000 chap-0.8.1/src/chap/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:27:48.561638 chap-0.8.1/src/chap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-03-08 20:27:48.000000 chap-0.8.1/src/chap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-08 20:27:48.000000 chap-0.8.1/src/chap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 20:27:48.000000 chap-0.8.1/src/chap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-08 20:27:48.000000 chap-0.8.1/src/chap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-08 20:27:48.000000 chap-0.8.1/src/chap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-08 20:27:48.000000 chap-0.8.1/src/chap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:09.676706 chap-0.8.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:09.668706 chap-0.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:09.672706 chap-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-17 15:48:58.000000 chap-0.8.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-17 15:48:58.000000 chap-0.8.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-17 15:48:58.000000 chap-0.8.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-17 15:48:58.000000 chap-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 15:48:58.000000 chap-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-04-17 15:48:58.000000 chap-0.8.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-17 15:48:58.000000 chap-0.8.2/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:09.672706 chap-0.8.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    17023 2024-04-17 15:48:58.000000 chap-0.8.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-17 15:48:58.000000 chap-0.8.2/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-17 15:48:58.000000 chap-0.8.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-17 15:48:58.000000 chap-0.8.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-17 15:48:58.000000 chap-0.8.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-17 15:49:09.676706 chap-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-17 15:48:58.000000 chap-0.8.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      574 2024-04-17 15:48:58.000000 chap-0.8.2/chap-dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)   336717 2024-04-17 15:48:59.000000 chap-0.8.2/chap.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 15:48:59.000000 chap-0.8.2/chap.gif.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-17 15:48:59.000000 chap-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 15:48:59.000000 chap-0.8.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 15:48:59.000000 chap-0.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:49:09.676706 chap-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:09.668706 chap-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:09.672706 chap-0.8.2/src/chap/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 15:49:09.000000 chap-0.8.2/src/chap/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:09.676706 chap-0.8.2/src/chap/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/backends/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/backends/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/backends/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/backends/lorem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/backends/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/backends/openai_chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/backends/textgen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:09.676706 chap-0.8.2/src/chap/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/commands/ask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/commands/cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/commands/grep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/commands/import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/commands/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/commands/tui.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/commands/tui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12512 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-17 15:48:59.000000 chap-0.8.2/src/chap/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:09.676706 chap-0.8.2/src/chap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-17 15:49:09.000000 chap-0.8.2/src/chap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-17 15:49:09.000000 chap-0.8.2/src/chap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:49:09.000000 chap-0.8.2/src/chap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 15:49:09.000000 chap-0.8.2/src/chap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 15:49:09.000000 chap-0.8.2/src/chap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 15:49:09.000000 chap-0.8.2/src/chap.egg-info/top_level.txt
```

### Comparing `chap-0.8.1/.github/workflows/codeql.yml` & `chap-0.8.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/.github/workflows/release.yml` & `chap-0.8.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/.github/workflows/test.yml` & `chap-0.8.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/.pre-commit-config.yaml` & `chap-0.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/CODE_OF_CONDUCT.md` & `chap-0.8.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/CONTRIBUTING.md` & `chap-0.8.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/LICENSES/CC-BY-4.0.txt` & `chap-0.8.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/LICENSES/CC0-1.0.txt` & `chap-0.8.2/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/LICENSES/MIT.txt` & `chap-0.8.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/LICENSES/Unlicense.txt` & `chap-0.8.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/PKG-INFO` & `chap-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chap
-Version: 0.8.1
+Version: 0.8.2
 Summary: Interact with the OpenAI ChatGPT API (and other text generators)
 Author-email: Jeff Epler <jepler@gmail.com>
 Project-URL: homepage, https://github.com/jepler/chap
 Project-URL: repository, https://github.com/jepler/chap
 Keywords: llm,tui,chatgpt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chap-0.8.1/README.md` & `chap-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/chap-dev.py` & `chap-0.8.2/chap-dev.py`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/chap.gif` & `chap-0.8.2/chap.gif`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/pyproject.toml` & `chap-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/src/chap/backends/anthropic.py` & `chap-0.8.2/src/chap/backends/anthropic.py`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/src/chap/backends/huggingface.py` & `chap-0.8.2/src/chap/backends/huggingface.py`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/src/chap/backends/llama_cpp.py` & `chap-0.8.2/src/chap/backends/llama_cpp.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 
 class LlamaCpp(AutoAskMixin):
     @dataclass
     class Parameters:
         url: str = "http://localhost:8080/completion"
         """The URL of a llama.cpp server's completion endpoint."""
 
-        start_prompt: str = """<s>[INST] <<SYS>>\n"""
-        after_system: str = "\n<</SYS>>\n\n"
-        after_user: str = """ [/INST] """
-        after_assistant: str = """ </s><s>[INST] """
+        start_prompt: str = "<s>"
+        system_format: str = "<<SYS>>{}<</SYS>>"
+        user_format: str = " [INST] {} [/INST]"
+        assistant_format: str = " {}</s>"
 
     def __init__(self) -> None:
         super().__init__()
         self.parameters = self.Parameters()
 
     system_message = """\
 A dialog, where USER interacts with AI. AI is helpful, kind, obedient, honest, and knows its own limits.
 """
 
     def make_full_query(self, messages: Session, max_query_size: int) -> str:
         del messages[1:-max_query_size]
         result = [self.parameters.start_prompt]
+        formats = {
+            Role.SYSTEM: self.parameters.system_format,
+            Role.USER: self.parameters.user_format,
+            Role.ASSISTANT: self.parameters.assistant_format,
+        }
         for m in messages:
             content = (m.content or "").strip()
             if not content:
                 continue
-            result.append(content)
-            if m.role == Role.SYSTEM:
-                result.append(self.parameters.after_system)
-            elif m.role == Role.ASSISTANT:
-                result.append(self.parameters.after_assistant)
-            elif m.role == Role.USER:
-                result.append(self.parameters.after_user)
+            result.append(formats[m.role].format(content))
         full_query = "".join(result)
+        print("fq", full_query)
         return full_query
 
     async def aask(
         self,
         session: Session,
         query: str,
         *,
```

### Comparing `chap-0.8.1/src/chap/backends/lorem.py` & `chap-0.8.2/src/chap/backends/lorem.py`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/src/chap/backends/openai_chatgpt.py` & `chap-0.8.2/src/chap/backends/openai_chatgpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 
         return cls(encoding, tokens_per_message, tokens_per_name, tokens_overhead)
 
 
 class ChatGPT:
     @dataclass
     class Parameters:
-        model: str = "gpt-3.5-turbo"
-        """The model to use. The most common alternative value is 'gpt-4'."""
+        model: str = "gpt-4-turbo"
+        """The model to use. The most common alternative value is 'gpt-3.5-turbo'."""
 
         max_request_tokens: int = 1024
         """The approximate greatest number of tokens to send in a request. When the session is long, the system prompt and 1 or more of the most recent interaction steps are sent."""
 
     def __init__(self) -> None:
         self.parameters = self.Parameters()
```

### Comparing `chap-0.8.1/src/chap/backends/textgen.py` & `chap-0.8.2/src/chap/backends/textgen.py`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/src/chap/commands/ask.py` & `chap-0.8.2/src/chap/commands/ask.py`

 * *Files 12% similar despite different names*

```diff
@@ -96,29 +96,37 @@
     printer.add("\n")
     result = "".join(tokens)
     return result
 
 
 @command_uses_new_session
 @click.option("--print-prompt/--no-print-prompt", default=True)
-@click.argument("prompt", nargs=-1, required=True)
-def main(obj: Obj, prompt: str, print_prompt: bool) -> None:
+@click.option("--stdin/--no-stdin", "use_stdin", default=False)
+@click.argument("prompt", nargs=-1)
+def main(obj: Obj, prompt: list[str], use_stdin: bool, print_prompt: bool) -> None:
     """Ask a question (command-line argument is passed as prompt)"""
     session = obj.session
     assert session is not None
 
     session_filename = obj.session_filename
     assert session_filename is not None
 
     api = obj.api
     assert api is not None
 
+    if use_stdin:
+        if prompt:
+            raise click.UsageError("Can't use 'prompt' together with --stdin")
+
+        joined_prompt = sys.stdin.read()
+    else:
+        joined_prompt = " ".join(prompt)
     #    symlink_session_filename(session_filename)
 
-    response = verbose_ask(api, session, " ".join(prompt), print_prompt=print_prompt)
+    response = verbose_ask(api, session, joined_prompt, print_prompt=print_prompt)
 
     print(f"Saving session to {session_filename}", file=sys.stderr)
     if response is not None:
         session_to_file(session, session_filename)
 
 
 if __name__ == "__main__":
```

### Comparing `chap-0.8.1/src/chap/commands/cat.py` & `chap-0.8.2/src/chap/commands/cat.py`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/src/chap/commands/grep.py` & `chap-0.8.2/src/chap/commands/grep.py`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/src/chap/commands/import.py` & `chap-0.8.2/src/chap/commands/import.py`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/src/chap/commands/render.py` & `chap-0.8.2/src/chap/commands/render.py`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/src/chap/commands/tui.css` & `chap-0.8.2/src/chap/commands/tui.css`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/src/chap/commands/tui.py` & `chap-0.8.2/src/chap/commands/tui.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,17 @@
     assert api is not None
     session = obj.session
     assert session is not None
     session_filename = obj.session_filename
     assert session_filename is not None
 
     if replace_system_prompt:
-        session[0].content = obj.system_message or api.system_message
+        session[0].content = (
+            api.system_message if obj.system_message is None else obj.system_message
+        )
 
     tui = Tui(api, session)
     tui.run()
 
     sys.stdout.flush()
     sys.stderr.flush()
```

### Comparing `chap-0.8.1/src/chap/core.py` & `chap-0.8.2/src/chap/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: 2023 Jeff Epler <jepler@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
 
 import asyncio
 import datetime
+import io
 import importlib
 import os
 import pathlib
 import pkgutil
 import subprocess
 from dataclasses import MISSING, Field, dataclass, fields
 from typing import (
@@ -173,20 +174,31 @@
 def colonstr(arg: str) -> tuple[str, str]:
     if ":" not in arg:
         raise click.BadParameter("must be of the form 'name:value'")
     return cast(tuple[str, str], tuple(arg.split(":", 1)))
 
 
 def set_system_message(ctx: click.Context, param: click.Parameter, value: str) -> None:
-    if value and value.startswith("@"):
+    if value is None:
+        return
+    if value.startswith("@"):
         with open(value[1:], "r", encoding="utf-8") as f:
-            value = f.read().rstrip()
+            value = f.read().strip()
     ctx.obj.system_message = value
 
 
+def set_system_message_from_file(
+    ctx: click.Context, param: click.Parameter, value: io.TextIOWrapper
+) -> None:
+    if value is None:
+        return
+    content = value.read().strip()
+    ctx.obj.system_message = content
+
+
 def set_backend(ctx: click.Context, param: click.Parameter, value: str) -> None:
     if value == "list":
         formatter = ctx.make_formatter()
         format_backend_list(formatter)
         click.utils.echo(formatter.getvalue().rstrip("\n"))
         ctx.exit()
 
@@ -366,14 +378,21 @@
             ("--version",),
             is_flag=True,
             is_eager=True,
             help="Show the version and exit",
             callback=version_callback,
         ),
         click.Option(
+            ("--system-message-file", "-@"),
+            type=click.File("r"),
+            default=None,
+            callback=set_system_message_from_file,
+            expose_value=False,
+        ),
+        click.Option(
             ("--system-message", "-S"),
             type=str,
             default=None,
             callback=set_system_message,
             expose_value=False,
         ),
         click.Option(
```

### Comparing `chap-0.8.1/src/chap/key.py` & `chap-0.8.2/src/chap/key.py`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/src/chap/session.py` & `chap-0.8.2/src/chap/session.py`

 * *Files identical despite different names*

### Comparing `chap-0.8.1/src/chap.egg-info/PKG-INFO` & `chap-0.8.2/src/chap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chap
-Version: 0.8.1
+Version: 0.8.2
 Summary: Interact with the OpenAI ChatGPT API (and other text generators)
 Author-email: Jeff Epler <jepler@gmail.com>
 Project-URL: homepage, https://github.com/jepler/chap
 Project-URL: repository, https://github.com/jepler/chap
 Keywords: llm,tui,chatgpt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chap-0.8.1/src/chap.egg-info/SOURCES.txt` & `chap-0.8.2/src/chap.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 src/chap.egg-info/entry_points.txt
 src/chap.egg-info/requires.txt
 src/chap.egg-info/top_level.txt
 src/chap/backends/anthropic.py
 src/chap/backends/huggingface.py
 src/chap/backends/llama_cpp.py
 src/chap/backends/lorem.py
+src/chap/backends/mistral.py
 src/chap/backends/openai_chatgpt.py
 src/chap/backends/textgen.py
 src/chap/commands/ask.py
 src/chap/commands/cat.py
 src/chap/commands/grep.py
 src/chap/commands/import.py
 src/chap/commands/render.py
```

