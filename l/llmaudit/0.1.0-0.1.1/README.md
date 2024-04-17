# Comparing `tmp/llmaudit-0.1.0.tar.gz` & `tmp/llmaudit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmaudit-0.1.0.tar", last modified: Wed Apr 17 01:38:27 2024, max compression
+gzip compressed data, was "llmaudit-0.1.1.tar", last modified: Wed Apr 17 01:45:26 2024, max compression
```

## Comparing `llmaudit-0.1.0.tar` & `llmaudit-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 01:38:27.840486 llmaudit-0.1.0/
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)    11356 2024-04-16 23:43:48.000000 llmaudit-0.1.0/LICENSE
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 01:38:27.839842 llmaudit-0.1.0/PKG-INFO
-drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 01:38:27.833773 llmaudit-0.1.0/llmaudit/
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)        0 2024-04-16 23:48:32.000000 llmaudit-0.1.0/llmaudit/__init__.py
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)     1662 2024-04-17 00:29:07.000000 llmaudit-0.1.0/llmaudit/cli.py
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)     7405 2024-01-24 08:06:20.000000 llmaudit-0.1.0/llmaudit/logo.png
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)     4801 2024-04-17 01:38:03.000000 llmaudit-0.1.0/llmaudit/report_template.html
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)     2823 2024-04-17 00:29:22.000000 llmaudit-0.1.0/llmaudit/scan_github_repos.py
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)    15615 2024-04-17 01:00:12.000000 llmaudit-0.1.0/llmaudit/sprawl.py
-drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 01:38:27.838720 llmaudit-0.1.0/llmaudit.egg-info/
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 01:38:27.000000 llmaudit-0.1.0/llmaudit.egg-info/PKG-INFO
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      350 2024-04-17 01:38:27.000000 llmaudit-0.1.0/llmaudit.egg-info/SOURCES.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)        1 2024-04-17 01:38:27.000000 llmaudit-0.1.0/llmaudit.egg-info/dependency_links.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)       51 2024-04-17 01:38:27.000000 llmaudit-0.1.0/llmaudit.egg-info/entry_points.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)       37 2024-04-17 01:38:27.000000 llmaudit-0.1.0/llmaudit.egg-info/requires.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)        9 2024-04-17 01:38:27.000000 llmaudit-0.1.0/llmaudit.egg-info/top_level.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      777 2024-04-17 01:38:22.000000 llmaudit-0.1.0/pyproject.toml
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)       38 2024-04-17 01:38:27.840608 llmaudit-0.1.0/setup.cfg
+drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 01:45:26.653201 llmaudit-0.1.1/
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)    11356 2024-04-16 23:43:48.000000 llmaudit-0.1.1/LICENSE
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 01:45:26.652475 llmaudit-0.1.1/PKG-INFO
+drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 01:45:26.647888 llmaudit-0.1.1/llmaudit/
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)        0 2024-04-16 23:48:32.000000 llmaudit-0.1.1/llmaudit/__init__.py
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     1662 2024-04-17 00:29:07.000000 llmaudit-0.1.1/llmaudit/cli.py
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     7405 2024-01-24 08:06:20.000000 llmaudit-0.1.1/llmaudit/logo.png
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     5459 2024-04-17 01:45:07.000000 llmaudit-0.1.1/llmaudit/report_template.html
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     2823 2024-04-17 00:29:22.000000 llmaudit-0.1.1/llmaudit/scan_github_repos.py
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)    15615 2024-04-17 01:00:12.000000 llmaudit-0.1.1/llmaudit/sprawl.py
+drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 01:45:26.651568 llmaudit-0.1.1/llmaudit.egg-info/
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 01:45:26.000000 llmaudit-0.1.1/llmaudit.egg-info/PKG-INFO
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      350 2024-04-17 01:45:26.000000 llmaudit-0.1.1/llmaudit.egg-info/SOURCES.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)        1 2024-04-17 01:45:26.000000 llmaudit-0.1.1/llmaudit.egg-info/dependency_links.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)       51 2024-04-17 01:45:26.000000 llmaudit-0.1.1/llmaudit.egg-info/entry_points.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)       37 2024-04-17 01:45:26.000000 llmaudit-0.1.1/llmaudit.egg-info/requires.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)        9 2024-04-17 01:45:26.000000 llmaudit-0.1.1/llmaudit.egg-info/top_level.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      777 2024-04-17 01:45:14.000000 llmaudit-0.1.1/pyproject.toml
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)       38 2024-04-17 01:45:26.653372 llmaudit-0.1.1/setup.cfg
```

### Comparing `llmaudit-0.1.0/LICENSE` & `llmaudit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmaudit-0.1.0/PKG-INFO` & `llmaudit-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmaudit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI tool to find LLM usage accross your repos
 Author-email: PromptArmor <founders@promptarmor.com>
 Project-URL: Company Page, https://promptarmor.com/
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llmaudit-0.1.0/llmaudit/cli.py` & `llmaudit-0.1.1/llmaudit/cli.py`

 * *Files identical despite different names*

### Comparing `llmaudit-0.1.0/llmaudit/logo.png` & `llmaudit-0.1.1/llmaudit/logo.png`

 * *Files identical despite different names*

### Comparing `llmaudit-0.1.0/llmaudit/report_template.html` & `llmaudit-0.1.1/llmaudit/report_template.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <title>PromptArmor AI Usage Report</title>
+    <title>PromptArmor Gen AI Usage Report</title>
     <link href="https://fonts.googleapis.com/css?family=Roboto:400,700&display=swap" rel="stylesheet">
     <link rel="icon" type="image/png" href="logo.png">
     <style>
         body { 
             font-family: 'Roboto', sans-serif; 
             color: #333; 
             background-color: #f4f4f4; 
@@ -25,46 +25,48 @@
         .header .date {
             color: #757575;
         }
         .statistics { 
             display: flex; 
             justify-content: space-around;
             align-items: flex-start;
-            background: #fff; 
-            box-shadow: 0 2px 4px rgba(0,0,0,0.1); 
-            border-radius: 8px; 
-            padding: 20px; 
+            background: #f4f4f4; 
+            /* box-shadow: 0 2px 4px rgba(0,0,0,0.1);  */
+            /* border-radius: 8px;  */
+            /* padding: 20px;  */
             margin-bottom: 20px; 
             flex-wrap: wrap;
         }
         .section { 
             flex: 1;
             min-width: 150px;
             margin: 10px; 
             text-align: center; 
         }
         .section h2 {
             color: #1a1a1a;
+            text-align: left;
             font-weight: 700;
             margin-bottom: 10px;
         }
         .repo-stats-header {
             font-size: 1.5em;
             font-weight: bold;
-            margin-bottom: 20px;
+            /* margin-bottom: 20px; */
+            margin: 10px; 
         }
         .repo-stats { 
             display: flex; 
             flex-wrap: wrap;
             justify-content: space-between; /* Adjusted for consistent spacing */
             align-items: flex-start;
-            background: #fff; 
-            box-shadow: 0 2px 4px rgba(0,0,0,0.1); 
-            border-radius: 8px; 
-            padding: 20px; 
+            background: #f4f4f4; 
+            /* box-shadow: 0 2px 4px rgba(0,0,0,0.1);  */
+            border-radius: 0px; 
+            padding: 10px; 
             margin-bottom: 20px; 
         }
         .repo-section { 
             flex: 0 0 calc(50% - 20px); /* Adjusted to prevent boxes from shrinking */
             box-sizing: border-box;
             border: 1px solid #eaeaea; 
             border-radius: 8px; 
@@ -85,47 +87,54 @@
         }
     </style>
 </head>
 <body>
     <div class="header">
         <div style="display: flex; align-items: center; justify-content: center;">
             <img src="logo.png" alt="PromptArmor Logo" style="float:left; margin-right:10px; height:3em;">
-            <h1>PromptArmor AI Usage Report</h1>
+            <h1>PromptArmor Gen AI Usage Report</h1>
         </div>
         <p class="date" id="reportDate"></p>
     </div>
-    <div class="statistics">
-        <div class="section">
-            <h2>Total # Entrypoints</h2>
-            <p>{{ total_usages }}</p>
+<div class="statistics">
+    <div class="section">
+        <h2>Total # Entrypoints</h2>
+        <div style="padding: 20px; background: #fff; box-shadow: 0 2px 4px rgba(0,0,0,0.1); border-radius: 8px; min-height: 120px; justify-content: center;">
+            <p style="font-size: 80px; margin: 0; line-height: 120px; font-weight: bold;">{{ total_usages }}</p>
         </div>
-        <div class="section">
-            <h2>Entrypoints by LLM Provider</h2>
+    </div>
+    <div class="section">
+        <h2>Entrypoints by LLM Provider</h2>
+        <div style="padding: 20px; background: #fff; box-shadow: 0 2px 4px rgba(0,0,0,0.1); border-radius: 8px; min-height: 120px;">
             {% for library, count in total_usage_by_library.items() %}
             <p>{{ library }}: {{ count }}</p>
             {% endfor %}
         </div>
-        <div class="section">
-            <h2>Top Owners</h2>
+    </div>
+    <div class="section">
+        <h2>Top Owners</h2>
+        <div style="padding: 20px; background: #fff; box-shadow: 0 2px 4px rgba(0,0,0,0.1); border-radius: 8px; min-height: 120px;">
             {% for owner, count in top_owners %}
             <p>{{ owner }}: {{ count }} entrypoints</p>
             {% endfor %}
         </div>
     </div>
+</div>
     <div class="repo-stats-header">
         Stats by Repo
     </div>
     <div class="repo-stats">
         {% for repo_name, stats in repo_stats.items() %}
         <div class="repo-section">
             <h3>Repo: {{ repo_name }}</h3>
             <p><strong>Total Entrypoints:</strong> {{ stats.total_usages }}</p>
             <p><strong>Libraries:</strong> {{ stats.library_counts.keys()|join(', ') }}</p>
+            <p><strong>Top Owners:</strong></p>
             <ul>
-                <li><strong>Top Owners:</strong></li>
+                <!-- <li><strong>Top Owners:</strong></li> -->
                 {% for owner, count in stats.owner_counts.items() %}
                 <li>USERNAME, @{{ owner }}: {{ count }} entrypoints</li>
                 {% endfor %}
             </ul>
         </div>
         {% endfor %}
     </div>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 [PromptArmor Logo]
-************ PPrroommppttAArrmmoorr AAII UUssaaggee RReeppoorrtt ************
+************ PPrroommppttAArrmmoorr GGeenn AAII UUssaaggee RReeppoorrtt ************
 ********** TToottaall ## EEnnttrryyppooiinnttss **********
 {{ total_usages }}
 ********** EEnnttrryyppooiinnttss bbyy LLLLMM PPrroovviiddeerr **********
 {% for library, count in total_usage_by_library.items() %}
 {{ library }}: {{ count }}
 {% endfor %}
 ********** TToopp OOwwnneerrss **********
@@ -11,14 +11,14 @@
 {{ owner }}: {{ count }} entrypoints
 {% endfor %}
 Stats by Repo
 {% for repo_name, stats in repo_stats.items() %}
 ******** RReeppoo:: {{{{ rreeppoo__nnaammee }}}} ********
 TToottaall EEnnttrryyppooiinnttss:: {{ stats.total_usages }}
 LLiibbrraarriieess:: {{ stats.library_counts.keys()|join(', ') }}
-    * TToopp OOwwnneerrss::
+TToopp OOwwnneerrss::
     * {% for owner, count in stats.owner_counts.items() %}
     * USERNAME, @{{ owner }}: {{ count }} entrypoints
     * {% endfor %}
 {% endfor %}
 For more information, visit _P_r_o_m_p_t_A_r_m_o_r or reach out to
 founders@promptarmor.com
```

### Comparing `llmaudit-0.1.0/llmaudit/scan_github_repos.py` & `llmaudit-0.1.1/llmaudit/scan_github_repos.py`

 * *Files identical despite different names*

### Comparing `llmaudit-0.1.0/llmaudit/sprawl.py` & `llmaudit-0.1.1/llmaudit/sprawl.py`

 * *Files identical despite different names*

### Comparing `llmaudit-0.1.0/llmaudit.egg-info/PKG-INFO` & `llmaudit-0.1.1/llmaudit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmaudit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI tool to find LLM usage accross your repos
 Author-email: PromptArmor <founders@promptarmor.com>
 Project-URL: Company Page, https://promptarmor.com/
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llmaudit-0.1.0/pyproject.toml` & `llmaudit-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmaudit"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="PromptArmor", email="founders@promptarmor.com" },
 ]
 description = "A CLI tool to find LLM usage accross your repos"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

