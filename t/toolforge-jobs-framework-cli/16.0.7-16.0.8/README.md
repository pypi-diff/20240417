# Comparing `tmp/toolforge-jobs-framework-cli-16.0.7.tar.gz` & `tmp/toolforge_jobs_framework_cli-16.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge-jobs-framework-cli-16.0.7.tar", last modified: Wed Apr 10 14:58:03 2024, max compression
+gzip compressed data, was "toolforge_jobs_framework_cli-16.0.8.tar", last modified: Wed Apr 17 14:06:50 2024, max compression
```

## Comparing `toolforge-jobs-framework-cli-16.0.7.tar` & `toolforge_jobs_framework_cli-16.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:03.784200 toolforge-jobs-framework-cli-16.0.7/
--rw-rw-rw-   0 root         (0) root         (0)    35120 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      355 2024-04-10 14:58:03.784200 toolforge-jobs-framework-cli-16.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2318 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 14:58:03.784200 toolforge-jobs-framework-cli-16.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      487 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:03.784200 toolforge-jobs-framework-cli-16.0.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2651 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)    11090 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tests/test_dump.py
--rw-rw-rw-   0 root         (0) root         (0)     6173 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tests/test_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:03.784200 toolforge-jobs-framework-cli-16.0.7/tjf_cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tjf_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1938 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tjf_cli/api.py
--rw-rw-rw-   0 root         (0) root         (0)    32304 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tjf_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tjf_cli/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     3799 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tjf_cli/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:03.784200 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      355 2024-04-10 14:58:03.000000 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-10 14:58:03.000000 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 14:58:03.000000 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-10 14:58:03.000000 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-10 14:58:03.000000 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-10 14:58:03.000000 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:06:50.177981 toolforge_jobs_framework_cli-16.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)    35120 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      355 2024-04-17 14:06:50.177981 toolforge_jobs_framework_cli-16.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 14:06:50.177981 toolforge_jobs_framework_cli-16.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:06:50.173981 toolforge_jobs_framework_cli-16.0.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2651 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    11090 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tests/test_dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     6173 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tests/test_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:06:50.173981 toolforge_jobs_framework_cli-16.0.8/tjf_cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tjf_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tjf_cli/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    32304 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tjf_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tjf_cli/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3799 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tjf_cli/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:06:50.177981 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      355 2024-04-17 14:06:50.000000 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-17 14:06:50.000000 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 14:06:50.000000 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-17 14:06:50.000000 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-17 14:06:50.000000 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-17 14:06:50.000000 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/top_level.txt
```

### Comparing `toolforge-jobs-framework-cli-16.0.7/LICENSE` & `toolforge_jobs_framework_cli-16.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.7/README.md` & `toolforge_jobs_framework_cli-16.0.8/README.md`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.7/tests/test_api.py` & `toolforge_jobs_framework_cli-16.0.8/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.7/tests/test_dump.py` & `toolforge_jobs_framework_cli-16.0.8/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.7/tests/test_loader.py` & `toolforge_jobs_framework_cli-16.0.8/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.7/tjf_cli/api.py` & `toolforge_jobs_framework_cli-16.0.8/tjf_cli/api.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.7/tjf_cli/cli.py` & `toolforge_jobs_framework_cli-16.0.8/tjf_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1002,15 +1002,15 @@
     logging.addLevelName(
         logging.WARNING, "\033[1;33m%s\033[1;0m" % logging.getLevelName(logging.WARNING)
     )
     logging.addLevelName(
         logging.ERROR, "\033[1;31m%s\033[1;0m" % logging.getLevelName(logging.ERROR)
     )
     logging.basicConfig(
-        format=logging_format, level=logging_level, stream=sys.stdout, datefmt="%Y-%m-%d %H:%M:%S"
+        format=logging_format, level=logging_level, stream=sys.stderr, datefmt="%Y-%m-%d %H:%M:%S"
     )
 
     user = getpass.getuser()
     project_file = Path("/etc/wmcs-project")
     if project_file.exists():
         project = project_file.read_text().strip()
     else:
```

### Comparing `toolforge-jobs-framework-cli-16.0.7/tjf_cli/errors.py` & `toolforge_jobs_framework_cli-16.0.8/tjf_cli/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.7/tjf_cli/loader.py` & `toolforge_jobs_framework_cli-16.0.8/tjf_cli/loader.py`

 * *Files identical despite different names*

