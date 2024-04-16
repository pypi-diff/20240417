# Comparing `tmp/reprompt-0.0.7.2.tar.gz` & `tmp/reprompt-0.0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprompt-0.0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reprompt-0.0.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reprompt-0.0.7.2.tar` & `reprompt-0.0.7.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      334 2024-04-04 23:08:33.473524 reprompt-0.0.7.2/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-04 23:08:33.473643 reprompt-0.0.7.2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      417 2024-04-04 23:08:33.473790 reprompt-0.0.7.2/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-04 23:08:33.473883 reprompt-0.0.7.2/.github/template-sync.yml
--rw-r--r--   0        0        0      472 2024-04-07 21:52:20.071061 reprompt-0.0.7.2/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-07 21:52:20.071267 reprompt-0.0.7.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-04 23:08:33.474206 reprompt-0.0.7.2/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      368 2024-04-04 23:08:33.474380 reprompt-0.0.7.2/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-04 23:08:33.474462 reprompt-0.0.7.2/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-04 23:08:33.474551 reprompt-0.0.7.2/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-04 23:08:33.474640 reprompt-0.0.7.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-04 23:08:33.474722 reprompt-0.0.7.2/.pypirc
--rw-r--r--   0        0        0      459 2024-04-04 23:08:33.474853 reprompt-0.0.7.2/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-04 23:08:33.474937 reprompt-0.0.7.2/.vscode/settings.json
--rw-r--r--   0        0        0     1127 2024-04-07 21:52:20.071438 reprompt-0.0.7.2/LICENSE
--rw-r--r--   0        0        0    15834 2024-04-07 21:52:20.071934 reprompt-0.0.7.2/README.md
--rw-r--r--   0        0        0      634 2024-04-04 23:08:33.475348 reprompt-0.0.7.2/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-04 23:08:33.475439 reprompt-0.0.7.2/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-04 23:08:33.475525 reprompt-0.0.7.2/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-04 23:08:33.475604 reprompt-0.0.7.2/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-04 23:08:33.475685 reprompt-0.0.7.2/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-04 23:08:33.475772 reprompt-0.0.7.2/docs/make.bat
--rw-r--r--   0        0        0       51 2024-04-04 23:08:33.475852 reprompt-0.0.7.2/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-04 23:08:33.475929 reprompt-0.0.7.2/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-04 23:08:33.476081 reprompt-0.0.7.2/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-04 23:08:33.476163 reprompt-0.0.7.2/docs/pyproject.md
--rw-r--r--   0        0        0      425 2024-04-04 23:08:33.476254 reprompt-0.0.7.2/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      415 2024-04-04 23:08:33.476339 reprompt-0.0.7.2/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-04 23:08:33.476409 reprompt-0.0.7.2/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-04 23:08:33.476479 reprompt-0.0.7.2/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-04 23:08:33.476563 reprompt-0.0.7.2/docs/workflows.md
--rw-r--r--   0        0        0     6649 2024-04-07 21:52:20.072547 reprompt-0.0.7.2/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-04 23:08:33.476873 reprompt-0.0.7.2/src/README.md
--rw-r--r--   0        0        0     1241 2024-04-15 21:41:32.721094 reprompt-0.0.7.2/src/reprompt/__init__.py
--rw-r--r--   0        0        0      859 2024-04-07 23:40:24.407699 reprompt-0.0.7.2/src/reprompt/background_task_manager.py
--rw-r--r--   0        0        0      166 2024-04-08 17:02:10.738220 reprompt-0.0.7.2/src/reprompt/config.py
--rw-r--r--   0        0        0     3347 2024-04-15 21:39:48.952401 reprompt-0.0.7.2/src/reprompt/tracing.py
--rw-r--r--   0        0        0      989 2024-04-04 23:08:33.477233 reprompt-0.0.7.2/tests/conftest.py
--rw-r--r--   0        0        0      511 2024-04-07 21:52:20.073113 reprompt-0.0.7.2/tests/openai_example_script.py
--rw-r--r--   0        0        0      283 2024-04-07 21:52:20.073222 reprompt-0.0.7.2/tests/test_init.py
--rw-r--r--   0        0        0     1673 2024-04-07 21:52:20.073331 reprompt-0.0.7.2/tests/test_openai_tracing.py
--rw-r--r--   0        0        0    17737 1970-01-01 00:00:00.000000 reprompt-0.0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      417 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/template-sync.yml
+-rw-r--r--   0        0        0      472 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      368 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.vscode/settings.json
+-rw-r--r--   0        0        0     1127 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/LICENSE
+-rw-r--r--   0        0        0    15834 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/README.md
+-rw-r--r--   0        0        0      634 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/make.bat
+-rw-r--r--   0        0        0       51 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/pyproject.md
+-rw-r--r--   0        0        0      425 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      415 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/workflows.md
+-rw-r--r--   0        0        0     6649 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/src/README.md
+-rw-r--r--   0        0        0     1241 2024-04-16 22:28:54.157175 reprompt-0.0.7.3/src/reprompt/__init__.py
+-rw-r--r--   0        0        0      859 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/src/reprompt/background_task_manager.py
+-rw-r--r--   0        0        0      167 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/src/reprompt/config.py
+-rw-r--r--   0        0        0     3371 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/src/reprompt/tracing.py
+-rw-r--r--   0        0        0      989 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/tests/conftest.py
+-rw-r--r--   0        0        0      511 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/tests/openai_example_script.py
+-rw-r--r--   0        0        0      283 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/tests/test_init.py
+-rw-r--r--   0        0        0     1673 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/tests/test_openai_tracing.py
+-rw-r--r--   0        0        0    17737 1970-01-01 00:00:00.000000 reprompt-0.0.7.3/PKG-INFO
```

### Comparing `reprompt-0.0.7.2/.devcontainer/devcontainer.json` & `reprompt-0.0.7.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/.github/workflows/schedule-update-actions.yml` & `reprompt-0.0.7.3/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/.gitignore` & `reprompt-0.0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/.pre-commit-config.yaml` & `reprompt-0.0.7.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/.vscode/settings.json` & `reprompt-0.0.7.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/LICENSE` & `reprompt-0.0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/README.md` & `reprompt-0.0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/docs/Makefile` & `reprompt-0.0.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/docs/conf.py` & `reprompt-0.0.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/docs/make.bat` & `reprompt-0.0.7.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/docs/pylint.md` & `reprompt-0.0.7.3/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/pyproject.toml` & `reprompt-0.0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 spark = [
     "pyspark>=3.0.0"
 ]
 test = [
     "httpx>=0.21.0",
     "openai>=0.10.0",
     "bandit[toml]==1.7.5",
-    "black==23.3.0",
+    "black==24.4.0",
     "check-manifest==0.49",
     "flake8-bugbear==23.5.9",
     "flake8-docstrings",
     "flake8-formatter_junit_xml",
     "flake8",
     "flake8-pyproject",
     "pre-commit==3.7.0",
```

### Comparing `reprompt-0.0.7.2/src/reprompt/__init__.py` & `reprompt-0.0.7.3/src/reprompt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Reprompt"""
 
 from __future__ import annotations
 
 import logging
 
 from . import config
-from .tracing import FunctionTrace, write_traces, get_edits
+from .tracing import FunctionTrace, get_edits, write_traces
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 # IMPORTANT: setting version for Reprompt package
-__version__ = "0.0.7.2"
+__version__ = "0.0.7.3"
 # IMPORTANT: All the functions we want to expose publicly from the reprompt module
 __all__ = ["init", "FunctionTrace", "write_traces", "get_edits"]
 
 
 def init(api_base_url: str = None, api_key: str = None, debug: bool = False):
     if debug:
         logger.setLevel(logging.DEBUG)
```

### Comparing `reprompt-0.0.7.2/src/reprompt/background_task_manager.py` & `reprompt-0.0.7.3/src/reprompt/background_task_manager.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/src/reprompt/tracing.py` & `reprompt-0.0.7.3/src/reprompt/tracing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import annotations
 
+import asyncio
+import logging
 from datetime import datetime
+from functools import partial
 
 import aiohttp
-import asyncio
-
-import logging
 
 from . import config
-
 from .background_task_manager import BackgroundTaskManager
-from functools import partial
 
 logger = logging.getLogger(__name__)
 
 
 async def write_traces_task(traces):
     timestamp = datetime.now().isoformat()
     data = {"traces": [{"function_calls": traces, "timestamp": timestamp}]}
@@ -76,15 +74,15 @@
 
 async def get_edits(input: str) -> dict:
     try:
         async with aiohttp.ClientSession() as session:
             async with session.post(
                 f"{config.api_base_url}/api/overrides/get_example_overrides",
                 json={"input": input},
-                headers={"Content-Type": "application/json"},
+                headers={"Content-Type": "application/json", "apiKey": config.api_key},
             ) as response:
                 if response.status != 200:
                     logger.error(f"Failed to fetch edits: {response.status}")
                     return None
                 else:
                     logger.debug("fetched example overrides")
                     return await response.json()
```

### Comparing `reprompt-0.0.7.2/tests/conftest.py` & `reprompt-0.0.7.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/tests/test_openai_tracing.py` & `reprompt-0.0.7.3/tests/test_openai_tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.2/PKG-INFO` & `reprompt-0.0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprompt
-Version: 0.0.7.2
+Version: 0.0.7.3
 Summary: Reprompt
 Author-email: Lukas Martinelli <me@lukasmartinelli.ch>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -15,15 +15,15 @@
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: wrapt>=1.12.1
 Requires-Dist: pyspark>=3.0.0 ; extra == "spark"
 Requires-Dist: httpx>=0.21.0 ; extra == "test"
 Requires-Dist: openai>=0.10.0 ; extra == "test"
 Requires-Dist: bandit[toml]==1.7.5 ; extra == "test"
-Requires-Dist: black==23.3.0 ; extra == "test"
+Requires-Dist: black==24.4.0 ; extra == "test"
 Requires-Dist: check-manifest==0.49 ; extra == "test"
 Requires-Dist: flake8-bugbear==23.5.9 ; extra == "test"
 Requires-Dist: flake8-docstrings ; extra == "test"
 Requires-Dist: flake8-formatter_junit_xml ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
 Requires-Dist: flake8-pyproject ; extra == "test"
 Requires-Dist: pre-commit==3.7.0 ; extra == "test"
```

