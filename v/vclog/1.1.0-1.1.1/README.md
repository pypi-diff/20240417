# Comparing `tmp/vclog-1.1.0.tar.gz` & `tmp/vclog-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vclog-1.1.0.tar", last modified: Mon Feb  5 11:51:57 2024, max compression
+gzip compressed data, was "vclog-1.1.1.tar", last modified: Wed Apr 17 16:01:04 2024, max compression
```

## Comparing `vclog-1.1.0.tar` & `vclog-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vistor    (1000) vistor    (1000)        0 2024-02-05 11:51:57.076394 vclog-1.1.0/
--rw-r--r--   0 vistor    (1000) vistor    (1000)     1062 2024-02-05 08:41:38.000000 vclog-1.1.0/LICENSE
--rw-r--r--   0 vistor    (1000) vistor    (1000)     2844 2024-02-05 11:51:57.076394 vclog-1.1.0/PKG-INFO
--rw-r--r--   0 vistor    (1000) vistor    (1000)     2372 2024-02-05 11:44:43.000000 vclog-1.1.0/README.md
--rw-r--r--   0 vistor    (1000) vistor    (1000)      563 2024-02-05 11:30:38.000000 vclog-1.1.0/pyproject.toml
--rw-r--r--   0 vistor    (1000) vistor    (1000)       38 2024-02-05 11:51:57.076394 vclog-1.1.0/setup.cfg
-drwxr-xr-x   0 vistor    (1000) vistor    (1000)        0 2024-02-05 11:51:57.076394 vclog-1.1.0/tests/
--rw-r--r--   0 vistor    (1000) vistor    (1000)     6777 2024-02-05 11:29:39.000000 vclog-1.1.0/tests/test_logger.py
-drwxr-xr-x   0 vistor    (1000) vistor    (1000)        0 2024-02-05 11:51:57.076394 vclog-1.1.0/vclog/
--rw-r--r--   0 vistor    (1000) vistor    (1000)       35 2024-02-05 11:51:28.000000 vclog-1.1.0/vclog/__init__.py
--rw-r--r--   0 vistor    (1000) vistor    (1000)     9682 2024-02-05 11:46:09.000000 vclog-1.1.0/vclog/logger.py
-drwxr-xr-x   0 vistor    (1000) vistor    (1000)        0 2024-02-05 11:51:57.076394 vclog-1.1.0/vclog.egg-info/
--rw-r--r--   0 vistor    (1000) vistor    (1000)     2844 2024-02-05 11:51:57.000000 vclog-1.1.0/vclog.egg-info/PKG-INFO
--rw-r--r--   0 vistor    (1000) vistor    (1000)      203 2024-02-05 11:51:57.000000 vclog-1.1.0/vclog.egg-info/SOURCES.txt
--rw-r--r--   0 vistor    (1000) vistor    (1000)        1 2024-02-05 11:51:57.000000 vclog-1.1.0/vclog.egg-info/dependency_links.txt
--rw-r--r--   0 vistor    (1000) vistor    (1000)        6 2024-02-05 11:51:57.000000 vclog-1.1.0/vclog.egg-info/top_level.txt
+drwxr-xr-x   0 vistor    (1000) vistor    (1000)        0 2024-04-17 16:01:04.215628 vclog-1.1.1/
+-rw-r--r--   0 vistor    (1000) vistor    (1000)     1062 2024-04-17 16:00:29.000000 vclog-1.1.1/LICENSE
+-rw-r--r--   0 vistor    (1000) vistor    (1000)     3143 2024-04-17 16:01:04.214628 vclog-1.1.1/PKG-INFO
+-rw-r--r--   0 vistor    (1000) vistor    (1000)     2602 2024-04-17 16:00:29.000000 vclog-1.1.1/README.md
+-rw-r--r--   0 vistor    (1000) vistor    (1000)      632 2024-04-17 16:00:29.000000 vclog-1.1.1/pyproject.toml
+-rw-r--r--   0 vistor    (1000) vistor    (1000)       38 2024-04-17 16:01:04.215628 vclog-1.1.1/setup.cfg
+drwxr-xr-x   0 vistor    (1000) vistor    (1000)        0 2024-04-17 16:01:04.214628 vclog-1.1.1/tests/
+-rw-r--r--   0 vistor    (1000) vistor    (1000)     6889 2024-04-17 16:00:29.000000 vclog-1.1.1/tests/test_logger.py
+drwxr-xr-x   0 vistor    (1000) vistor    (1000)        0 2024-04-17 16:01:04.214628 vclog-1.1.1/vclog/
+-rw-r--r--   0 vistor    (1000) vistor    (1000)       35 2024-04-17 16:00:29.000000 vclog-1.1.1/vclog/__init__.py
+-rw-r--r--   0 vistor    (1000) vistor    (1000)     9876 2024-04-17 16:00:29.000000 vclog-1.1.1/vclog/logger.py
+drwxr-xr-x   0 vistor    (1000) vistor    (1000)        0 2024-04-17 16:01:04.214628 vclog-1.1.1/vclog.egg-info/
+-rw-r--r--   0 vistor    (1000) vistor    (1000)     3143 2024-04-17 16:01:04.000000 vclog-1.1.1/vclog.egg-info/PKG-INFO
+-rw-r--r--   0 vistor    (1000) vistor    (1000)      203 2024-04-17 16:01:04.000000 vclog-1.1.1/vclog.egg-info/SOURCES.txt
+-rw-r--r--   0 vistor    (1000) vistor    (1000)        1 2024-04-17 16:01:04.000000 vclog-1.1.1/vclog.egg-info/dependency_links.txt
+-rw-r--r--   0 vistor    (1000) vistor    (1000)        6 2024-04-17 16:01:04.000000 vclog-1.1.1/vclog.egg-info/top_level.txt
```

### Comparing `vclog-1.1.0/LICENSE` & `vclog-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vclog-1.1.0/PKG-INFO` & `vclog-1.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vclog
-Version: 1.1.0
-Summary: A minimal logger for a minimal experience
+Version: 1.1.1
+Summary: Vistor's Console Logger (VCLog) offers a minimal and colorful console logging. Single-script. No dependencies.
 Author: Vistor
 Project-URL: Homepage, https://github.com/vistormu/vclog
 Project-URL: Bug Tracker, https://github.com/vistormu/vclog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -40,14 +40,20 @@
 ```
 
 It also has a `plain` method in which color, background color, and style can be specified.
 ```python
 Logger.plain("plain text with format", color="blue", bg_color="green", style="bold")
 ```
 
+The logger can also be disabled by setting the `disable` attribute to `True`. This only works for the instantiated logger.
+```python
+logger = Logger("instance", disable=True)
+logger.info("this message will not be displayed")
+```
+
 The package also offers a `format` method to get the formatted string directly.
 ```python
 from vclog import format
 
 message: str = format("Hello, World!", color="red")
 ```
```

### Comparing `vclog-1.1.0/README.md` & `vclog-1.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 ```
 
 It also has a `plain` method in which color, background color, and style can be specified.
 ```python
 Logger.plain("plain text with format", color="blue", bg_color="green", style="bold")
 ```
 
+The logger can also be disabled by setting the `disable` attribute to `True`. This only works for the instantiated logger.
+```python
+logger = Logger("instance", disable=True)
+logger.info("this message will not be displayed")
+```
+
 The package also offers a `format` method to get the formatted string directly.
 ```python
 from vclog import format
 
 message: str = format("Hello, World!", color="red")
 ```
```

### Comparing `vclog-1.1.0/pyproject.toml` & `vclog-1.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vclog"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Vistor"},
 ]
-description = "A minimal logger for a minimal experience"
+description = "Vistor's Console Logger (VCLog) offers a minimal and colorful console logging. Single-script. No dependencies."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `vclog-1.1.0/tests/test_logger.py` & `vclog-1.1.1/tests/test_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,10 +144,13 @@
     print(f'Elapsed time: {(after - before)*1000:.2f} ms')
 
     flush_logger = Logger('flush')
     for i in range(100):
         flush_logger.error(f"flushing: {i}%", flush=True)
         time.sleep(0.1)
 
+    disabled_logger = Logger('disabled', disable=True)
+    disabled_logger.error('this should not be printed')
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `vclog-1.1.0/vclog/logger.py` & `vclog-1.1.1/vclog/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
                   sep: str = " ",
                   end: str = "\n",
                   prefix: str = "",
                   ) -> None:
     result: str = ""
 
     if isinstance(messages[0], Logger):
+        if messages[0].disable:
+            return
+
         result += f"[{messages[0].name}] "
         messages = messages[1:]
 
     result += sep.join(map(str, messages))
     result = format(result, color, bg_color, style)
 
     print(prefix+result, end=end)
@@ -149,24 +152,27 @@
     - `plain`: prints a message with the given color, background color and style.
     - `info`: prints a message to the info level.
     - `debug`: prints a message to the debug level.
     - `warning`: prints a message to the warning level.
     - `error`: prints a message to the error level.
     """
 
-    def __init__(self, name: str) -> None:
+    def __init__(self, name: str, disable: bool = False) -> None:
         """
         Initialize the logger with a name.
 
         Arguments
         ---------
         name : str
             The name of the logger.
+        disable : bool, optional
+            Wether to disable the logger or not.
         """
         self.name: str = name
+        self.disable: bool = disable
 
     @ContextAware
     @staticmethod
     def plain(*messages,
               color: str | None = None,
               bg_color: str | None = None,
               style: str | list[str] | None = None,
```

### Comparing `vclog-1.1.0/vclog.egg-info/PKG-INFO` & `vclog-1.1.1/vclog.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vclog
-Version: 1.1.0
-Summary: A minimal logger for a minimal experience
+Version: 1.1.1
+Summary: Vistor's Console Logger (VCLog) offers a minimal and colorful console logging. Single-script. No dependencies.
 Author: Vistor
 Project-URL: Homepage, https://github.com/vistormu/vclog
 Project-URL: Bug Tracker, https://github.com/vistormu/vclog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -40,14 +40,20 @@
 ```
 
 It also has a `plain` method in which color, background color, and style can be specified.
 ```python
 Logger.plain("plain text with format", color="blue", bg_color="green", style="bold")
 ```
 
+The logger can also be disabled by setting the `disable` attribute to `True`. This only works for the instantiated logger.
+```python
+logger = Logger("instance", disable=True)
+logger.info("this message will not be displayed")
+```
+
 The package also offers a `format` method to get the formatted string directly.
 ```python
 from vclog import format
 
 message: str = format("Hello, World!", color="red")
 ```
```

