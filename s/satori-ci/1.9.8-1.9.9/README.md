# Comparing `tmp/satori_ci-1.9.8.tar.gz` & `tmp/satori_ci-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_ci-1.9.8.tar", last modified: Tue Sep 26 21:44:22 2023, max compression
+gzip compressed data, was "satori_ci-1.9.9.tar", last modified: Tue Sep 26 22:30:04 2023, max compression
```

## Comparing `satori_ci-1.9.8.tar` & `satori_ci-1.9.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-09-26 21:44:06.719470 satori_ci-1.9.8/LICENSE
--rw-r--r--   0        0        0     6987 2023-09-26 21:44:06.719470 satori_ci-1.9.8/README.md
--rw-r--r--   0        0        0      703 2023-09-26 21:44:22.855886 satori_ci-1.9.8/pyproject.toml
--rw-r--r--   0        0        0       22 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/__init__.py
--rw-r--r--   0        0        0       27 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/__main__.py
--rw-r--r--   0        0        0      526 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/api.py
--rw-r--r--   0        0        0     1614 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/bundler.py
--rw-r--r--   0        0        0     1225 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/__init__.py
--rw-r--r--   0        0        0      617 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/arguments.py
--rw-r--r--   0        0        0     1607 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/base.py
--rw-r--r--   0        0        0     1367 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/config.py
--rw-r--r--   0        0        0     1588 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/dashboard.py
--rw-r--r--   0        0        0      428 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/help.py
--rw-r--r--   0        0        0     2752 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/monitor.py
--rw-r--r--   0        0        0     1910 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/outputs.py
--rw-r--r--   0        0        0     2384 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/playbook.py
--rw-r--r--   0        0        0     6660 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/repo.py
--rw-r--r--   0        0        0     2917 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/report.py
--rw-r--r--   0        0        0     1196 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/root.py
--rw-r--r--   0        0        0    10408 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/run.py
--rw-r--r--   0        0        0     4785 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/scan.py
--rw-r--r--   0        0        0     3694 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/team.py
--rw-r--r--   0        0        0      589 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/commands/update.py
--rw-r--r--   0        0        0    13794 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/cli/utils.py
--rw-r--r--   0        0        0     3368 2023-09-26 21:44:06.719470 satori_ci-1.9.8/src/satoricli/playbooks.py
--rw-r--r--   0        0        0      527 2023-09-26 21:44:06.723470 satori_ci-1.9.8/src/satoricli/utils.py
--rw-r--r--   0        0        0     2189 2023-09-26 21:44:06.723470 satori_ci-1.9.8/src/satoricli/validations.py
--rw-r--r--   0        0        0    48099 1970-01-01 00:00:00.000000 satori_ci-1.9.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-09-26 22:29:48.504932 satori_ci-1.9.9/LICENSE
+-rw-r--r--   0        0        0     6987 2023-09-26 22:29:48.504932 satori_ci-1.9.9/README.md
+-rw-r--r--   0        0        0      703 2023-09-26 22:30:04.011597 satori_ci-1.9.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/__init__.py
+-rw-r--r--   0        0        0       27 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/__main__.py
+-rw-r--r--   0        0        0      526 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/api.py
+-rw-r--r--   0        0        0     1614 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/bundler.py
+-rw-r--r--   0        0        0     1225 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/__init__.py
+-rw-r--r--   0        0        0      617 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/arguments.py
+-rw-r--r--   0        0        0     1607 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/base.py
+-rw-r--r--   0        0        0     1367 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/config.py
+-rw-r--r--   0        0        0     1588 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/dashboard.py
+-rw-r--r--   0        0        0      428 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/help.py
+-rw-r--r--   0        0        0     2752 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/monitor.py
+-rw-r--r--   0        0        0     1910 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/outputs.py
+-rw-r--r--   0        0        0     2384 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/playbook.py
+-rw-r--r--   0        0        0     6660 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/repo.py
+-rw-r--r--   0        0        0     2917 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/report.py
+-rw-r--r--   0        0        0     1196 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/root.py
+-rw-r--r--   0        0        0    10404 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/run.py
+-rw-r--r--   0        0        0     4785 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/scan.py
+-rw-r--r--   0        0        0     3694 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/team.py
+-rw-r--r--   0        0        0      589 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/commands/update.py
+-rw-r--r--   0        0        0    13794 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/cli/utils.py
+-rw-r--r--   0        0        0     3368 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/playbooks.py
+-rw-r--r--   0        0        0      527 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/utils.py
+-rw-r--r--   0        0        0     2189 2023-09-26 22:29:48.508933 satori_ci-1.9.9/src/satoricli/validations.py
+-rw-r--r--   0        0        0    48099 1970-01-01 00:00:00.000000 satori_ci-1.9.9/PKG-INFO
```

### Comparing `satori_ci-1.9.8/LICENSE` & `satori_ci-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/README.md` & `satori_ci-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/pyproject.toml` & `satori_ci-1.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-ci"
-version = "1.9.8"
+version = "1.9.9"
 description = "Satori CI - Automated Software Testing Platform"
 authors = [
     { name = "Satori CI CLI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "satori-playbook-validator==3.3.2",
     "satori-docs==1.3.1",
```

### Comparing `satori_ci-1.9.8/src/satoricli/api.py` & `satori_ci-1.9.9/src/satoricli/api.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/bundler.py` & `satori_ci-1.9.9/src/satoricli/bundler.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/__init__.py` & `satori_ci-1.9.9/src/satoricli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/arguments.py` & `satori_ci-1.9.9/src/satoricli/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/commands/base.py` & `satori_ci-1.9.9/src/satoricli/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/commands/config.py` & `satori_ci-1.9.9/src/satoricli/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/commands/dashboard.py` & `satori_ci-1.9.9/src/satoricli/cli/commands/dashboard.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/commands/monitor.py` & `satori_ci-1.9.9/src/satoricli/cli/commands/monitor.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/commands/outputs.py` & `satori_ci-1.9.9/src/satoricli/cli/commands/outputs.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/commands/playbook.py` & `satori_ci-1.9.9/src/satoricli/cli/commands/playbook.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/commands/repo.py` & `satori_ci-1.9.9/src/satoricli/cli/commands/repo.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/commands/report.py` & `satori_ci-1.9.9/src/satoricli/cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/commands/root.py` & `satori_ci-1.9.9/src/satoricli/cli/commands/root.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/commands/run.py` & `satori_ci-1.9.9/src/satoricli/cli/commands/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 
             progress.update(task, description=status)
             time.sleep(1)
 
     result = report_data.get("result", "Unknown")
     if not any((report, output, files)) or result == "Unknown":
         if comments := report_data.get("user_warnings"):
-            error_console.print(f"[warning]WARNING:[/] {comments}")
+            error_console.print(f"[error]Error:[/] {comments}")
 
         if result == "Unknown":
             console.print("Result: Unknown")
             return 1
 
         fails = report_data["fails"]
```

### Comparing `satori_ci-1.9.8/src/satoricli/cli/commands/scan.py` & `satori_ci-1.9.9/src/satoricli/cli/commands/scan.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/commands/team.py` & `satori_ci-1.9.9/src/satoricli/cli/commands/team.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/commands/update.py` & `satori_ci-1.9.9/src/satoricli/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/cli/utils.py` & `satori_ci-1.9.9/src/satoricli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/playbooks.py` & `satori_ci-1.9.9/src/satoricli/playbooks.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/utils.py` & `satori_ci-1.9.9/src/satoricli/utils.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/src/satoricli/validations.py` & `satori_ci-1.9.9/src/satoricli/validations.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.9.8/PKG-INFO` & `satori_ci-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-ci
-Version: 1.9.8
+Version: 1.9.9
 Summary: Satori CI - Automated Software Testing Platform
 Author-Email: Satori CI CLI <info@satori-ci.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

