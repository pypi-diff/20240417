# Comparing `tmp/pydal2sql-1.1.3.tar.gz` & `tmp/pydal2sql-1.1.4.tar.gz`

## Comparing `pydal2sql-1.1.3.tar` & `pydal2sql-1.1.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/coverage.svg
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/example-pydal.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/example-typedal.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/.github/workflows/su6.yml
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/examples/alter.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/examples/examples.sh
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/examples/magic.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/examples/settings_in_code.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/examples/settings_via_cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
--rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
--rw-r--r--   0        0        0    66916 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_cli_old_py.html
--rw-r--r--   0        0        0    65014 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
--rw-r--r--   0        0        0   104236 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_cli_support_py.html
--rw-r--r--   0        0        0    57024 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
--rw-r--r--   0        0        0    27846 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
--rw-r--r--   0        0        0    93519 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html
--rw-r--r--   0        0        0    95939 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_typer_support_py.html
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/htmlcov/style.css
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/pytest_examples/common.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/pytest_examples/magic_post.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/pytest_examples/magic_pre.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/pytest_examples/magic_with_function.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/pytest_examples/magic_with_import.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/pytest_examples/some_config.toml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/src/pydal2sql/__about__.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/src/pydal2sql/__init__.py
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/src/pydal2sql/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/src/pydal2sql/py.typed
--rw-r--r--   0        0        0    12251 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/src/pydal2sql/typer_support.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/src/pydal2sql/types.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/tests/__init__.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/tests/mock_git.py
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/tests/test_cli.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/tests/test_typer_support.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/LICENSE.txt
--rw-r--r--   0        0        0     7354 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/README.md
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     8964 2020-02-02 00:00:00.000000 pydal2sql-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/coverage.svg
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/example-pydal.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/example-typedal.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/.github/workflows/su6.yml
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/examples/alter.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/examples/examples.sh
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/examples/magic.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/examples/settings_in_code.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/examples/settings_via_cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
+-rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
+-rw-r--r--   0        0        0    66916 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_cli_old_py.html
+-rw-r--r--   0        0        0    65014 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
+-rw-r--r--   0        0        0   104236 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_cli_support_py.html
+-rw-r--r--   0        0        0    57024 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
+-rw-r--r--   0        0        0    27846 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
+-rw-r--r--   0        0        0    93519 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html
+-rw-r--r--   0        0        0    95939 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_typer_support_py.html
+-rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/htmlcov/style.css
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/pytest_examples/common.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/pytest_examples/magic_post.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/pytest_examples/magic_pre.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/pytest_examples/magic_with_function.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/pytest_examples/magic_with_import.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/pytest_examples/some_config.toml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/src/pydal2sql/__about__.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/src/pydal2sql/__init__.py
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/src/pydal2sql/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/src/pydal2sql/py.typed
+-rw-r--r--   0        0        0    12251 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/src/pydal2sql/typer_support.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/src/pydal2sql/types.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/tests/mock_git.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/tests/test_cli.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/tests/test_typer_support.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     7354 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/README.md
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     8964 2020-02-02 00:00:00.000000 pydal2sql-1.1.4/PKG-INFO
```

### Comparing `pydal2sql-1.1.3/CHANGELOG.md` & `pydal2sql-1.1.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.1.4 (2024-04-17)
+
+### Fix
+
+* **bump-core:** If 'default=' is a callable, it's result is NOT stored in the CREATE statement ([`cdc28ee`](https://github.com/robinvandernoord/pydal2sql/commit/cdc28ee408458e5b71ce5fa716cf131756eb921b))
+
 ## v1.1.3 (2024-03-20)
 
 ### Fix
 
 * Bump pydal2sql-core ([`972cf36`](https://github.com/robinvandernoord/pydal2sql/commit/972cf36bccd8323aff5d9e336fbcfd3037fdc4a8))
 
 ## v1.1.2 (2023-12-04)
```

### Comparing `pydal2sql-1.1.3/coverage.svg` & `pydal2sql-1.1.4/coverage.svg`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/example-pydal.py` & `pydal2sql-1.1.4/example-pydal.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/example-typedal.py` & `pydal2sql-1.1.4/example-typedal.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/examples/alter.py` & `pydal2sql-1.1.4/examples/alter.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/coverage_html.js` & `pydal2sql-1.1.4/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74___about___py.html` & `pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74___about___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74___init___py.html` & `pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74___init___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_cli_old_py.html` & `pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_cli_old_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html` & `pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_cli_support_py.html` & `pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_cli_support_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_core_py.html` & `pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_core_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html` & `pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html` & `pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_typer_support_py.html` & `pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_typer_support_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/d_8bc7b9c2c0d01e74_types_py.html` & `pydal2sql-1.1.4/htmlcov/d_8bc7b9c2c0d01e74_types_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/favicon_32.png` & `pydal2sql-1.1.4/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/index.html` & `pydal2sql-1.1.4/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/keybd_closed.png` & `pydal2sql-1.1.4/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/keybd_open.png` & `pydal2sql-1.1.4/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/status.json` & `pydal2sql-1.1.4/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/htmlcov/style.css` & `pydal2sql-1.1.4/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/src/pydal2sql/cli.py` & `pydal2sql-1.1.4/src/pydal2sql/cli.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/src/pydal2sql/typer_support.py` & `pydal2sql-1.1.4/src/pydal2sql/typer_support.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/src/pydal2sql/types.py` & `pydal2sql-1.1.4/src/pydal2sql/types.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/tests/mock_git.py` & `pydal2sql-1.1.4/tests/mock_git.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/tests/test_cli.py` & `pydal2sql-1.1.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/tests/test_typer_support.py` & `pydal2sql-1.1.4/tests/test_typer_support.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/LICENSE.txt` & `pydal2sql-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/README.md` & `pydal2sql-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pydal2sql-1.1.3/pyproject.toml` & `pydal2sql-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "pydal2sql-core >= 0.3.5",
+    "pydal2sql-core >= 0.3.6",
     "su6", # bare without any checkers
     "rich",
     "pydal",
     "typer",
     "configuraptor >= 1.23",
     "GitPython",
 ]
```

### Comparing `pydal2sql-1.1.3/PKG-INFO` & `pydal2sql-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal2sql
-Version: 1.1.3
+Version: 1.1.4
 Summary: Convert pydal define_tables to SQL using pydal's CREATE TABLE logic.
 Project-URL: Documentation, https://github.com/robinvandernoord/pydal2sql#readme
 Project-URL: Issues, https://github.com/robinvandernoord/pydal2sql/issues
 Project-URL: Source, https://github.com/robinvandernoord/pydal2sql
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: configuraptor>=1.23
 Requires-Dist: gitpython
 Requires-Dist: pydal
-Requires-Dist: pydal2sql-core>=0.3.5
+Requires-Dist: pydal2sql-core>=0.3.6
 Requires-Dist: rich
 Requires-Dist: su6
 Requires-Dist: typer
 Provides-Extra: all
 Requires-Dist: pydal2sql-core[all]; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: contextlib-chdir; extra == 'dev'
```

