# Comparing `tmp/log-time-to-tempo-0.0.1.tar.gz` & `tmp/log_time_to_tempo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log-time-to-tempo-0.0.1.tar", last modified: Mon Mar 25 08:02:23 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `log-time-to-tempo-0.0.1.tar` & `log_time_to_tempo-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,30 @@
-drwxr-xr-x   0 main       (501) staff       (20)        0 2024-03-25 08:02:23.719833 log-time-to-tempo-0.0.1/
--rw-r--r--   0 main       (501) staff       (20)      779 2024-02-27 18:10:24.000000 log-time-to-tempo-0.0.1/LICENSE
--rw-r--r--   0 main       (501) staff       (20)     4490 2024-03-25 08:02:23.719643 log-time-to-tempo-0.0.1/PKG-INFO
--rw-r--r--   0 main       (501) staff       (20)     2171 2024-03-01 15:20:54.000000 log-time-to-tempo-0.0.1/README.md
--rw-r--r--   0 main       (501) staff       (20)     2839 2024-03-01 12:28:15.000000 log-time-to-tempo-0.0.1/pyproject.toml
--rw-r--r--   0 main       (501) staff       (20)       38 2024-03-25 08:02:23.719879 log-time-to-tempo-0.0.1/setup.cfg
-drwxr-xr-x   0 main       (501) staff       (20)        0 2024-03-25 08:02:23.711566 log-time-to-tempo-0.0.1/src/
-drwxr-xr-x   0 main       (501) staff       (20)        0 2024-03-25 08:02:23.713791 log-time-to-tempo-0.0.1/src/log_time_to_tempo/
--rw-r--r--   0 main       (501) staff       (20)       71 2024-02-26 08:26:30.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo/__init__.py
--rw-r--r--   0 main       (501) staff       (20)     1103 2024-02-28 13:25:15.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo/_jira.py
--rw-r--r--   0 main       (501) staff       (20)       50 2024-02-21 15:49:58.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo/_logging.py
--rw-r--r--   0 main       (501) staff       (20)     5966 2024-03-25 07:58:57.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo/_time.py
--rw-r--r--   0 main       (501) staff       (20)     2290 2024-03-01 14:57:47.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo/caching.py
-drwxr-xr-x   0 main       (501) staff       (20)        0 2024-03-25 08:02:23.715968 log-time-to-tempo-0.0.1/src/log_time_to_tempo/cli/
--rw-r--r--   0 main       (501) staff       (20)     1537 2024-03-01 14:08:00.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo/cli/__init__.py
--rw-r--r--   0 main       (501) staff       (20)     1418 2024-03-01 11:40:05.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo/cli/completions.py
--rw-r--r--   0 main       (501) staff       (20)     4723 2024-03-01 08:02:24.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo/cli/config.py
--rw-r--r--   0 main       (501) staff       (20)     9726 2024-03-04 08:24:21.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo/cli/main.py
--rw-r--r--   0 main       (501) staff       (20)     1783 2024-02-27 17:21:25.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo/tempo.py
-drwxr-xr-x   0 main       (501) staff       (20)        0 2024-03-25 08:02:23.719127 log-time-to-tempo-0.0.1/src/log_time_to_tempo.egg-info/
--rw-r--r--   0 main       (501) staff       (20)     4490 2024-03-25 08:02:23.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo.egg-info/PKG-INFO
--rw-r--r--   0 main       (501) staff       (20)     1007 2024-03-25 08:02:23.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo.egg-info/SOURCES.txt
--rw-r--r--   0 main       (501) staff       (20)        1 2024-03-25 08:02:23.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo.egg-info/dependency_links.txt
--rw-r--r--   0 main       (501) staff       (20)       96 2024-03-25 08:02:23.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo.egg-info/entry_points.txt
--rw-r--r--   0 main       (501) staff       (20)      131 2024-03-25 08:02:23.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo.egg-info/requires.txt
--rw-r--r--   0 main       (501) staff       (20)       41 2024-03-25 08:02:23.000000 log-time-to-tempo-0.0.1/src/log_time_to_tempo.egg-info/top_level.txt
-drwxr-xr-x   0 main       (501) staff       (20)        0 2024-03-25 08:02:23.716641 log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/
-drwxr-xr-x   0 main       (501) staff       (20)        0 2024-03-25 08:02:23.717418 log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/_jira/
--rw-r--r--   0 main       (501) staff       (20)      837 2024-03-01 11:41:02.000000 log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/_jira/conftest.py
--rw-r--r--   0 main       (501) staff       (20)      826 2024-03-01 11:41:37.000000 log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/_jira/test_jira.py
-drwxr-xr-x   0 main       (501) staff       (20)        0 2024-03-25 08:02:23.718780 log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/cli/
--rw-r--r--   0 main       (501) staff       (20)     1113 2024-03-01 10:52:57.000000 log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/cli/conftest.py
--rw-r--r--   0 main       (501) staff       (20)      584 2024-02-27 14:45:57.000000 log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/cli/test_cli_config.py
--rw-r--r--   0 main       (501) staff       (20)     4007 2024-03-01 13:35:05.000000 log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/cli/test_cli_log.py
--rw-r--r--   0 main       (501) staff       (20)       47 2024-03-01 11:01:02.000000 log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/cli/test_cli_main.py
--rw-r--r--   0 main       (501) staff       (20)     3153 2024-03-01 14:13:17.000000 log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/test_cache.py
--rw-r--r--   0 main       (501) staff       (20)     5835 2024-03-25 07:57:04.000000 log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/test_time.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   443365 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/logo.png
+-rw-r--r--   0        0        0   160666 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/logo.webp
+-rw-r--r--   0        0        0    92529 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/logo_256.png
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/.vscode/launch.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/log_time_to_tempo/__init__.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/log_time_to_tempo/_jira.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/log_time_to_tempo/_logging.py
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/log_time_to_tempo/_time.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/log_time_to_tempo/caching.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/log_time_to_tempo/tempo.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/log_time_to_tempo/cli/__init__.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/log_time_to_tempo/cli/completions.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/log_time_to_tempo/cli/config.py
+-rw-r--r--   0        0        0     9889 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/log_time_to_tempo/cli/main.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/test_cache.py
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/test_time.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/_jira/conftest.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/_jira/test_jira.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/cli/conftest.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/cli/test_cli_config.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/cli/test_cli_log.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/cli/test_cli_main.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/.gitignore
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/README.md
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 log_time_to_tempo-0.0.2/PKG-INFO
```

### Comparing `log-time-to-tempo-0.0.1/LICENSE` & `log_time_to_tempo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `log-time-to-tempo-0.0.1/PKG-INFO` & `log_time_to_tempo-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: log-time-to-tempo
-Version: 0.0.1
+Version: 0.0.2
 Summary: Log your work time to tempo from the command line.
+Project-URL: Documentation, https://github.com/jannismain/log-time-to-tempo#readme
+Project-URL: Issues, https://github.com/jannismain/log-time-to-tempo/issues
+Project-URL: Source, https://github.com/jannismain/log-time-to-tempo
 Author-email: Jannis Mainczyk <jannis.mainczyk@codecentric.de>
 License: ISC License
         
         Copyright (c) 2024 Jannis Mainczyk <jannis.mainczyk@codecentric.de>
         
         Permission to use, copy, modify, and/or distribute this software for any
         purpose with or without fee is hereby granted, provided that the above
@@ -14,45 +17,41 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
         AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
         INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
         LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
         OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
         PERFORMANCE OF THIS SOFTWARE.
-        
-Project-URL: Documentation, https://github.com/jannismain/log-time-to-tempo#readme
-Project-URL: Issues, https://github.com/jannismain/log-time-to-tempo/issues
-Project-URL: Source, https://github.com/jannismain/log-time-to-tempo
-Keywords: jira,tempo,cli
+License-File: LICENSE
+Keywords: cli,jira,tempo
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: coloredlogs
 Requires-Dist: jira
-Requires-Dist: typer[all]
-Requires-Dist: rich
-Requires-Dist: python-dotenv
 Requires-Dist: keyring
-Requires-Dist: coloredlogs
-Requires-Dist: requests
 Requires-Dist: pydantic
 Requires-Dist: python-dateutil
+Requires-Dist: python-dotenv
+Requires-Dist: requests
+Requires-Dist: rich
+Requires-Dist: typer[all]
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
-Requires-Dist: hypothesis; extra == "test"
-Requires-Dist: ruff; extra == "test"
+Requires-Dist: hypothesis; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: ruff; extra == 'test'
+Description-Content-Type: text/markdown
 
 # Log Time to Tempo
 
 [![PyPI - Version](https://img.shields.io/pypi/v/log-time-to-tempo.svg)](https://pypi.org/project/log-time-to-tempo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/log-time-to-tempo.svg)](https://pypi.org/project/log-time-to-tempo)
 
 -----
@@ -122,14 +121,26 @@
 ```
 
 ## Changes
 
 ### [latest] - 2024-XX-XX
 [latest]: https://gitlab.codecentric.de/jmm/log-time-to-tempo/-/blob/main/README.md
 
+### [0.0.2] - 2024-04-17
+[0.0.2]: https://gitlab.codecentric.de/jmm/log-time-to-tempo/-/blob/0.0.2/README.md
+
+- add `log --lunch` option to reduce the amount of math you have to do in your head when entering your time
+  - lunch will simply be deducted from the total duration and your end time
+- rename `log --from-time '' --to-time ''` options to `log --start '' --end ''`
+- `log --day` is now case-insensitive (so `Mo` will be recognized as `monday`)
+- add `--version` flag
+
+### [0.0.1] - 2024-03-25
+[0.0.1]: https://gitlab.codecentric.de/jmm/log-time-to-tempo/-/blob/0.0.1/README.md
+
 - authorize with JIRA instance using personal access token
   - prompt for token and persist using [`keyring`][python-keyring] package
 - create and list worklogs via tempo's REST API
 - list projects and issues using [`jira`][python-jira] API
 - cache projects and issues for faster responses and shell completion
 
 [python-jira]: https://github.com/pycontribs/jira
```

### Comparing `log-time-to-tempo-0.0.1/pyproject.toml` & `log_time_to_tempo-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
 [project]
 name = "log-time-to-tempo"
-version = "0.0.1"
 description = 'Log your work time to tempo from the command line.'
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["jira", "tempo", "cli"]
 authors = [
   { name = "Jannis Mainczyk", email = "jannis.mainczyk@codecentric.de" },
 ]
+dynamic = ["version"]
 dependencies = [
   "jira",
   "typer[all]",
   "rich",
   "python-dotenv",
   "keyring",
   "coloredlogs",
@@ -41,22 +45,27 @@
 Issues = "https://github.com/jannismain/log-time-to-tempo/issues"
 Source = "https://github.com/jannismain/log-time-to-tempo"
 
 [project.scripts]
 log-time = "log_time_to_tempo.cli.main:app"
 lt = "log_time_to_tempo.cli.main:app"
 
+[tool.hatch.version]
+path = "src/log_time_to_tempo/__init__.py"
+
 [tool.hatch.envs.default]
 dependencies = ["ruff"]
 [tool.hatch.envs.default.scripts]
 test = "hatch run test:test"
+release = "hatch run test:release"
 
 [tool.hatch.envs.test]
 dependencies = ["pytest", "pytest-cov", "hypothesis"]
-scripts = { "test" = "pytest --cov-config=pyproject.toml --cov-report=term --cov-report html:build/coverage --cov=log_time_to_tempo --cov-report xml" }
+[tool.hatch.envs.test.scripts]
+test = "pytest --cov-config=pyproject.toml --cov-report=term --cov-report html:build/coverage --cov=log_time_to_tempo --cov-report xml"
 release = """\
 hatch run test:test
 git tag -m 'bump version to '`hatch version` v`hatch version` --sign
 git push --tags
 echo "Forgot anything? Press CTRL+C to abort..."
 sleep 5
 hatch build --clean
```

### Comparing `log-time-to-tempo-0.0.1/src/log_time_to_tempo/_jira.py` & `log_time_to_tempo-0.0.2/src/log_time_to_tempo/_jira.py`

 * *Files identical despite different names*

### Comparing `log-time-to-tempo-0.0.1/src/log_time_to_tempo/_time.py` & `log_time_to_tempo-0.0.2/src/log_time_to_tempo/_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,16 @@
     date_args = {k: v for k, v in zip(['day', 'month', 'year'], parts)}
     if 'year' in date_args and date_args['year'] < 100:
         date_args['year'] += date.today().year // 100 * 100
     return date.today().replace(**date_args)
 
 
 def parse_past_weekday_relative(value: str) -> date:
+    original_value = value
+    value = value.lower()
     if value == 'today':
         return date.today()
     elif value in {'yesterday', 'y'}:
         return date.today() - timedelta(days=1)
     elif value in {'monday', 'mon', 'mo', 'm', 'montag'}:
         day = MONDAY
     elif value in {'tuesday', 'tue', 'tu', 'di', 'dienstag'}:
@@ -77,15 +79,15 @@
     elif value in {'wednesday', 'wed', 'we', 'w', 'mi', 'mittwoch'}:
         day = WEDNESDAY
     elif value in {'thursday', 'thu', 'th', 'do', 'donnerstag'}:
         day = THURSDAY
     elif value in {'friday', 'fri', 'fr', 'f', 'freitag'}:
         day = FRIDAY
     else:
-        raise ValueError(f'Unknown relative date: {value}')
+        raise ValueError(f'Unknown relative date: {original_value}')
     # if day is in the future, assume last week
     if day > date.today().weekday():
         return date.today() - timedelta(weeks=1, days=date.today().weekday() - day)
     else:
         return date.today() - timedelta(days=date.today().weekday() - day)
```

### Comparing `log-time-to-tempo-0.0.1/src/log_time_to_tempo/caching.py` & `log_time_to_tempo-0.0.2/src/log_time_to_tempo/caching.py`

 * *Files identical despite different names*

### Comparing `log-time-to-tempo-0.0.1/src/log_time_to_tempo/cli/__init__.py` & `log_time_to_tempo-0.0.2/src/log_time_to_tempo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `log-time-to-tempo-0.0.1/src/log_time_to_tempo/cli/completions.py` & `log_time_to_tempo-0.0.2/src/log_time_to_tempo/cli/completions.py`

 * *Files identical despite different names*

### Comparing `log-time-to-tempo-0.0.1/src/log_time_to_tempo/cli/config.py` & `log_time_to_tempo-0.0.2/src/log_time_to_tempo/cli/config.py`

 * *Files identical despite different names*

### Comparing `log-time-to-tempo-0.0.1/src/log_time_to_tempo/cli/main.py` & `log_time_to_tempo-0.0.2/src/log_time_to_tempo/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,23 @@
 import keyring
 import rich
 import typer
 from keyring.errors import PasswordDeleteError
 from rich.table import Table
 from typing_extensions import Annotated
 
-from .. import _jira, _time, caching, cfg, name, tempo
+from .. import __version__, _jira, _time, caching, cfg, name, tempo
 from .._logging import log
 from . import app, config, error, link
 from .completions import complete_issue, complete_project
 
 token_found_in_environment = os.getenv('JIRA_API_TOKEN')
 config.load()
 
 
-def cb_duration(ctx: typer.Context, value: str) -> timedelta:
-    if value:
-        return _time.parse_duration(value)
-
-
 @app.callback(
     invoke_without_command=True,
     context_settings=dict(auto_envvar_prefix=name.upper(), show_default=False),
 )
 def main(
     ctx: typer.Context,
     token: Annotated[str, typer.Option(envvar='JIRA_API_TOKEN', show_default='prompt')] = None,
@@ -41,14 +36,17 @@
             show_envvar=False,
             show_default=False,
             help='Show logging output',
         ),
     ] = 0,
     persist_token: Annotated[bool, typer.Option(hidden=True)] = True,
     cache: Annotated[bool, typer.Option(hidden=True)] = True,
+    version: Annotated[
+        bool, typer.Option('--version', callback=lambda v: print(__version__) if v else None)
+    ] = False,
 ):
     """Log time to tempo."""
     if ctx.resilient_parsing:  # script is running for completion purposes, nocov
         return
     ctx.obj = cfg  # make the config object available to subcommands
     if verbose:
         import coloredlogs
@@ -118,44 +116,47 @@
     ] = '8',
     issue: Annotated[
         str, typer.Argument(envvar='LT_LOG_ISSUE', shell_complete=complete_issue)
     ] = 'TSI-7',
     day: Annotated[
         date, typer.Option(parser=_time.parse_date, show_envvar=False, show_default='today')
     ] = datetime.now().date(),
-    from_time: Annotated[time, typer.Option(parser=_time.parse_time, show_default='9')] = None,
-    to_time: Annotated[time, typer.Option(parser=_time.parse_time)] = None,
+    start: Annotated[time, typer.Option(parser=_time.parse_time, show_default='9')] = None,
+    end: Annotated[time, typer.Option(parser=_time.parse_time)] = None,
+    lunch: Annotated[timedelta, typer.Option(parser=_time.parse_duration)] = None,
     message: Annotated[str, typer.Option('--message', '-m')] = None,
     yes: Annotated[bool, typer.Option('--yes', '-y', help='log time without confirmation')] = False,
 ):
     "Log time entry."
     if ctx.resilient_parsing:  # script is running for completion purposes
         return
     cfg = ctx.obj
     cfg.issue = cfg.jira.issue(issue, fields='summary,comment')
 
     worklogs = tempo.get_worklogs(ctx.obj.myself['key'], day, day)
     seconds_logged = sum(worklog.timeSpentSeconds for worklog in worklogs)
     duration_logged = timedelta(seconds=seconds_logged)
-    if worklogs and from_time is None:
+    if worklogs and start is None:
         last_worklog = worklogs[-1]
-        from_time = (last_worklog.started + timedelta(seconds=last_worklog.timeSpentSeconds)).time()
-    elif from_time is None:
-        from_time = _time.parse_time(os.getenv('LT_LOG_FROM_TIME', '9'))
-
-    started = datetime.combine(day, from_time)
-    if to_time is not None:
-        duration = datetime.combine(day, to_time) - started
-    else:
-        to_time = (started + duration).time()
+        start = (last_worklog.started + timedelta(seconds=last_worklog.timeSpentSeconds)).time()
+    elif start is None:
+        start = _time.parse_time(os.getenv('LT_LOG_START', '9'))
+    started = datetime.combine(day, start)
+    if end is not None:
+        duration = datetime.combine(day, end) - started
+    if end is None:
+        end = (started + duration).time()
+    if lunch:
+        duration -= lunch
+        end = (datetime.combine(day, end) - lunch).time()
 
     rich.print(
         'Log',
         _time.format_duration(duration),
-        f'({from_time.strftime('%H:%M')} - {to_time.strftime('%H:%M')})',
+        f'({start.strftime('%H:%M')} - {end.strftime('%H:%M')})',
         f'as [italic]{cfg.issue.fields.summary} ({cfg.issue.key})[/italic]',
         f'for {_time.format_date_relative(day)}',
     )
 
     if duration_logged + duration > timedelta(hours=10):
         error(
             f'You already have {_time.format_duration(duration_logged)} logged on that day. Cannot log more than 10h per day.'
```

### Comparing `log-time-to-tempo-0.0.1/src/log_time_to_tempo/tempo.py` & `log_time_to_tempo-0.0.2/src/log_time_to_tempo/tempo.py`

 * *Files identical despite different names*

### Comparing `log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/_jira/conftest.py` & `log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/_jira/conftest.py`

 * *Files identical despite different names*

### Comparing `log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/_jira/test_jira.py` & `log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/_jira/test_jira.py`

 * *Files identical despite different names*

### Comparing `log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/cli/conftest.py` & `log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/cli/test_cli_config.py` & `log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/cli/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/cli/test_cli_log.py` & `log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/cli/test_cli_log.py`

 * *Files identical despite different names*

### Comparing `log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/test_cache.py` & `log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/test_cache.py`

 * *Files identical despite different names*

### Comparing `log-time-to-tempo-0.0.1/src/test_log_time_to_tempo/test_time.py` & `log_time_to_tempo-0.0.2/src/test_log_time_to_tempo/test_time.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,16 @@
         # trailing dot should be stripped before parsing
         ('22.2.', date(year=date.today().year, month=2, day=22)),
         # default values might be None or date object -> should be passed through.
         (None, None),
         (date(year=2022, month=2, day=22), date(year=2022, month=2, day=22)),
         ('today', date.today()),
         ('yesterday', date.today() - timedelta(days=1)),
+        ('y', date.today() - timedelta(days=1)),
+        ('Y', date.today() - timedelta(days=1)),
     ],
 )
 def test_parse_date(given, expected):
     assert _time.parse_date(given) == expected
 
 
 @pytest.mark.parametrize(
```

