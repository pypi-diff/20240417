# Comparing `tmp/snakemake_executor_plugin_slurm-0.4.4.tar.gz` & `tmp/snakemake_executor_plugin_slurm-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_executor_plugin_slurm-0.4.4.tar", max compression
+gzip compressed data, was "snakemake_executor_plugin_slurm-0.4.5.tar", max compression
```

## Comparing `snakemake_executor_plugin_slurm-0.4.4.tar` & `snakemake_executor_plugin_slurm-0.4.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2024-04-15 09:17:24.183849 snakemake_executor_plugin_slurm-0.4.4/LICENSE
--rw-r--r--   0        0        0      319 2024-04-15 09:17:24.183849 snakemake_executor_plugin_slurm-0.4.4/README.md
--rw-r--r--   0        0        0     1151 2024-04-15 09:17:24.183849 snakemake_executor_plugin_slurm-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    20100 2024-04-15 09:17:24.183849 snakemake_executor_plugin_slurm-0.4.4/snakemake_executor_plugin_slurm/__init__.py
--rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 snakemake_executor_plugin_slurm-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-17 12:12:52.719136 snakemake_executor_plugin_slurm-0.4.5/LICENSE
+-rw-r--r--   0        0        0      319 2024-04-17 12:12:52.719136 snakemake_executor_plugin_slurm-0.4.5/README.md
+-rw-r--r--   0        0        0     1151 2024-04-17 12:12:52.719136 snakemake_executor_plugin_slurm-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0    20094 2024-04-17 12:12:52.719136 snakemake_executor_plugin_slurm-0.4.5/snakemake_executor_plugin_slurm/__init__.py
+-rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 snakemake_executor_plugin_slurm-0.4.5/PKG-INFO
```

### Comparing `snakemake_executor_plugin_slurm-0.4.4/LICENSE` & `snakemake_executor_plugin_slurm-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_slurm-0.4.4/pyproject.toml` & `snakemake_executor_plugin_slurm-0.4.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-executor-plugin-slurm"
-version = "0.4.4"
+version = "0.4.5"
 description = "A Snakemake executor plugin for submitting jobs to a SLURM cluster."
 authors = [
     "Christian Meesters <meesters@uni-mainz.de>",
     "David Lähnemann <david.laehnemann@dkfz-heidelberg.de>",
     "Johannes Koester <johannes.koester@uni-due.de>",
 ]
 readme = "README.md"
```

### Comparing `snakemake_executor_plugin_slurm-0.4.4/snakemake_executor_plugin_slurm/__init__.py` & `snakemake_executor_plugin_slurm-0.4.5/snakemake_executor_plugin_slurm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         # self.report_job_submission(job_info).
         # with job_info being of type
         # snakemake_interface_executor_plugins.executors.base.SubmittedJobInfo.
 
         group_or_rule = f"group_{job.name}" if job.is_group() else f"rule_{job.name}"
 
         try:
-            wildcard_str = f"_{'_'.join(job.wildcards)}" if job.wildcards else ""
+            wildcard_str = "_".join(job.wildcards) if job.wildcards else ""
         except AttributeError:
             wildcard_str = ""
 
         slurm_logfile = os.path.abspath(
             f".snakemake/slurm_logs/{group_or_rule}/{wildcard_str}/%j.log"
         )
         logdir = os.path.dirname(slurm_logfile)
```

### Comparing `snakemake_executor_plugin_slurm-0.4.4/PKG-INFO` & `snakemake_executor_plugin_slurm-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-executor-plugin-slurm
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Snakemake executor plugin for submitting jobs to a SLURM cluster.
 Home-page: https://github.com/snakemake/snakemake-executor-plugin-slurm
 License: MIT
 Keywords: snakemake,plugin,executor,cluster,slurm
 Author: Christian Meesters
 Author-email: meesters@uni-mainz.de
 Requires-Python: >=3.11,<4.0
```

