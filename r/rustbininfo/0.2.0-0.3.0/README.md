# Comparing `tmp/rustbininfo-0.2.0.tar.gz` & `tmp/rustbininfo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustbininfo-0.2.0.tar", max compression
+gzip compressed data, was "rustbininfo-0.3.0.tar", max compression
```

## Comparing `rustbininfo-0.2.0.tar` & `rustbininfo-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1597 2024-03-18 23:10:11.776476 rustbininfo-0.2.0/README.md
--rw-r--r--   0        0        0      695 2024-03-21 22:28:45.956022 rustbininfo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      252 2024-03-21 22:27:17.892017 rustbininfo-0.2.0/src/rustbininfo/__init__.py
--rw-r--r--   0        0        0       47 2024-03-14 19:00:56.059969 rustbininfo-0.2.0/src/rustbininfo/exception.py
--rw-r--r--   0        0        0     1603 2024-03-21 22:29:50.996025 rustbininfo-0.2.0/src/rustbininfo/info/compiler.py
--rw-r--r--   0        0        0      659 2024-03-18 23:08:28.600471 rustbininfo-0.2.0/src/rustbininfo/info/dependencies.py
--rw-r--r--   0        0        0     3405 2024-03-18 23:08:28.648471 rustbininfo-0.2.0/src/rustbininfo/info/models/crate.py
--rw-r--r--   0        0        0     1939 2024-03-18 22:40:37.316390 rustbininfo-0.2.0/src/rustbininfo/info/models/info.py
--rw-r--r--   0        0        0       93 2024-03-14 17:49:03.271839 rustbininfo-0.2.0/src/rustbininfo/logger.py
--rw-r--r--   0        0        0     3309 2024-03-18 23:08:28.640471 rustbininfo-0.2.0/src/rustbininfo/main.py
--rw-r--r--   0        0        0     1523 2024-03-18 23:08:28.612471 rustbininfo-0.2.0/src/rustbininfo/utils.py
--rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 rustbininfo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1624 2024-04-17 11:43:03.125461 rustbininfo-0.3.0/README.md
+-rw-r--r--   0        0        0      648 2024-04-17 11:48:43.423061 rustbininfo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      204 2024-04-17 11:43:14.069384 rustbininfo-0.3.0/src/rustbininfo/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-17 11:43:14.069384 rustbininfo-0.3.0/src/rustbininfo/exception.py
+-rw-r--r--   0        0        0     1604 2024-04-17 11:43:14.069384 rustbininfo-0.3.0/src/rustbininfo/info/compiler.py
+-rw-r--r--   0        0        0      962 2024-04-17 11:43:14.069384 rustbininfo-0.3.0/src/rustbininfo/info/dependencies.py
+-rw-r--r--   0        0        0     3404 2024-04-17 11:43:14.069384 rustbininfo-0.3.0/src/rustbininfo/info/models/crate.py
+-rw-r--r--   0        0        0     1939 2024-04-17 11:43:14.073384 rustbininfo-0.3.0/src/rustbininfo/info/models/info.py
+-rw-r--r--   0        0        0       93 2024-04-17 11:43:14.073384 rustbininfo-0.3.0/src/rustbininfo/logger.py
+-rw-r--r--   0        0        0     3308 2024-04-17 11:43:14.073384 rustbininfo-0.3.0/src/rustbininfo/main.py
+-rw-r--r--   0        0        0     1561 2024-04-17 11:43:14.073384 rustbininfo-0.3.0/src/rustbininfo/utils.py
+-rw-r--r--   0        0        0     2056 1970-01-01 00:00:00.000000 rustbininfo-0.3.0/PKG-INFO
```

### Comparing `rustbininfo-0.2.0/README.md` & `rustbininfo-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: rustbininfo
+Version: 0.3.0
+Summary: 
+Author: Nofix
+Author-email: 16479266+N0fix@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pytz (>=2024.1,<2025.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Description-Content-Type: text/markdown
+
 Get information about a stripped rust executable.
 
 This tool is mentioned in [this](https://nofix.re/posts/2024-11-02-rust-symbs/) and [this](https://nofix.re/posts/2024-08-03-arti-rust/) blogposts.
 
 ## Example
 
 ```
@@ -47,9 +61,11 @@
 ## Tests
 
 Tests requieres git-lfs to retrive the test executable.
 
 Then, execute the following command:
 
 ```
+git lfs fetch
+git lfs pull
 pytest -s
-```
+```
```

### Comparing `rustbininfo-0.2.0/pyproject.toml` & `rustbininfo-0.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "rustbininfo"
-version = "0.2.0"
-description = "Get information about stripped rust executables"
+version = "0.3.0"
+description = ""
 authors = ["Nofix <16479266+N0fix@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "rustbininfo", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pytz = "^2024.1"
```

### Comparing `rustbininfo-0.2.0/src/rustbininfo/info/compiler.py` & `rustbininfo-0.3.0/src/rustbininfo/info/compiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def get_rustc_commit(target: pathlib.Path) -> Optional[str]:
     data = open(target, "rb").read()
     res = re.search(b"rustc/([a-z0-9]{40})", data)
 
     if res is None:
         return None
 
-    return res.group(0)[len("rustc/") :].decode()
+    return res.group(0)[len("rustc/"):].decode()
 
 
 def _get_version_from_commit(commit: str):
     url = f"https://github.com/rust-lang/rust/branch_commits/{commit}"
     res = requests.get(url, timeout=20).text
     regex = re.compile(r'href="/rust-lang/rust/releases/tag/([0-9\.]+)"')
 
@@ -38,22 +38,21 @@
 def get_rustc_version(target: pathlib.Path) -> Tuple[Optional[str], Optional[str]]:
     """Get rustc version used in target executable.
 
     Args:
         target (pathlib.Path)
 
     Returns:
-        Tuple[str, str]: Returns Tuple(commit, version).
-        If search failed, returns Tuple(None, None) instead.
+        Tuple[str, str]: Returns Tuple(commit, version). If search failed, returns Tuple(None, None) instead.
     """
     commit = get_rustc_commit(target)
     if commit is None:
         return (None, None)
 
     log.debug(f"Found commit {commit}")
     version = _get_version_from_commit(commit)
     if version is None:
         log.debug("No tag matching this commit, getting latest version")
-        return _get_latest_rustc_version()
+        return (commit, _get_latest_rustc_version())
 
     log.debug(f"Found tag {version}")
     return (commit, version)
```

### Comparing `rustbininfo-0.2.0/src/rustbininfo/info/models/crate.py` & `rustbininfo-0.3.0/src/rustbininfo/info/models/crate.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         try:
             name, version = dep_str.rsplit("-", 1)
             obj = cls(
                 name=name,
                 version=str(semver.Version.parse(version)),
             )
 
-        except:  # noqa E722
+        except: # noqa E722
             name, version, _ = dep_str.rsplit("-", 2)
             obj = cls(
                 name=name,
                 version=str(semver.Version.parse(version)),
             )
 
         obj._fast_load = fast_load
```

### Comparing `rustbininfo-0.2.0/src/rustbininfo/info/models/info.py` & `rustbininfo-0.3.0/src/rustbininfo/info/models/info.py`

 * *Files identical despite different names*

### Comparing `rustbininfo-0.2.0/src/rustbininfo/main.py` & `rustbininfo-0.3.0/src/rustbininfo/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     subparsers.add_parser(
         "info", help="Get information about an executable", parents=[target]
     )
 
     subparsers.add_parser(
         "guess_project_date",
         parents=[target],
-        help="Tries to guess date latest depdnency got added to the project, based on dependencies version",  # noqa E501
+        help="Tries to guess date latest depdnency got added to the project, based on dependencies version", # noqa E501
     )
 
     download_parser = subparsers.add_parser(
         "download", help="Download a crate. Exemple: rand_chacha-0.3.1"
     )
 
     download_parser.add_argument("crate")
```

### Comparing `rustbininfo-0.2.0/src/rustbininfo/utils.py` & `rustbininfo-0.3.0/src/rustbininfo/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         datetime.now()
     )
 
     for dep in crates:
         # print(dep.metadata)
         for i, version in enumerate(dep.metadata["versions"]):
             if version["num"] == dep.version:
-                d = datetime.strptime(version["created_at"], "%Y-%m-%dT%H:%M:%S.%f%z")
+                d = datetime.strptime(
+                    version["created_at"], "%Y-%m-%dT%H:%M:%S.%f%z"
+                )
                 min_date = max(d, min_date)
                 break
 
     for dep in crates:
         for i, version in enumerate(dep.metadata["versions"]):
             if version["num"] == dep.version:
                 if i != 0:
```

