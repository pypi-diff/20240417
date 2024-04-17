# Comparing `tmp/autodoc_traits-1.2.1.tar.gz` & `tmp/autodoc_traits-1.2.2.tar.gz`

## Comparing `autodoc_traits-1.2.1.tar` & `autodoc_traits-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/.flake8
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/CHANGELOG.md
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/MANIFEST.in
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/RELEASE.md
--rw-r--r--   0        0        0    10849 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/autodoc_traits.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/.github/dependabot.yaml
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/README.md
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/conftest.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/test_autodoc_traits.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/test_fixtures.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/sample_module.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/conf.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/index.rst
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/autoclass/members.rst
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/autoclass/undoc_members.rst
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/autoconfigurable/exclude_members.rst
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/autoconfigurable/inherited_members.rst
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/autoconfigurable/members.rst
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/autoconfigurable/no_members.rst
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/autoconfigurable/non_configurable_raises_error.rst
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/autoconfigurable/specified_members.rst
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/automodule/members.rst
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/autotrait/help.rst
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/autotrait/noconfig.rst
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/autotrait/nohelp.rst
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/tests/docs/source/autotrait/non_trait_raises_error.rst
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/LICENSE
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/README.md
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 autodoc_traits-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/.flake8
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8674 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/MANIFEST.in
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/RELEASE.md
+-rw-r--r--   0        0        0    10849 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/autodoc_traits.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/.github/dependabot.yaml
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/README.md
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/conftest.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/test_autodoc_traits.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/test_fixtures.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/sample_module.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/conf.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/index.rst
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/autoclass/members.rst
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/autoclass/undoc_members.rst
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/autoconfigurable/exclude_members.rst
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/autoconfigurable/inherited_members.rst
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/autoconfigurable/members.rst
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/autoconfigurable/no_members.rst
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/autoconfigurable/non_configurable_raises_error.rst
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/autoconfigurable/specified_members.rst
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/automodule/members.rst
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/autotrait/help.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/autotrait/noconfig.rst
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/autotrait/nohelp.rst
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/tests/docs/source/autotrait/non_trait_raises_error.rst
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/LICENSE
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/README.md
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 autodoc_traits-1.2.2/PKG-INFO
```

### Comparing `autodoc_traits-1.2.1/.pre-commit-config.yaml` & `autodoc_traits-1.2.2/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -7,58 +7,58 @@
 #
 # - Run on all files:   pre-commit run --all-files
 # - Register git hooks: pre-commit install --install-hooks
 #
 repos:
   # Autoformat: Python code, syntax patterns are modernized
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.10.1
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
         args:
           - --py37-plus
 
   # Autoformat: Python code
   - repo: https://github.com/PyCQA/autoflake
-    rev: v2.2.1
+    rev: v2.3.1
     hooks:
       - id: autoflake
         # args ref: https://github.com/PyCQA/autoflake#advanced-usage
         args:
           - --in-place
 
   # Autoformat: Python code
   - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
       - id: isort
 
   # Autoformat: Python code
   - repo: https://github.com/psf/black
-    rev: 23.7.0
+    rev: 24.3.0
     hooks:
       - id: black
 
   # Autoformat: markdown, yaml
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.3
+    rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
 
   # Autoformat and linting, misc. details
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
       - id: end-of-file-fixer
       - id: requirements-txt-fixer
       - id: check-case-conflict
       - id: check-executables-have-shebangs
 
   # Linting: Python code (see the file .flake8)
   - repo: https://github.com/PyCQA/flake8
-    rev: "6.1.0"
+    rev: "7.0.0"
     hooks:
       - id: flake8
 
 # pre-commit.ci config reference: https://pre-commit.ci/#configuration
 ci:
   autoupdate_schedule: monthly
```

### Comparing `autodoc_traits-1.2.1/CHANGELOG.md` & `autodoc_traits-1.2.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # Changes in autodoc-traits
 
 ## 1.2
 
+### 1.2.2 - 2024-04-17
+
+([full changelog](https://github.com/jupyterhub/autodoc-traits/compare/1.2.1...1.2.2))
+
+#### Maintenance and upkeep improvements
+
+- Remove no longer needed upper bound pin on traitlets [#64](https://github.com/jupyterhub/autodoc-traits/pull/64) ([@consideRatio](https://github.com/consideRatio))
+
+#### Continuous integration improvements
+
+- build(deps): bump actions/setup-python from 4 to 5 [#61](https://github.com/jupyterhub/autodoc-traits/pull/61) ([@consideRatio](https://github.com/consideRatio))
+- build(deps): bump actions/checkout from 3 to 4 [#57](https://github.com/jupyterhub/autodoc-traits/pull/57) ([@consideRatio](https://github.com/consideRatio))
+
 ### 1.2.1 - 2023-09-27
 
 ([full changelog](https://github.com/jupyterhub/autodoc-traits/compare/1.2.0...1.2.1))
 
 #### Maintenance and upkeep improvements
 
 - Bound `traitlets<5.10` and add test for issue observed in newer versions [#54](https://github.com/jupyterhub/autodoc-traits/pull/54) ([@consideRatio](https://github.com/consideRatio), [@manics](https://github.com/manics))
```

### Comparing `autodoc_traits-1.2.1/RELEASE.md` & `autodoc_traits-1.2.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/autodoc_traits.py` & `autodoc_traits-1.2.2/autodoc_traits.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from sphinx.ext.autodoc import AttributeDocumenter, ClassDocumenter, ObjectMember
 from sphinx.util.inspect import safe_getattr
 from traitlets import MetaHasTraits, TraitType, Undefined
 
 # __version__ should be updated using tbump, based on configuration in
 # pyproject.toml, according to instructions in RELEASE.md.
 #
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 
 class ConfigurableDocumenter(ClassDocumenter):
     """
     Specialized Documenter subclass for traits with config=True
 
     Links to relevant source code in sphinx.ext.autodoc:
```

### Comparing `autodoc_traits-1.2.1/.github/dependabot.yaml` & `autodoc_traits-1.2.2/.github/dependabot.yaml`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/.github/workflows/release.yaml` & `autodoc_traits-1.2.2/.github/workflows/release.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
       - "**"
   workflow_dispatch:
 
 jobs:
   build-release:
     runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - name: install build package
         run: |
           pip install --upgrade pip
           pip install build
```

### Comparing `autodoc_traits-1.2.1/tests/README.md` & `autodoc_traits-1.2.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/tests/conftest.py` & `autodoc_traits-1.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/tests/test_autodoc_traits.py` & `autodoc_traits-1.2.2/tests/test_autodoc_traits.py`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/tests/test_fixtures.py` & `autodoc_traits-1.2.2/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/tests/docs/sample_module.py` & `autodoc_traits-1.2.2/tests/docs/sample_module.py`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/tests/docs/source/conf.py` & `autodoc_traits-1.2.2/tests/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/tests/docs/source/autoconfigurable/exclude_members.rst` & `autodoc_traits-1.2.2/tests/docs/source/autoconfigurable/exclude_members.rst`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/tests/docs/source/autoconfigurable/specified_members.rst` & `autodoc_traits-1.2.2/tests/docs/source/autoconfigurable/specified_members.rst`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/tests/docs/source/autotrait/help.rst` & `autodoc_traits-1.2.2/tests/docs/source/autotrait/help.rst`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/.gitignore` & `autodoc_traits-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/LICENSE` & `autodoc_traits-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/README.md` & `autodoc_traits-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `autodoc_traits-1.2.1/pyproject.toml` & `autodoc_traits-1.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 dynamic = ["version"]
 requires-python = ">=3.7"
 dependencies = [
     "sphinx>=4",
-    # FIXME: traitlets are upper bounded as a workaround to
-    #        https://github.com/jupyterhub/autodoc-traits/issues/55
-    "traitlets>=4,<5.10",
+    "traitlets>=4",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
 ]
 
@@ -95,15 +93,15 @@
 
 # tbump is used to simplify and standardize the release process when updating
 # the version, making a git commit and tag, and pushing changes.
 #
 # ref: https://github.com/your-tools/tbump#readme
 #
 [tool.tbump.version]
-current = "1.2.1"
+current = "1.2.2"
 
 # Example of a pep440 regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `autodoc_traits-1.2.1/PKG-INFO` & `autodoc_traits-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: autodoc-traits
-Version: 1.2.1
+Version: 1.2.2
 Summary: Sphinx extension to autodoc traitlets
 Project-URL: Documentation, https://github.com/jupyterhub/autodoc-traits#readme
 Project-URL: Issues, https://github.com/jupyterhub/autodoc-traits/issues
 Project-URL: Source, https://github.com/jupyterhub/autodoc-traits
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -38,15 +38,15 @@
 License-File: LICENSE
 Keywords: autodoc,extension,sphinx,traitlets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: sphinx>=4
-Requires-Dist: traitlets<5.10,>=4
+Requires-Dist: traitlets>=4
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 # autodoc-traits
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/autodoc-traits?logo=pypi)](https://pypi.python.org/pypi/autodoc-traits)
```

