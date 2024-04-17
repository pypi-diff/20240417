# Comparing `tmp/types-pyOpenSSL-24.0.0.20240311.tar.gz` & `tmp/types-pyOpenSSL-24.0.0.20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyOpenSSL-24.0.0.20240311.tar", last modified: Mon Mar 11 02:18:00 2024, max compression
+gzip compressed data, was "types-pyOpenSSL-24.0.0.20240417.tar", last modified: Wed Apr 17 02:17:32 2024, max compression
```

## Comparing `types-pyOpenSSL-24.0.0.20240311.tar` & `types-pyOpenSSL-24.0.0.20240417.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:00.033003 types-pyOpenSSL-24.0.0.20240311/
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-03-11 02:17:59.000000 types-pyOpenSSL-24.0.0.20240311/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 02:17:59.000000 types-pyOpenSSL-24.0.0.20240311/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:00.033003 types-pyOpenSSL-24.0.0.20240311/OpenSSL-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-11 02:17:59.000000 types-pyOpenSSL-24.0.0.20240311/OpenSSL-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-03-11 02:14:35.000000 types-pyOpenSSL-24.0.0.20240311/OpenSSL-stubs/SSL.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 02:14:35.000000 types-pyOpenSSL-24.0.0.20240311/OpenSSL-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-03-11 02:14:35.000000 types-pyOpenSSL-24.0.0.20240311/OpenSSL-stubs/crypto.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 02:17:59.000000 types-pyOpenSSL-24.0.0.20240311/OpenSSL-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-11 02:14:35.000000 types-pyOpenSSL-24.0.0.20240311/OpenSSL-stubs/rand.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-11 02:14:35.000000 types-pyOpenSSL-24.0.0.20240311/OpenSSL-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-11 02:18:00.033003 types-pyOpenSSL-24.0.0.20240311/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 02:18:00.033003 types-pyOpenSSL-24.0.0.20240311/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-11 02:17:59.000000 types-pyOpenSSL-24.0.0.20240311/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:00.033003 types-pyOpenSSL-24.0.0.20240311/types_pyOpenSSL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-11 02:18:00.000000 types-pyOpenSSL-24.0.0.20240311/types_pyOpenSSL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-11 02:18:00.000000 types-pyOpenSSL-24.0.0.20240311/types_pyOpenSSL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 02:18:00.000000 types-pyOpenSSL-24.0.0.20240311/types_pyOpenSSL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 02:18:00.000000 types-pyOpenSSL-24.0.0.20240311/types_pyOpenSSL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-11 02:18:00.000000 types-pyOpenSSL-24.0.0.20240311/types_pyOpenSSL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:32.517490 types-pyOpenSSL-24.0.0.20240417/
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:32.517490 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-17 02:16:41.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/SSL.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-04-17 02:16:41.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/crypto.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 02:16:41.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/rand.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 02:16:41.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-17 02:17:32.517490 types-pyOpenSSL-24.0.0.20240417/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:17:32.517490 types-pyOpenSSL-24.0.0.20240417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:32.517490 types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/top_level.txt
```

### Comparing `types-pyOpenSSL-24.0.0.20240311/CHANGELOG.md` & `types-pyOpenSSL-24.0.0.20240417/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 24.0.0.20240417 (2024-04-17)
+
+Remove remaining bare `Incomplete`s (#11768)
+
+Enable Y065
+
 ## 24.0.0.20240311 (2024-03-11)
 
 Use PEP 570 syntax in third party stubs (#11554)
 
 ## 24.0.0.20240228 (2024-02-28)
 
 pyOpenSSL: Add DTLS_* constants (#11486)
```

### Comparing `types-pyOpenSSL-24.0.0.20240311/OpenSSL-stubs/SSL.pyi` & `types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/SSL.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import socket
 from _socket import _Address, _RetAddress
 from _typeshed import Incomplete, ReadableBuffer
 from collections.abc import Callable, MutableSequence, Sequence
 from typing import Any, TypeVar
 
+import _cffi_backend as cffi
 from OpenSSL.crypto import X509, PKey, X509Name
 
 OPENSSL_VERSION_NUMBER: int
 SSLEAY_VERSION: int
 SSLEAY_CFLAGS: int
 SSLEAY_PLATFORM: int
 SSLEAY_DIR: int
@@ -160,17 +161,15 @@
     def get_protocol_version(self) -> int: ...
     def get_shutdown(self) -> int: ...
     def set_shutdown(self, state: int) -> None: ...
     def get_state_string(self) -> bytes: ...
     def server_random(self) -> bytes | None: ...
     def client_random(self) -> bytes | None: ...
     def master_key(self) -> bytes | None: ...
-    def export_keying_material(
-        self, label: Incomplete, olen: Incomplete, context: Incomplete = None
-    ) -> Incomplete: ...  # TODO: type, see RFC-5705
+    def export_keying_material(self, label: bytes, olen: int, context: bytes | None = None) -> cffi.buffer: ...
     def get_app_data(self) -> Any: ...
     def set_app_data(self, data: Any) -> None: ...
     def sock_shutdown(self, how: int, /) -> None: ...  # alias to `_socket.socket.shutdown`
     def want_read(self) -> bool: ...
     def want_write(self) -> bool: ...
     def get_session(self) -> Session | None: ...
     def set_session(self, session: Session) -> None: ...
```

### Comparing `types-pyOpenSSL-24.0.0.20240311/OpenSSL-stubs/crypto.pyi` & `types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/crypto.pyi`

 * *Files identical despite different names*

### Comparing `types-pyOpenSSL-24.0.0.20240311/PKG-INFO` & `types-pyOpenSSL-24.0.0.20240417/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyOpenSSL
-Version: 24.0.0.20240311
+Version: 24.0.0.20240417
 Summary: Typing stubs for pyOpenSSL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-pyOpenSSL-24.0.0.20240311/setup.py` & `types-pyOpenSSL-24.0.0.20240417/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,32 +21,32 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="24.0.0.20240311",
+      version="24.0.0.20240417",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
-      install_requires=['cryptography>=35.0.0'],
+      install_requires=['types-cffi', 'cryptography>=35.0.0'],
       packages=['OpenSSL-stubs'],
       package_data={'OpenSSL-stubs': ['SSL.pyi', '__init__.pyi', 'crypto.pyi', 'rand.pyi', 'version.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
```

### Comparing `types-pyOpenSSL-24.0.0.20240311/types_pyOpenSSL.egg-info/PKG-INFO` & `types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyOpenSSL
-Version: 24.0.0.20240311
+Version: 24.0.0.20240417
 Summary: Typing stubs for pyOpenSSL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

