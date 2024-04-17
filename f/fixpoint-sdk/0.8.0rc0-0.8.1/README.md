# Comparing `tmp/fixpoint_sdk-0.8.0rc0.tar.gz` & `tmp/fixpoint_sdk-0.8.1.tar.gz`

## Comparing `fixpoint_sdk-0.8.0rc0.tar` & `fixpoint_sdk-0.8.1.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.editorconfig
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.lintstagedrc.json
--rw-r--r--   0        0        0    21726 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.pylintrc
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/mypy.ini
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/pytest.ini
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/requirements.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/test-requirements.txt
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.github/workflows/pypi-release-prod.yml
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.github/workflows/pypi-release-test.yml
--rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/bin/pip-freeze
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/bin/pip-install
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/examples/__init__.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/examples/direct_logging.py
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/examples/function_calling.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/examples/main.py
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/examples/router.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/examples/streaming.py
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/githooks/pre-commit
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/__init__.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/_logging_api.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/_mock_completions.py
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/client.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/compat.py
--rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/completions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/__init__.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/_mock_requests.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/debugging.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/env.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/exc.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/iterwrapper.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/logging.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/requests.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/openapi/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/openapi/exceptions.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/types/__init__.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/types/_utils.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/types/openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/__init__.py
--rw-r--r--   0        0        0    15061 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/mock_completions.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/test_client.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/test_completions.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/test_types.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/lib/test_iterwrapper.py
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/lib/test_requests.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/types/test_openai.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.gitignore
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/LICENSE
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/README.md
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/pyproject.toml
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/.editorconfig
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/.lintstagedrc.json
+-rw-r--r--   0        0        0    21726 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/.pylintrc
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/mypy.ini
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/pytest.ini
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/test-requirements.txt
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/.github/workflows/pypi-release-prod.yml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/.github/workflows/pypi-release-test.yml
+-rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/bin/pip-freeze
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/bin/pip-install
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/examples/__init__.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/examples/direct_logging.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/examples/function_calling.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/examples/main.py
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/examples/router.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/examples/streaming.py
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/githooks/pre-commit
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/__init__.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/_logging_api.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/_mock_completions.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/client.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/compat.py
+-rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/completions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/__init__.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/_mock_requests.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/debugging.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/env.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/exc.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/iterwrapper.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/logging.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/requests.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/openapi/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/openapi/exceptions.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/types/__init__.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/types/_utils.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/src/fixpoint_sdk/types/openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0    15061 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/tests/mock_completions.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/tests/test_client.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/tests/test_completions.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/tests/test_types.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/tests/lib/test_iterwrapper.py
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/tests/lib/test_requests.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/tests/types/test_openai.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/.gitignore
+-rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/README.md
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.1/PKG-INFO
```

### Comparing `fixpoint_sdk-0.8.0rc0/.pylintrc` & `fixpoint_sdk-0.8.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/mypy.ini` & `fixpoint_sdk-0.8.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/.github/workflows/ci.yml` & `fixpoint_sdk-0.8.1/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -27,16 +27,14 @@
 
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: 'pip'
-          cache-dependency-path: ${{ github.workspace }}/requirements.txt
-      - run: pip install -r ${{ github.workspace }}/requirements.txt
 
       - run: pip install -e '.[dev]'
         working-directory: ${{ github.workspace }}
 
       - name: Typecheck Python
         run: mypy .
         working-directory: ${{ github.workspace }}
```

### Comparing `fixpoint_sdk-0.8.0rc0/.github/workflows/pypi-release-prod.yml` & `fixpoint_sdk-0.8.1/.github/workflows/pypi-release-prod.yml`

 * *Files 12% similar despite different names*

```diff
@@ -12,18 +12,20 @@
         uses: actions/checkout@v4
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
           cache: 'pip'
-          cache-dependency-path: ${{ github.workspace }}/requirements.txt
+
+      - name: Upgrade pip
+        run: pip install --upgrade pip
 
       - name: Install dependencies
-        run: pip install -r requirements.txt
+        run: pip install '.[dev]'
 
       - name: Build package
         run: python -m build
         working-directory: ${{ github.workspace }}
 
       - name: Publish to PyPI prod repository
         run: python -m twine upload --verbose --non-interactive --repository pypi dist/*
```

### Comparing `fixpoint_sdk-0.8.0rc0/.github/workflows/pypi-release-test.yml` & `fixpoint_sdk-0.8.1/.github/workflows/pypi-release-test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -12,18 +12,20 @@
         uses: actions/checkout@v4
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
           cache: 'pip'
-          cache-dependency-path: ${{ github.workspace }}/requirements.txt
+
+      - name: Upgrade pip
+        run: pip install --upgrade pip
 
       - name: Install dependencies
-        run: pip install -r requirements.txt
+        run: pip install '.[dev]'
 
       - name: Build package
         run: python -m build
         working-directory: ${{ github.workspace }}
 
       - name: Publish to PyPI test repository
         run: python -m twine upload --verbose --non-interactive --repository testpypi dist/*
```

### Comparing `fixpoint_sdk-0.8.0rc0/bin/pip-freeze` & `fixpoint_sdk-0.8.1/bin/pip-freeze`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/examples/direct_logging.py` & `fixpoint_sdk-0.8.1/examples/direct_logging.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/examples/function_calling.py` & `fixpoint_sdk-0.8.1/examples/function_calling.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/examples/main.py` & `fixpoint_sdk-0.8.1/examples/main.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/examples/router.py` & `fixpoint_sdk-0.8.1/examples/router.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/examples/streaming.py` & `fixpoint_sdk-0.8.1/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/__init__.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/_logging_api.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/_logging_api.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/_mock_completions.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/_mock_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/client.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/client.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/compat.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/compat.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/completions.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/_mock_requests.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/_mock_requests.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/debugging.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/debugging.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/env.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/env.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/exc.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/exc.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/iterwrapper.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/iterwrapper.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/requests.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/lib/requests.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/types/__init__.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/types/_utils.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/types/_utils.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/types/openai.py` & `fixpoint_sdk-0.8.1/src/fixpoint_sdk/types/openai.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/tests/mock_completions.py` & `fixpoint_sdk-0.8.1/tests/mock_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/tests/test_client.py` & `fixpoint_sdk-0.8.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/tests/test_completions.py` & `fixpoint_sdk-0.8.1/tests/test_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/tests/test_types.py` & `fixpoint_sdk-0.8.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/tests/lib/test_iterwrapper.py` & `fixpoint_sdk-0.8.1/tests/lib/test_iterwrapper.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/tests/lib/test_requests.py` & `fixpoint_sdk-0.8.1/tests/lib/test_requests.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/tests/types/test_openai.py` & `fixpoint_sdk-0.8.1/tests/types/test_openai.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/LICENSE` & `fixpoint_sdk-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/README.md` & `fixpoint_sdk-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.0rc0/pyproject.toml` & `fixpoint_sdk-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fixpoint_sdk"
-version = "0.8.0-rc00"
+version = "0.8.1"
 
 authors = [
 { name="Jakub Cichon", email="jakub@fixpoint.co" },
 { name="Dylan Mikus", email="dylan@fixpoint.co" },
 ]
 description = "Python SDK for Fixpoint - Auto-improvement to make your LLM apps smarter"
 readme = "README.md"
```

### Comparing `fixpoint_sdk-0.8.0rc0/PKG-INFO` & `fixpoint_sdk-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fixpoint_sdk
-Version: 0.8.0rc0
+Version: 0.8.1
 Summary: Python SDK for Fixpoint - Auto-improvement to make your LLM apps smarter
 Project-URL: Homepage, https://github.com/gofixpoint/python-sdk
 Project-URL: Issues, https://github.com/gofixpoint/python-sdk/issues
 Author-email: Jakub Cichon <jakub@fixpoint.co>, Dylan Mikus <dylan@fixpoint.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

