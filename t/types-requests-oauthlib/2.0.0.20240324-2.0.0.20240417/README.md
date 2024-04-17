# Comparing `tmp/types-requests-oauthlib-2.0.0.20240324.tar.gz` & `tmp/types-requests-oauthlib-2.0.0.20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-requests-oauthlib-2.0.0.20240324.tar", last modified: Sun Mar 24 02:17:54 2024, max compression
+gzip compressed data, was "types-requests-oauthlib-2.0.0.20240417.tar", last modified: Wed Apr 17 02:17:41 2024, max compression
```

## Comparing `types-requests-oauthlib-2.0.0.20240324.tar` & `types-requests-oauthlib-2.0.0.20240417.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 02:17:54.027828 types-requests-oauthlib-2.0.0.20240324/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-24 02:17:53.000000 types-requests-oauthlib-2.0.0.20240324/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-24 02:17:53.000000 types-requests-oauthlib-2.0.0.20240324/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-24 02:17:54.027828 types-requests-oauthlib-2.0.0.20240324/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 02:17:54.023827 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-24 02:17:53.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 02:17:54.027828 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/compliance_fixes/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/compliance_fixes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/compliance_fixes/douban.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/compliance_fixes/ebay.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/compliance_fixes/facebook.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/compliance_fixes/fitbit.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/compliance_fixes/instagram.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/compliance_fixes/mailchimp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/compliance_fixes/plentymarkets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/compliance_fixes/slack.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/compliance_fixes/weibo.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/oauth1_auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/oauth1_session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/oauth2_auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-03-24 02:17:38.000000 types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/oauth2_session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 02:17:54.027828 types-requests-oauthlib-2.0.0.20240324/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-24 02:17:53.000000 types-requests-oauthlib-2.0.0.20240324/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 02:17:54.027828 types-requests-oauthlib-2.0.0.20240324/types_requests_oauthlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-24 02:17:53.000000 types-requests-oauthlib-2.0.0.20240324/types_requests_oauthlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-24 02:17:54.000000 types-requests-oauthlib-2.0.0.20240324/types_requests_oauthlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 02:17:53.000000 types-requests-oauthlib-2.0.0.20240324/types_requests_oauthlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-24 02:17:53.000000 types-requests-oauthlib-2.0.0.20240324/types_requests_oauthlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-24 02:17:53.000000 types-requests-oauthlib-2.0.0.20240324/types_requests_oauthlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:41.285591 types-requests-oauthlib-2.0.0.20240417/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-17 02:17:40.000000 types-requests-oauthlib-2.0.0.20240417/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 02:17:40.000000 types-requests-oauthlib-2.0.0.20240417/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-17 02:17:41.285591 types-requests-oauthlib-2.0.0.20240417/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:41.281591 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-17 02:17:40.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:41.285591 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/compliance_fixes/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/compliance_fixes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/compliance_fixes/douban.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/compliance_fixes/ebay.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/compliance_fixes/facebook.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/compliance_fixes/fitbit.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/compliance_fixes/instagram.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/compliance_fixes/mailchimp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/compliance_fixes/plentymarkets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/compliance_fixes/slack.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/compliance_fixes/weibo.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/oauth1_auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/oauth1_session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/oauth2_auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-17 02:16:41.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/oauth2_session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:40.000000 types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:17:41.285591 types-requests-oauthlib-2.0.0.20240417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-17 02:17:40.000000 types-requests-oauthlib-2.0.0.20240417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:41.285591 types-requests-oauthlib-2.0.0.20240417/types_requests_oauthlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-17 02:17:41.000000 types-requests-oauthlib-2.0.0.20240417/types_requests_oauthlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 02:17:41.000000 types-requests-oauthlib-2.0.0.20240417/types_requests_oauthlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:17:41.000000 types-requests-oauthlib-2.0.0.20240417/types_requests_oauthlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 02:17:41.000000 types-requests-oauthlib-2.0.0.20240417/types_requests_oauthlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 02:17:41.000000 types-requests-oauthlib-2.0.0.20240417/types_requests_oauthlib.egg-info/top_level.txt
```

### Comparing `types-requests-oauthlib-2.0.0.20240324/CHANGELOG.md` & `types-requests-oauthlib-2.0.0.20240417/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.0.0.20240417 (2024-04-17)
+
+Remove remaining bare `Incomplete`s (#11768)
+
+Enable Y065
+
 ## 2.0.0.20240324 (2024-03-24)
 
 [stubsabot] Bump requests-oauthlib to 2.0.* (#11649)
 
 Release: https://pypi.org/pypi/requests-oauthlib/2.0.0
 Homepage: https://github.com/requests/requests-oauthlib
 Repository: https://github.com/requests/requests-oauthlib
```

### Comparing `types-requests-oauthlib-2.0.0.20240324/PKG-INFO` & `types-requests-oauthlib-2.0.0.20240417/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-requests-oauthlib
-Version: 2.0.0.20240324
+Version: 2.0.0.20240417
 Summary: Typing stubs for requests-oauthlib
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests-oauthlib.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-requests-oauthlib` aims to provide accurate annotations
 for `requests-oauthlib==2.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests-oauthlib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f337eb8a5149a05528d19605b7ddd0bc9b5125e4` and was tested
-with mypy 1.9.0, pyright 1.1.355, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/compliance_fixes/__init__.pyi` & `types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/compliance_fixes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/oauth1_auth.pyi` & `types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/oauth1_auth.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/oauth1_session.pyi` & `types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/oauth1_session.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-oauthlib-2.0.0.20240324/requests_oauthlib-stubs/oauth2_session.pyi` & `types-requests-oauthlib-2.0.0.20240417/requests_oauthlib-stubs/oauth2_session.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 class _AccessTokenResponseHook(Protocol):
     def __call__(self, response: requests.Response, /) -> requests.Response: ...
 
 class _RefreshTokenResponseHook(Protocol):
     def __call__(self, response: requests.Response, /) -> requests.Response: ...
 
 class _ProtectedRequestHook(Protocol):
-    def __call__(
-        self, url: Incomplete, headers: Incomplete, data: Incomplete, /
-    ) -> tuple[Incomplete, Incomplete, Incomplete]: ...
+    def __call__(self, url, headers, data, /) -> tuple[Incomplete, Incomplete, Incomplete]: ...
 
 class _ComplianceHooks(TypedDict):
     access_token_response: set[_AccessTokenResponseHook]
     refresh_token_response: set[_RefreshTokenResponseHook]
     protected_request: set[_ProtectedRequestHook]
 
 log: Logger
```

### Comparing `types-requests-oauthlib-2.0.0.20240324/setup.py` & `types-requests-oauthlib-2.0.0.20240417/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-requests-oauthlib` aims to provide accurate annotations
 for `requests-oauthlib==2.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests-oauthlib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f337eb8a5149a05528d19605b7ddd0bc9b5125e4` and was tested
-with mypy 1.9.0, pyright 1.1.355, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.0.0.20240324",
+      version="2.0.0.20240417",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests-oauthlib.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-oauthlib', 'types-requests'],
       packages=['requests_oauthlib-stubs'],
-      package_data={'requests_oauthlib-stubs': ['__init__.pyi', 'compliance_fixes/__init__.pyi', 'compliance_fixes/douban.pyi', 'compliance_fixes/ebay.pyi', 'compliance_fixes/facebook.pyi', 'compliance_fixes/fitbit.pyi', 'compliance_fixes/instagram.pyi', 'compliance_fixes/mailchimp.pyi', 'compliance_fixes/plentymarkets.pyi', 'compliance_fixes/slack.pyi', 'compliance_fixes/weibo.pyi', 'oauth1_auth.pyi', 'oauth1_session.pyi', 'oauth2_auth.pyi', 'oauth2_session.pyi', 'METADATA.toml']},
+      package_data={'requests_oauthlib-stubs': ['__init__.pyi', 'compliance_fixes/__init__.pyi', 'compliance_fixes/douban.pyi', 'compliance_fixes/ebay.pyi', 'compliance_fixes/facebook.pyi', 'compliance_fixes/fitbit.pyi', 'compliance_fixes/instagram.pyi', 'compliance_fixes/mailchimp.pyi', 'compliance_fixes/plentymarkets.pyi', 'compliance_fixes/slack.pyi', 'compliance_fixes/weibo.pyi', 'oauth1_auth.pyi', 'oauth1_session.pyi', 'oauth2_auth.pyi', 'oauth2_session.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-requests-oauthlib-2.0.0.20240324/types_requests_oauthlib.egg-info/PKG-INFO` & `types-requests-oauthlib-2.0.0.20240417/types_requests_oauthlib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-requests-oauthlib
-Version: 2.0.0.20240324
+Version: 2.0.0.20240417
 Summary: Typing stubs for requests-oauthlib
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests-oauthlib.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-requests-oauthlib` aims to provide accurate annotations
 for `requests-oauthlib==2.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests-oauthlib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f337eb8a5149a05528d19605b7ddd0bc9b5125e4` and was tested
-with mypy 1.9.0, pyright 1.1.355, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-requests-oauthlib-2.0.0.20240324/types_requests_oauthlib.egg-info/SOURCES.txt` & `types-requests-oauthlib-2.0.0.20240417/types_requests_oauthlib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 requests_oauthlib-stubs/METADATA.toml
 requests_oauthlib-stubs/__init__.pyi
 requests_oauthlib-stubs/oauth1_auth.pyi
 requests_oauthlib-stubs/oauth1_session.pyi
 requests_oauthlib-stubs/oauth2_auth.pyi
 requests_oauthlib-stubs/oauth2_session.pyi
+requests_oauthlib-stubs/py.typed
 requests_oauthlib-stubs/compliance_fixes/__init__.pyi
 requests_oauthlib-stubs/compliance_fixes/douban.pyi
 requests_oauthlib-stubs/compliance_fixes/ebay.pyi
 requests_oauthlib-stubs/compliance_fixes/facebook.pyi
 requests_oauthlib-stubs/compliance_fixes/fitbit.pyi
 requests_oauthlib-stubs/compliance_fixes/instagram.pyi
 requests_oauthlib-stubs/compliance_fixes/mailchimp.pyi
```

