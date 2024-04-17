# Comparing `tmp/mozilla-version-2.1.0.tar.gz` & `tmp/mozilla-version-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-version-2.1.0.tar", last modified: Tue May 23 08:17:29 2023, max compression
+gzip compressed data, was "mozilla-version-2.2.0.tar", last modified: Wed Apr 17 14:23:32 2024, max compression
```

## Comparing `mozilla-version-2.1.0.tar` & `mozilla-version-2.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2023-05-23 08:17:29.100549 mozilla-version-2.1.0/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    15922 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/LICENSE
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      139 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/MANIFEST.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      451 2023-05-23 08:17:29.100439 mozilla-version-2.1.0/PKG-INFO
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7491 2022-11-25 16:16:39.000000 mozilla-version-2.1.0/README.md
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2023-05-23 08:17:29.098031 mozilla-version-2.1.0/mozilla_version/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      262 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/__init__.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     4961 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/balrog.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     2468 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/errors.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      199 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/mozilla_version/fenix.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    24783 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/gecko.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1988 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/maven.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     9520 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/mobile.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1335 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/parser.py
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2023-05-23 08:17:29.099702 mozilla-version-2.1.0/mozilla_version/test/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       87 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/mozilla_version/test/__init__.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7839 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/mozilla_version/test/test_balrog.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      268 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/test/test_default_imports.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      933 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/mozilla_version/test/test_errors.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      193 2022-07-07 15:15:03.000000 mozilla-version-2.1.0/mozilla_version/test/test_fenix.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    24494 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/test/test_gecko.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     3526 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/test/test_maven.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    11948 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/test/test_mobile.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7441 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/mozilla_version/test/test_version.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7929 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/version.py
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2023-05-23 08:17:29.098649 mozilla-version-2.1.0/mozilla_version.egg-info/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      451 2023-05-23 08:17:28.000000 mozilla-version-2.1.0/mozilla_version.egg-info/PKG-INFO
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      973 2023-05-23 08:17:29.000000 mozilla-version-2.1.0/mozilla_version.egg-info/SOURCES.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2023-05-23 08:17:28.000000 mozilla-version-2.1.0/mozilla_version.egg-info/dependency_links.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2022-11-25 13:12:40.000000 mozilla-version-2.1.0/mozilla_version.egg-info/not-zip-safe
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       12 2023-05-23 08:17:29.000000 mozilla-version-2.1.0/mozilla_version.egg-info/requires.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       16 2023-05-23 08:17:29.000000 mozilla-version-2.1.0/mozilla_version.egg-info/top_level.txt
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2023-05-23 08:17:29.100285 mozilla-version-2.1.0/requirements/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       12 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/requirements/base.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      363 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/requirements/base.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       70 2022-11-25 14:28:49.000000 mozilla-version-2.1.0/requirements/docs.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    15614 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/requirements/docs.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      143 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/requirements/test.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     8589 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/requirements/test.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       38 2023-05-23 08:17:29.100584 mozilla-version-2.1.0/setup.cfg
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1194 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/setup.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)        6 2023-05-23 08:16:04.000000 mozilla-version-2.1.0/version.txt
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 14:23:32.204070 mozilla-version-2.2.0/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    15922 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/LICENSE
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      139 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/MANIFEST.in
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      451 2024-04-17 14:23:32.203953 mozilla-version-2.2.0/PKG-INFO
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     7491 2022-11-25 16:16:39.000000 mozilla-version-2.2.0/README.md
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 14:23:32.200083 mozilla-version-2.2.0/mozilla_version/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      262 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/__init__.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     4961 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/balrog.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     2468 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/errors.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      199 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/mozilla_version/fenix.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    28669 2024-04-17 14:22:13.000000 mozilla-version-2.2.0/mozilla_version/gecko.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     1988 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/maven.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     9520 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/mobile.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     1335 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/parser.py
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 14:23:32.202441 mozilla-version-2.2.0/mozilla_version/test/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       87 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/mozilla_version/test/__init__.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     7839 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/mozilla_version/test/test_balrog.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      268 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/test/test_default_imports.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      933 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/mozilla_version/test/test_errors.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      193 2022-07-07 15:15:03.000000 mozilla-version-2.2.0/mozilla_version/test/test_fenix.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    41476 2024-04-17 14:22:13.000000 mozilla-version-2.2.0/mozilla_version/test/test_gecko.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     3526 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/test/test_maven.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    11948 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/test/test_mobile.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     7441 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/mozilla_version/test/test_version.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     7929 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/version.py
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 14:23:32.200849 mozilla-version-2.2.0/mozilla_version.egg-info/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      451 2024-04-17 14:23:31.000000 mozilla-version-2.2.0/mozilla_version.egg-info/PKG-INFO
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      973 2024-04-17 14:23:32.000000 mozilla-version-2.2.0/mozilla_version.egg-info/SOURCES.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2024-04-17 14:23:31.000000 mozilla-version-2.2.0/mozilla_version.egg-info/dependency_links.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2024-04-17 08:07:18.000000 mozilla-version-2.2.0/mozilla_version.egg-info/not-zip-safe
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       12 2024-04-17 14:23:32.000000 mozilla-version-2.2.0/mozilla_version.egg-info/requires.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       16 2024-04-17 14:23:32.000000 mozilla-version-2.2.0/mozilla_version.egg-info/top_level.txt
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 14:23:32.203642 mozilla-version-2.2.0/requirements/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       12 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/requirements/base.in
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      363 2024-04-17 07:59:45.000000 mozilla-version-2.2.0/requirements/base.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       70 2022-11-25 14:28:49.000000 mozilla-version-2.2.0/requirements/docs.in
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    15614 2024-04-17 07:59:45.000000 mozilla-version-2.2.0/requirements/docs.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      143 2024-04-17 07:59:39.000000 mozilla-version-2.2.0/requirements/test.in
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     8589 2024-04-17 07:59:45.000000 mozilla-version-2.2.0/requirements/test.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       38 2024-04-17 14:23:32.204112 mozilla-version-2.2.0/setup.cfg
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     1194 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/setup.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)        6 2024-04-17 14:22:13.000000 mozilla-version-2.2.0/version.txt
```

### Comparing `mozilla-version-2.1.0/LICENSE` & `mozilla-version-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/README.md` & `mozilla-version-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/mozilla_version/balrog.py` & `mozilla-version-2.2.0/mozilla_version/balrog.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/mozilla_version/errors.py` & `mozilla-version-2.2.0/mozilla_version/errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/mozilla_version/gecko.py` & `mozilla-version-2.2.0/mozilla_version/gecko.py`

 * *Files 12% similar despite different names*

```diff
@@ -153,14 +153,32 @@
             pattern_message
             for condition, pattern_message in ((
                 not self.is_four_digit_scheme and self.old_fourth_number is not None,
                 'The old fourth number can only be defined on Gecko 1.5.x.y or 2.0.x.y',
             ), (
                 self.beta_number is not None and self.patch_number is not None,
                 'Beta number and patch number cannot be both defined',
+            ), (
+                self.is_major and self.is_esr,
+                'Version cannot be both a major and an ESR one',
+            ), (
+                self.is_major and self.is_stability,
+                'Version cannot be both a major and a stability one',
+            ), (
+                self.is_major and self.is_development,
+                'Version cannot be both a major and a development one',
+            ), (
+                self.is_stability and self.is_esr,
+                'Version cannot be both a stability and an ESR one',
+            ), (
+                self.is_stability and self.is_development,
+                'Version cannot be both a stability and a development one',
+            ), (
+                self.is_development and self.is_esr,
+                'Version cannot be both a development and an ESR one',
             ))
             if condition
         ]
 
         # Firefox 5 is the first version to implement the rapid release model, which defines
         # the scheme used so far.
         if self.is_rapid_release_scheme:
@@ -257,14 +275,59 @@
     def is_release(self):
         """Return `True` if `GeckoVersion` was built with a string matching a release version."""
         return not any((
             self.is_nightly, self.is_aurora_or_devedition, self.is_beta,
             self.is_release_candidate, self.is_esr
         ))
 
+    @property
+    def is_major(self):
+        """Return `True` if `GeckoVersion` is considered to be a major version.
+
+        It's usually the .0 release but some exceptions may occur. ESR are not considered
+        major versions.
+        """
+        return all((
+            not self.is_development,
+            not self.is_esr,
+            self.minor_number == 0,
+            self.patch_number is None
+        ))
+
+    @property
+    def is_stability(self):
+        """Return `True` if `GeckoVersion` is a version that fixed a major one."""
+        conditions = [
+            not self.is_development,
+            not self.is_major,
+            not self.is_esr,
+        ]
+        if self.is_four_digit_scheme:
+            conditions.extend([
+                self.patch_number == 0,
+                self.old_fourth_number != 0,
+            ])
+        else:
+            conditions.append(
+                self.minor_number != 0 or self.patch_number != 0
+            )
+
+        return all(conditions)
+
+    @property
+    def is_development(self):
+        """Return `True` if `GeckoVersion` was known to require further development.
+
+        It's usually a beta or before the rapid release scheme, a release candidate.
+        """
+        return any((
+            self.is_beta,
+            self.is_release_candidate,
+        ))
+
     def __str__(self):
         """Implement string representation.
 
         Computes a new string based on the given attributes.
         """
         string = super().__str__()
 
@@ -464,26 +527,40 @@
 
         return bump_version_type_kwargs
 
 
 class _VersionWithEdgeCases(GeckoVersion):
     def __attrs_post_init__(self):
         for edge_case in self._RELEASED_EDGE_CASES:
-            if all(
-                getattr(self, number_type) == edge_case.get(number_type, None)
-                for number_type in self._ALL_NUMBERS
-                if number_type != 'build_number'
-            ):
-                if self.build_number is None:
-                    return
-                elif self.build_number == edge_case.get('build_number', None):
-                    return
+            if self._do_all_numbers_match(edge_case):
+                return
 
         super().__attrs_post_init__()
 
+    @property
+    def is_major(self):
+        for edge_case in self._RELEASED_EDGE_CASES_MAJOR:
+            if self._do_all_numbers_match(edge_case):
+                return True
+
+        return super().is_major
+
+    def _do_all_numbers_match(self, edge_case):
+        if all(
+            getattr(self, number_type) == edge_case.get(number_type, None)
+            for number_type in self._ALL_NUMBERS
+            if number_type != 'build_number'
+        ):
+            if self.build_number is None:
+                return True
+            elif self.build_number == edge_case.get('build_number', None):
+                return True
+
+        return False
+
 
 class FirefoxVersion(_VersionWithEdgeCases):
     """Class that validates and handles Firefox version numbers."""
 
     _RELEASED_EDGE_CASES = ({
         'major_number': 1,
         'minor_number': 5,
@@ -524,14 +601,47 @@
         'major_number': 38,
         'minor_number': 0,
         'patch_number': 5,
         'beta_number': 3,
         'build_number': 1,
     })
 
+    _RELEASED_EDGE_CASES_MAJOR = ({
+        'major_number': 1,
+        'minor_number': 5,
+    }, {
+        'major_number': 3,
+        'minor_number': 5,
+    }, {
+        'major_number': 3,
+        'minor_number': 6,
+    }, {
+        'major_number': 14,
+        'minor_number': 0,
+        'patch_number': 1,
+        'build_number': 1,
+    }, {
+        'major_number': 33,
+        'minor_number': 1,
+        'build_number': 1,
+    }, {
+        'major_number': 33,
+        'minor_number': 1,
+        'build_number': 2,
+    }, {
+        'major_number': 33,
+        'minor_number': 1,
+        'build_number': 3,
+    }, {
+        'major_number': 125,
+        'minor_number': 0,
+        'patch_number': 1,
+        'build_number': 1,
+    })
+
 
 class DeveditionVersion(GeckoVersion):
     """Class that validates and handles Devedition after it became an equivalent to beta."""
 
     # No edge case were shipped
 
     def __attrs_post_init__(self):
@@ -561,14 +671,31 @@
         'major_number': 38,
         'minor_number': 0,
         'patch_number': 5,
         'beta_number': 4,
         'build_number': 1,
     })
 
+    _RELEASED_EDGE_CASES_MAJOR = ({
+        'major_number': 1,
+        'minor_number': 1,
+    }, {
+        'major_number': 14,
+        'minor_number': 0,
+        'patch_number': 1,
+    }, {
+        'major_number': 33,
+        'minor_number': 1,
+        'build_number': 1,
+    }, {
+        'major_number': 68,
+        'minor_number': 1,
+        'build_number': 1,
+    })
+
     _LAST_FENNEC_VERSION = 68
 
     def __attrs_post_init__(self):
         """Ensure attributes are sane all together."""
         # Versions matching 68.Xa1, 68.XbN, or simply 68.X are expected since bug 1523402. The
         # latter is needed because of the version.txt of beta
         if (
@@ -632,14 +759,27 @@
     }, {
         'major_number': 45,
         'minor_number': 2,
         'beta_number': 1,
         'build_number': 2,
     })
 
+    _RELEASED_EDGE_CASES_MAJOR = ({
+        'major_number': 1,
+        'minor_number': 5,
+    }, {
+        'major_number': 3,
+        'minor_number': 1,
+    }, {
+        'major_number': 38,
+        'minor_number': 0,
+        'patch_number': 1,
+        'build_number': 1,
+    })
+
 
 class GeckoSnapVersion(GeckoVersion):
     """Class that validates and handles Gecko's Snap version numbers.
 
     Snap is a Linux packaging format developped by Canonical. Valid numbers are like "63.0b7-1",
     "1" stands for "build1". Release Engineering set this scheme at the beginning of Snap and now
     we can't rename published snap to the regular pattern like "63.0b7-build1".
```

### Comparing `mozilla-version-2.1.0/mozilla_version/maven.py` & `mozilla-version-2.2.0/mozilla_version/maven.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/mozilla_version/mobile.py` & `mozilla-version-2.2.0/mozilla_version/mobile.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/mozilla_version/parser.py` & `mozilla-version-2.2.0/mozilla_version/parser.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/mozilla_version/test/test_balrog.py` & `mozilla-version-2.2.0/mozilla_version/test/test_balrog.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/mozilla_version/test/test_errors.py` & `mozilla-version-2.2.0/mozilla_version/test/test_errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/mozilla_version/test/test_maven.py` & `mozilla-version-2.2.0/mozilla_version/test/test_maven.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/mozilla_version/test/test_mobile.py` & `mozilla-version-2.2.0/mozilla_version/test/test_mobile.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/mozilla_version/test/test_version.py` & `mozilla-version-2.2.0/mozilla_version/test/test_version.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/mozilla_version/version.py` & `mozilla-version-2.2.0/mozilla_version/version.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/mozilla_version.egg-info/SOURCES.txt` & `mozilla-version-2.2.0/mozilla_version.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/requirements/docs.txt` & `mozilla-version-2.2.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/requirements/test.txt` & `mozilla-version-2.2.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.1.0/setup.py` & `mozilla-version-2.2.0/setup.py`

 * *Files identical despite different names*

