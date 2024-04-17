# Comparing `tmp/dependence-0.0.6.tar.gz` & `tmp/dependence-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dependence-0.0.6.tar", last modified: Mon Feb 19 00:35:47 2024, max compression
+gzip compressed data, was "dependence-0.1.0.tar", last modified: Wed Apr 17 20:34:52 2024, max compression
```

## Comparing `dependence-0.0.6.tar` & `dependence-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:35:47.262992 dependence-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-02-19 00:35:47.262992 dependence-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-02-19 00:35:29.000000 dependence-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:35:47.258992 dependence-0.0.6/dependence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 00:35:29.000000 dependence-0.0.6/dependence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-19 00:35:29.000000 dependence-0.0.6/dependence/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-02-19 00:35:29.000000 dependence-0.0.6/dependence/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-02-19 00:35:29.000000 dependence-0.0.6/dependence/freeze.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 00:35:29.000000 dependence-0.0.6/dependence/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16603 2024-02-19 00:35:29.000000 dependence-0.0.6/dependence/update.py
--rw-r--r--   0 runner    (1001) docker     (127)    30894 2024-02-19 00:35:29.000000 dependence-0.0.6/dependence/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:35:47.262992 dependence-0.0.6/dependence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-02-19 00:35:47.000000 dependence-0.0.6/dependence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-02-19 00:35:47.000000 dependence-0.0.6/dependence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 00:35:47.000000 dependence-0.0.6/dependence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-19 00:35:47.000000 dependence-0.0.6/dependence.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-19 00:35:47.000000 dependence-0.0.6/dependence.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-19 00:35:47.000000 dependence-0.0.6/dependence.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-19 00:35:29.000000 dependence-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-19 00:35:47.262992 dependence-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-19 00:35:29.000000 dependence-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:35:47.262992 dependence-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-02-19 00:35:29.000000 dependence-0.0.6/tests/test_requirements_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:52.152799 dependence-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-17 20:34:52.152799 dependence-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-17 20:34:32.000000 dependence-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:52.152799 dependence-0.1.0/dependence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:32.000000 dependence-0.1.0/dependence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-17 20:34:32.000000 dependence-0.1.0/dependence/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-17 20:34:32.000000 dependence-0.1.0/dependence/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-04-17 20:34:32.000000 dependence-0.1.0/dependence/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:32.000000 dependence-0.1.0/dependence/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16603 2024-04-17 20:34:32.000000 dependence-0.1.0/dependence/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31133 2024-04-17 20:34:32.000000 dependence-0.1.0/dependence/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:52.152799 dependence-0.1.0/dependence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-17 20:34:52.000000 dependence-0.1.0/dependence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-17 20:34:52.000000 dependence-0.1.0/dependence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:34:52.000000 dependence-0.1.0/dependence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 20:34:52.000000 dependence-0.1.0/dependence.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 20:34:52.000000 dependence-0.1.0/dependence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 20:34:52.000000 dependence-0.1.0/dependence.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-17 20:34:32.000000 dependence-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-17 20:34:52.152799 dependence-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 20:34:32.000000 dependence-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:52.152799 dependence-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-17 20:34:32.000000 dependence-0.1.0/tests/test_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-17 20:34:32.000000 dependence-0.1.0/tests/test_update.py
```

### Comparing `dependence-0.0.6/PKG-INFO` & `dependence-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dependence
-Version: 0.0.6
+Version: 0.1.0
 Summary: Requirement (dependency) management for python projects
 Home-page: https://github.com/enorganic/dependence
 Author-email: david@belais.me
 License: MIT
 Keywords: requirements,dependencies
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
@@ -92,44 +92,53 @@
 ```
 
 #### dependence freeze
 
 ```console
 $ dependence freeze -h
 usage: dependence freeze [-h] [-e EXCLUDE] [-er EXCLUDE_RECURSIVE]
-                           [-nv NO_VERSION]
-                           requirement [requirement ...]
+                         [-nv NO_VERSION] [-do] [--reverse]
+                         requirement [requirement ...]
 
-This command prints dependencies inferred from an installed distribution or
-project, in a similar format to the output of `pip freeze`, except that all
-generated requirements are specified in the format "distribution-
-name==0.0.0" (including for editable installations). Using this command
-instead of `pip freeze` to generate requirement files ensures that you don't
-bloat your requirements files with superfluous distributions.
+This command prints dependencies inferred from an installed
+distribution or project, in a similar format to the output of `pip
+freeze`, except that all generated requirements are specified in the
+format "distribution-name==0.0.0" (including for editable
+installations). Using this command instead of `pip freeze` to generate
+requirement files ensures that you don't bloat your requirements files
+with superfluous distributions. The default sorting starts with
+directly specified requirements, followed by recursively discovered
+requirements, in the order of discovery.
 
 positional arguments:
-  requirement           One or more requirement specifiers (for example:
-                        "requirement-name", "requirement-
-                        name[extra-a,extra-b]", ".[extra-a, extra-b]" or
-                        "../other-editable-package-directory[extra-a,
-                        extra-b]) and/or paths to a setup.py, setup.cfg,
-                        pyproject.toml, tox.ini or requirements.txt file
+  requirement           One or more requirement specifiers (for
+                        example: "requirement-name", "requirement-
+                        name[extra-a,extra-b]", ".[extra-a, extra-b]"
+                        or "../other-editable-package-
+                        directory[extra-a, extra-b]) and/or paths to a
+                        setup.py, setup.cfg, pyproject.toml, tox.ini or
+                        requirements.txt file
 
 optional arguments:
   -h, --help            show this help message and exit
   -e EXCLUDE, --exclude EXCLUDE
                         A distribution (or comma-separated list of
                         distributions) to exclude from the output
   -er EXCLUDE_RECURSIVE, --exclude-recursive EXCLUDE_RECURSIVE
                         A distribution (or comma-separated list of
-                        distributions) to exclude from the output. Unlike -e
-                        / --exclude, this argument also precludes recursive
-                        requirement discovery for the specified packages,
-                        thereby excluding all of the excluded package's
-                        requirements which are not required by another (non-
-                        excluded) distribution.
+                        distributions) to exclude from the output.
+                        Unlike -e / --exclude, this argument also
+                        precludes recursive requirement discovery for
+                        the specified packages, thereby excluding all
+                        of the excluded package's requirements which
+                        are not required by another (non-excluded)
+                        distribution.
   -nv NO_VERSION, --no-version NO_VERSION
-                        Don't include versions (only output distribution
-                        names) for packages matching this/these glob
-                        pattern(s) (note: the value must be single-quoted if
-                        it contains wildcards)
+                        Don't include versions (only output
+                        distribution names) for packages matching
+                        this/these glob pattern(s) (note: the value
+                        must be single-quoted if it contains wildcards)
+  -do, --dependency-order
+                        Sort requirements so that dependents precede
+                        dependencies
+  --reverse             Print requirements in reverse order
 ```
```

### Comparing `dependence-0.0.6/README.md` & `dependence-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -75,44 +75,53 @@
 ```
 
 #### dependence freeze
 
 ```console
 $ dependence freeze -h
 usage: dependence freeze [-h] [-e EXCLUDE] [-er EXCLUDE_RECURSIVE]
-                           [-nv NO_VERSION]
-                           requirement [requirement ...]
+                         [-nv NO_VERSION] [-do] [--reverse]
+                         requirement [requirement ...]
 
-This command prints dependencies inferred from an installed distribution or
-project, in a similar format to the output of `pip freeze`, except that all
-generated requirements are specified in the format "distribution-
-name==0.0.0" (including for editable installations). Using this command
-instead of `pip freeze` to generate requirement files ensures that you don't
-bloat your requirements files with superfluous distributions.
+This command prints dependencies inferred from an installed
+distribution or project, in a similar format to the output of `pip
+freeze`, except that all generated requirements are specified in the
+format "distribution-name==0.0.0" (including for editable
+installations). Using this command instead of `pip freeze` to generate
+requirement files ensures that you don't bloat your requirements files
+with superfluous distributions. The default sorting starts with
+directly specified requirements, followed by recursively discovered
+requirements, in the order of discovery.
 
 positional arguments:
-  requirement           One or more requirement specifiers (for example:
-                        "requirement-name", "requirement-
-                        name[extra-a,extra-b]", ".[extra-a, extra-b]" or
-                        "../other-editable-package-directory[extra-a,
-                        extra-b]) and/or paths to a setup.py, setup.cfg,
-                        pyproject.toml, tox.ini or requirements.txt file
+  requirement           One or more requirement specifiers (for
+                        example: "requirement-name", "requirement-
+                        name[extra-a,extra-b]", ".[extra-a, extra-b]"
+                        or "../other-editable-package-
+                        directory[extra-a, extra-b]) and/or paths to a
+                        setup.py, setup.cfg, pyproject.toml, tox.ini or
+                        requirements.txt file
 
 optional arguments:
   -h, --help            show this help message and exit
   -e EXCLUDE, --exclude EXCLUDE
                         A distribution (or comma-separated list of
                         distributions) to exclude from the output
   -er EXCLUDE_RECURSIVE, --exclude-recursive EXCLUDE_RECURSIVE
                         A distribution (or comma-separated list of
-                        distributions) to exclude from the output. Unlike -e
-                        / --exclude, this argument also precludes recursive
-                        requirement discovery for the specified packages,
-                        thereby excluding all of the excluded package's
-                        requirements which are not required by another (non-
-                        excluded) distribution.
+                        distributions) to exclude from the output.
+                        Unlike -e / --exclude, this argument also
+                        precludes recursive requirement discovery for
+                        the specified packages, thereby excluding all
+                        of the excluded package's requirements which
+                        are not required by another (non-excluded)
+                        distribution.
   -nv NO_VERSION, --no-version NO_VERSION
-                        Don't include versions (only output distribution
-                        names) for packages matching this/these glob
-                        pattern(s) (note: the value must be single-quoted if
-                        it contains wildcards)
+                        Don't include versions (only output
+                        distribution names) for packages matching
+                        this/these glob pattern(s) (note: the value
+                        must be single-quoted if it contains wildcards)
+  -do, --dependency-order
+                        Sort requirements so that dependents precede
+                        dependencies
+  --reverse             Print requirements in reverse order
 ```
```

### Comparing `dependence-0.0.6/dependence/__main__.py` & `dependence-0.1.0/dependence/__main__.py`

 * *Files identical despite different names*

### Comparing `dependence-0.0.6/dependence/_utilities.py` & `dependence-0.1.0/dependence/_utilities.py`

 * *Files identical despite different names*

### Comparing `dependence-0.0.6/dependence/freeze.py` & `dependence-0.1.0/dependence/freeze.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,85 @@
 import argparse
 from fnmatch import fnmatch
 from importlib.metadata import Distribution
 from importlib.metadata import distribution as _get_distribution
 from itertools import chain
-from typing import Iterable, Set, Tuple
+from typing import Dict, Iterable, MutableSet, Tuple, cast
 
 from more_itertools import unique_everseen
 
 from ._utilities import iter_parse_delimited_values
 from .utilities import (
     get_distribution,
     get_required_distribution_names,
     get_requirement_string_distribution_name,
     install_requirement,
     is_configuration_file,
     iter_configuration_file_requirement_strings,
     normalize_name,
 )
 
-_DO_NOT_PIN_DISTRIBUTION_NAMES: Set[str] = {
-    # standard library
+_DO_NOT_PIN_DISTRIBUTION_NAMES: MutableSet[str] = {
     "importlib-metadata",
     "importlib-resources",
 }
 
 
+def _iter_sort_dependents_last(requirements: Iterable[str]) -> Iterable[str]:
+    """
+    Sort requirements such that dependents are first and dependencies are last.
+    """
+    requirements = list(requirements)
+    distribution_name: str
+    distribution_requirement: Dict[str, str] = {
+        get_requirement_string_distribution_name(requirement): requirement
+        for requirement in requirements
+    }
+    dependent_dependencies: Dict[str, MutableSet[str]] = {
+        distribution_name: get_required_distribution_names(requirement)
+        for distribution_name, requirement in distribution_requirement.items()
+    }
+    while dependent_dependencies:
+        dependent: str
+        dependencies: MutableSet[str]
+        item: Tuple[str, MutableSet[str]]
+        for dependent, dependencies in sorted(
+            tuple(dependent_dependencies.items()),
+            key=lambda item: item[0].lower(),
+        ):
+
+            def is_non_circular_requirement(dependency: str) -> bool:
+                """
+                Return `True` if the dependency is still among the unaccounted
+                for requirements, and is not a circular reference
+                """
+                return (dependency in dependent_dependencies) and (
+                    # Exclude interdependent distributions
+                    # (circular references)
+                    dependent
+                    not in dependent_dependencies[dependency]
+                )
+
+            if (not dependencies) or not any(
+                map(
+                    is_non_circular_requirement,
+                    dependencies,
+                )
+            ):
+                yield distribution_requirement.pop(dependent)
+                del dependent_dependencies[dependent]
+
+
 def get_frozen_requirements(
     requirements: Iterable[str] = (),
     exclude: Iterable[str] = (),
     exclude_recursive: Iterable[str] = (),
     no_version: Iterable[str] = (),
+    dependency_order: bool = False,
+    reverse: bool = False,
 ) -> Tuple[str, ...]:
     """
     Get the (frozen) requirements for one or more specified distributions or
     configuration files.
 
     Parameters:
 
@@ -43,71 +89,85 @@
     - exclude ([str]): One or more distributions to exclude/ignore
     - exclude_recursive ([str]): One or more distributions to exclude/ignore.
       Note: Excluding a distribution here excludes all requirements which would
       be identified through recursively.
       those requirements occur elsewhere.
     - no_version ([str]) = (): Exclude version numbers from the output
       (only return distribution names)
+    - dependency_order (bool) = False: Sort requirements so that dependents
+      precede dependencies
     """
     # Separate requirement strings from requirement files
     if isinstance(requirements, str):
-        requirements = {requirements}
+        requirements = set((requirements,))
     else:
         requirements = set(requirements)
     if isinstance(no_version, str):
         no_version = (no_version,)
     elif not isinstance(no_version, tuple):
         no_version = tuple(no_version)
-    requirement_files: Set[str] = set(
+    requirement_files: MutableSet[str] = set(
         filter(is_configuration_file, requirements)
     )
-    requirement_strings: Set[str] = requirements - requirement_files
-    name: str
-    return tuple(
-        sorted(
-            _iter_frozen_requirements(
-                unique_everseen(
-                    chain(
-                        requirement_strings,
-                        *map(
-                            iter_configuration_file_requirement_strings,
-                            requirement_files,
-                        ),
-                    )
+    requirement_strings: MutableSet[str] = cast(
+        MutableSet[str], requirements - requirement_files
+    )
+    frozen_requirements: Iterable[str] = _iter_frozen_requirements(
+        unique_everseen(
+            chain(
+                requirement_strings,
+                *map(
+                    iter_configuration_file_requirement_strings,
+                    requirement_files,
                 ),
-                exclude=set(
-                    chain(
-                        # Exclude requirement strings which are *not*
-                        # distribution names (such as editable package paths),
-                        # as in these cases we are typically looking for this
-                        # package's dependencies
-                        (
-                            set(
-                                map(
-                                    get_requirement_string_distribution_name,
-                                    requirement_strings,
-                                )
-                            )
-                            - set(map(normalize_name, requirement_strings))
-                        ),
-                        map(normalize_name, exclude),
+            )
+        ),
+        exclude=set(
+            chain(
+                # Exclude requirement strings which are *not*
+                # distribution names (such as editable package paths),
+                # as in these cases we are typically looking for this
+                # package's dependencies
+                (
+                    set(
+                        map(
+                            get_requirement_string_distribution_name,
+                            requirement_strings,
+                        )
                     )
+                    - set(map(normalize_name, requirement_strings))
                 ),
-                exclude_recursive=set(map(normalize_name, exclude_recursive)),
-                no_version=no_version,
-            ),
-            key=lambda name: name.lower(),
-        )
+                map(normalize_name, exclude),
+            )
+        ),
+        exclude_recursive=set(map(normalize_name, exclude_recursive)),
+        no_version=no_version,
     )
+    if dependency_order:
+        frozen_requirements = tuple(
+            _iter_sort_dependents_last(frozen_requirements)
+        )
+        if not reverse:
+            frozen_requirements = tuple(reversed(frozen_requirements))
+    else:
+        name: str
+        frozen_requirements = tuple(
+            sorted(
+                frozen_requirements,
+                key=lambda name: name.lower(),
+                reverse=reverse,
+            )
+        )
+    return frozen_requirements
 
 
 def _iter_frozen_requirements(
     requirement_strings: Iterable[str],
-    exclude: Set[str],
-    exclude_recursive: Set[str],
+    exclude: MutableSet[str],
+    exclude_recursive: MutableSet[str],
     no_version: Iterable[str] = (),
 ) -> Iterable[str]:
     def get_requirement_string(distribution_name: str) -> str:
         def distribution_name_matches_pattern(pattern: str) -> bool:
             return fnmatch(distribution_name, pattern)
 
         if (distribution_name in _DO_NOT_PIN_DISTRIBUTION_NAMES) or any(
@@ -119,40 +179,48 @@
             distribution = get_distribution(distribution_name)
         except KeyError:
             # If the distribution is missing, install it
             install_requirement(distribution_name, echo=False)
             distribution = _get_distribution(distribution_name)
         return f"{distribution.metadata['Name']}=={distribution.version}"
 
-    def get_required_distribution_names_(requirement_string: str) -> Set[str]:
+    def get_required_distribution_names_(
+        requirement_string: str,
+    ) -> MutableSet[str]:
         name: str = get_requirement_string_distribution_name(
             requirement_string
         )
         if name in exclude_recursive:
             return set()
-        return (
-            get_required_distribution_names(
-                requirement_string, exclude=exclude_recursive
+        return cast(
+            MutableSet[str],
+            (
+                set((name,))
+                | get_required_distribution_names(
+                    requirement_string, exclude=exclude_recursive
+                )
             )
-            | {name}
-        ) - exclude
+            - exclude,
+        )
 
     requirements: Iterable[str] = unique_everseen(
         chain(*map(get_required_distribution_names_, requirement_strings)),
     )
 
     requirements = map(get_requirement_string, requirements)
     return requirements
 
 
 def freeze(
     requirements: Iterable[str] = (),
     exclude: Iterable[str] = (),
     exclude_recursive: Iterable[str] = (),
     no_version: Iterable[str] = (),
+    dependency_order: bool = False,
+    reverse: bool = False,
 ) -> None:
     """
     Print the (frozen) requirements for one or more specified requirements or
     configuration files.
 
     Parameters:
 
@@ -164,22 +232,26 @@
     - exclude_recursive ([str]): One or more distributions to exclude/ignore.
       Note: Excluding a distribution here excludes all requirements which would
       be identified through recursively.
       those requirements occur elsewhere.
     - no_version ([str]) = (): Exclude version numbers from the output
       (only print distribution names) for package names matching any of these
       patterns
+    - dependency_order (bool) = False: Sort requirements so that dependents
+      precede dependencies
     """
     print(
         "\n".join(
             get_frozen_requirements(
                 requirements=requirements,
                 exclude=exclude,
                 exclude_recursive=exclude_recursive,
                 no_version=no_version,
+                dependency_order=dependency_order,
+                reverse=reverse,
             )
         )
     )
 
 
 def main() -> None:
     parser: argparse.ArgumentParser = argparse.ArgumentParser(
@@ -188,15 +260,17 @@
             "This command prints dependencies inferred from an installed "
             "distribution or project, in a similar format to the "
             "output of `pip freeze`, except that all generated requirements "
             'are specified in the format "distribution-name==0.0.0" '
             "(including for editable installations). Using this command "
             "instead of `pip freeze` to generate requirement files ensures "
             "that you don't bloat your requirements files with superfluous "
-            "distributions."
+            "distributions. The default sorting starts with directly "
+            "specified requirements, followed by recursively discovered "
+            "requirements, in the order of discovery."
         ),
     )
     parser.add_argument(
         "requirement",
         nargs="+",
         type=str,
         help=(
@@ -242,20 +316,34 @@
         action="append",
         help=(
             "Don't include versions (only output distribution names) "
             "for packages matching this/these glob pattern(s) (note: the "
             "value must be single-quoted if it contains wildcards)"
         ),
     )
+    parser.add_argument(
+        "-do",
+        "--dependency-order",
+        default=False,
+        action="store_true",
+        help="Sort requirements so that dependents precede dependencies",
+    )
+    parser.add_argument(
+        "--reverse",
+        default=False,
+        action="store_true",
+        help="Print requirements in reverse order",
+    )
     arguments: argparse.Namespace = parser.parse_args()
     freeze(
         requirements=arguments.requirement,
         exclude=tuple(iter_parse_delimited_values(arguments.exclude)),
         exclude_recursive=tuple(
             iter_parse_delimited_values(arguments.exclude_recursive)
         ),
         no_version=arguments.no_version,
+        dependency_order=arguments.dependency_order,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dependence-0.0.6/dependence/update.py` & `dependence-0.1.0/dependence/update.py`

 * *Files identical despite different names*

### Comparing `dependence-0.0.6/dependence/utilities.py` & `dependence-0.1.0/dependence/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 from typing import (
     IO,
     Any,
     Container,
     Dict,
     Iterable,
     List,
+    MutableSet,
     Optional,
-    Set,
     Tuple,
     Union,
+    cast,
 )
 from warnings import warn
 
 import tomli
 from more_itertools import unique_everseen
 from packaging.requirements import InvalidRequirement, Requirement
 from packaging.utils import canonicalize_name
@@ -631,17 +632,17 @@
 
 
 def get_required_distribution_names(
     requirement_string: str,
     exclude: Iterable[str] = (),
     recursive: bool = True,
     echo: bool = False,
-) -> Set[str]:
+) -> MutableSet[str]:
     """
-    Return a `set` of all distribution names which are required by the
+    Return a `tuple` of all distribution names which are required by the
     distribution specified in `requirement_string`.
 
     Parameters:
 
     - requirement_string (str): A distribution name, or a requirement string
       indicating both a distribution name and extras.
     - exclude ([str]): The name of one or more distributions to *exclude*
@@ -649,15 +650,15 @@
       also halt recursive lookup of requirements for that distribution.
     - recursive (bool): If `True` (the default), required distributions will
       be obtained recursively.
     - echo (bool) = False: If `True`, commands and responses executed in
       subprocesses will be printed to `sys.stdout`
     """
     if isinstance(exclude, str):
-        exclude = {normalize_name(exclude)}
+        exclude = set((normalize_name(exclude),))
     else:
         exclude = set(map(normalize_name, exclude))
     return set(
         _iter_requirement_names(
             get_requirement(requirement_string),
             exclude=exclude,
             recursive=recursive,
@@ -809,15 +810,15 @@
             )
         ) and (normalize_name(requirement.name) not in exclude):
             yield requirement
 
 
 def _iter_requirement_names(
     requirement: Requirement,
-    exclude: Set[str],
+    exclude: MutableSet[str],
     recursive: bool = True,
     echo: bool = False,
 ) -> Iterable[str]:
     name: str = normalize_name(requirement.name)
     extras: Tuple[str, ...] = tuple(requirement.extras)
     if name in exclude:
         return ()
@@ -834,24 +835,28 @@
             _iter_distribution_requirements(
                 distribution,
                 extras=extras,
                 exclude=exclude,
             ),
         )
     )
-    lateral_exclude: Set[str] = set()
+    lateral_exclude: MutableSet[str] = set()
 
     def iter_requirement_names_(
         requirement_: Requirement,
     ) -> Iterable[str]:
         return _iter_requirement_names(
             requirement_,
-            exclude=(
+            exclude=cast(
+                MutableSet[str],
                 exclude
-                | (lateral_exclude - {_get_requirement_name(requirement_)})
+                | (
+                    lateral_exclude
+                    - set((_get_requirement_name(requirement_),))
+                ),
             ),
             recursive=recursive,
             echo=echo,
         )
 
     def not_excluded(name: str) -> bool:
         if name not in exclude:
@@ -868,76 +873,81 @@
     return requirement_names
 
 
 def _iter_requirement_strings_required_distribution_names(
     requirement_strings: Iterable[str],
     echo: bool = False,
 ) -> Iterable[str]:
-    visited_requirement_strings: Set[str] = set()
+    visited_requirement_strings: MutableSet[str] = set()
     if isinstance(requirement_strings, str):
         requirement_strings = (requirement_strings,)
 
-    def get_required_distribution_names_(requirement_string: str) -> Set[str]:
+    def get_required_distribution_names_(
+        requirement_string: str,
+    ) -> MutableSet[str]:
         if requirement_string not in visited_requirement_strings:
             try:
                 name: str = get_requirement_string_distribution_name(
                     requirement_string
                 )
                 visited_requirement_strings.add(requirement_string)
-                return get_required_distribution_names(
-                    requirement_string, echo=echo
-                ) | {name}
+                return cast(
+                    MutableSet[str],
+                    set((name,))
+                    | get_required_distribution_names(
+                        requirement_string, echo=echo
+                    ),
+                )
             except KeyError:
                 pass
         return set()
 
     return unique_everseen(
         chain(*map(get_required_distribution_names_, requirement_strings)),
     )
 
 
 def get_requirements_required_distribution_names(
     requirements: Iterable[str] = (),
     echo: bool = False,
-) -> Set[str]:
+) -> MutableSet[str]:
     """
     Get the distributions required by one or more specified distributions or
     configuration files.
 
     Parameters:
 
     - requirements ([str]): One or more requirement specifiers (for example:
       "requirement-name[extra-a,extra-b]" or ".[extra-a, extra-b]) and/or paths
       to a setup.cfg, pyproject.toml, tox.ini or requirements.txt file
     """
     # Separate requirement strings from requirement files
     if isinstance(requirements, str):
-        requirements = {requirements}
+        requirements = set((requirements,))
     else:
         requirements = set(requirements)
-    requirement_files: Set[str] = set(
+    requirement_files: MutableSet[str] = set(
         filter(is_configuration_file, requirements)
     )
-    requirement_strings: Set[str] = requirements - requirement_files
+    requirement_strings: MutableSet[str] = cast(
+        MutableSet[str], requirements - requirement_files
+    )
     name: str
     return set(
-        sorted(
-            _iter_requirement_strings_required_distribution_names(
-                unique_everseen(
-                    chain(
-                        requirement_strings,
-                        *map(
-                            iter_configuration_file_requirement_strings,
-                            requirement_files,
-                        ),
-                    )
-                ),
-                echo=echo,
+        _iter_requirement_strings_required_distribution_names(
+            unique_everseen(
+                chain(
+                    requirement_strings,
+                    *map(
+                        iter_configuration_file_requirement_strings,
+                        requirement_files,
+                    ),
+                )
             ),
-            key=lambda name: name.lower(),
+            echo=echo,
         )
     )
 
 
 def iter_distribution_location_file_paths(location: str) -> Iterable[str]:
     location = os.path.abspath(location)
     name: str = get_setup_distribution_name(location)
```

### Comparing `dependence-0.0.6/dependence.egg-info/PKG-INFO` & `dependence-0.1.0/dependence.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dependence
-Version: 0.0.6
+Version: 0.1.0
 Summary: Requirement (dependency) management for python projects
 Home-page: https://github.com/enorganic/dependence
 Author-email: david@belais.me
 License: MIT
 Keywords: requirements,dependencies
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
@@ -92,44 +92,53 @@
 ```
 
 #### dependence freeze
 
 ```console
 $ dependence freeze -h
 usage: dependence freeze [-h] [-e EXCLUDE] [-er EXCLUDE_RECURSIVE]
-                           [-nv NO_VERSION]
-                           requirement [requirement ...]
+                         [-nv NO_VERSION] [-do] [--reverse]
+                         requirement [requirement ...]
 
-This command prints dependencies inferred from an installed distribution or
-project, in a similar format to the output of `pip freeze`, except that all
-generated requirements are specified in the format "distribution-
-name==0.0.0" (including for editable installations). Using this command
-instead of `pip freeze` to generate requirement files ensures that you don't
-bloat your requirements files with superfluous distributions.
+This command prints dependencies inferred from an installed
+distribution or project, in a similar format to the output of `pip
+freeze`, except that all generated requirements are specified in the
+format "distribution-name==0.0.0" (including for editable
+installations). Using this command instead of `pip freeze` to generate
+requirement files ensures that you don't bloat your requirements files
+with superfluous distributions. The default sorting starts with
+directly specified requirements, followed by recursively discovered
+requirements, in the order of discovery.
 
 positional arguments:
-  requirement           One or more requirement specifiers (for example:
-                        "requirement-name", "requirement-
-                        name[extra-a,extra-b]", ".[extra-a, extra-b]" or
-                        "../other-editable-package-directory[extra-a,
-                        extra-b]) and/or paths to a setup.py, setup.cfg,
-                        pyproject.toml, tox.ini or requirements.txt file
+  requirement           One or more requirement specifiers (for
+                        example: "requirement-name", "requirement-
+                        name[extra-a,extra-b]", ".[extra-a, extra-b]"
+                        or "../other-editable-package-
+                        directory[extra-a, extra-b]) and/or paths to a
+                        setup.py, setup.cfg, pyproject.toml, tox.ini or
+                        requirements.txt file
 
 optional arguments:
   -h, --help            show this help message and exit
   -e EXCLUDE, --exclude EXCLUDE
                         A distribution (or comma-separated list of
                         distributions) to exclude from the output
   -er EXCLUDE_RECURSIVE, --exclude-recursive EXCLUDE_RECURSIVE
                         A distribution (or comma-separated list of
-                        distributions) to exclude from the output. Unlike -e
-                        / --exclude, this argument also precludes recursive
-                        requirement discovery for the specified packages,
-                        thereby excluding all of the excluded package's
-                        requirements which are not required by another (non-
-                        excluded) distribution.
+                        distributions) to exclude from the output.
+                        Unlike -e / --exclude, this argument also
+                        precludes recursive requirement discovery for
+                        the specified packages, thereby excluding all
+                        of the excluded package's requirements which
+                        are not required by another (non-excluded)
+                        distribution.
   -nv NO_VERSION, --no-version NO_VERSION
-                        Don't include versions (only output distribution
-                        names) for packages matching this/these glob
-                        pattern(s) (note: the value must be single-quoted if
-                        it contains wildcards)
+                        Don't include versions (only output
+                        distribution names) for packages matching
+                        this/these glob pattern(s) (note: the value
+                        must be single-quoted if it contains wildcards)
+  -do, --dependency-order
+                        Sort requirements so that dependents precede
+                        dependencies
+  --reverse             Print requirements in reverse order
 ```
```

### Comparing `dependence-0.0.6/setup.cfg` & `dependence-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dependence
-version = 0.0.6
+version = 0.1.0
 author_email = david@belais.me
 description = Requirement (dependency) management for python projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = 
 	requirements
 	dependencies
```

### Comparing `dependence-0.0.6/tests/test_requirements_update.py` & `dependence-0.1.0/tests/test_update.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import unittest
 from collections import deque
 from configparser import ConfigParser
 from pathlib import Path
 from typing import Iterable
 
+import pytest
 import tomli
 from packaging.requirements import Requirement
 from packaging.specifiers import Specifier
 from packaging.version import Version
 
 from dependence.update import (
     get_updated_pyproject_toml,
@@ -70,138 +70,125 @@
 
 def validate_requirements(requirements: Iterable[str]) -> None:
     if isinstance(requirements, str):
         requirements = requirements.split("\n")
     list(map(validate_requirement, requirements))
 
 
-class TestRequirementsUpdate(unittest.TestCase):
+def test_get_updated_setup_cfg() -> None:
     """
-    This test case validates functionality for
-    `requirements.update`
+    Ensure that updating a setup.cfg file occurs without problems
     """
+    setup_cfg_path: Path = TEST_PROJECT_A.joinpath("setup.cfg")
+    updated_setup_cfg_data: str
+    with open(setup_cfg_path) as setup_cfg_io:
+        setup_cfg_data: str = setup_cfg_io.read()
+        # Update versions for all packages *except* pip
+        print(setup_cfg_data)
+        updated_setup_cfg_data = get_updated_setup_cfg(
+            setup_cfg_data,
+            ignore=("pip", "setuptools"),
+            all_extra_name="all",
+        )
+        print(
+            f"{str(setup_cfg_path).strip()}\n\n"
+            "Before:\n\n"
+            f"{setup_cfg_data.strip()}\n\n"
+            "After:\n\n"
+            f"{updated_setup_cfg_data.strip()}\n"
+        )
+        assert updated_setup_cfg_data != setup_cfg_data
+    # Ensure all versions are updated to a non-zero release number
+    parser: ConfigParser = ConfigParser()
+    parser.read_string(updated_setup_cfg_data)
+    validate_requirements(parser["options"]["install_requires"])
+    extra_requirements_string: str
+    for extra_requirements_string in parser["options.extras_require"].values():
+        validate_requirements(extra_requirements_string)
 
-    def test_get_updated_setup_cfg(self) -> None:
-        """
-        Ensure that updating a setup.cfg file occurs without problems
-        """
-        setup_cfg_path: Path = TEST_PROJECT_A.joinpath("setup.cfg")
-        updated_setup_cfg_data: str
-        with open(setup_cfg_path) as setup_cfg_io:
-            setup_cfg_data: str = setup_cfg_io.read()
-            # Update versions for all packages *except* pip
-            print(setup_cfg_data)
-            updated_setup_cfg_data = get_updated_setup_cfg(
-                setup_cfg_data,
-                ignore=("pip", "setuptools"),
-                all_extra_name="all",
-            )
-            print(
-                f"{str(setup_cfg_path).strip()}\n\n"
-                "Before:\n\n"
-                f"{setup_cfg_data.strip()}\n\n"
-                "After:\n\n"
-                f"{updated_setup_cfg_data.strip()}\n"
-            )
-            assert updated_setup_cfg_data != setup_cfg_data
-        # Ensure all versions are updated to a non-zero release number
-        parser: ConfigParser = ConfigParser()
-        parser.read_string(updated_setup_cfg_data)
-        validate_requirements(parser["options"]["install_requires"])
-        extra_requirements_string: str
-        for extra_requirements_string in parser[
-            "options.extras_require"
-        ].values():
-            validate_requirements(extra_requirements_string)
-
-    def test_get_updated_pyproject_toml_a(self) -> None:
-        """
-        Ensure that updating a pyproject.toml file occurs without problems
-        """
-        pyproject_toml_path: Path = TEST_PROJECT_A.joinpath("pyproject.toml")
-        updated_pyproject_toml_data: str
-        with open(pyproject_toml_path) as pyproject_toml_io:
-            pyproject_toml_data: str = pyproject_toml_io.read()
-            # Update versions for all packages *except* pip
-            updated_pyproject_toml_data = get_updated_pyproject_toml(
-                pyproject_toml_data,
-                ignore=("pip", "setuptools"),
-            )
-            print(
-                f"{str(pyproject_toml_path).strip()}\n\n"
-                "Before:\n\n"
-                f"{pyproject_toml_data.strip()}\n\n"
-                "After:\n\n"
-                f"{updated_pyproject_toml_data.strip()}\n"
-            )
-            assert updated_pyproject_toml_data != pyproject_toml_data
-        # Ensure all versions are updated to a non-zero release number
-        validate_requirements(
-            tomli.loads(updated_pyproject_toml_data)["build-system"][
-                "requires"
-            ]
-        )
-
-    def test_get_updated_pyproject_toml_b(self) -> None:
-        """
-        Ensure that updating a pyproject.toml file occurs without problems
-        """
-        pyproject_toml_path: Path = TEST_PROJECT_B.joinpath("pyproject.toml")
-        updated_pyproject_toml_data: str
-        with open(pyproject_toml_path) as pyproject_toml_io:
-            pyproject_toml_data: str = pyproject_toml_io.read()
-            # Update versions for all packages *except* pip
-            updated_pyproject_toml_data = get_updated_pyproject_toml(
-                pyproject_toml_data,
-                ignore=("pip", "setuptools"),
+
+def test_get_updated_pyproject_toml_a() -> None:
+    """
+    Ensure that updating a pyproject.toml file occurs without problems
+    """
+    pyproject_toml_path: Path = TEST_PROJECT_A.joinpath("pyproject.toml")
+    updated_pyproject_toml_data: str
+    with open(pyproject_toml_path) as pyproject_toml_io:
+        pyproject_toml_data: str = pyproject_toml_io.read()
+        # Update versions for all packages *except* pip
+        updated_pyproject_toml_data = get_updated_pyproject_toml(
+            pyproject_toml_data,
+            ignore=("pip", "setuptools"),
+        )
+        print(
+            f"{str(pyproject_toml_path).strip()}\n\n"
+            "Before:\n\n"
+            f"{pyproject_toml_data.strip()}\n\n"
+            "After:\n\n"
+            f"{updated_pyproject_toml_data.strip()}\n"
+        )
+        assert updated_pyproject_toml_data != pyproject_toml_data
+    # Ensure all versions are updated to a non-zero release number
+    validate_requirements(
+        tomli.loads(updated_pyproject_toml_data)["build-system"]["requires"]
+    )
+
+
+def test_get_updated_pyproject_toml_b() -> None:
+    """
+    Ensure that updating a pyproject.toml file occurs without problems
+    """
+    pyproject_toml_path: Path = TEST_PROJECT_B.joinpath("pyproject.toml")
+    updated_pyproject_toml_data: str
+    with open(pyproject_toml_path) as pyproject_toml_io:
+        pyproject_toml_data: str = pyproject_toml_io.read()
+        # Update versions for all packages *except* pip
+        updated_pyproject_toml_data = get_updated_pyproject_toml(
+            pyproject_toml_data,
+            ignore=("pip", "setuptools"),
+        )
+        print(
+            f"{str(pyproject_toml_path).strip()}\n\n"
+            "Before:\n\n"
+            f"{pyproject_toml_data.strip()}\n\n"
+            "After:\n\n"
+            f"{updated_pyproject_toml_data.strip()}\n"
+        )
+        assert updated_pyproject_toml_data != pyproject_toml_data
+    # Ensure all versions are updated to a non-zero release number
+    validate_requirements(
+        tomli.loads(updated_pyproject_toml_data)["build-system"]["requires"]
+        + tomli.loads(updated_pyproject_toml_data)["project"]["dependencies"]
+        + tomli.loads(updated_pyproject_toml_data)["project"][
+            "optional-dependencies"
+        ]["twine"]
+        + tomli.loads(updated_pyproject_toml_data)["project"][
+            "optional-dependencies"
+        ]["wheel"]
+    )
+
+
+def test_get_updated_requirements_txt() -> None:
+    """
+    Ensure that updating a setup.cfg file occurs without problems
+    """
+    project: Path
+    for project in (TEST_PROJECT_A, TEST_PROJECT_B):
+        requirements_txt_path: Path = project.joinpath("requirements.txt")
+        with open(requirements_txt_path) as requirements_txt_io:
+            requirements_txt_data: str = requirements_txt_io.read()
+            updated_requirements_txt_data: str = get_updated_requirements_txt(
+                requirements_txt_data, ignore=("pip", "setuptools")
             )
             print(
-                f"{str(pyproject_toml_path).strip()}\n\n"
+                f"{str(requirements_txt_path).strip()}\n\n"
                 "Before:\n\n"
-                f"{pyproject_toml_data.strip()}\n\n"
+                f"{requirements_txt_data.strip()}\n\n"
                 "After:\n\n"
-                f"{updated_pyproject_toml_data.strip()}\n"
+                f"{updated_requirements_txt_data.strip()}\n"
             )
-            assert updated_pyproject_toml_data != pyproject_toml_data
-        # Ensure all versions are updated to a non-zero release number
-        validate_requirements(
-            tomli.loads(updated_pyproject_toml_data)["build-system"][
-                "requires"
-            ]
-            + tomli.loads(updated_pyproject_toml_data)["project"][
-                "dependencies"
-            ]
-            + tomli.loads(updated_pyproject_toml_data)["project"][
-                "optional-dependencies"
-            ]["twine"]
-            + tomli.loads(updated_pyproject_toml_data)["project"][
-                "optional-dependencies"
-            ]["wheel"]
-        )
-
-    def test_get_updated_requirements_txt(self) -> None:
-        """
-        Ensure that updating a setup.cfg file occurs without problems
-        """
-        project: Path
-        for project in (TEST_PROJECT_A, TEST_PROJECT_B):
-            requirements_txt_path: Path = project.joinpath("requirements.txt")
-            with open(requirements_txt_path) as requirements_txt_io:
-                requirements_txt_data: str = requirements_txt_io.read()
-                updated_requirements_txt_data: str = (
-                    get_updated_requirements_txt(
-                        requirements_txt_data, ignore=("pip", "setuptools")
-                    )
-                )
-                print(
-                    f"{str(requirements_txt_path).strip()}\n\n"
-                    "Before:\n\n"
-                    f"{requirements_txt_data.strip()}\n\n"
-                    "After:\n\n"
-                    f"{updated_requirements_txt_data.strip()}\n"
-                )
-                assert updated_requirements_txt_data != requirements_txt_data
-                validate_requirements(updated_requirements_txt_data)
+            assert updated_requirements_txt_data != requirements_txt_data
+            validate_requirements(updated_requirements_txt_data)
 
 
 if __name__ == "__main__":
-    unittest.main()
+    pytest.main()
```

