# Comparing `tmp/knowledge_engineer-0.2.0.tar.gz` & `tmp/knowledge_engineer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledge_engineer-0.2.0.tar", last modified: Tue Apr 16 16:31:47 2024, max compression
+gzip compressed data, was "knowledge_engineer-0.2.1.tar", last modified: Wed Apr 17 02:15:45 2024, max compression
```

## Comparing `knowledge_engineer-0.2.0.tar` & `knowledge_engineer-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2024-04-16 16:31:47.594835 knowledge_engineer-0.2.0/
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1071 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/LICENSE
--rw-r--r--   0 jerry     (1000) jerry     (1000)     2482 2024-04-16 16:31:47.594835 knowledge_engineer-0.2.0/PKG-INFO
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1827 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/README.md
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2024-04-16 16:31:47.590835 knowledge_engineer-0.2.0/knowledge_engineer/
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2432 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/AI_API_Costs.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)        0 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/__init__.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    15290 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/ai.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     3771 2024-04-03 04:38:09.000000 knowledge_engineer-0.2.0/knowledge_engineer/create_new_process.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     8985 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/db.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     9259 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/ke.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     8217 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/line_statement.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     6240 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/logger.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     4436 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/step.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      360 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/version.py
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2024-04-16 16:31:47.594835 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/
--rw-r--r--   0 jerry     (1000) jerry     (1000)     2482 2024-04-16 16:31:47.000000 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/PKG-INFO
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      601 2024-04-16 16:31:47.000000 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/SOURCES.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)        1 2024-04-16 16:31:47.000000 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/dependency_links.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)       66 2024-04-16 16:31:47.000000 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/entry_points.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)       70 2024-04-16 16:31:47.000000 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/requires.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)       19 2024-04-16 16:31:47.000000 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/top_level.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      737 2024-04-16 16:22:25.000000 knowledge_engineer-0.2.0/pyproject.toml
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      627 2024-04-16 16:31:47.594835 knowledge_engineer-0.2.0/setup.cfg
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2024-04-17 02:15:45.006233 knowledge_engineer-0.2.1/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1071 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.1/LICENSE
+-rw-r--r--   0 jerry     (1000) jerry     (1000)     2637 2024-04-17 02:15:45.006233 knowledge_engineer-0.2.1/PKG-INFO
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1982 2024-04-17 02:11:38.000000 knowledge_engineer-0.2.1/README.md
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2024-04-17 02:15:45.006233 knowledge_engineer-0.2.1/knowledge_engineer/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2432 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.1/knowledge_engineer/AI_API_Costs.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)        0 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.1/knowledge_engineer/__init__.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    15290 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.1/knowledge_engineer/ai.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     3771 2024-04-17 02:12:24.000000 knowledge_engineer-0.2.1/knowledge_engineer/create_new_process.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     8985 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.1/knowledge_engineer/db.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     9259 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.1/knowledge_engineer/ke.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     8217 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.1/knowledge_engineer/line_statement.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     6240 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.1/knowledge_engineer/logger.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     4436 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.1/knowledge_engineer/step.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      360 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.1/knowledge_engineer/version.py
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2024-04-17 02:15:45.006233 knowledge_engineer-0.2.1/knowledge_engineer.egg-info/
+-rw-r--r--   0 jerry     (1000) jerry     (1000)     2637 2024-04-17 02:15:44.000000 knowledge_engineer-0.2.1/knowledge_engineer.egg-info/PKG-INFO
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      601 2024-04-17 02:15:44.000000 knowledge_engineer-0.2.1/knowledge_engineer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)        1 2024-04-17 02:15:44.000000 knowledge_engineer-0.2.1/knowledge_engineer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)       66 2024-04-17 02:15:44.000000 knowledge_engineer-0.2.1/knowledge_engineer.egg-info/entry_points.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)       70 2024-04-17 02:15:44.000000 knowledge_engineer-0.2.1/knowledge_engineer.egg-info/requires.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)       19 2024-04-17 02:15:44.000000 knowledge_engineer-0.2.1/knowledge_engineer.egg-info/top_level.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      737 2024-04-17 02:12:01.000000 knowledge_engineer-0.2.1/pyproject.toml
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      627 2024-04-17 02:15:45.006233 knowledge_engineer-0.2.1/setup.cfg
```

### Comparing `knowledge_engineer-0.2.0/LICENSE` & `knowledge_engineer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.2.0/PKG-INFO` & `knowledge_engineer-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledge_engineer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Engineer GPT Knowledge within a process
 Home-page: https://github.com/JerryWestrick/Knowledge_Engineer
 Author: Jerry Westrick
 Author-email: Jerry Westrick <jerry@westrick.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,14 +26,23 @@
 
 
 OpenAI GPT Chat is the first to be supported, but the program is designed to be extensible to other LLMs. The program can be extended by modifying the "Knowledge Engineer Prompt File" Domain Specific Language (DSL).  
 
 (That is a fancy way to say:  "by modifying the syntax of the **.kepf** files.")
 
 # Quick Start
+### Preparation
+    mkdir ke
+    python -m venv .venv
+
+###### Dos/Windows
+    .venv\Scripts\activate
+###### Linux/MacOS
+    source .venv/bin/activate
+    
 ### Installation
     pip install knowledge-engineer
 
 ### Create New Project
     knowledge_engineer --create=snake
 
 ### Setup Project
```

### Comparing `knowledge_engineer-0.2.0/README.md` & `knowledge_engineer-0.2.1/knowledge_engineer.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,48 @@
+Metadata-Version: 2.1
+Name: knowledge_engineer
+Version: 0.2.1
+Summary: Engineer GPT Knowledge within a process
+Home-page: https://github.com/JerryWestrick/Knowledge_Engineer
+Author: Jerry Westrick
+Author-email: Jerry Westrick <jerry@westrick.com>
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: rich
+Requires-Dist: openai
+Requires-Dist: mistralai
+Requires-Dist: python-dotenv
+Requires-Dist: lark
+Requires-Dist: databases
+Requires-Dist: knowledge_engineer
+
 # Knowledge Engineer
 
 ***Command Line Program allowing for the Engineering of Knowledge for LLM's.***
 
 
 
 OpenAI GPT Chat is the first to be supported, but the program is designed to be extensible to other LLMs. The program can be extended by modifying the "Knowledge Engineer Prompt File" Domain Specific Language (DSL).  
 
 (That is a fancy way to say:  "by modifying the syntax of the **.kepf** files.")
 
 # Quick Start
+### Preparation
+    mkdir ke
+    python -m venv .venv
+
+###### Dos/Windows
+    .venv\Scripts\activate
+###### Linux/MacOS
+    source .venv/bin/activate
+    
 ### Installation
     pip install knowledge-engineer
 
 ### Create New Project
     knowledge_engineer --create=snake
 
 ### Setup Project
```

### Comparing `knowledge_engineer-0.2.0/knowledge_engineer/AI_API_Costs.py` & `knowledge_engineer-0.2.1/knowledge_engineer/AI_API_Costs.py`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.2.0/knowledge_engineer/ai.py` & `knowledge_engineer-0.2.1/knowledge_engineer/ai.py`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.2.0/knowledge_engineer/create_new_process.py` & `knowledge_engineer-0.2.1/knowledge_engineer/create_new_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  - list all the rules to be implemented
  - implement all the requirements in the prompts
 Write the prompt to 'Planning/Gen_Code_Prompt.md' using function 'write_file'.
 .exec
 """,
 
     # ==========================================
-    '2- Make Mines Game.kepf':
+    '2- Make Snake Game.kepf':
         """.llm "llm_name": "OpenAI", "model": "gpt-4-0125-preview", "max_tokens": 50000
 
 .system
 You are an IT Engineer, programming a Python 3 Application
 Do not explain yourself.
 Do not apologize.
 Check all code for completeness, correctness, and make sure it is executable.
```

### Comparing `knowledge_engineer-0.2.0/knowledge_engineer/db.py` & `knowledge_engineer-0.2.1/knowledge_engineer/db.py`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.2.0/knowledge_engineer/ke.py` & `knowledge_engineer-0.2.1/knowledge_engineer/ke.py`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.2.0/knowledge_engineer/line_statement.py` & `knowledge_engineer-0.2.1/knowledge_engineer/line_statement.py`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.2.0/knowledge_engineer/logger.py` & `knowledge_engineer-0.2.1/knowledge_engineer/logger.py`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.2.0/knowledge_engineer/step.py` & `knowledge_engineer-0.2.1/knowledge_engineer/step.py`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.2.0/knowledge_engineer.egg-info/SOURCES.txt` & `knowledge_engineer-0.2.1/knowledge_engineer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.2.0/pyproject.toml` & `knowledge_engineer-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 include-package-data = true
 
 [tool.setuptools.package-data]
 knowledge_engineer = ["*.md"]
 
 [project]
 name = "knowledge_engineer"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name = "Jerry Westrick", email = "jerry@westrick.com" },
 ]
 description = "Engineer GPT Knowledge within a process"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `knowledge_engineer-0.2.0/setup.cfg` & `knowledge_engineer-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = knowledge_engineer
-version = 0.2.0
+version = 0.2.1
 author = Jerry Westrick
 author_email = jerry@westrick.com
 description = Engineer GPT Knowledge within a process
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JerryWestrick/Knowledge_Engineer
 classifiers =
```

