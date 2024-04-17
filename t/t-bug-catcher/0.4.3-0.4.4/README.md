# Comparing `tmp/t_bug_catcher-0.4.3.tar.gz` & `tmp/t_bug_catcher-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-5govxv9y/t_bug_catcher-0.4.3.tar", last modified: Mon Apr 15 11:02:43 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-rt3__0l8/t_bug_catcher-0.4.4.tar", last modified: Wed Apr 17 08:22:43 2024, max compression
```

## Comparing `t_bug_catcher-0.4.3.tar` & `t_bug_catcher-0.4.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/t_bug_catcher/
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10746 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/bug_catcher.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/bug_snag.py
--rw-rw-rw-   0 root         (0) root         (0)     1537 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/config.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    45412 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/jira.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/t_bug_catcher/resources/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/resources/whispers_config.yml
--rw-rw-rw-   0 root         (0) root         (0)     5578 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/stack_saver.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/t_bug_catcher/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2051 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/utils/common.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/workitems.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-15 11:02:43.000000 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      668 2024-04-15 11:02:43.000000 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-15 11:02:43.000000 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-15 11:02:43.000000 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-15 11:02:43.000000 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-15 11:02:43.000000 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/tests/test_t_bug_catcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 08:22:43.301112 t_bug_catcher-0.4.4/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-17 08:22:43.301112 t_bug_catcher-0.4.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-17 08:22:43.301112 t_bug_catcher-0.4.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 08:22:43.297112 t_bug_catcher-0.4.4/t_bug_catcher/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11049 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/bug_catcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/bug_snag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    45412 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/jira.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 08:22:43.297112 t_bug_catcher-0.4.4/t_bug_catcher/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/resources/whispers_config.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5578 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/stack_saver.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 08:22:43.301112 t_bug_catcher-0.4.4/t_bug_catcher/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2051 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/utils/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/workitems.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 08:22:43.301112 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-17 08:22:43.000000 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      668 2024-04-17 08:22:43.000000 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-17 08:22:43.000000 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-17 08:22:43.000000 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-17 08:22:43.000000 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-17 08:22:43.000000 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 08:22:43.301112 t_bug_catcher-0.4.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/tests/test_t_bug_catcher.py
```

### Comparing `t_bug_catcher-0.4.3/PKG-INFO` & `t_bug_catcher-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.3
+Version: 0.4.4
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.3/README.rst` & `t_bug_catcher-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.3/setup.py` & `t_bug_catcher-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,13 +22,13 @@
     description="Bug catcher",
     long_description=readme,
     keywords="t_bug_catcher",
     name="t_bug_catcher",
     packages=find_packages(include=["t_bug_catcher", "t_bug_catcher.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.4.3",
+    version="0.4.4",
     zip_safe=False,
     install_requires=install_requirements,
     include_package_data=True,
     package_data={"": ["resources/*.yml"]},
 )
```

### Comparing `t_bug_catcher-0.4.3/t_bug_catcher/bug_catcher.py` & `t_bug_catcher-0.4.4/t_bug_catcher/bug_catcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,22 @@
         if not self.__configurator.is_jira_configured and not self.__configurator.is_bugsnag_configured:
             logger.warning("Jira and BugSnag are not configured. Please configure them before reporting an error.")
             return
 
         if not exception:
             _, exception, _ = sys.exc_info()
 
+        if not isinstance(exception, Exception):
+            logger.warning("Exception must be an instance of Exception.")
+            return
+
+        if not getattr(exception, "__traceback__", None):
+            logger.warning("No traceback available. Please provide a traceback.")
+            return
+
         handled_error = getattr(exception, "handled_error", None)
         if handled_error:
             logger.warning(f"Exception {handled_error} already reported.")
             return
 
         stack_trace = self.__stack_saver.save_stack_trace(exception)
```

### Comparing `t_bug_catcher-0.4.3/t_bug_catcher/bug_snag.py` & `t_bug_catcher-0.4.4/t_bug_catcher/bug_snag.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.3/t_bug_catcher/config.py` & `t_bug_catcher-0.4.4/t_bug_catcher/config.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.3/t_bug_catcher/jira.py` & `t_bug_catcher-0.4.4/t_bug_catcher/jira.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.3/t_bug_catcher/resources/whispers_config.yml` & `t_bug_catcher-0.4.4/t_bug_catcher/resources/whispers_config.yml`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.3/t_bug_catcher/stack_saver.py` & `t_bug_catcher-0.4.4/t_bug_catcher/stack_saver.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.3/t_bug_catcher/utils/common.py` & `t_bug_catcher-0.4.4/t_bug_catcher/utils/common.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.3/t_bug_catcher/utils/logger.py` & `t_bug_catcher-0.4.4/t_bug_catcher/utils/logger.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.3/t_bug_catcher.egg-info/PKG-INFO` & `t_bug_catcher-0.4.4/t_bug_catcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.3
+Version: 0.4.4
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.3/t_bug_catcher.egg-info/SOURCES.txt` & `t_bug_catcher-0.4.4/t_bug_catcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.3/tests/test_t_bug_catcher.py` & `t_bug_catcher-0.4.4/tests/test_t_bug_catcher.py`

 * *Files identical despite different names*

