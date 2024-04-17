# Comparing `tmp/types-tqdm-4.66.0.4.tar.gz` & `tmp/types-tqdm-4.66.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tqdm-4.66.0.4.tar", last modified: Tue Nov  7 02:17:40 2023, max compression
+gzip compressed data, was "types-tqdm-4.66.0.5.tar", last modified: Fri Nov 24 02:18:25 2023, max compression
```

## Comparing `types-tqdm-4.66.0.4.tar` & `types-tqdm-4.66.0.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 02:17:40.549656 types-tqdm-4.66.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2023-11-07 02:17:40.000000 types-tqdm-4.66.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-07 02:17:40.000000 types-tqdm-4.66.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2023-11-07 02:17:40.549656 types-tqdm-4.66.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-07 02:17:40.549656 types-tqdm-4.66.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-11-07 02:17:40.000000 types-tqdm-4.66.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 02:17:40.545656 types-tqdm-4.66.0.4/tqdm-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-11-07 02:17:40.000000 types-tqdm-4.66.0.4/tqdm-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/_dist_ver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/_main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/_monitor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/_tqdm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/_tqdm_gui.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/_tqdm_notebook.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/_tqdm_pandas.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/asyncio.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/auto.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/autonotebook.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/cli.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 02:17:40.549656 types-tqdm-4.66.0.4/tqdm-stubs/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/contrib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/contrib/bells.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/contrib/concurrent.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/contrib/discord.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/contrib/itertools.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/contrib/logging.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/contrib/slack.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/contrib/telegram.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/contrib/utils_worker.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      939 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/dask.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/gui.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/keras.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/notebook.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/rich.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/std.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/tk.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-07 02:17:24.000000 types-tqdm-4.66.0.4/tqdm-stubs/version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 02:17:40.549656 types-tqdm-4.66.0.4/types_tqdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2023-11-07 02:17:40.000000 types-tqdm-4.66.0.4/types_tqdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-11-07 02:17:40.000000 types-tqdm-4.66.0.4/types_tqdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 02:17:40.000000 types-tqdm-4.66.0.4/types_tqdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-07 02:17:40.000000 types-tqdm-4.66.0.4/types_tqdm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 02:18:25.252152 types-tqdm-4.66.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2023-11-24 02:18:24.000000 types-tqdm-4.66.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-24 02:18:24.000000 types-tqdm-4.66.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2023-11-24 02:18:25.252152 types-tqdm-4.66.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-24 02:18:25.252152 types-tqdm-4.66.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-11-24 02:18:24.000000 types-tqdm-4.66.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 02:18:25.248151 types-tqdm-4.66.0.5/tqdm-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2023-11-24 02:18:24.000000 types-tqdm-4.66.0.5/tqdm-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/_dist_ver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/_main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/_monitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/_tqdm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/_tqdm_gui.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/_tqdm_notebook.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/_tqdm_pandas.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6904 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/asyncio.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/auto.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/autonotebook.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/cli.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 02:18:25.252152 types-tqdm-4.66.0.5/tqdm-stubs/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/contrib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/contrib/bells.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/contrib/concurrent.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/contrib/discord.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/contrib/itertools.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/contrib/logging.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/contrib/slack.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/contrib/telegram.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/contrib/utils_worker.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/dask.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/gui.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/keras.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/notebook.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/rich.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/std.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/tk.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-24 02:17:58.000000 types-tqdm-4.66.0.5/tqdm-stubs/version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 02:18:25.252152 types-tqdm-4.66.0.5/types_tqdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2023-11-24 02:18:25.000000 types-tqdm-4.66.0.5/types_tqdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2023-11-24 02:18:25.000000 types-tqdm-4.66.0.5/types_tqdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-24 02:18:25.000000 types-tqdm-4.66.0.5/types_tqdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-24 02:18:25.000000 types-tqdm-4.66.0.5/types_tqdm.egg-info/top_level.txt
```

### Comparing `types-tqdm-4.66.0.4/CHANGELOG.md` & `types-tqdm-4.66.0.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 4.66.0.5 (2023-11-24)
+
+Third-party stubs: remove unused `type: ignore`s (#11063)
+
 ## 4.66.0.4 (2023-11-07)
 
 Remove redundant inheritances from `Generic` and various `typing` protocols (#10981)
 
 ## 4.66.0.3 (2023-10-27)
 
 Remove many redundant inheritances from `Generic[]` (#10933)
```

### Comparing `types-tqdm-4.66.0.4/PKG-INFO` & `types-tqdm-4.66.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tqdm
-Version: 4.66.0.4
+Version: 4.66.0.5
 Summary: Typing stubs for tqdm
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tqdm.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-tqdm` aims to provide accurate annotations
 for `tqdm==4.66.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tqdm. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `820be9bfe94a14b7b5b8a265806f4523d564cedf` and was tested
-with mypy 1.6.1, pyright 1.1.334, and
-pytype 2023.10.17.
+This package was generated from typeshed commit `81633e27097228a8a7eb0f963c62916ecea78abc` and was tested
+with mypy 1.7.1, pyright 1.1.334, and
+pytype 2023.11.21.
```

### Comparing `types-tqdm-4.66.0.4/setup.py` & `types-tqdm-4.66.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-tqdm` aims to provide accurate annotations
 for `tqdm==4.66.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tqdm. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `820be9bfe94a14b7b5b8a265806f4523d564cedf` and was tested
-with mypy 1.6.1, pyright 1.1.334, and
-pytype 2023.10.17.
+This package was generated from typeshed commit `81633e27097228a8a7eb0f963c62916ecea78abc` and was tested
+with mypy 1.7.1, pyright 1.1.334, and
+pytype 2023.11.21.
 '''.lstrip()
 
 setup(name=name,
-      version="4.66.0.4",
+      version="4.66.0.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tqdm.md",
```

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/__init__.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/_monitor.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/_monitor.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/asyncio.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/asyncio.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/contrib/__init__.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/contrib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/contrib/discord.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/contrib/discord.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/contrib/slack.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/contrib/slack.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/contrib/telegram.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/contrib/telegram.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/dask.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/dask.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/gui.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/gui.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/keras.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/keras.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/notebook.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/notebook.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/rich.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/rich.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/std.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/std.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/tk.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/tk.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/tqdm-stubs/utils.pyi` & `types-tqdm-4.66.0.5/tqdm-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.66.0.4/types_tqdm.egg-info/PKG-INFO` & `types-tqdm-4.66.0.5/types_tqdm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tqdm
-Version: 4.66.0.4
+Version: 4.66.0.5
 Summary: Typing stubs for tqdm
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tqdm.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-tqdm` aims to provide accurate annotations
 for `tqdm==4.66.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tqdm. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `820be9bfe94a14b7b5b8a265806f4523d564cedf` and was tested
-with mypy 1.6.1, pyright 1.1.334, and
-pytype 2023.10.17.
+This package was generated from typeshed commit `81633e27097228a8a7eb0f963c62916ecea78abc` and was tested
+with mypy 1.7.1, pyright 1.1.334, and
+pytype 2023.11.21.
```

### Comparing `types-tqdm-4.66.0.4/types_tqdm.egg-info/SOURCES.txt` & `types-tqdm-4.66.0.5/types_tqdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

