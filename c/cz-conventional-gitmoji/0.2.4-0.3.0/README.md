# Comparing `tmp/cz_conventional_gitmoji-0.2.4.tar.gz` & `tmp/cz_conventional_gitmoji-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz_conventional_gitmoji-0.2.4.tar", max compression
+gzip compressed data, was "cz_conventional_gitmoji-0.3.0.tar", max compression
```

## Comparing `cz_conventional_gitmoji-0.2.4.tar` & `cz_conventional_gitmoji-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2509 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/README.md
--rw-r--r--   0        0        0     2594 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/src/cz_gitmoji/__init__.py
--rw-r--r--   0        0        0     1285 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/src/cz_gitmoji/conventional_gitmojis_info.txt
--rw-r--r--   0        0        0    13515 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/src/cz_gitmoji/main.py
--rw-r--r--   0        0        0        0 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/src/cz_gitmoji/py.typed
--rw-r--r--   0        0        0        0 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/src/gitmojify/__init__.py
--rw-r--r--   0        0        0     1687 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/src/gitmojify/mojify.py
--rw-r--r--   0        0        0        0 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/src/gitmojify/py.typed
--rw-r--r--   0        0        0        0 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/src/shared/__init__.py
--rw-r--r--   0        0        0     2667 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/src/shared/gitmojis.py
--rw-r--r--   0        0        0      406 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/src/shared/model.py
--rw-r--r--   0        0        0        0 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/src/shared/py.typed
--rw-r--r--   0        0        0    10608 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/src/shared/spec.py
--rw-r--r--   0        0        0      817 2024-01-30 18:57:35.053188 cz_conventional_gitmoji-0.2.4/src/shared/utils.py
--rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 cz_conventional_gitmoji-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2615 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/README.md
+-rw-r--r--   0        0        0     2631 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/cz_gitmoji/__init__.py
+-rw-r--r--   0        0        0     1285 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/cz_gitmoji/conventional_gitmojis_info.txt
+-rw-r--r--   0        0        0    13466 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/cz_gitmoji/main.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/cz_gitmoji/py.typed
+-rw-r--r--   0        0        0        0 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/gitmojify/__init__.py
+-rw-r--r--   0        0        0     1687 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/gitmojify/mojify.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/gitmojify/py.typed
+-rw-r--r--   0        0        0        0 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/shared/__init__.py
+-rw-r--r--   0        0        0     2701 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/shared/gitmojis.py
+-rw-r--r--   0        0        0      406 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/shared/model.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/shared/py.typed
+-rw-r--r--   0        0        0    10765 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/shared/spec.py
+-rw-r--r--   0        0        0      817 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/shared/utils.py
+-rw-r--r--   0        0        0     3574 1970-01-01 00:00:00.000000 cz_conventional_gitmoji-0.3.0/PKG-INFO
```

### Comparing `cz_conventional_gitmoji-0.2.4/README.md` & `cz_conventional_gitmoji-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,25 +41,31 @@
 ```
 
 To use it as a pre-commit hook, install this packages as well as `commitizen` and put the following into your **.pre-commit-config.yaml**
 
 ```yaml
 repos:
   - repo: https://github.com/ljnsn/cz-conventional-gitmoji
-    rev: main
+    rev: 0.2.4
     hooks:
       - id: conventional-gitmoji
 ```
 
+Make sure to install the relevant pre-commit hooks with
+
+```bash
+pre-commit install --install-hooks
+```
+
 Commit with a message in conventional format that contains a valid type mapped by conventional gitmoji and the gitmoji will automagically be added.
 
 ## Features
 
 - [x] Enable conventional gitmoji commit messages via `cz commit`.
+- [x] Add hook to automatically prepend the appropriate gitmoji for the commit's type.
 - [ ] Add `--simple-emojis` option to use only the emojis relating to `cz_conventional_commits` types.
 - [ ] Add `--simple-types` option to use only the types used by `cz_conventional_commits`.
 - [ ] Add `--conventional` option to put the emoji in the commit message, making it compatible with `cz_conventional_commits`.
-- [x] Add hook to automatically prepend the appropriate gitmoji for the commit's type.
 
 ## Inspiration
 
 - [`commitizen-emoji`](https://github.com/marcelomaia/commitizen-emoji)
```

### Comparing `cz_conventional_gitmoji-0.2.4/pyproject.toml` & `cz_conventional_gitmoji-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cz-conventional-gitmoji"
-version = "0.2.4"
+version = "0.3.0"
 description = "A commitizen plugin that combines gitmoji and conventional."
 authors = ["ljnsn <82611987+ljnsn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "shared", from = "src" },
   { include = "cz_gitmoji", from = "src" },
@@ -25,54 +25,56 @@
 setuptools = { version = "*", python = ">=3.12" }
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22.12,<24.0"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 coverage = { extras = ["toml"], version = "^7.0.1" }
-ruff = ">=0.0.246,<0.1.16"
+ruff = ">=0.0.246,<0.3.8"
 mypy = "^1.3.0"
 pre-commit = ">=2.0"
 
 [tool.commitizen]
 name = "cz_gitmoji"
-version = "0.2.4"
+version = "0.3.0"
 bump_message = "🔖 bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 version_files = ["pyproject.toml:^version"]
 update_changelog_on_bump = true
 
 [tool.black]
 target-version = ["py37", "py38", "py39", "py310", "py311"]
 
 [tool.ruff]
+fix = true
+src = ["src", "test"]
+
+[tool.ruff.lint]
 ignore = [
   # Line too long
   "E501",
   # unable to detect undefined names
   "F403",
   # may be undefined or defined from star imports
   "F405",
 ]
-fix = true
 unfixable = ["F401", "F841"]
-src = ["src", "test"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # ignore usage of `assert` in tests
 "*/tests/*" = ["S101"]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 # Disallow all relative imports.
 ban-relative-imports = "all"
 
-[tool.ruff.pep8-naming]
+[tool.ruff.lint.pep8-naming]
 # Allow Pydantic's `@validator` decorator to trigger class method treatment.
 classmethod-decorators = ["classmethod", "pydantic.validator"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 command_line = "--module pytest"
```

### Comparing `cz_conventional_gitmoji-0.2.4/src/cz_gitmoji/conventional_gitmojis_info.txt` & `cz_conventional_gitmoji-0.3.0/src/cz_gitmoji/conventional_gitmojis_info.txt`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.2.4/src/cz_gitmoji/main.py` & `cz_conventional_gitmoji-0.3.0/src/cz_gitmoji/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 
 
 def parse_scope(text: str) -> str:
     if not text:
         return ""
 
     scope = text.strip().split()
-    if len(scope) == 1:
-        return scope[0]
-
     return "-".join(scope)
 
 
 def parse_subject(text: str) -> str:
     if isinstance(text, str):
         text = text.strip(".").strip()
```

### Comparing `cz_conventional_gitmoji-0.2.4/src/gitmojify/mojify.py` & `cz_conventional_gitmoji-0.3.0/src/gitmojify/mojify.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.2.4/src/shared/gitmojis.py` & `cz_conventional_gitmoji-0.3.0/src/shared/gitmojis.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     "GJ_LOGIC",
     "GJ_HEALTH",
     "GJ_INFRA",
     "GJ_DEVXP",
     "GJ_MONEY",
     "GJ_THREADING",
     "GJ_VALIDATION",
+    "GJ_CHORE",
 )
 
 GJ_FIX = "🐛"
 GJ_FEAT = "✨"
 GJ_DOCS = "📝"
 GJ_STYLE = "🎨"
 GJ_REFACTOR = "♻️ "
@@ -143,7 +144,8 @@
 GJ_LOGIC = "👔"
 GJ_HEALTH = "🩺"
 GJ_INFRA = "🧱"
 GJ_DEVXP = "🧑‍💻"
 GJ_MONEY = "💸"
 GJ_THREADING = "🧵"
 GJ_VALIDATION = "🦺"
+GJ_CHORE = "🧹"
```

### Comparing `cz_conventional_gitmoji-0.2.4/src/shared/spec.py` & `cz_conventional_gitmoji-0.3.0/src/shared/spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,8 +435,14 @@
     },
     {
         "type": "validation",
         "icon": GJ_VALIDATION,
         "code": ":safety_vest:",
         "desc": "Add or update code related to validation.",
     },
+    {
+        "type": "chore",
+        "icon": GJ_CHORE,
+        "code": ":broom:",
+        "desc": "Commit changes related to miscelaneous chores.",
+    },
 ]
```

### Comparing `cz_conventional_gitmoji-0.2.4/src/shared/utils.py` & `cz_conventional_gitmoji-0.3.0/src/shared/utils.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.2.4/PKG-INFO` & `cz_conventional_gitmoji-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz-conventional-gitmoji
-Version: 0.2.4
+Version: 0.3.0
 Summary: A commitizen plugin that combines gitmoji and conventional.
 Home-page: https://github.com/ljnsn/cz-conventional-gitmoji
 License: MIT
 Author: ljnsn
 Author-email: 82611987+ljnsn@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -64,26 +64,32 @@
 ```
 
 To use it as a pre-commit hook, install this packages as well as `commitizen` and put the following into your **.pre-commit-config.yaml**
 
 ```yaml
 repos:
   - repo: https://github.com/ljnsn/cz-conventional-gitmoji
-    rev: main
+    rev: 0.2.4
     hooks:
       - id: conventional-gitmoji
 ```
 
+Make sure to install the relevant pre-commit hooks with
+
+```bash
+pre-commit install --install-hooks
+```
+
 Commit with a message in conventional format that contains a valid type mapped by conventional gitmoji and the gitmoji will automagically be added.
 
 ## Features
 
 - [x] Enable conventional gitmoji commit messages via `cz commit`.
+- [x] Add hook to automatically prepend the appropriate gitmoji for the commit's type.
 - [ ] Add `--simple-emojis` option to use only the emojis relating to `cz_conventional_commits` types.
 - [ ] Add `--simple-types` option to use only the types used by `cz_conventional_commits`.
 - [ ] Add `--conventional` option to put the emoji in the commit message, making it compatible with `cz_conventional_commits`.
-- [x] Add hook to automatically prepend the appropriate gitmoji for the commit's type.
 
 ## Inspiration
 
 - [`commitizen-emoji`](https://github.com/marcelomaia/commitizen-emoji)
```

