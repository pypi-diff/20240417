# Comparing `tmp/dycw_pre_commit_hooks-0.9.8.tar.gz` & `tmp/dycw_pre_commit_hooks-0.9.9.tar.gz`

## Comparing `dycw_pre_commit_hooks-0.9.8.tar` & `dycw_pre_commit_hooks-0.9.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/.envrc
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/.rgignore
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/requirements.txt
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/.github/workflows/push.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/__init__.py
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/py.typed
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_bump2version/__init__.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_bump2version/__main__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_dockfmt/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_dockfmt/__main__.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_hatch_version/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_hatch_version/__main__.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_ruff_format/__init__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_ruff_format/__main__.py
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_uv_pip_compile/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_uv_pip_compile/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/tests/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/tests/test_main.py
--rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/try-repo/run-bump2version.sh
--rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/try-repo/run-dockfmt.sh
--rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/try-repo/run-hatch-version.sh
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/try-repo/run-ruff-format.sh
--rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/try-repo/run-uv-pip-compile.sh
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/.gitignore
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/README.md
--rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/.envrc
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/.rgignore
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/requirements.txt
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/.github/workflows/push.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/__init__.py
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/py.typed
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_bump2version/__init__.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_bump2version/__main__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_dockfmt/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_dockfmt/__main__.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_hatch_version/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_hatch_version/__main__.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_ruff_format/__init__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_ruff_format/__main__.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_uv_pip_compile/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_uv_pip_compile/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/tests/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/tests/test_main.py
+-rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/try-repo/run-bump2version.sh
+-rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/try-repo/run-dockfmt.sh
+-rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/try-repo/run-hatch-version.sh
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/try-repo/run-ruff-format.sh
+-rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/try-repo/run-uv-pip-compile.sh
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/.gitignore
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/README.md
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 dycw_pre_commit_hooks-0.9.9/PKG-INFO
```

### Comparing `dycw_pre_commit_hooks-0.9.8/.pre-commit-config.yaml` & `dycw_pre_commit_hooks-0.9.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dycw_pre_commit_hooks-0.9.8/.pre-commit-hooks.yaml` & `dycw_pre_commit_hooks-0.9.9/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `dycw_pre_commit_hooks-0.9.8/.github/workflows/push.yml` & `dycw_pre_commit_hooks-0.9.9/.github/workflows/push.yml`

 * *Files identical despite different names*

### Comparing `dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/common.py` & `dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/common.py`

 * *Files identical despite different names*

### Comparing `dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_bump2version/__init__.py` & `dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_bump2version/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_dockfmt/__init__.py` & `dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_dockfmt/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_hatch_version/__init__.py` & `dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_hatch_version/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_ruff_format/__init__.py` & `dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_ruff_format/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_pre_commit_hooks-0.9.8/pre_commit_hooks/run_uv_pip_compile/__init__.py` & `dycw_pre_commit_hooks-0.9.9/pre_commit_hooks/run_uv_pip_compile/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_pre_commit_hooks-0.9.8/.gitignore` & `dycw_pre_commit_hooks-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dycw_pre_commit_hooks-0.9.8/README.md` & `dycw_pre_commit_hooks-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `dycw_pre_commit_hooks-0.9.8/pyproject.toml` & `dycw_pre_commit_hooks-0.9.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 # project
 [project]
 authors = [{name = "Derek Wan", email = "d.wan@icloud.com"}]
 dependencies = [
-  "dycw-utilities >= 0.25.0, < 0.26",
+  "click >= 8.1.7, < 8.2",
+  "dycw-utilities >= 0.25.1, < 0.26",
+  "loguru >= 0.7.2, < 0.8",
+  "semver >= 3.0.2, < 3.1",
   "tomlkit >= 0.12.3, < 0.13",
   "xdg-base-dirs >= 6.0.1, < 6.1",
 ]
 dynamic = ["version"]
 name = "dycw-pre-commit-hooks"
 readme = "README.md"
 requires-python = ">= 3.10"
 
 [project.optional-dependencies]
-dev = ["dycw-utilities[test]", "hatch", "pre-commit"]
+dev = ["hatch", "pre-commit", "pytest"]
 
 [project.scripts]
 run-bump2version = "pre_commit_hooks.run_bump2version:main"
 run-dockfmt = "pre_commit_hooks.run_dockfmt:main"
 run-hatch-version = "pre_commit_hooks.run_hatch_version:main"
 run-ruff-format = "pre_commit_hooks.run_ruff_format:main"
 run-uv-pip-compile = "pre_commit_hooks.run_uv_pip_compile:main"
```

### Comparing `dycw_pre_commit_hooks-0.9.8/PKG-INFO` & `dycw_pre_commit_hooks-0.9.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: dycw-pre-commit-hooks
-Version: 0.9.8
+Version: 0.9.9
 Author-email: Derek Wan <d.wan@icloud.com>
 Requires-Python: >=3.10
-Requires-Dist: dycw-utilities<0.26,>=0.25.0
+Requires-Dist: click<8.2,>=8.1.7
+Requires-Dist: dycw-utilities<0.26,>=0.25.1
+Requires-Dist: loguru<0.8,>=0.7.2
+Requires-Dist: semver<3.1,>=3.0.2
 Requires-Dist: tomlkit<0.13,>=0.12.3
 Requires-Dist: xdg-base-dirs<6.1,>=6.0.1
 Provides-Extra: dev
-Requires-Dist: dycw-utilities[test]; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # pre-commit-hooks
 
 ## Overview
 
 My [`pre-commit`](https://pre-commit.com/) hooks.
```

