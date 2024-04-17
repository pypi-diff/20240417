# Comparing `tmp/songbirdcore-0.0.5.tar.gz` & `tmp/songbirdcore-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songbirdcore-0.0.5.tar", last modified: Tue Apr 16 20:52:05 2024, max compression
+gzip compressed data, was "songbirdcore-0.0.6.tar", last modified: Wed Apr 17 16:09:48 2024, max compression
```

## Comparing `songbirdcore-0.0.5.tar` & `songbirdcore-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:52:05.507411 songbirdcore-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:52:05.499411 songbirdcore-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:52:05.503411 songbirdcore-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/.github/workflows/style.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-16 20:52:05.507411 songbirdcore-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:52:05.507411 songbirdcore-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:52:05.503411 songbirdcore-0.0.5/songbirdcore/
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/songbirdcore/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/songbirdcore/gdrive.py
--rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/songbirdcore/itunes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:52:05.503411 songbirdcore-0.0.5/songbirdcore/models/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/songbirdcore/models/itunes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/songbirdcore/models/modes.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/songbirdcore/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/songbirdcore/requirements.txt.blank
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/songbirdcore/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/songbirdcore/web.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/songbirdcore/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:52:05.507411 songbirdcore-0.0.5/songbirdcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-16 20:52:05.000000 songbirdcore-0.0.5/songbirdcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-16 20:52:05.000000 songbirdcore-0.0.5/songbirdcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:52:05.000000 songbirdcore-0.0.5/songbirdcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-16 20:52:05.000000 songbirdcore-0.0.5/songbirdcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 20:52:05.000000 songbirdcore-0.0.5/songbirdcore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:52:05.499411 songbirdcore-0.0.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:52:05.507411 songbirdcore-0.0.5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/tests/unit/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/tests/unit/test_gdrive.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/tests/unit/test_itunes.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/tests/unit/test_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-16 20:52:00.000000 songbirdcore-0.0.5/tests/unit/test_youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.185462 songbirdcore-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.177462 songbirdcore-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.181462 songbirdcore-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/.github/workflows/pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/.github/workflows/style.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-17 16:09:48.185462 songbirdcore-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.181462 songbirdcore-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.181462 songbirdcore-0.0.6/docs/songbirdcore/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/gdrive.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/itunes.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.181462 songbirdcore-0.0.6/docs/songbirdcore/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/models/itunes_api.md
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/models/modes.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/web.md
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/youtube.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:09:48.185462 songbirdcore-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.181462 songbirdcore-0.0.6/songbirdcore/
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/itunes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.181462 songbirdcore-0.0.6/songbirdcore/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/models/itunes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/models/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/requirements.txt.blank
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.185462 songbirdcore-0.0.6/songbirdcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-17 16:09:48.000000 songbirdcore-0.0.6/songbirdcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-17 16:09:48.000000 songbirdcore-0.0.6/songbirdcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:09:48.000000 songbirdcore-0.0.6/songbirdcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-17 16:09:48.000000 songbirdcore-0.0.6/songbirdcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 16:09:48.000000 songbirdcore-0.0.6/songbirdcore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.177462 songbirdcore-0.0.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.185462 songbirdcore-0.0.6/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/tests/unit/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/tests/unit/test_gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/tests/unit/test_itunes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/tests/unit/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/tests/unit/test_youtube.py
```

### Comparing `songbirdcore-0.0.5/.github/workflows/pypi-publish.yaml` & `songbirdcore-0.0.6/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.5/.github/workflows/tests.yaml` & `songbirdcore-0.0.6/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.5/LICENSE` & `songbirdcore-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.5/Makefile` & `songbirdcore-0.0.6/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 # variables as a list, required for pytest targets
 # in this makefile
 
 .PHONY: setup
 setup: env
 	@echo sets up the development environment
+	npm install -g markdownlint-cli
 	python3 -m venv venv
 	@echo activate venv with 'source venv/bin/activate'
 
 .PHONY: requirements
 requirements: env
 	pip install -r $(APP_NAME)/$(REQUIREMENTS_FILE)
 # only install dependencies locally if in dev env
@@ -43,13 +44,29 @@
 update-requirements: env
 	pip uninstall requests-htmlc
 	pip freeze --exclude-editable | xargs pip uninstall -y
 	rm $(APP_NAME)/$(REQUIREMENTS_FILE) || true
 	pip install -r $(APP_NAME)/requirements.txt.blank
 	pip freeze --exclude-editable > $(APP_NAME)/$(REQUIREMENTS_FILE)
 
+# documentation targets
+.PHONY: docs-lint
+docs-lint:
+	@echo linting files at docs/**/*.md
+	markdownlint docs/**/*.md
+
+.PHONY: docs-serve
+docs-serve:
+	@echo serving the site on http://localhost:8000
+	mkdocs serve
+
+.PHONY: docs-build
+docs-build:
+	@echo building the site
+	mkdocs build --strict --verbose --site-dir public
+
 lint:
 	black $(APP_NAME)/.
 	black tests
 
 test:
 	python -m pytest --doctest-modules --junitxml=junit/test-results.xml --cov=songbirdcore --cov-report=xml --cov-report=html tests/unit -v
```

### Comparing `songbirdcore-0.0.5/PKG-INFO` & `songbirdcore-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songbirdcore
-Version: 0.0.5
+Version: 0.0.6
 Summary: core low level api for songbird
 Author: Christian Boin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: beautifulsoup4==4.12.3
@@ -60,28 +60,36 @@
 Requires-Dist: yt-dlp==2024.4.9
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: click; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mike; extra == "dev"
+Requires-Dist: mkdocstrings-python; extra == "dev"
 Provides-Extra: package
 Requires-Dist: build; extra == "package"
 Requires-Dist: twine; extra == "package"
 
 # songbirdcore 🐦
 
 Low-level package with common code used across songbird's
 cli and api.
 
 See: 
 
 - [songbirdcli](https://github.com/cboin1996/songbird.git)
 - [songbirdapi](https://github.com/cboin1996/songbirdapi.git)
 
+## Documentation
+
+`songbirdcore`'s documentation may be found [here](https://cboin1996.github.io/songbirdcore)
+
 ## Requirements
 
 - Python version >= 3.11
 
 ## Installation
 
 To install, run
```

### Comparing `songbirdcore-0.0.5/README.md` & `songbirdcore-0.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 cli and api.
 
 See: 
 
 - [songbirdcli](https://github.com/cboin1996/songbird.git)
 - [songbirdapi](https://github.com/cboin1996/songbirdapi.git)
 
+## Documentation
+
+`songbirdcore`'s documentation may be found [here](https://cboin1996.github.io/songbirdcore)
+
 ## Requirements
 
 - Python version >= 3.11
 
 ## Installation
 
 To install, run
```

### Comparing `songbirdcore-0.0.5/songbirdcore/common.py` & `songbirdcore-0.0.6/songbirdcore/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,29 +19,31 @@
         data = tomllib.load(f)
     return data
 
 
 def set_logger_config_globally(log_level=logging.INFO) -> None:
     """Sets the python logging module settings for output
     to stdout and to file.
+
     Args:
-        timestamp (str): the timestamp to name the log file.
+        log_level (str): the log level
+
     """
     logging.basicConfig(
         level=log_level,
         format="[%(levelname)s] %(name)s: %(message)s",
         handlers=[logging.StreamHandler()],
     )
 
 
-def name_plate(entries: List[str]):
-    """
-    Produces the application nameplate.
-    Args: two command line argumates, debug mode on or off, operating system
-    Returns: operating system
+def name_plate(entries: List[str]) -> None:
+    """renders the songbird entrypoint name plate
+
+    Args:
+        entries (List[str]): add additional entries to the nameplate via this list
     """
     # load project version from file
     print("===============================")
     print("=----Welcome to songbird🐦----=")
     print("===============================")
     print(f"--songbirdcore {version}")
     for entry in entries:
@@ -55,15 +57,15 @@
         "\t- If you encounter errors, please create an issue here https://github.com/cboin1996/songbirdcore/issues/"
     )
     print(
         f"At the main menu, type one of {[mode.value for mode in modes.Modes]} to switch modes!"
     )
 
 
-def fname_duper(fname: str, limit: int, count: int, dup_key: str):
+def fname_duper(fname: str, limit: int, count: int, dup_key: str) -> Optional[str]:
     """Generates a duplicate filename for when a filename already exists
 
     Args:
         fname (str): filename
         limit (int): a limit of dups before quitting the attempt
         count (int): recursive count tracker
         dup_key (str): the key to use as the duplicate addon
@@ -81,20 +83,23 @@
         return None
     if os.path.exists(fname):
         fname = fname_duper(fname_noext + dup_key + ext, limit, count + 1, dup_key)
 
     return fname
 
 
-def remove_illegal_characters(filename):
+def remove_illegal_characters(filename) -> str:
     """
     Used for stripping file names of illegal characters used for saving
+
     Args:
-        filename(str): the file's name to strip
-    Returns: stipped file name
+        filename (str): the file's name to strip illegal characters from
+
+    Returns:
+        str: stripped file name
     """
     return (
         filename.replace("\\", "")
         .replace('"', "")
         .replace("/", "")
         .replace("*", "")
         .replace("?", "")
@@ -116,20 +121,23 @@
     Returns:
         List[str]: list of paths found that match
     """
     paths = glob.glob(os.path.join(path, filename))
     return paths
 
 
-def pretty_list_of_basemodel_printer(list_of_dicts: List[BaseModel], ignore_keys=None):
+def pretty_list_of_basemodel_printer(
+    list_of_dicts: List[BaseModel], ignore_keys: Optional[List[str]] = None
+):
     """
-    prints list from top down so its more user friendly, items are pretty big
-    params:
-        list_of_dicts: list of dictionaries to print
-        ignore_keys: any keys not to print
+    renders a list to stdio given a list of pydantic BaseModel objects
+
+    Args:
+        list_of_dicts (List[BaseModel]): list of dictionaries to print
+        ignore_keys (Optional[List[str]], optional): any keys/fields in BaseModel not to print
     """
     i = len(list_of_dicts) - 1
     logger.info("------------------------")
     for element in reversed(list_of_dicts):
         logger.info(i)
         for k, v in element.model_dump().items():
             if ignore_keys is not None:
@@ -141,9 +149,14 @@
             else:  # (default case) print the key and value
                 print("\t%s - %s" % (k, v))
         i -= 1
         print("------------------------")
 
 
 def pretty_lst_printer(lyst: List):
+    """print a list to stdio
+
+    Args:
+        lyst (List): the list to print
+    """
     for idx, item in enumerate(lyst):
         logger.info(f"\t [{idx}] - {item}")
```

### Comparing `songbirdcore-0.0.5/songbirdcore/gdrive.py` & `songbirdcore-0.0.6/songbirdcore/gdrive.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,29 @@
     gdrive_folder_id: str,
     credentials_path: str,
     token_path: str,
     song_name: str,
     song_path: str,
     auth_port: int,
     bind_addr: Optional[str] = None,
-):
+) -> str:
+    """save a song to google drive
+
+    Args:
+        gdrive_folder_id (str): google drive folder id
+        credentials_path (str): path to a credentials.json file
+        token_path (str): path to a google cloud token file
+        song_name (str): the name of the song (filename)
+        song_path (str): the path of the song locally
+        auth_port (int): the port to use for oauth
+        bind_addr (Optional[str], optional): optionally specify the bind address, otherwise localhost is used. Defaults to None.
+
+    Returns:
+        str: the file id of the upload
+    """
     creds = None
     # The file token.json stores the user's access and refresh tokens, and is
     # created automatically when the authorization flow completes for the first
     # time.
     scopes = ["https://www.googleapis.com/auth/drive"]
     if os.path.exists(token_path):
         creds = Credentials.from_authorized_user_file(token_path, scopes)
```

### Comparing `songbirdcore-0.0.5/songbirdcore/itunes.py` & `songbirdcore-0.0.6/songbirdcore/itunes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, Optional, Union
 import glob
 from pydantic import ValidationError
 import requests
+from requests import Response
 import json
 import os, sys
 import eyed3
 from mutagen.mp4 import MP4, MP4Cover
 import logging
 
 from . import common
@@ -17,19 +18,21 @@
 def itunes_lib_search(
     itunes_lib_path: str,
     search_parameters: str,
     album_properties: Optional[itunes_api.ItunesApiAlbumKeys] = None,
 ) -> List[str]:
     """
     Performs a search on users iTunes library by album, artist and genre
+
     Args:
         itunes_lib_path (str): path to itunes song library on disk
         search_parameters (str): search term
         album_properties (itunes_api.ItunesApiAlbumKeys): determines whether to do a smarter search based on given album properties
-    Returns: iTunesPaths dict with songs matching the search added
+
+    Returns: a list of songpaths found
     """
     itunes_songs = glob.glob(
         os.path.join(itunes_lib_path, "*", "*", f"*.*"), recursive=True
     )
     matches = []
     for song_path in itunes_songs:
         # song_name_split is list of itunes file path.. artist is -3 from length, song is -1
@@ -58,32 +61,38 @@
     # returns sorted alphabetical list of matches.
     matches.sort()
     return matches
 
 
 def m4a_tagger(file_path: str, song_tag_data: itunes_api.ItunesApiSongModel) -> bool:
     """Tag an m4a file using iTunes recognized tags.
-    Legend taken from mutagen website.
-    Text values
-    '\xa9nam' - track title
-    '\xa9alb' - album
-    '\xa9ART' - artist
+
+    The below is a tag legend taken from mutagen website.
+    Text values:
+
+    ```
+    '\\xa9nam' - track title
+    '\\xa9alb' - album
+    '\\xa9ART' - artist
     'aART' - album artist
-    '\xa9day' - year
+    '\\xa9day' - year
     'purd' - purchase date
-    '\xa9gen' - genre
+    '\\xa9gen' - genre
     Tuples of ints (multiple values per key are supported):
     'trkn' - track number, total tracks
     'disk' - disc number, total discs
     'covr' - cover artwork, list of MP4Cover objects (which are tagged strs)
+    ```
 
     Args:
         file_path (str): path to the m4a file
-        song_keys (itunes_api.ItunesApiSongModel): The model for the songs relevant metadata collected from itunes search api
-    Returns: bool: true if tagging was successful.
+        song_tag_data (itunes_api.ItunesApiSongModel): The model for the songs relevant metadata collected from itunes search api
+
+    Returns:
+        bool: true if tagging was successful.
     """
     try:
         logger.info(f"Adding tags to m4a file : {file_path}")
 
         response = artwork_searcher(url=song_tag_data.artworkUrl100)
         audiofile = MP4(file_path)
 
@@ -112,17 +121,24 @@
     except Exception as e:
         logger.exception(
             f"Unexpected error occured while trying to tag your m4a file: {e}"
         )
         return False
 
 
-def mp3ID3Tagger(mp3_path: str, song_tag_data: itunes_api.ItunesApiSongModel):
+def mp3ID3Tagger(mp3_path: str, song_tag_data: itunes_api.ItunesApiSongModel) -> bool:
     """
-    Tags an mp3 file at mp3_path given a dictionary of tags
+    Tags an mp3 file at mp3_path given a itunes_api.ItunesApiSongModel object
+
+    Args:
+        mp3_path (str): file path of mp3 file
+        song_tag_data (itunes_api.ItunesApiSongModel): the model with tag fields
+
+    Returns:
+        bool: true if tagging was a success
     """
     try:
         # Create MP3File instance.
         logger.info(f"Adding your tags to mp3 file: {mp3_path}")
         # Have to call MP3File twice for it to work.
 
         # Get the image to show for a song .. but get high res
@@ -130,15 +146,15 @@
 
         response = artwork_searcher(url=song_tag_data.artworkUrl100)
 
         # Set all the tags for the mp3, all without if statement were checked for existence.
         audiofile = eyed3.load(mp3_path)
         audiofile.tag.artist = song_tag_data.artistName
         audiofile.tag.album = song_tag_data.collectionName
-        audiofile.tag.title = song_tag_data.trackName
+        audiofile.tag.title = song_tag_data.TRACK_NAME
         audiofile.tag.genre = song_tag_data.primaryGenreName
         audiofile.tag.track_num = (song_tag_data.trackNumber, song_tag_data.trackCount)
         audiofile.tag.disc_num = (song_tag_data.discNumber, song_tag_data.discCount)
         audiofile.tag.recording_date = song_tag_data.releaseDate
 
         if (
             song_tag_data.collectionArtistName is not None
@@ -179,19 +195,22 @@
     return output_filename
 
 
 def query_api(
     search_variable: str, limit: int, mode: modes.Modes, lookup: bool = False
 ) -> List[Union[itunes_api.ItunesApiSongModel, itunes_api.ItunesApiAlbumKeys]]:
     """
-    params:
+    Args:
         search_variable (str): the term to search itunes api for
-        limit (int): limit of the search in the api
-        entity (modes.Modes): value of album, or song for now
-        lookup: if true, perform a lookup search via itunes api rather than a default search
+        limit  (int): limit of the search in the api
+        mode (modes.Modes): value of album, or song for now
+        lookup (bool): if true, perform a lookup search via itunes api rather than a default search
+    Returns
+        List[Union[itunes_api.ItunesApiSongModel, itunes_api.ItunesApiAlbumKeys]]: a list containing a
+            tuple with itunes song properties and album properties
     """
     parsed_results_list = []
     result_dict = {}
     if not lookup:  # perform general search
         search_parameters = {
             "term": search_variable,
             "entity": mode.value,
@@ -238,22 +257,22 @@
             logger.warn(
                 f"Skipping the display of song at index [{index}] as it could not be loaded into expected format.\n{e}"
             )
 
     return parsed_results_list
 
 
-def artwork_searcher(url):
+def artwork_searcher(url: str) -> Optional[Response]:
     """Album artwork searcher.
 
     Args:
         url (str): the url for the artwork
 
     Returns:
-        requests.Response: the response for the artwork request
+        Response: the response for the artwork request
     """
     artwork_size_list = [
         "100x100",
         "500x500",
         "1000x1000",
         "1500x1500",
         "2000x2000",
```

### Comparing `songbirdcore-0.0.5/songbirdcore/requirements.txt` & `songbirdcore-0.0.6/songbirdcore/requirements.txt`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.5/songbirdcore/web.py` & `songbirdcore-0.0.6/songbirdcore/web.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional, List, Dict
 import logging
 from requests_html import HTMLSession
 import requests
+from requests import Response
 
 logger = logging.getLogger(__name__)
 
 
 class SimpleSession:
     def __init__(
         self,
@@ -34,21 +35,25 @@
         self.current_url = ""
 
         # initialize a session for this class.. to be used for all requests
         self.s = HTMLSession()
 
     def get_form_inputs(
         self, form_url: str, payload={}, log_calls: Optional[bool] = True
-    ):
+    ) -> Optional[dict]:
         """Get the inputs for a form on a webpage
 
         Args:
             form_url (str): the url for the form
-            user_input_on (bool, optional): _description_. Defaults to True.
-            payload (dict, optional): _description_. Defaults to {}.
+            payload (dict, optional): the payload to insert into the form. Defaults to {}.
+            log_calls (Optional[bool], optional): whether to log information within this method
+
+        Returns:
+            Optional[dict]: a dictionary containing the form
+                inputs for the form_url, updated with payload
         """
         # initialize form_inputs to be empty each request
         form_inputs = {}
         try:
             form_response = self.s.get(form_url, headers=self.headers)
         except requests.exceptions.RequestException as e:
             logger.error(f"Error submitting request to: {form_url}", e)
@@ -83,24 +88,24 @@
         search_url: str,
         form_url: Optional[str] = None,
         payload: Optional[dict] = None,
         render_timeout: Optional[int] = 10,
         render_wait: Optional[float] = 0.2,
         render_sleep: Optional[int] = 1,
         log_calls: Optional[bool] = True,
-    ):
+    ) -> Optional[Response]:
         """
         Enter into a search form for a website
         Args:
             form_url (Optional[str]): the url for the html form. If not passed, uses the root_url for the class.
             search_url (str): the url to perform the search against
             payload (Optional[dict]): optionally include a payload for the request
 
         Returns:
-            requests.Response: the rendered html response
+            Optional[Response]: the rendered html response, or None if failure occurs
         """
         if form_url is None:
             form_url = self.root_url
 
         form_inputs = self.get_form_inputs(form_url, payload, log_calls)
 
         if form_inputs is None:
@@ -108,15 +113,14 @@
         try:
             response = self.s.get(search_url, params=form_inputs, headers=self.headers)
         except requests.exceptions.RequestException as e:
             logger.error(f"Error submitting request to: {search_url}", e)
             return None
 
         logger.debug("Rendering html for : " + response.url)
-        # TODO: FIX RENDER TIMEOUT ISSUE
         response.html.render(
             timeout=render_timeout, wait=render_wait, sleep=render_sleep
         )
         logger.debug("Rendering complete for : " + response.url)
 
         response.close()
         return response
```

### Comparing `songbirdcore-0.0.5/songbirdcore/youtube.py` & `songbirdcore-0.0.6/songbirdcore/youtube.py`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.5/songbirdcore.egg-info/PKG-INFO` & `songbirdcore-0.0.6/songbirdcore.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songbirdcore
-Version: 0.0.5
+Version: 0.0.6
 Summary: core low level api for songbird
 Author: Christian Boin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: beautifulsoup4==4.12.3
@@ -60,28 +60,36 @@
 Requires-Dist: yt-dlp==2024.4.9
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: click; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mike; extra == "dev"
+Requires-Dist: mkdocstrings-python; extra == "dev"
 Provides-Extra: package
 Requires-Dist: build; extra == "package"
 Requires-Dist: twine; extra == "package"
 
 # songbirdcore 🐦
 
 Low-level package with common code used across songbird's
 cli and api.
 
 See: 
 
 - [songbirdcli](https://github.com/cboin1996/songbird.git)
 - [songbirdapi](https://github.com/cboin1996/songbirdapi.git)
 
+## Documentation
+
+`songbirdcore`'s documentation may be found [here](https://cboin1996.github.io/songbirdcore)
+
 ## Requirements
 
 - Python version >= 3.11
 
 ## Installation
 
 To install, run
```

### Comparing `songbirdcore-0.0.5/songbirdcore.egg-info/SOURCES.txt` & `songbirdcore-0.0.6/songbirdcore.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 .gitignore
 LICENSE
 Makefile
 README.md
+markdownlint.yaml
+mkdocs.yml
 pyproject.toml
+.github/workflows/pages.yaml
 .github/workflows/pypi-publish.yaml
 .github/workflows/style.yaml
 .github/workflows/tests.yaml
+docs/index.md
+docs/songbirdcore/common.md
+docs/songbirdcore/gdrive.md
+docs/songbirdcore/itunes.md
+docs/songbirdcore/web.md
+docs/songbirdcore/youtube.md
+docs/songbirdcore/models/itunes_api.md
+docs/songbirdcore/models/modes.md
 songbirdcore/common.py
 songbirdcore/gdrive.py
 songbirdcore/itunes.py
 songbirdcore/requirements.txt
 songbirdcore/requirements.txt.blank
 songbirdcore/version.py
 songbirdcore/web.py
```

### Comparing `songbirdcore-0.0.5/tests/unit/test_youtube.py` & `songbirdcore-0.0.6/tests/unit/test_youtube.py`

 * *Files identical despite different names*

