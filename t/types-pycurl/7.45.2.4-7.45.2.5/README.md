# Comparing `tmp/types-pycurl-7.45.2.4.tar.gz` & `tmp/types-pycurl-7.45.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pycurl-7.45.2.4.tar", last modified: Wed Mar 29 03:16:26 2023, max compression
+gzip compressed data, was "types-pycurl-7.45.2.5.tar", last modified: Sun Aug 13 21:11:19 2023, max compression
```

## Comparing `types-pycurl-7.45.2.4.tar` & `types-pycurl-7.45.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 03:16:26.435176 types-pycurl-7.45.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-29 03:16:24.000000 types-pycurl-7.45.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-29 03:16:24.000000 types-pycurl-7.45.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-29 03:16:26.431176 types-pycurl-7.45.2.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 03:16:26.431176 types-pycurl-7.45.2.4/pycurl-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-29 03:16:24.000000 types-pycurl-7.45.2.4/pycurl-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    14953 2023-03-29 03:16:24.000000 types-pycurl-7.45.2.4/pycurl-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 03:16:26.435176 types-pycurl-7.45.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-29 03:16:24.000000 types-pycurl-7.45.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 03:16:26.431176 types-pycurl-7.45.2.4/types_pycurl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-29 03:16:26.000000 types-pycurl-7.45.2.4/types_pycurl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-29 03:16:26.000000 types-pycurl-7.45.2.4/types_pycurl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 03:16:26.000000 types-pycurl-7.45.2.4/types_pycurl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-29 03:16:26.000000 types-pycurl-7.45.2.4/types_pycurl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 21:11:19.225383 types-pycurl-7.45.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-08-13 21:11:18.000000 types-pycurl-7.45.2.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-13 21:11:18.000000 types-pycurl-7.45.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-13 21:11:19.225383 types-pycurl-7.45.2.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 21:11:19.221383 types-pycurl-7.45.2.5/pycurl-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-13 21:11:18.000000 types-pycurl-7.45.2.5/pycurl-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    14953 2023-08-13 21:11:18.000000 types-pycurl-7.45.2.5/pycurl-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-13 21:11:19.225383 types-pycurl-7.45.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-13 21:11:18.000000 types-pycurl-7.45.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 21:11:19.225383 types-pycurl-7.45.2.5/types_pycurl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-13 21:11:19.000000 types-pycurl-7.45.2.5/types_pycurl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-13 21:11:19.000000 types-pycurl-7.45.2.5/types_pycurl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-13 21:11:19.000000 types-pycurl-7.45.2.5/types_pycurl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-13 21:11:19.000000 types-pycurl-7.45.2.5/types_pycurl.egg-info/top_level.txt
```

### Comparing `types-pycurl-7.45.2.4/CHANGELOG.md` & `types-pycurl-7.45.2.5/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 7.45.2.5 (2023-08-13)
+
+Fill in all missing `upstream_repository` fields (#10571)
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 7.45.2.4 (2023-03-29)
 
 Fix a default in `pycurl` and update `apt_dependencies` (#9961)
 
 Fix 1 default and update apt dependencies
 
 ## 7.45.2.3 (2023-02-21)
```

### Comparing `types-pycurl-7.45.2.4/PKG-INFO` & `types-pycurl-7.45.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pycurl
-Version: 7.45.2.4
+Version: 7.45.2.5
 Summary: Typing stubs for pycurl
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pycurl.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pycurl`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pycurl. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d00bc529fa3cf7a90c3fb2682c1c624ad91c7ff9`.
+This package was generated from typeshed commit `22b055a147b5d672bf7e1f58cc6bf52cc526b35f` and was tested
+with mypy 1.4.1, pyright 1.1.320, and
+pytype 2023.7.21.
```

### Comparing `types-pycurl-7.45.2.4/pycurl-stubs/METADATA.toml` & `types-pycurl-7.45.2.5/pycurl-stubs/METADATA.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 version = "7.45.2"
+upstream_repository = "https://github.com/pycurl/pycurl"
 
 [tool.stubtest]
 # Install on Windows requires building PycURL from source
 #
 # Install on MacOS is too complicated for the CI and does not work with stubtest:
 # % brew install openssl
 # % export LDFLAGS="-L/usr/local/opt/openssl@3/lib"
```

### Comparing `types-pycurl-7.45.2.4/pycurl-stubs/__init__.pyi` & `types-pycurl-7.45.2.5/pycurl-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pycurl-7.45.2.4/setup.py` & `types-pycurl-7.45.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pycurl`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pycurl. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d00bc529fa3cf7a90c3fb2682c1c624ad91c7ff9`.
+This package was generated from typeshed commit `22b055a147b5d672bf7e1f58cc6bf52cc526b35f` and was tested
+with mypy 1.4.1, pyright 1.1.320, and
+pytype 2023.7.21.
 '''.lstrip()
 
 setup(name=name,
-      version="7.45.2.4",
+      version="7.45.2.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pycurl.md",
```

### Comparing `types-pycurl-7.45.2.4/types_pycurl.egg-info/PKG-INFO` & `types-pycurl-7.45.2.5/types_pycurl.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pycurl
-Version: 7.45.2.4
+Version: 7.45.2.5
 Summary: Typing stubs for pycurl
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pycurl.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pycurl`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pycurl. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d00bc529fa3cf7a90c3fb2682c1c624ad91c7ff9`.
+This package was generated from typeshed commit `22b055a147b5d672bf7e1f58cc6bf52cc526b35f` and was tested
+with mypy 1.4.1, pyright 1.1.320, and
+pytype 2023.7.21.
```

