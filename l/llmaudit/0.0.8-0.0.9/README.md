# Comparing `tmp/llmaudit-0.0.8.tar.gz` & `tmp/llmaudit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmaudit-0.0.8.tar", last modified: Wed Apr 17 00:49:02 2024, max compression
+gzip compressed data, was "llmaudit-0.0.9.tar", last modified: Wed Apr 17 00:52:29 2024, max compression
```

## Comparing `llmaudit-0.0.8.tar` & `llmaudit-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 00:49:02.739395 llmaudit-0.0.8/
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)    11356 2024-04-16 23:43:48.000000 llmaudit-0.0.8/LICENSE
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 00:49:02.738481 llmaudit-0.0.8/PKG-INFO
-drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 00:49:02.731713 llmaudit-0.0.8/llmaudit/
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)        0 2024-04-16 23:48:32.000000 llmaudit-0.0.8/llmaudit/__init__.py
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)     1662 2024-04-17 00:29:07.000000 llmaudit-0.0.8/llmaudit/cli.py
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)     7405 2024-01-24 08:06:20.000000 llmaudit-0.0.8/llmaudit/logo.png
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)     4801 2024-04-17 00:40:39.000000 llmaudit-0.0.8/llmaudit/report_template.html
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)     2823 2024-04-17 00:29:22.000000 llmaudit-0.0.8/llmaudit/scan_github_repos.py
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)    15516 2024-04-17 00:40:31.000000 llmaudit-0.0.8/llmaudit/sprawl.py
-drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 00:49:02.737090 llmaudit-0.0.8/llmaudit.egg-info/
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 00:49:02.000000 llmaudit-0.0.8/llmaudit.egg-info/PKG-INFO
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      350 2024-04-17 00:49:02.000000 llmaudit-0.0.8/llmaudit.egg-info/SOURCES.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)        1 2024-04-17 00:49:02.000000 llmaudit-0.0.8/llmaudit.egg-info/dependency_links.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)       51 2024-04-17 00:49:02.000000 llmaudit-0.0.8/llmaudit.egg-info/entry_points.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)       37 2024-04-17 00:49:02.000000 llmaudit-0.0.8/llmaudit.egg-info/requires.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)        9 2024-04-17 00:49:02.000000 llmaudit-0.0.8/llmaudit.egg-info/top_level.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      777 2024-04-17 00:48:44.000000 llmaudit-0.0.8/pyproject.toml
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)       38 2024-04-17 00:49:02.739614 llmaudit-0.0.8/setup.cfg
+drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 00:52:29.592206 llmaudit-0.0.9/
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)    11356 2024-04-16 23:43:48.000000 llmaudit-0.0.9/LICENSE
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 00:52:29.591494 llmaudit-0.0.9/PKG-INFO
+drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 00:52:29.584205 llmaudit-0.0.9/llmaudit/
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)        0 2024-04-16 23:48:32.000000 llmaudit-0.0.9/llmaudit/__init__.py
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     1662 2024-04-17 00:29:07.000000 llmaudit-0.0.9/llmaudit/cli.py
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     7405 2024-01-24 08:06:20.000000 llmaudit-0.0.9/llmaudit/logo.png
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     4801 2024-04-17 00:40:39.000000 llmaudit-0.0.9/llmaudit/report_template.html
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     2823 2024-04-17 00:29:22.000000 llmaudit-0.0.9/llmaudit/scan_github_repos.py
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)    15574 2024-04-17 00:52:09.000000 llmaudit-0.0.9/llmaudit/sprawl.py
+drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 00:52:29.590778 llmaudit-0.0.9/llmaudit.egg-info/
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 00:52:29.000000 llmaudit-0.0.9/llmaudit.egg-info/PKG-INFO
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      350 2024-04-17 00:52:29.000000 llmaudit-0.0.9/llmaudit.egg-info/SOURCES.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)        1 2024-04-17 00:52:29.000000 llmaudit-0.0.9/llmaudit.egg-info/dependency_links.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)       51 2024-04-17 00:52:29.000000 llmaudit-0.0.9/llmaudit.egg-info/entry_points.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)       37 2024-04-17 00:52:29.000000 llmaudit-0.0.9/llmaudit.egg-info/requires.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)        9 2024-04-17 00:52:29.000000 llmaudit-0.0.9/llmaudit.egg-info/top_level.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      777 2024-04-17 00:52:24.000000 llmaudit-0.0.9/pyproject.toml
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)       38 2024-04-17 00:52:29.592402 llmaudit-0.0.9/setup.cfg
```

### Comparing `llmaudit-0.0.8/LICENSE` & `llmaudit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llmaudit-0.0.8/PKG-INFO` & `llmaudit-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmaudit
-Version: 0.0.8
+Version: 0.0.9
 Summary: A CLI tool to find LLM usage accross your repos
 Author-email: PromptArmor <founders@promptarmor.com>
 Project-URL: Company Page, https://promptarmor.com/
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llmaudit-0.0.8/llmaudit/cli.py` & `llmaudit-0.0.9/llmaudit/cli.py`

 * *Files identical despite different names*

### Comparing `llmaudit-0.0.8/llmaudit/logo.png` & `llmaudit-0.0.9/llmaudit/logo.png`

 * *Files identical despite different names*

### Comparing `llmaudit-0.0.8/llmaudit/report_template.html` & `llmaudit-0.0.9/llmaudit/report_template.html`

 * *Files identical despite different names*

### Comparing `llmaudit-0.0.8/llmaudit/scan_github_repos.py` & `llmaudit-0.0.9/llmaudit/scan_github_repos.py`

 * *Files identical despite different names*

### Comparing `llmaudit-0.0.8/llmaudit/sprawl.py` & `llmaudit-0.0.9/llmaudit/sprawl.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,16 @@
         # Identifying top owners based on the number of occurrences across repos
         top_owners = sorted(owner_usage.items(), key=lambda x: x[1], reverse=True)
 
         return {"total_usage_by_library": total_usage_by_library, "total_usages": total_usages, "top_owners": top_owners}
     
     @staticmethod
     def generate_report():
-        env = Environment(loader=FileSystemLoader('.'))
+        template_dir = os.path.dirname(__file__)
+        env = Environment(loader=FileSystemLoader(template_dir))
         template = env.get_template('report_template.html')
 
         aggregate_stats = LLMUsageScanner._aggregate_usage()
         repo_stats = {repo_name: {"total_usages": stats[0], 
                                   "library_counts": stats[1], 
                                   "owner_counts": dict(sorted(stats[2].items(), key=lambda item: item[1], reverse=True)[:3])}
                       for repo_name, stats in LLMUsageScanner.stats.items()}
```

### Comparing `llmaudit-0.0.8/llmaudit.egg-info/PKG-INFO` & `llmaudit-0.0.9/llmaudit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmaudit
-Version: 0.0.8
+Version: 0.0.9
 Summary: A CLI tool to find LLM usage accross your repos
 Author-email: PromptArmor <founders@promptarmor.com>
 Project-URL: Company Page, https://promptarmor.com/
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llmaudit-0.0.8/pyproject.toml` & `llmaudit-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmaudit"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="PromptArmor", email="founders@promptarmor.com" },
 ]
 description = "A CLI tool to find LLM usage accross your repos"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

