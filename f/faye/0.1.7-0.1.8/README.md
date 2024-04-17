# Comparing `tmp/faye-0.1.7.tar.gz` & `tmp/faye-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faye-0.1.7.tar", last modified: Sun Dec 25 10:25:55 2022, max compression
+gzip compressed data, was "faye-0.1.8.tar", last modified: Fri Dec 30 06:36:03 2022, max compression
```

## Comparing `faye-0.1.7.tar` & `faye-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-12-25 10:25:55.737509 faye-0.1.7/
--rw-rw-rw-   0        0        0     1323 2022-12-25 10:21:47.000000 faye-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     1594 2022-12-25 10:25:55.737061 faye-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2022-12-25 10:24:49.000000 faye-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2022-12-25 10:25:55.695135 faye-0.1.7/faye/
--rw-rw-rw-   0        0        0      109 2022-12-25 10:23:03.000000 faye-0.1.7/faye/__init__.py
--rw-rw-rw-   0        0        0     1111 2022-12-25 10:25:24.000000 faye-0.1.7/faye/faye.py
-drwxrwxrwx   0        0        0        0 2022-12-25 10:25:55.736132 faye-0.1.7/faye.egg-info/
--rw-rw-rw-   0        0        0     1594 2022-12-25 10:25:55.000000 faye-0.1.7/faye.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2022-12-25 10:25:55.000000 faye-0.1.7/faye.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-25 10:25:55.000000 faye-0.1.7/faye.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-12-25 10:25:55.000000 faye-0.1.7/faye.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-25 10:25:55.738547 faye-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      814 2022-12-25 10:23:32.000000 faye-0.1.7/setup.py
+drwxrwxr-x   0 azazel    (1000) azazel    (1000)        0 2022-12-30 06:36:03.980228 faye-0.1.8/
+-rw-rw-r--   0 azazel    (1000) azazel    (1000)     1301 2022-12-30 06:35:48.000000 faye-0.1.8/LICENSE
+-rw-rw-r--   0 azazel    (1000) azazel    (1000)     1557 2022-12-30 06:36:03.980228 faye-0.1.8/PKG-INFO
+-rw-rw-r--   0 azazel    (1000) azazel    (1000)     1119 2022-12-30 06:34:52.000000 faye-0.1.8/README.md
+drwxrwxr-x   0 azazel    (1000) azazel    (1000)        0 2022-12-30 06:36:03.980228 faye-0.1.8/faye/
+-rw-rw-r--   0 azazel    (1000) azazel    (1000)      109 2022-12-30 06:35:26.000000 faye-0.1.8/faye/__init__.py
+-rw-rw-r--   0 azazel    (1000) azazel    (1000)     1071 2022-12-30 06:35:30.000000 faye-0.1.8/faye/faye.py
+drwxrwxr-x   0 azazel    (1000) azazel    (1000)        0 2022-12-30 06:36:03.980228 faye-0.1.8/faye.egg-info/
+-rw-rw-r--   0 azazel    (1000) azazel    (1000)     1557 2022-12-30 06:36:03.000000 faye-0.1.8/faye.egg-info/PKG-INFO
+-rw-rw-r--   0 azazel    (1000) azazel    (1000)      168 2022-12-30 06:36:03.000000 faye-0.1.8/faye.egg-info/SOURCES.txt
+-rw-rw-r--   0 azazel    (1000) azazel    (1000)        1 2022-12-30 06:36:03.000000 faye-0.1.8/faye.egg-info/dependency_links.txt
+-rw-rw-r--   0 azazel    (1000) azazel    (1000)        5 2022-12-30 06:36:03.000000 faye-0.1.8/faye.egg-info/top_level.txt
+-rw-rw-r--   0 azazel    (1000) azazel    (1000)       38 2022-12-30 06:36:03.980228 faye-0.1.8/setup.cfg
+-rw-rw-r--   0 azazel    (1000) azazel    (1000)      792 2022-12-30 06:35:15.000000 faye-0.1.8/setup.py
```

### Comparing `faye-0.1.7/LICENSE` & `faye-0.1.8/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-BSD 2-Clause License
-
-Copyright (c) 2022, Hifumi1337
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 2-Clause License
+
+Copyright (c) 2022, azazelm3dj3d
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `faye-0.1.7/PKG-INFO` & `faye-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 2.1
-Name: faye
-Version: 0.1.7
-Summary: Basic logging library with a customizable log message, progress bar, and more!
-Home-page: https://github.com/shinigamilib/faye
-Author: Hifumi1337
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<img src="https://raw.githubusercontent.com/shinigamilib/faye/main/assets/faye.jpg" />
-
-Basic logging library with a customizable log message, progress bar, and more!
-
-This logging library was created specifically for [Shinigami (Python)](https://github.com/shinigamilib/shinigami-py), but you should have no issues integrating it into your codebase as long as you're running Python 3.
-
-The best way to utilize the Faye library is by using `pip`. You can install the library by running the following command:
-```bash
-pip install faye
-```
-
-## Usage
-The library is currently limited due to it being updated on a necessity basis, but there are a few examples below to help with using it.
-
-```python
-# Imports the Faye library
-from faye.faye import Faye
-
-# Prints a "CRITICAL" log message to stdout
-print(Faye.log(msg="Faye is awesome!", level="CRITICAL"))
-
-# Prints a basic progress bar to stdout
-print(Faye.progress(total=100, description="Downloading..."))
-```
-
-Even though Faye should be compatible with most Python 3 projects, it is still in an early stage of development. This means Faye could be altered at any time.
+Metadata-Version: 2.1
+Name: faye
+Version: 0.1.8
+Summary: Basic logging library with a customizable log message, progress bar, and more!
+Home-page: https://github.com/shinigamilib/faye
+Author: azazelm3dj3d
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<img src="https://raw.githubusercontent.com/shinigamilib/faye/main/assets/faye.jpg" />
+
+Basic logging library with a customizable log message, progress bar, and more!
+
+This logging library was created specifically for [Shinigami (Python)](https://github.com/shinigamilib/shinigami-py), but you should have no issues integrating it into your codebase as long as you're running Python 3.
+
+The best way to utilize the Faye library is by using `pip`. You can install the library by running the following command:
+```bash
+pip install faye
+```
+
+## Usage
+The library is currently limited due to it being updated on a necessity basis, but there are a few examples below to help with using it.
+
+```python
+# Imports the Faye library
+from faye.faye import Faye
+
+# Prints a "CRITICAL" log message to stdout
+print(Faye.log(msg="Faye is awesome!", level="CRITICAL"))
+
+# Prints a basic progress bar to stdout
+print(Faye.progress(total=100, description="Downloading..."))
+```
+
+Even though Faye should be compatible with most Python 3 projects, it is still in an early stage of development. This means Faye could be altered at any time.
```

### Comparing `faye-0.1.7/README.md` & `faye-0.1.8/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-<img src="https://raw.githubusercontent.com/shinigamilib/faye/main/assets/faye.jpg" />
-
-Basic logging library with a customizable log message, progress bar, and more!
-
-This logging library was created specifically for [Shinigami (Python)](https://github.com/shinigamilib/shinigami-py), but you should have no issues integrating it into your codebase as long as you're running Python 3.
-
-The best way to utilize the Faye library is by using `pip`. You can install the library by running the following command:
-```bash
-pip install faye
-```
-
-## Usage
-The library is currently limited due to it being updated on a necessity basis, but there are a few examples below to help with using it.
-
-```python
-# Imports the Faye library
-from faye.faye import Faye
-
-# Prints a "CRITICAL" log message to stdout
-print(Faye.log(msg="Faye is awesome!", level="CRITICAL"))
-
-# Prints a basic progress bar to stdout
-print(Faye.progress(total=100, description="Downloading..."))
-```
-
+<img src="https://raw.githubusercontent.com/shinigamilib/faye/main/assets/faye.jpg" />
+
+Basic logging library with a customizable log message, progress bar, and more!
+
+This logging library was created specifically for [Shinigami (Python)](https://github.com/shinigamilib/shinigami-py), but you should have no issues integrating it into your codebase as long as you're running Python 3.
+
+The best way to utilize the Faye library is by using `pip`. You can install the library by running the following command:
+```bash
+pip install faye
+```
+
+## Usage
+The library is currently limited due to it being updated on a necessity basis, but there are a few examples below to help with using it.
+
+```python
+# Imports the Faye library
+from faye.faye import Faye
+
+# Prints a "CRITICAL" log message to stdout
+print(Faye.log(msg="Faye is awesome!", level="CRITICAL"))
+
+# Prints a basic progress bar to stdout
+print(Faye.progress(total=100, description="Downloading..."))
+```
+
 Even though Faye should be compatible with most Python 3 projects, it is still in an early stage of development. This means Faye could be altered at any time.
```

### Comparing `faye-0.1.7/faye/faye.py` & `faye-0.1.8/faye/faye.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-"""
-    Owner: Hifumi1337 (https://github.com/hifumi1337)
-    Project: Faye
-    License: BSD 2-Clause
-"""
-
-class Faye:
-
-    def log(self, msg: str = "Logger init", level: str = "INFO") -> str:
-        """
-        Generic logging method that allows the user to set a message and log level.
-
-        @params
-        
-        msg (str): Log message
-        
-        level (str): Level string
-
-        @rtype: str
-        """
-
-        # Checks for empty string parameters
-        if level != "" and msg != "":
-            return f"[{level}] => {msg}"
-        else:
-            raise NameError
-
-    def progress(self, total: int = 0, description: str = ""):
-        """
-        Simple progress bar built with tqdm to allow quick terminal visualization.
-
-        @params
-
-        total (int): The length of the progress bar
-
-        description (str): Description to display beside the progress bar
-
-        @rtype: None
-        """
-
-        from tqdm import tqdm
-
-        # Progress bar configuration
-        for p in tqdm(range(total), desc=description):
+"""
+    Owner: azazelm3dj3d (https://github.com/azazelm3dj3d)
+    Project: Faye
+    License: BSD 2-Clause
+"""
+
+class Faye:
+
+    def log(self, msg: str = "Logger init", level: str = "INFO") -> str:
+        """
+        Generic logging method that allows the user to set a message and log level.
+
+        @params
+        
+        msg (str): Log message
+        
+        level (str): Level string
+
+        @rtype: str
+        """
+
+        # Checks for empty string parameters
+        if level != "" and msg != "":
+            return f"[{level}] => {msg}"
+        else:
+            raise NameError
+
+    def progress(self, total: int = 0, description: str = ""):
+        """
+        Simple progress bar built with tqdm to allow quick terminal visualization.
+
+        @params
+
+        total (int): The length of the progress bar
+
+        description (str): Description to display beside the progress bar
+
+        @rtype: None
+        """
+
+        from tqdm import tqdm
+
+        # Progress bar configuration
+        for p in tqdm(range(total), desc=description):
             pass
```

### Comparing `faye-0.1.7/faye.egg-info/PKG-INFO` & `faye-0.1.8/faye.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 2.1
-Name: faye
-Version: 0.1.7
-Summary: Basic logging library with a customizable log message, progress bar, and more!
-Home-page: https://github.com/shinigamilib/faye
-Author: Hifumi1337
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<img src="https://raw.githubusercontent.com/shinigamilib/faye/main/assets/faye.jpg" />
-
-Basic logging library with a customizable log message, progress bar, and more!
-
-This logging library was created specifically for [Shinigami (Python)](https://github.com/shinigamilib/shinigami-py), but you should have no issues integrating it into your codebase as long as you're running Python 3.
-
-The best way to utilize the Faye library is by using `pip`. You can install the library by running the following command:
-```bash
-pip install faye
-```
-
-## Usage
-The library is currently limited due to it being updated on a necessity basis, but there are a few examples below to help with using it.
-
-```python
-# Imports the Faye library
-from faye.faye import Faye
-
-# Prints a "CRITICAL" log message to stdout
-print(Faye.log(msg="Faye is awesome!", level="CRITICAL"))
-
-# Prints a basic progress bar to stdout
-print(Faye.progress(total=100, description="Downloading..."))
-```
-
-Even though Faye should be compatible with most Python 3 projects, it is still in an early stage of development. This means Faye could be altered at any time.
+Metadata-Version: 2.1
+Name: faye
+Version: 0.1.8
+Summary: Basic logging library with a customizable log message, progress bar, and more!
+Home-page: https://github.com/shinigamilib/faye
+Author: azazelm3dj3d
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<img src="https://raw.githubusercontent.com/shinigamilib/faye/main/assets/faye.jpg" />
+
+Basic logging library with a customizable log message, progress bar, and more!
+
+This logging library was created specifically for [Shinigami (Python)](https://github.com/shinigamilib/shinigami-py), but you should have no issues integrating it into your codebase as long as you're running Python 3.
+
+The best way to utilize the Faye library is by using `pip`. You can install the library by running the following command:
+```bash
+pip install faye
+```
+
+## Usage
+The library is currently limited due to it being updated on a necessity basis, but there are a few examples below to help with using it.
+
+```python
+# Imports the Faye library
+from faye.faye import Faye
+
+# Prints a "CRITICAL" log message to stdout
+print(Faye.log(msg="Faye is awesome!", level="CRITICAL"))
+
+# Prints a basic progress bar to stdout
+print(Faye.progress(total=100, description="Downloading..."))
+```
+
+Even though Faye should be compatible with most Python 3 projects, it is still in an early stage of development. This means Faye could be altered at any time.
```

### Comparing `faye-0.1.7/setup.py` & `faye-0.1.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-"""
-    Owner: Hifumi1337 (https://github.com/hifumi1337)
-    Project: Faye
-    License: BSD 2-Clause
-"""
-
-import setuptools
-
-with open("README.md", "r", encoding = "utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name = "faye",
-    version = "0.1.7",
-    author = "Hifumi1337",
-    description = "Basic logging library with a customizable log message, progress bar, and more!",
-    long_description = long_description,
-    long_description_content_type = "text/markdown",
-    url = "https://github.com/shinigamilib/faye",
-    classifiers = [
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: BSD License",
-        "Operating System :: OS Independent",
-    ],
-    packages = [
-        "faye"
-    ],
-    python_requires = ">=3.6"
+"""
+    Owner: azazelm3dj3d (https://github.com/azazelm3dj3d)
+    Project: Faye
+    License: BSD 2-Clause
+"""
+
+import setuptools
+
+with open("README.md", "r", encoding = "utf-8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name = "faye",
+    version = "0.1.8",
+    author = "azazelm3dj3d",
+    description = "Basic logging library with a customizable log message, progress bar, and more!",
+    long_description = long_description,
+    long_description_content_type = "text/markdown",
+    url = "https://github.com/shinigamilib/faye",
+    classifiers = [
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: OS Independent",
+    ],
+    packages = [
+        "faye"
+    ],
+    python_requires = ">=3.6"
 )
```

