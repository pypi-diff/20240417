# Comparing `tmp/pydal2sql_core-0.3.5.tar.gz` & `tmp/pydal2sql_core-0.3.6.tar.gz`

## Comparing `pydal2sql_core-0.3.5.tar` & `pydal2sql_core-0.3.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/coverage.svg
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/.github/workflows/su6.yml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/examples/alter.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/examples/examples.sh
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/examples/magic.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/examples/settings_in_code.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/examples/settings_via_cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
--rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
--rw-r--r--   0        0        0    66916 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_cli_old_py.html
--rw-r--r--   0        0        0    71509 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
--rw-r--r--   0        0        0   104236 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_cli_support_py.html
--rw-r--r--   0        0        0    57024 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
--rw-r--r--   0        0        0    27846 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
--rw-r--r--   0        0        0    93519 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html
--rw-r--r--   0        0        0    96080 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_typer_support_py.html
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660___about___py.html
--rw-r--r--   0        0        0     9361 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660___init___py.html
--rw-r--r--   0        0        0   271713 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660_cli_support_py.html
--rw-r--r--   0        0        0    73018 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660_core_py.html
--rw-r--r--   0        0        0    33315 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660_helpers_py.html
--rw-r--r--   0        0        0    93963 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660_magic_py.html
--rw-r--r--   0        0        0    31174 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660_types_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/htmlcov/style.css
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/pytest_examples/common.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/pytest_examples/magic_post.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/pytest_examples/magic_pre.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/pytest_examples/magic_with_function.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/pytest_examples/magic_with_import.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/pytest_examples/pydal_before.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/pytest_examples/some_config.toml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/pytest_examples/typedal_after.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/src/pydal2sql_core/__about__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/src/pydal2sql_core/__init__.py
--rw-r--r--   0        0        0    37098 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/src/pydal2sql_core/cli_support.py
--rw-r--r--   0        0        0    10394 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/src/pydal2sql_core/core.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/src/pydal2sql_core/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/src/pydal2sql_core/py.typed
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/src/pydal2sql_core/types.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/tests/__init__.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/tests/mock_git.py
--rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/tests/test_cli_support.py
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/tests/test_core.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/tests/test_helpers.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/LICENSE.txt
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/README.md
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/coverage.svg
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/.github/workflows/su6.yml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/examples/alter.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/examples/examples.sh
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/examples/magic.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/examples/settings_in_code.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/examples/settings_via_cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
+-rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
+-rw-r--r--   0        0        0    66916 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_cli_old_py.html
+-rw-r--r--   0        0        0    71509 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
+-rw-r--r--   0        0        0   104236 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_cli_support_py.html
+-rw-r--r--   0        0        0    57024 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
+-rw-r--r--   0        0        0    27846 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
+-rw-r--r--   0        0        0    93519 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html
+-rw-r--r--   0        0        0    96080 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_typer_support_py.html
+-rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660___about___py.html
+-rw-r--r--   0        0        0     9361 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660___init___py.html
+-rw-r--r--   0        0        0   271713 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_cli_support_py.html
+-rw-r--r--   0        0        0    73018 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_core_py.html
+-rw-r--r--   0        0        0    33315 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_helpers_py.html
+-rw-r--r--   0        0        0    93963 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_magic_py.html
+-rw-r--r--   0        0        0    31174 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_types_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/style.css
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/common.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/magic_post.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/magic_pre.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/magic_with_function.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/magic_with_import.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/pydal_before.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/some_config.toml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/typedal_after.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/__about__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/__init__.py
+-rw-r--r--   0        0        0    37107 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/cli_support.py
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/core.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/py.typed
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/types.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/tests/__init__.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/tests/mock_git.py
+-rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/tests/test_cli_support.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/tests/test_core.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/tests/test_helpers.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/LICENSE.txt
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/README.md
+-rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/PKG-INFO
```

### Comparing `pydal2sql_core-0.3.5/CHANGELOG.md` & `pydal2sql_core-0.3.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.6 (2024-04-17)
+
+### Fix
+
+* If 'default=' is a callable, it's result is NOT stored in the CREATE statement ([`3548347`](https://github.com/robinvandernoord/pydal2sql-core/commit/35483479c63986110e69dfd61a7d75ede15262be))
+
 ## v0.3.5 (2024-03-20)
 
 ### Fix
 
 * Require 'black' as a dependency ([`3cf51d3`](https://github.com/robinvandernoord/pydal2sql-core/commit/3cf51d3894e90ddd5ea6677c4fdb70a1b03a364b))
 
 ## v0.3.4 (2023-12-05)
```

### Comparing `pydal2sql_core-0.3.5/coverage.svg` & `pydal2sql_core-0.3.6/coverage.svg`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/examples/alter.py` & `pydal2sql_core-0.3.6/examples/alter.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/coverage_html.js` & `pydal2sql_core-0.3.6/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74___about___py.html` & `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74___about___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74___init___py.html` & `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74___init___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_cli_old_py.html` & `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_cli_old_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html` & `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_cli_support_py.html` & `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_cli_support_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_core_py.html` & `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_core_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html` & `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html` & `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_typer_support_py.html` & `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_typer_support_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_8bc7b9c2c0d01e74_types_py.html` & `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_types_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660___about___py.html` & `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660___about___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660___init___py.html` & `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660___init___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660_cli_support_py.html` & `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_cli_support_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660_core_py.html` & `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_core_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660_helpers_py.html` & `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_helpers_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660_magic_py.html` & `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_magic_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/d_ed2881eaa6b25660_types_py.html` & `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_types_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/favicon_32.png` & `pydal2sql_core-0.3.6/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/index.html` & `pydal2sql_core-0.3.6/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/keybd_closed.png` & `pydal2sql_core-0.3.6/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/keybd_open.png` & `pydal2sql_core-0.3.6/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/status.json` & `pydal2sql_core-0.3.6/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/htmlcov/style.css` & `pydal2sql_core-0.3.6/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/pytest_examples/pydal_before.py` & `pydal2sql_core-0.3.6/pytest_examples/pydal_before.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/pytest_examples/typedal_after.py` & `pydal2sql_core-0.3.6/pytest_examples/typedal_after.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/src/pydal2sql_core/__init__.py` & `pydal2sql_core-0.3.6/src/pydal2sql_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/src/pydal2sql_core/cli_support.py` & `pydal2sql_core-0.3.6/src/pydal2sql_core/cli_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 CLI-Agnostic support.
 """
+
 import contextlib
 import io
 import os
 import re
 import select
 import string
 import sys
@@ -289,17 +290,17 @@
 
     Returns:
         tuple[tuple[str, str | None], tuple[str, str | None]]:
             A tuple of two tuples, each containing the version and path of the before and after files.
     """
     version_before, filepath_before = extract_file_version_and_path(
         filename_before,
-        default_version="current"
-        if filename_after and filename_before and filename_after != filename_before
-        else "latest",
+        default_version=(
+            "current" if filename_after and filename_before and filename_after != filename_before else "latest"
+        ),
     )
     version_after, filepath_after = extract_file_version_and_path(filename_after, default_version="current")
 
     if not (filepath_before or filepath_after):
         raise ValueError("Please supply at least one file name.")
     elif not filepath_after:
         filepath_after = filepath_before
```

### Comparing `pydal2sql_core-0.3.5/src/pydal2sql_core/core.py` & `pydal2sql_core-0.3.6/src/pydal2sql_core/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,90 @@
 """
 Main functionality.
 """
+
+import functools
 import pickle  # nosec: B403
 import typing
 from pathlib import Path
 from typing import Any
 
 from pydal.adapters import MySQL, Postgre, SQLite
-from pydal.dialects import Dialect, MySQLDialect, PostgreDialect, SQLiteDialect
+from pydal.dialects import (
+    Dialect,
+    MySQLDialect,
+    PostgreDialect,
+    SQLDialect,
+    SQLiteDialect,
+)
 from pydal.migrator import Migrator
 from pydal.objects import Table
 
 from .helpers import TempdirOrExistingDir, get_typing_args
 from .types import (
     SUPPORTED_DATABASE_TYPES,
     SUPPORTED_DATABASE_TYPES_WITH_ALIASES,
     CustomAdapter,
     DummyDAL,
     SQLAdapter,
 )
 
 
+def sql_not_null(self: SQLDialect, default: Any, field_type: Any) -> str:
+    """
+    Generate a SQL NOT NULL constraint for a field.
+
+    If the default value of the field is callable (e.g., a function like uuid.uuid, datetime.now or a lambda),
+    the function returns "NOT NULL". Otherwise, it returns "NOT NULL DEFAULT %s" where %s is the
+    representation of the default value in SQL.
+
+    Args:
+        self (SQLDialect): The SQL dialect to use.
+        default (Any): The default value of the field.
+        field_type (Any): The type of the field.
+
+    Returns:
+        str: A string representing the SQL NOT NULL constraint for the field.
+    """
+    # default:
+    # if field.notnull and field.default is not None:
+    # return "NOT NULL DEFAULT %s" % self.adapter.represent(default, field_type)
+    # but if 'default' is not a static value (-> callable),
+    # it should not be hardcoded in the migration statement (e.g. default=uuid.uuid, datetime.now etc.)
+    if callable(default):
+        return "NOT NULL"
+    else:
+        return "NOT NULL DEFAULT %s" % self.adapter.represent(default, field_type)
+
+
+def _modify_migrator(self: Migrator) -> Migrator:
+    """
+    Modify the SQL NOT NULL constraint logic of a Migrator object.
+
+    If the Migrator's SQL dialect uses the base SQL NOT NULL logic, this function replaces it with
+    the logic defined in the sql_not_null function. Otherwise, it leaves the Migrator unchanged.
+
+    Args:
+        self (Migrator): The Migrator object to modify.
+
+    Returns:
+        Migrator: The modified Migrator object.
+    """
+    # __func__ to get the function underneath a bound method:
+    if self.adapter.dialect.not_null.__func__ == SQLDialect.not_null:
+        # only modify base SQL notnull.
+        # if dialect has modified logic, that should just be used.
+        # bind 'self' parameter already:
+        bound_method = functools.partial(sql_not_null, self.adapter.dialect)
+        # monkey patch default logic:
+        self.adapter.dialect.not_null = bound_method
+
+    return self
+
+
 def _build_dummy_migrator(_driver_name: SUPPORTED_DATABASE_TYPES_WITH_ALIASES, /, db_folder: str) -> Migrator:
     """
     Create a Migrator specific to the sql dialect of _driver_name.
     """
     db = DummyDAL(None, migrate=False, folder=db_folder)
 
     aliases = {
@@ -74,15 +134,17 @@
         commit_on_alter_table = True
 
     adapter = DummyAdapter(db, "", adapter_args={"driver": installed_driver})
 
     adapter.dialect = sql_dialect(adapter)
     db._adapter = adapter
 
-    return Migrator(adapter)
+    dummy_migrator = Migrator(adapter)
+
+    return _modify_migrator(dummy_migrator)
 
 
 def generate_create_statement(
     define_table: Table, db_type: SUPPORTED_DATABASE_TYPES_WITH_ALIASES = None, *, db_folder: str = None
 ) -> str:
     """
     Given a Table object (result of `db.define_table('mytable')` or simply db.mytable) \
```

### Comparing `pydal2sql_core-0.3.5/src/pydal2sql_core/helpers.py` & `pydal2sql_core-0.3.6/src/pydal2sql_core/helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/src/pydal2sql_core/types.py` & `pydal2sql_core-0.3.6/src/pydal2sql_core/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains types for core.py.
 """
+
 import typing
 import warnings
 from typing import Any
 
 import pydal
 from pydal.adapters import SQLAdapter as _SQLAdapter
 from witchery import Empty
```

### Comparing `pydal2sql_core-0.3.5/tests/mock_git.py` & `pydal2sql_core-0.3.6/tests/mock_git.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/tests/test_cli_support.py` & `pydal2sql_core-0.3.6/tests/test_cli_support.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/tests/test_core.py` & `pydal2sql_core-0.3.6/tests/test_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     db.define_table(
         "person",
         Field(
             "name",
             "string",
             notnull=True,
         ),
-        Field("age", "integer", default=18),
+        Field("age", "integer", default=18, notnull=True),
         Field("float", "decimal(2,3)"),
         Field("nicknames", "list:string"),
-        Field("obj", "json"),
+        Field("obj", "json", notnull=True, default=lambda: ["exclude from default"]),
     )
 
     generated = {}
 
     with pytest.raises(ValueError):
         # db type can't be guessed if the db connection string is None and db_type is also None:
         generate_sql(db.person, db_type=None)
@@ -49,14 +49,18 @@
         assert "name" in sql
         assert "CHAR" in sql
 
         text_type = "LONGTEXT" if database_type == "pymysql" else "TEXT"
 
         assert f"nicknames {text_type}" in sql
         assert "age INTEGER" in sql
+        assert "18" in sql  # notnull default
+
+        assert "obj" in sql
+        assert "exclude from default" not in sql  # notnull lambda default
 
     # sqlite
     print(generated["sqlite3"])
 
     # psql
     print(generated["psycopg2"])
```

### Comparing `pydal2sql_core-0.3.5/tests/test_helpers.py` & `pydal2sql_core-0.3.6/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/LICENSE.txt` & `pydal2sql_core-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/README.md` & `pydal2sql_core-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/pyproject.toml` & `pydal2sql_core-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.5/PKG-INFO` & `pydal2sql_core-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal2sql-core
-Version: 0.3.5
+Version: 0.3.6
 Summary: CLI-agnostic pydal2sql code; Convert pydal define_tables to SQL using pydal's CREATE TABLE logic.
 Project-URL: Documentation, https://github.com/robinvandernoord/pydal2sql-core#readme
 Project-URL: Issues, https://github.com/robinvandernoord/pydal2sql-core/issues
 Project-URL: Source, https://github.com/robinvandernoord/pydal2sql-core
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

