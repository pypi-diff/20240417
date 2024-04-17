# Comparing `tmp/cz_legacy-1.0.1.tar.gz` & `tmp/cz_legacy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz_legacy-1.0.1.tar", max compression
+gzip compressed data, was "cz_legacy-1.0.2.tar", max compression
```

## Comparing `cz_legacy-1.0.1.tar` & `cz_legacy-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-04-08 17:52:27.966560 cz_legacy-1.0.1/LICENSE
--rw-r--r--   0        0        0     1850 2024-04-01 02:32:34.511217 cz_legacy-1.0.1/cz_legacy/__init__.py
--rw-r--r--   0        0        0     2080 2024-04-01 02:29:44.449115 cz_legacy-1.0.1/cz_legacy/cz_legacy.py
--rw-r--r--   0        0        0     3333 2024-04-01 02:32:50.331995 cz_legacy-1.0.1/docs/README.md
--rw-r--r--   0        0        0     2100 2024-04-01 02:32:34.528322 cz_legacy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4710 1970-01-01 00:00:00.000000 cz_legacy-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-08 17:52:27.966560 cz_legacy-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2108 2024-04-17 02:00:54.614671 cz_legacy-1.0.2/cz_legacy/__init__.py
+-rw-r--r--   0        0        0     2080 2024-04-01 02:29:44.449115 cz_legacy-1.0.2/cz_legacy/cz_legacy.py
+-rw-r--r--   0        0        0     3333 2024-04-17 02:00:58.593523 cz_legacy-1.0.2/docs/README.md
+-rw-r--r--   0        0        0     2066 2024-04-17 02:00:54.632116 cz_legacy-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 cz_legacy-1.0.2/PKG-INFO
```

### Comparing `cz_legacy-1.0.1/LICENSE` & `cz_legacy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cz_legacy-1.0.1/cz_legacy/__init__.py` & `cz_legacy-1.0.2/cz_legacy/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 """cz_legacy."""
 
 from datetime import datetime, timezone
 from enum import Enum
 from os import getenv
 from warnings import filterwarnings
 
-from beartype import BeartypeConf
-from beartype.claw import beartype_this_package
-from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
-from typing_extensions import Self
-
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 __pkg_name__ = 'cz_legacy'
 
 
-class _RuntimeTypeCheckingModes(Enum):
-    """Supported global runtime type checking modes."""
-
-    ERROR = 'ERROR'
-    WARNING = 'WARNING'
-    OFF = None
-
-    @classmethod
-    def from_environment(cls) -> Self:  # pragma: no cover
-        """Return the configured mode."""
-        rtc_mode = getenv('RUNTIME_TYPE_CHECKING_MODE') or None
-        try:
-            return cls(rtc_mode)
-        except ValueError:
-            modes = [_e.value for _e in cls]
-            msg = f"'RUNTIME_TYPE_CHECKING_MODE={rtc_mode}' is not an allowed mode from {modes}"
-            raise ValueError(msg) from None
-
-
-def configure_runtime_type_checking_mode() -> None:  # pragma: no cover
-    """Optionally configure runtime type checking mode globally."""
-    rtc_mode = _RuntimeTypeCheckingModes.from_environment()
-
-    if rtc_mode is not _RuntimeTypeCheckingModes.OFF:
-        from beartype.roar import BeartypeClawDecorWarning  # noqa: PLC0415
-
-        beartype_this_package(conf=BeartypeConf(
-            warning_cls_on_decorator_exception=(
-                None if rtc_mode is _RuntimeTypeCheckingModes.ERROR else BeartypeClawDecorWarning
-            ),
-        ))
-
-
-_PEP585_DATE = 2025
-if datetime.now(tz=timezone.utc).year <= _PEP585_DATE:  # pragma: no cover
-    filterwarnings('ignore', category=BeartypeDecorHintPep585DeprecationWarning)
-configure_runtime_type_checking_mode()
+try:  # Beartype is only available on Python ^3.8.0
+    from beartype import BeartypeConf
+    from beartype.claw import beartype_this_package
+    from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
+    from typing_extensions import Self
+
+    class _RuntimeTypeCheckingModes(Enum):
+        """Supported global runtime type checking modes."""
+
+        ERROR = 'ERROR'
+        WARNING = 'WARNING'
+        OFF = None
+
+        @classmethod
+        def from_environment(cls) -> Self:  # pragma: no cover
+            """Return the configured mode."""
+            rtc_mode = getenv('RUNTIME_TYPE_CHECKING_MODE') or None
+            try:
+                return cls(rtc_mode)
+            except ValueError:
+                modes = [_e.value for _e in cls]
+                msg = f"'RUNTIME_TYPE_CHECKING_MODE={rtc_mode}' is not an allowed mode from {modes}"
+                raise ValueError(msg) from None
+
+    def configure_runtime_type_checking_mode() -> None:  # pragma: no cover
+        """Optionally configure runtime type checking mode globally."""
+        rtc_mode = _RuntimeTypeCheckingModes.from_environment()
+
+        if rtc_mode is not _RuntimeTypeCheckingModes.OFF:
+            from beartype.roar import BeartypeClawDecorWarning  # noqa: PLC0415
+
+            beartype_this_package(
+                conf=BeartypeConf(
+                    warning_cls_on_decorator_exception=(
+                        None if rtc_mode is _RuntimeTypeCheckingModes.ERROR else BeartypeClawDecorWarning
+                    ),
+                ),
+            )
+
+    _PEP585_DATE = 2025
+    if datetime.now(tz=timezone.utc).year <= _PEP585_DATE:  # pragma: no cover
+        filterwarnings('ignore', category=BeartypeDecorHintPep585DeprecationWarning)
+    configure_runtime_type_checking_mode()
+except ImportError:
+    pass
 
 # ====== Above is the recommended code from calcipy_template and may be updated on new releases ======
```

### Comparing `cz_legacy-1.0.1/cz_legacy/cz_legacy.py` & `cz_legacy-1.0.2/cz_legacy/cz_legacy.py`

 * *Files identical despite different names*

### Comparing `cz_legacy-1.0.1/docs/README.md` & `cz_legacy-1.0.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `cz_legacy-1.0.1/pyproject.toml` & `cz_legacy-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.0.1"
+version = "1.0.2"
 version_files = ["cz_legacy/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
@@ -25,25 +25,25 @@
 include = ["LICENSE"]
 keywords = ["commitizen", "conventional commits", "git"]
 license = "MIT"
 maintainers = []
 name = "cz_legacy"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/cz_legacy"
-version = "1.0.1"
+version = "1.0.2"
 
 [tool.poetry.dependencies]
 # Keep in sync with commitizen (Note: v3 will be ^3.7)
 # https://github.com/commitizen-tools/commitizen/blob/378a42881891633d8a81939cb46426eb36ed01aa/pyproject.toml#L50
 python = "^3.7"
+beartype = {python = "^3.8.0", version = ">=0.18.2"}
 commitizen = ">=3.0.0"
 
 [tool.poetry.group.dev.dependencies]
-calcipy = {python = "^3.9.13", extras = ["ddict", "doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=2.0.1"}
-mkdocs_build_plantuml_plugin = "1.9.0" # Issue with Python 3.8 and unknown Path.walk()
+calcipy = {python = "^3.9.13", extras = ["ddict", "doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=2.0.4"}
 
 # Required for discovery by 'commitizen'
 [tool.poetry.plugins."commitizen.plugin"]
 "cz_legacy" = "cz_legacy.cz_legacy:_LegacyCz"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/kyleking/cz_legacy/issues"
```

### Comparing `cz_legacy-1.0.1/PKG-INFO` & `cz_legacy-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz_legacy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Extends Conventional Commits Change Types with User-Defined Legacy Types for Commitizen
 Home-page: https://github.com/kyleking/cz_legacy
 License: MIT
 Keywords: commitizen,conventional commits,git
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Dist: beartype (>=0.18.2) ; python_full_version >= "3.8.0" and python_full_version < "4.0.0"
 Requires-Dist: commitizen (>=3.0.0)
 Project-URL: Bug Tracker, https://github.com/kyleking/cz_legacy/issues
 Project-URL: Changelog, https://github.com/kyleking/cz_legacy/blob/main/docs/docs/CHANGELOG.md
 Project-URL: Documentation, https://cz_legacy.kyleking.me
 Project-URL: Repository, https://github.com/kyleking/cz_legacy
 Description-Content-Type: text/markdown
```

