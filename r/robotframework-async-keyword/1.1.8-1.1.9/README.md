# Comparing `tmp/robotframework-async-keyword-1.1.8.tar.gz` & `tmp/robotframework_async_keyword-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-async-keyword-1.1.8.tar", last modified: Fri Mar 15 21:18:51 2024, max compression
+gzip compressed data, was "robotframework_async_keyword-1.1.9.tar", last modified: Wed Apr 17 09:10:46 2024, max compression
```

## Comparing `robotframework-async-keyword-1.1.8.tar` & `robotframework_async_keyword-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 21:18:51.567269 robotframework-async-keyword-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 21:18:51.563269 robotframework-async-keyword-1.1.8/AsyncLibrary/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-15 21:18:45.000000 robotframework-async-keyword-1.1.8/AsyncLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-15 21:18:51.000000 robotframework-async-keyword-1.1.8/AsyncLibrary/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-15 21:18:45.000000 robotframework-async-keyword-1.1.8/AsyncLibrary/protected_ordered_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    16901 2024-03-15 21:18:45.000000 robotframework-async-keyword-1.1.8/AsyncLibrary/robot_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-03-15 21:18:45.000000 robotframework-async-keyword-1.1.8/AsyncLibrary/scoped_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-15 21:18:45.000000 robotframework-async-keyword-1.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-15 21:18:45.000000 robotframework-async-keyword-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-15 21:18:51.567269 robotframework-async-keyword-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-03-15 21:18:45.000000 robotframework-async-keyword-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-15 21:18:45.000000 robotframework-async-keyword-1.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 21:18:51.567269 robotframework-async-keyword-1.1.8/robotframework_async_keyword.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-15 21:18:51.000000 robotframework-async-keyword-1.1.8/robotframework_async_keyword.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-15 21:18:51.000000 robotframework-async-keyword-1.1.8/robotframework_async_keyword.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 21:18:51.000000 robotframework-async-keyword-1.1.8/robotframework_async_keyword.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-15 21:18:51.000000 robotframework-async-keyword-1.1.8/robotframework_async_keyword.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-15 21:18:51.000000 robotframework-async-keyword-1.1.8/robotframework_async_keyword.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 21:18:51.567269 robotframework-async-keyword-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-15 21:18:45.000000 robotframework-async-keyword-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 21:18:51.567269 robotframework-async-keyword-1.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-15 21:18:45.000000 robotframework-async-keyword-1.1.8/test/test.robot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:10:46.348472 robotframework_async_keyword-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:10:46.344472 robotframework_async_keyword-1.1.9/AsyncLibrary/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-17 09:10:40.000000 robotframework_async_keyword-1.1.9/AsyncLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 09:10:45.000000 robotframework_async_keyword-1.1.9/AsyncLibrary/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-17 09:10:40.000000 robotframework_async_keyword-1.1.9/AsyncLibrary/protected_ordered_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17015 2024-04-17 09:10:40.000000 robotframework_async_keyword-1.1.9/AsyncLibrary/robot_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-17 09:10:40.000000 robotframework_async_keyword-1.1.9/AsyncLibrary/scoped_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-17 09:10:40.000000 robotframework_async_keyword-1.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 09:10:40.000000 robotframework_async_keyword-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-17 09:10:46.344472 robotframework_async_keyword-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-17 09:10:40.000000 robotframework_async_keyword-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-17 09:10:40.000000 robotframework_async_keyword-1.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:10:46.344472 robotframework_async_keyword-1.1.9/robotframework_async_keyword.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-17 09:10:46.000000 robotframework_async_keyword-1.1.9/robotframework_async_keyword.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 09:10:46.000000 robotframework_async_keyword-1.1.9/robotframework_async_keyword.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:10:46.000000 robotframework_async_keyword-1.1.9/robotframework_async_keyword.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 09:10:46.000000 robotframework_async_keyword-1.1.9/robotframework_async_keyword.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 09:10:46.000000 robotframework_async_keyword-1.1.9/robotframework_async_keyword.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:10:46.348472 robotframework_async_keyword-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 09:10:40.000000 robotframework_async_keyword-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:10:46.344472 robotframework_async_keyword-1.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-17 09:10:40.000000 robotframework_async_keyword-1.1.9/test/test.robot
```

### Comparing `robotframework-async-keyword-1.1.8/AsyncLibrary/__init__.py` & `robotframework_async_keyword-1.1.9/AsyncLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-async-keyword-1.1.8/AsyncLibrary/protected_ordered_dict.py` & `robotframework_async_keyword-1.1.9/AsyncLibrary/protected_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `robotframework-async-keyword-1.1.8/AsyncLibrary/robot_async.py` & `robotframework_async_keyword-1.1.9/AsyncLibrary/robot_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,28 +369,32 @@
 
     def _run(self, scope, postpone_id, func, *args, **kwargs):
         with self._postpone(postpone_id), scope:
             if _RUN_REQUIRES_KEYWORDRESULT:
                 kwargs['result'] = KeywordResult()
             return func(*args, **kwargs)
 
-    def async_run(self, keyword, *args):
+    def async_run(self, keyword, *args, **kwargs):
         '''
         Executes the provided Robot Framework keyword in a separate thread
         and immediately returns a handle to be used with _*Async Get*_
         '''
         context = BuiltIn()._get_context()    # noqa, E501  pylint: disable=protected-access
         runner = context.get_runner(keyword)
         scope = ScopedContext()
         postpone_id = self._postpone.fork()
 
         with BlockSignals():
             future = self._executor.submit(
                 self._run, scope, postpone_id,
-                runner.run, KeywordData(keyword, args=args), context=context
+                runner.run,
+                KeywordData(
+                    keyword,
+                    args=tuple(args) + tuple(kwargs.items())),
+                context=context
             )
         future._scope = scope    # pylint: disable=protected-access
         future._postpone_id = postpone_id    # pylint: disable=protected-access
         with self._lock:
             handle = self._last_thread_handle
             self._last_thread_handle += 1
             self._futures[handle] = future
```

### Comparing `robotframework-async-keyword-1.1.8/AsyncLibrary/scoped_value.py` & `robotframework_async_keyword-1.1.9/AsyncLibrary/scoped_value.py`

 * *Files identical despite different names*

### Comparing `robotframework-async-keyword-1.1.8/LICENSE.txt` & `robotframework_async_keyword-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework-async-keyword-1.1.8/PKG-INFO` & `robotframework_async_keyword-1.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-async-keyword
-Version: 1.1.8
+Version: 1.1.9
 Summary: Generic Robot Framework library for asynchronous keyword execution
 Author-email: René Lehfeld <54720674+rlehfeld@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/rlehfeld/robotframework-async-keyword
 Project-URL: Bug Reports, https://github.com/rlehfeld/robotframework-async-keyword/issues
 Project-URL: Source, https://github.com/rlehfeld/robotframework-async-keyword/
 Keywords: async,robotframework
```

### Comparing `robotframework-async-keyword-1.1.8/README.rst` & `robotframework_async_keyword-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework-async-keyword-1.1.8/pyproject.toml` & `robotframework_async_keyword-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotframework-async-keyword-1.1.8/robotframework_async_keyword.egg-info/PKG-INFO` & `robotframework_async_keyword-1.1.9/robotframework_async_keyword.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-async-keyword
-Version: 1.1.8
+Version: 1.1.9
 Summary: Generic Robot Framework library for asynchronous keyword execution
 Author-email: René Lehfeld <54720674+rlehfeld@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/rlehfeld/robotframework-async-keyword
 Project-URL: Bug Reports, https://github.com/rlehfeld/robotframework-async-keyword/issues
 Project-URL: Source, https://github.com/rlehfeld/robotframework-async-keyword/
 Keywords: async,robotframework
```

### Comparing `robotframework-async-keyword-1.1.8/test/test.robot` & `robotframework_async_keyword-1.1.9/test/test.robot`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Example
     ${handle 1}    Async Run    Deeply Nested Keyword    ${1}
     ${handle 2}    Async Run    Nested Keyword    ${2}
     ${handle 3}    Async Run    Set Variable    ${3}
     ${handle 4}    Async Run    Deeply Nested Fail    ${4}
     ${handle 5}    Async Run    Deeply Nested Fail    ${5}
     ${handle 6}    Async Run    Deeply Nested Fail    ${6}
+    ${handle 7}    Async Run    Nested Keyword    ${2}    value2=${5}
 
     ${handles}    Create List
     ...    ${handle 3}
     ...    ${handle 2}
     ...    ${handle 1}
 
     ${return_value}    Async Get    ${handles}
@@ -27,18 +28,19 @@
     ...    Async Get    ${handle 4}
 
     [Teardown]        Run Keyword And Expect Error    should fail ${5}
     ...    Async Get    ${handle 5}
 
 *** Keywords ***
 Nested Keyword
-    [Arguments]    ${value}
+    [Arguments]    ${value1}    ${value2}=${2}
     Sleep    1 sec
-    Log To Console    Got Value ${value}
-    ${return}    Set Variable    ${value}
+    Log To Console    Got Value1 ${value1}
+    Log To Console    Got Value2 ${value2}
+    ${return}    Set Variable    ${value1}
     RETURN    ${return}
 
 Deeply Nested Keyword
     [Arguments]    ${value}
     Log To Console    Deeply Nested Keyword ${value}
     ${return}    Nested Keyword    ${value}
     RETURN    ${return}
```

