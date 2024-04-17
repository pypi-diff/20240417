# Comparing `tmp/py-codeforce-1.1.dev0.tar.gz` & `tmp/py_codeforce-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-codeforce-1.1.dev0.tar", last modified: Tue Apr  9 05:07:11 2024, max compression
+gzip compressed data, was "py_codeforce-1.3.tar", last modified: Wed Apr 17 20:46:48 2024, max compression
```

## Comparing `py-codeforce-1.1.dev0.tar` & `py_codeforce-1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:07:11.109817 py-codeforce-1.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)    34823 2024-04-09 05:07:06.000000 py-codeforce-1.1.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41328 2024-04-09 05:07:11.109817 py-codeforce-1.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 05:07:06.000000 py-codeforce-1.1.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:07:11.109817 py-codeforce-1.1.dev0/py_codeforce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41328 2024-04-09 05:07:11.000000 py-codeforce-1.1.dev0/py_codeforce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 05:07:11.000000 py-codeforce-1.1.dev0/py_codeforce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:07:11.000000 py-codeforce-1.1.dev0/py_codeforce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 05:07:11.000000 py-codeforce-1.1.dev0/py_codeforce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 05:07:11.000000 py-codeforce-1.1.dev0/py_codeforce.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:07:11.109817 py-codeforce-1.1.dev0/pycodeforces/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 05:07:06.000000 py-codeforce-1.1.dev0/pycodeforces/__clients__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-09 05:07:06.000000 py-codeforce-1.1.dev0/pycodeforces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39313 2024-04-09 05:07:06.000000 py-codeforce-1.1.dev0/pycodeforces/__processors__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:07:11.109817 py-codeforce-1.1.dev0/pycodeforces/abc/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 05:07:06.000000 py-codeforce-1.1.dev0/pycodeforces/abc/__cobjects__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-09 05:07:06.000000 py-codeforce-1.1.dev0/pycodeforces/abc/__endpoints__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-09 05:07:06.000000 py-codeforce-1.1.dev0/pycodeforces/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 05:07:06.000000 py-codeforce-1.1.dev0/pycodeforces/abc/__interactions__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26183 2024-04-09 05:07:06.000000 py-codeforce-1.1.dev0/pycodeforces/abc/__objects__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-09 05:07:06.000000 py-codeforce-1.1.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:07:11.109817 py-codeforce-1.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-09 05:07:06.000000 py-codeforce-1.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:46:48.899486 py_codeforce-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34823 2024-04-17 20:46:44.000000 py_codeforce-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44414 2024-04-17 20:46:48.899486 py_codeforce-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-17 20:46:44.000000 py_codeforce-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:46:48.899486 py_codeforce-1.3/py_codeforce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44414 2024-04-17 20:46:48.000000 py_codeforce-1.3/py_codeforce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-17 20:46:48.000000 py_codeforce-1.3/py_codeforce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:46:48.000000 py_codeforce-1.3/py_codeforce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 20:46:48.000000 py_codeforce-1.3/py_codeforce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 20:46:48.000000 py_codeforce-1.3/py_codeforce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:46:48.899486 py_codeforce-1.3/pycodeforces/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-17 20:46:44.000000 py_codeforce-1.3/pycodeforces/__clients__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-17 20:46:44.000000 py_codeforce-1.3/pycodeforces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39814 2024-04-17 20:46:44.000000 py_codeforce-1.3/pycodeforces/__processors__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:46:48.899486 py_codeforce-1.3/pycodeforces/abc/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-17 20:46:44.000000 py_codeforce-1.3/pycodeforces/abc/__cobjects__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-17 20:46:44.000000 py_codeforce-1.3/pycodeforces/abc/__endpoints__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-17 20:46:44.000000 py_codeforce-1.3/pycodeforces/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-17 20:46:44.000000 py_codeforce-1.3/pycodeforces/abc/__interactions__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26183 2024-04-17 20:46:44.000000 py_codeforce-1.3/pycodeforces/abc/__objects__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-17 20:46:44.000000 py_codeforce-1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:46:48.899486 py_codeforce-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-17 20:46:44.000000 py_codeforce-1.3/setup.py
```

### Comparing `py-codeforce-1.1.dev0/LICENSE` & `py_codeforce-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-codeforce-1.1.dev0/PKG-INFO` & `py_codeforce-1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-codeforce
-Version: 1.1.dev0
+Version: 1.3
 Summary: Py-Codeforces is a high-performance and type-safe Python library designed for seamless interaction with Codeforces. It offers both asynchronous and synchronous client handlers, allowing developers to choose the appropriate method based on their requirements.
 Home-page: https://github.com/halfstackpgr/py-codeforces
 Author: Parth Mishra
 Author-email: halfstackpgr <halfstackpgr@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -690,8 +690,99 @@
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: codespell; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 
-# py-codeforces
+# Py-Codeforce
+## Faster | Better | Type-Safe
+
+
+![Ruff](https://camo.githubusercontent.com/18c26428c337f9d641fa09b629a3a03b514e8ac84b57974a0ed7d1b38e14e060/68747470733a2f2f696d672e736869656c64732e696f2f656e64706f696e743f75726c3d68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f61737472616c2d73682f727566662f6d61696e2f6173736574732f62616467652f76322e6a736f6e) ![Passing Package](https://github.com/halfstackpgr/py-codeforces/actions/workflows/python-publish.yml/badge.svg) 
+![Static Badge](https://img.shields.io/badge/python-Strict-checking?style=plastic&logo=python&label=Type-Checking&labelColor=yellow)
+
+
+![image](https://github.com/halfstackpgr/py-codeforces/assets/118044992/cdb54788-3fbc-48db-b936-7f0e883f9709)
+
+
+## Py-Codeforces
+
+Py-Codeforces is a high-performance and type-safe Python library designed for seamless interaction with Codeforces. It offers both asynchronous and synchronous client handlers, allowing developers to choose the appropriate method based on their requirements.
+
+Key Features:
+1. ### Client Handlers:
+   - Synchronous Handler: `SyncMethod`
+   - Asynchronous Handler: `AsyncMethod`
+
+2. ### Functionality:
+   Both client handlers offer the same set of functionalities, ensuring consistency and flexibility in usage.
+
+3. ### Authentication:
+   To access user-related attributes, authentication must be enabled by setting the `enable_auth` parameter to `True`.
+
+4. ### API Documentation:
+   This library is built entirely based on the official [Codeforces API Documentation](https://codeforces.com/apiHelp/), ensuring reliability and adherence to best practices.
+
+Example Usage:
+
+### Asynchronous usage:
+
+```python
+import asyncio
+import pycodeforces
+
+async def main():
+    api = pycodeforces.AsyncMethod()
+    users = await api.get_user_info(handles="DmitriyH;Fefer_Ivan")
+    # use `;` to add multiple parameters.
+    async for user in users:
+        print(user.avatar)
+
+asyncio.run(main())
+```
+
+### Synchronous usage:
+
+```python
+import pycodeforces
+
+async def main():
+    get = pycodeforces.SyncMethod()
+    users = get.get_user_info(handles="DmitriyH;Fefer_Ivan")
+    # use `;` to add multiple parameters.
+    for user in users:
+        print(user.avatar)
+```
+
+## Features
+
+- Is 100% type safe.
+- For customisation in types, a specific module `abc` has been provided within the head module.
+- Dual modes for specific requirements regarding auth.
+-- Can be enabled by passing a `True` to `Method` constructor 
+
+## Uses:
+1. [msgspec](https://github.com/jcrist/msgspec) - for data validation and then serialisation. 
+2. [ruff](https://github.com/astral-sh/ruff) - for linear code formatting and consistency.
+
+
+## Installation
+Installing as a user:
+```sh
+pip install py-codeforce
+```
+
+Installing as a developer:
+```sh
+pip install py-codeforce[dev]
+```
+
+## Open Source Contribution:
+Want to contribute? Great!
+Check the `Issues` for getting to know about further updates and solutions to occurring problems. 
+Maintain the type-checking as strict.
+Stack a PR to the production 
+
+
+Thank you for checking out the repo. 
+Give it a star if you've found it worthy.
```

### Comparing `py-codeforce-1.1.dev0/py_codeforce.egg-info/PKG-INFO` & `py_codeforce-1.3/py_codeforce.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-codeforce
-Version: 1.1.dev0
+Version: 1.3
 Summary: Py-Codeforces is a high-performance and type-safe Python library designed for seamless interaction with Codeforces. It offers both asynchronous and synchronous client handlers, allowing developers to choose the appropriate method based on their requirements.
 Home-page: https://github.com/halfstackpgr/py-codeforces
 Author: Parth Mishra
 Author-email: halfstackpgr <halfstackpgr@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -690,8 +690,99 @@
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: codespell; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 
-# py-codeforces
+# Py-Codeforce
+## Faster | Better | Type-Safe
+
+
+![Ruff](https://camo.githubusercontent.com/18c26428c337f9d641fa09b629a3a03b514e8ac84b57974a0ed7d1b38e14e060/68747470733a2f2f696d672e736869656c64732e696f2f656e64706f696e743f75726c3d68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f61737472616c2d73682f727566662f6d61696e2f6173736574732f62616467652f76322e6a736f6e) ![Passing Package](https://github.com/halfstackpgr/py-codeforces/actions/workflows/python-publish.yml/badge.svg) 
+![Static Badge](https://img.shields.io/badge/python-Strict-checking?style=plastic&logo=python&label=Type-Checking&labelColor=yellow)
+
+
+![image](https://github.com/halfstackpgr/py-codeforces/assets/118044992/cdb54788-3fbc-48db-b936-7f0e883f9709)
+
+
+## Py-Codeforces
+
+Py-Codeforces is a high-performance and type-safe Python library designed for seamless interaction with Codeforces. It offers both asynchronous and synchronous client handlers, allowing developers to choose the appropriate method based on their requirements.
+
+Key Features:
+1. ### Client Handlers:
+   - Synchronous Handler: `SyncMethod`
+   - Asynchronous Handler: `AsyncMethod`
+
+2. ### Functionality:
+   Both client handlers offer the same set of functionalities, ensuring consistency and flexibility in usage.
+
+3. ### Authentication:
+   To access user-related attributes, authentication must be enabled by setting the `enable_auth` parameter to `True`.
+
+4. ### API Documentation:
+   This library is built entirely based on the official [Codeforces API Documentation](https://codeforces.com/apiHelp/), ensuring reliability and adherence to best practices.
+
+Example Usage:
+
+### Asynchronous usage:
+
+```python
+import asyncio
+import pycodeforces
+
+async def main():
+    api = pycodeforces.AsyncMethod()
+    users = await api.get_user_info(handles="DmitriyH;Fefer_Ivan")
+    # use `;` to add multiple parameters.
+    async for user in users:
+        print(user.avatar)
+
+asyncio.run(main())
+```
+
+### Synchronous usage:
+
+```python
+import pycodeforces
+
+async def main():
+    get = pycodeforces.SyncMethod()
+    users = get.get_user_info(handles="DmitriyH;Fefer_Ivan")
+    # use `;` to add multiple parameters.
+    for user in users:
+        print(user.avatar)
+```
+
+## Features
+
+- Is 100% type safe.
+- For customisation in types, a specific module `abc` has been provided within the head module.
+- Dual modes for specific requirements regarding auth.
+-- Can be enabled by passing a `True` to `Method` constructor 
+
+## Uses:
+1. [msgspec](https://github.com/jcrist/msgspec) - for data validation and then serialisation. 
+2. [ruff](https://github.com/astral-sh/ruff) - for linear code formatting and consistency.
+
+
+## Installation
+Installing as a user:
+```sh
+pip install py-codeforce
+```
+
+Installing as a developer:
+```sh
+pip install py-codeforce[dev]
+```
+
+## Open Source Contribution:
+Want to contribute? Great!
+Check the `Issues` for getting to know about further updates and solutions to occurring problems. 
+Maintain the type-checking as strict.
+Stack a PR to the production 
+
+
+Thank you for checking out the repo. 
+Give it a star if you've found it worthy.
```

### Comparing `py-codeforce-1.1.dev0/pycodeforces/__init__.py` & `py_codeforce-1.3/pycodeforces/__init__.py`

 * *Files identical despite different names*

### Comparing `py-codeforce-1.1.dev0/pycodeforces/__processors__.py` & `py_codeforce-1.3/pycodeforces/__processors__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import urllib.parse
 from pycodeforces.__clients__ import AsyncClient, SyncClient
 from pycodeforces.abc.__endpoints__ import CodeForcesAPI
 from pycodeforces.abc.__objects__ import (
     User,
     Comment,
     BlogEntry,
     Hack,
@@ -32,14 +33,16 @@
 
 
 import time
 import msgspec
 import random
 import typing as t
 import hashlib
+import collections
+import urllib
 
 
 class AsyncMethod:
     def __init__(
         self,
         enable_auth: t.Optional[bool] = False,
         auth_key: t.Optional[str] = None,
@@ -78,17 +81,20 @@
         if self._auth_enabled is True:
             if not self._time:
                 self._time = int(time.time())
             randon_six_digit_num = random.randint(111111, 999999)
             head = end_point_url.removeprefix(
                 f"https://codeforces.com/api/{method_name}?"
             )
-            to_hash = f"{randon_six_digit_num}/{method_name}?apiKey={self._auth_key}&{head}&time={self._time}#{self._secret}"
+            params = dict(x.split("=") for x in head.split("&"))
+            params = collections.OrderedDict(sorted(params.items()))
+            encoded_params = urllib.parse.urlencode(params, safe=";")
+            to_hash = f"{randon_six_digit_num}/{method_name}?apiKey={self._auth_key}&{encoded_params}&time={self._time}#{self._secret}"
             hashed_string = (hashlib.sha512(to_hash.encode("utf8"))).hexdigest()
-            final_url = f"https://codeforces.com/api/{method_name}?{head}&apiKey={self._auth_key}&time={self._time}&apiSig={randon_six_digit_num}{hashed_string}"
+            final_url = f"https://codeforces.com/api/{method_name}?{encoded_params}&apiKey={self._auth_key}&time={self._time}&apiSig={randon_six_digit_num}{hashed_string}"
             return final_url
         else:
             return end_point_url
 
     async def _generate_response(self, url: str) -> bytes:
         async with self._client as socket:
             response = await socket.get(url=url)
@@ -592,17 +598,20 @@
         if self._auth_enabled is True:
             if not self._time:
                 self._time = int(time.time())
             randon_six_digit_num = random.randint(111111, 999999)
             head = end_point_url.removeprefix(
                 f"https://codeforces.com/api/{method_name}?"
             )
-            to_hash = f"{randon_six_digit_num}/{method_name}?apiKey={self._auth_key}&{head}&time={self._time}#{self._secret}"
+            params = dict(x.split("=") for x in head.split("&"))
+            params = collections.OrderedDict(sorted(params.items()))
+            encoded_params = urllib.parse.urlencode(params, safe=";")
+            to_hash = f"{randon_six_digit_num}/{method_name}?apiKey={self._auth_key}&{encoded_params}&time={self._time}#{self._secret}"
             hashed_string = (hashlib.sha512(to_hash.encode("utf8"))).hexdigest()
-            final_url = f"https://codeforces.com/api/{method_name}?{head}&apiKey={self._auth_key}&time={self._time}&apiSig={randon_six_digit_num}{hashed_string}"
+            final_url = f"https://codeforces.com/api/{method_name}?{encoded_params}&apiKey={self._auth_key}&time={self._time}&apiSig={randon_six_digit_num}{hashed_string}"
             return final_url
         else:
             return end_point_url
 
     def _generate_response(self, url: str) -> bytes:
         with self._client as socket:
             response = socket.get(url=url)
```

### Comparing `py-codeforce-1.1.dev0/pycodeforces/abc/__cobjects__.py` & `py_codeforce-1.3/pycodeforces/abc/__cobjects__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import msgspec
 import typing as t
-from pycodeforces.abc.__objects__ import Problem, Contest, RankListRow, ProblemStatistics
+from pycodeforces.abc.__objects__ import (
+    Problem,
+    Contest,
+    RankListRow,
+    ProblemStatistics,
+)
 
 
 class Standings(msgspec.Struct):
     contest: t.Optional[t.Union[t.List[Contest], Contest]] = None
     problems: t.Optional[t.Union[t.List[Problem], Problem]] = None
     rows: t.Optional[t.Union[t.List[RankListRow], RankListRow]] = None
```

### Comparing `py-codeforce-1.1.dev0/pycodeforces/abc/__endpoints__.py` & `py_codeforce-1.3/pycodeforces/abc/__endpoints__.py`

 * *Files identical despite different names*

### Comparing `py-codeforce-1.1.dev0/pycodeforces/abc/__init__.py` & `py_codeforce-1.3/pycodeforces/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `py-codeforce-1.1.dev0/pycodeforces/abc/__interactions__.py` & `py_codeforce-1.3/pycodeforces/abc/__interactions__.py`

 * *Files identical despite different names*

### Comparing `py-codeforce-1.1.dev0/pycodeforces/abc/__objects__.py` & `py_codeforce-1.3/pycodeforces/abc/__objects__.py`

 * *Files identical despite different names*

### Comparing `py-codeforce-1.1.dev0/pyproject.toml` & `py_codeforce-1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-codeforce"
-version = "1.1dev"
+version = "1.3"
 description = "Py-Codeforces is a high-performance and type-safe Python library designed for seamless interaction with Codeforces. It offers both asynchronous and synchronous client handlers, allowing developers to choose the appropriate method based on their requirements."
 readme = "README.md"
 authors = [{ name = "halfstackpgr", email = "halfstackpgr@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
@@ -53,7 +53,10 @@
     "{pep440_version}",
 ]
 "README.md" = [
     "{version}",
     "{pep440_version}",
 ]
 
+[tool.type]
+safe = true
+
```

### Comparing `py-codeforce-1.1.dev0/setup.py` & `py_codeforce-1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="py-codeforces",
     packages=["pycodeforces", "pycodeforces.abc"],
-    version="1.1dev",
+    version="1.3",
     license="GPL 3.0",
     description="Py-Codeforces is a high-performance and type-safe Python library designed for seamless interaction with Codeforces. It offers both asynchronous and synchronous client handlers, allowing developers to choose the appropriate method based on their requirements.",
     author="Parth Mishra",
     author_email="halfstackpgr@gmail.com",
     url="https://github.com/halfstackpgr/py-codeforces",
     keywords=["python", "codeforces", "api", "wrapper", "async", "sync"],
     install_requires=[
```

