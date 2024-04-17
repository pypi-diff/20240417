# Comparing `tmp/llmaudit-0.0.4.tar.gz` & `tmp/llmaudit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmaudit-0.0.4.tar", last modified: Wed Apr 17 00:29:49 2024, max compression
+gzip compressed data, was "llmaudit-0.0.5.tar", last modified: Wed Apr 17 00:36:55 2024, max compression
```

## Comparing `llmaudit-0.0.4.tar` & `llmaudit-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 00:29:49.270978 llmaudit-0.0.4/
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)    11356 2024-04-16 23:43:48.000000 llmaudit-0.0.4/LICENSE
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 00:29:49.270462 llmaudit-0.0.4/PKG-INFO
-drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 00:29:49.265623 llmaudit-0.0.4/llmaudit/
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)        0 2024-04-16 23:48:32.000000 llmaudit-0.0.4/llmaudit/__init__.py
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)     1662 2024-04-17 00:29:07.000000 llmaudit-0.0.4/llmaudit/cli.py
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)     2823 2024-04-17 00:29:22.000000 llmaudit-0.0.4/llmaudit/scan_github_repos.py
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)    15523 2024-04-16 23:50:36.000000 llmaudit-0.0.4/llmaudit/sprawl.py
-drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 00:29:49.269882 llmaudit-0.0.4/llmaudit.egg-info/
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 00:29:49.000000 llmaudit-0.0.4/llmaudit.egg-info/PKG-INFO
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      302 2024-04-17 00:29:49.000000 llmaudit-0.0.4/llmaudit.egg-info/SOURCES.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)        1 2024-04-17 00:29:49.000000 llmaudit-0.0.4/llmaudit.egg-info/dependency_links.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)       51 2024-04-17 00:29:49.000000 llmaudit-0.0.4/llmaudit.egg-info/entry_points.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)       37 2024-04-17 00:29:49.000000 llmaudit-0.0.4/llmaudit.egg-info/requires.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)        9 2024-04-17 00:29:49.000000 llmaudit-0.0.4/llmaudit.egg-info/top_level.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      712 2024-04-17 00:29:32.000000 llmaudit-0.0.4/pyproject.toml
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)       38 2024-04-17 00:29:49.271100 llmaudit-0.0.4/setup.cfg
+drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 00:36:55.477078 llmaudit-0.0.5/
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)    11356 2024-04-16 23:43:48.000000 llmaudit-0.0.5/LICENSE
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 00:36:55.476541 llmaudit-0.0.5/PKG-INFO
+drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 00:36:55.472435 llmaudit-0.0.5/llmaudit/
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)        0 2024-04-16 23:48:32.000000 llmaudit-0.0.5/llmaudit/__init__.py
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     1662 2024-04-17 00:29:07.000000 llmaudit-0.0.5/llmaudit/cli.py
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     2823 2024-04-17 00:29:22.000000 llmaudit-0.0.5/llmaudit/scan_github_repos.py
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)    15523 2024-04-16 23:50:36.000000 llmaudit-0.0.5/llmaudit/sprawl.py
+drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 00:36:55.475947 llmaudit-0.0.5/llmaudit.egg-info/
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 00:36:55.000000 llmaudit-0.0.5/llmaudit.egg-info/PKG-INFO
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      302 2024-04-17 00:36:55.000000 llmaudit-0.0.5/llmaudit.egg-info/SOURCES.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)        1 2024-04-17 00:36:55.000000 llmaudit-0.0.5/llmaudit.egg-info/dependency_links.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)       51 2024-04-17 00:36:55.000000 llmaudit-0.0.5/llmaudit.egg-info/entry_points.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)       37 2024-04-17 00:36:55.000000 llmaudit-0.0.5/llmaudit.egg-info/requires.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)        9 2024-04-17 00:36:55.000000 llmaudit-0.0.5/llmaudit.egg-info/top_level.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      768 2024-04-17 00:36:43.000000 llmaudit-0.0.5/pyproject.toml
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)       38 2024-04-17 00:36:55.477208 llmaudit-0.0.5/setup.cfg
```

### Comparing `llmaudit-0.0.4/LICENSE` & `llmaudit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llmaudit-0.0.4/PKG-INFO` & `llmaudit-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmaudit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A CLI tool to find LLM usage accross your repos
 Author-email: PromptArmor <founders@promptarmor.com>
 Project-URL: Company Page, https://promptarmor.com/
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llmaudit-0.0.4/llmaudit/cli.py` & `llmaudit-0.0.5/llmaudit/cli.py`

 * *Files identical despite different names*

### Comparing `llmaudit-0.0.4/llmaudit/scan_github_repos.py` & `llmaudit-0.0.5/llmaudit/scan_github_repos.py`

 * *Files identical despite different names*

### Comparing `llmaudit-0.0.4/llmaudit/sprawl.py` & `llmaudit-0.0.5/llmaudit/sprawl.py`

 * *Files identical despite different names*

### Comparing `llmaudit-0.0.4/llmaudit.egg-info/PKG-INFO` & `llmaudit-0.0.5/llmaudit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmaudit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A CLI tool to find LLM usage accross your repos
 Author-email: PromptArmor <founders@promptarmor.com>
 Project-URL: Company Page, https://promptarmor.com/
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llmaudit-0.0.4/pyproject.toml` & `llmaudit-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmaudit"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="PromptArmor", email="founders@promptarmor.com" },
 ]
 description = "A CLI tool to find LLM usage accross your repos"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -20,11 +20,15 @@
   "PyGithub"
 ]
 
 [project.scripts]
 llmaudit = "llmaudit.cli:main_cli"
 
 
+[tool.setuptools.package-data]
+llmaudit = ['assets/']
+
+
 [project.urls]
 "Company Page" = "https://promptarmor.com/"
 Homepage = "https://github.com/pypa/sampleproject"
 Issues = "https://github.com/pypa/sampleproject/issues"
```

