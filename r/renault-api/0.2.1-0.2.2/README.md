# Comparing `tmp/renault_api-0.2.1.tar.gz` & `tmp/renault_api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renault_api-0.2.1.tar", max compression
+gzip compressed data, was "renault_api-0.2.2.tar", max compression
```

## Comparing `renault_api-0.2.1.tar` & `renault_api-0.2.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1078 2023-12-14 08:50:37.327698 renault_api-0.2.1/LICENSE.rst
--rw-r--r--   0        0        0     5197 2023-12-14 08:50:37.327698 renault_api-0.2.1/README.rst
--rw-r--r--   0        0        0     3832 2023-12-14 08:50:47.627678 renault_api-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       19 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/__init__.py
--rw-r--r--   0        0        0       19 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/__init__.py
--rw-r--r--   0        0        0     7178 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/__main__.py
--rw-r--r--   0        0        0       19 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/charge/__init__.py
--rw-r--r--   0        0        0      404 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/charge/commands.py
--rw-r--r--   0        0        0     1660 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/charge/control.py
--rw-r--r--   0        0        0     3900 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/charge/history.py
--rw-r--r--   0        0        0     6996 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/charge/schedule.py
--rw-r--r--   0        0        0     6415 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/helpers.py
--rw-r--r--   0        0        0       19 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/hvac/__init__.py
--rw-r--r--   0        0        0      300 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/hvac/commands.py
--rw-r--r--   0        0        0     1484 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/hvac/control.py
--rw-r--r--   0        0        0     1432 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/hvac/history.py
--rw-r--r--   0        0        0     4202 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/renault_account.py
--rw-r--r--   0        0        0     5635 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/renault_client.py
--rw-r--r--   0        0        0     1821 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/renault_settings.py
--rw-r--r--   0        0        0    13061 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/cli/renault_vehicle.py
--rw-r--r--   0        0        0     8205 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/const.py
--rw-r--r--   0        0        0      760 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/credential.py
--rw-r--r--   0        0        0     4189 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/credential_store.py
--rw-r--r--   0        0        0      289 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/exceptions.py
--rw-r--r--   0        0        0     3318 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/gigya/__init__.py
--rw-r--r--   0        0        0      603 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/gigya/exceptions.py
--rw-r--r--   0        0        0     2829 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/gigya/models.py
--rw-r--r--   0        0        0      616 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/gigya/schemas.py
--rw-r--r--   0        0        0     4290 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/helpers.py
--rw-r--r--   0        0        0    10968 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/kamereon/__init__.py
--rw-r--r--   0        0        0      688 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/kamereon/enums.py
--rw-r--r--   0        0        0     1336 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/kamereon/exceptions.py
--rw-r--r--   0        0        0     1869 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/kamereon/helpers.py
--rw-r--r--   0        0        0    22093 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/kamereon/models.py
--rw-r--r--   0        0        0     4087 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/kamereon/schemas.py
--rw-r--r--   0        0        0      672 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/models.py
--rw-r--r--   0        0        0        0 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/py.typed
--rw-r--r--   0        0        0     2807 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/renault_account.py
--rw-r--r--   0        0        0     2410 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/renault_client.py
--rw-r--r--   0        0        0    10287 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/renault_session.py
--rw-r--r--   0        0        0    21852 2023-12-14 08:50:37.331698 renault_api-0.2.1/src/renault_api/renault_vehicle.py
--rw-r--r--   0        0        0     6252 1970-01-01 00:00:00.000000 renault_api-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-17 06:31:37.718461 renault_api-0.2.2/LICENSE.rst
+-rw-r--r--   0        0        0     5253 2024-04-17 06:31:37.718461 renault_api-0.2.2/README.rst
+-rw-r--r--   0        0        0     4555 2024-04-17 06:31:50.662495 renault_api-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       19 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/__init__.py
+-rw-r--r--   0        0        0       19 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/__init__.py
+-rw-r--r--   0        0        0     7178 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/__main__.py
+-rw-r--r--   0        0        0       19 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/charge/__init__.py
+-rw-r--r--   0        0        0      405 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/charge/commands.py
+-rw-r--r--   0        0        0     1661 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/charge/control.py
+-rw-r--r--   0        0        0     3901 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/charge/history.py
+-rw-r--r--   0        0        0     7029 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/charge/schedule.py
+-rw-r--r--   0        0        0     6415 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/helpers.py
+-rw-r--r--   0        0        0       19 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/hvac/__init__.py
+-rw-r--r--   0        0        0      301 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/hvac/commands.py
+-rw-r--r--   0        0        0     1485 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/hvac/control.py
+-rw-r--r--   0        0        0     1433 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/hvac/history.py
+-rw-r--r--   0        0        0     4203 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/renault_account.py
+-rw-r--r--   0        0        0     5636 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/renault_client.py
+-rw-r--r--   0        0        0     1818 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/renault_settings.py
+-rw-r--r--   0        0        0    13062 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/cli/renault_vehicle.py
+-rw-r--r--   0        0        0     8206 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/const.py
+-rw-r--r--   0        0        0      761 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/credential.py
+-rw-r--r--   0        0        0     4190 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/credential_store.py
+-rw-r--r--   0        0        0      289 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/exceptions.py
+-rw-r--r--   0        0        0     3142 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/gigya/__init__.py
+-rw-r--r--   0        0        0      604 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/gigya/exceptions.py
+-rw-r--r--   0        0        0     2830 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/gigya/models.py
+-rw-r--r--   0        0        0      616 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/gigya/schemas.py
+-rw-r--r--   0        0        0     4291 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/helpers.py
+-rw-r--r--   0        0        0    10936 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/kamereon/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/kamereon/enums.py
+-rw-r--r--   0        0        0     1337 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/kamereon/exceptions.py
+-rw-r--r--   0        0        0     1810 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/kamereon/helpers.py
+-rw-r--r--   0        0        0    22094 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/kamereon/models.py
+-rw-r--r--   0        0        0     4087 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/kamereon/schemas.py
+-rw-r--r--   0        0        0      673 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/models.py
+-rw-r--r--   0        0        0        0 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/py.typed
+-rw-r--r--   0        0        0     2807 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/renault_account.py
+-rw-r--r--   0        0        0     2410 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/renault_client.py
+-rw-r--r--   0        0        0    10287 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/renault_session.py
+-rw-r--r--   0        0        0    20451 2024-04-17 06:31:37.722461 renault_api-0.2.2/src/renault_api/renault_vehicle.py
+-rw-r--r--   0        0        0     6355 1970-01-01 00:00:00.000000 renault_api-0.2.2/PKG-INFO
```

### Comparing `renault_api-0.2.1/LICENSE.rst` & `renault_api-0.2.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `renault_api-0.2.1/README.rst` & `renault_api-0.2.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Renault API
 ===========
 
 |PyPI| |Python Version| |License|
 
 |Read the Docs| |Tests| |Codecov|
 
-|pre-commit| |Black|
+|pre-commit| |Ruff|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/renault-api.svg
    :target: https://pypi.org/project/renault-api/
    :alt: PyPI
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/renault-api
    :target: https://pypi.org/project/renault-api
    :alt: Python Version
@@ -24,17 +24,17 @@
    :alt: Tests
 .. |Codecov| image:: https://codecov.io/gh/hacf-fr/renault-api/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/hacf-fr/renault-api
    :alt: Codecov
 .. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
-.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Black
+.. |Ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
 
 
 Features
 --------
 
 This Python package manages the communication with the private Renault API used by the official MyRenault application.
```

### Comparing `renault_api-0.2.1/pyproject.toml` & `renault_api-0.2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "renault-api"
-version = "0.2.1"
+version = "0.2.2"
 description = "Renault API"
 authors = ["epenet"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/hacf-fr/renault-api"
 repository = "https://github.com/hacf-fr/renault-api"
 documentation = "https://renault-api.readthedocs.io"
@@ -20,51 +20,45 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 #ensure aiohttp is greater than 3.8.5 to account for CVE-2023-30589
 aiohttp = ">=3.8.5"
 # Warning: as of 2022-05-16, pyjwt is pinned to 2.4.0 on HA-core
 pyjwt = ">=2.4.0"
+#ensure cryptography (for pyjwt) is greater than 42.0.5 to account for PVE-2024-65647
+cryptography = "^42.0.5"
+
 marshmallow-dataclass = ">=8.2.0"
 click = { version = ">=8.0.1", optional = true }
 tabulate = { version = ">=0.8.7", optional = true }
 dateparser = {version = ">=1.0.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.3.1"
+pytest = ">=7.3.1,<9.0.0"
 coverage = {extras = ["toml"], version = "^7.2"}
-safety = "^2.3.5"
+safety = ">=2.3.5,<4.0.0"
 mypy = "^1.2"
-typeguard = "^2.13.3"
+typeguard = ">=2.13.3,<5.0.0"
 xdoctest = {extras = ["colors"], version = "^1.1.1"}
 sphinx = ">=4.3.2,<8.0.0"
 sphinx-autobuild = "^2021.3.14"
 pre-commit = ">=2.21,<4.0"
-bandit = "^1.7.5"
-flake8 = ">=4.0.1,<6.0.0"
-black = ">=22.12,<24.0"
-flake8-bugbear = ">=22.12.6,<24.0.0"
-flake8-docstrings = "^1.7.0"
-flake8-rst-docstrings = "^0.3.0"
-pep8-naming = "^0.13.2"
+ruff = ">=0.3.7"
 darglint = "^1.8.1"
-reorder-python-imports = "^3.9.0"
 pre-commit-hooks = ">=4.4,<6.0"
 sphinx-rtd-theme = ">=1.2,<3.0"
 sphinx-click = ">=4.4,<6.0"
 Pygments = "^2.15.0"
-pytest-asyncio = "^0.21.0"
+pytest-asyncio = ">=0.21,<0.24"
 aioresponses = "^0.7.4"
-pytest-cov = "^4.0.0"
+pytest-cov = ">=4,<6"
 #ensure urllib3 (for requests/sphinx) is greater than 1.26.5 to account for CVE-2021-33503
 urllib3 = ">=1.26.15,<3.0.0"
 #ensure certifi (for requests/sphinx) is greater than 2023.7.22 to account for CVE-2023-37920
-certifi = "^2023.7.22"
-#ensure gitpython (for bandit/flake8-bandit) is greater than 3.1.32 to account for CVE-2022-24439
-gitpython = "^3.1.32"
+certifi = ">=2023.7.22,<2025.0.0"
 #ensure setuptools (for safety) is greater than 65.5.1 to account for CVE-2022-40897
 setuptools = ">=67.6.1,<70.0.0"
 #ensure frozenlist (for aiohttp) is greater than 1.3.1 to account for Python 3.11
 frozenlist = "^1.3.1"
 #ensure multidict (for aiohttp) is greater than 6.0.3 to account for Python 3.11
 multidict = "^6.0.3"
 #ensure regex (for dateparser) is greater than 2022.9.11 to account for Python 3.11
@@ -112,10 +106,49 @@
 strict_equality = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
+[tool.ruff]
+line-length = 88
+target-version = "py38"
+
+[tool.ruff.lint]
+ignore = [
+    "A001",    # Variable is shadowing a Python builtin
+    "A002",    # Argument is shadowing a Python builtin
+    "N815",    # Variable in class scope should not be mixedCase
+    "PLR0911", # Too many return statements
+    "PLR0913", # Too many arguments in function definition
+]
+select = [
+    "A",     # flake8-builtins
+    "B",     # flake8-bugbear
+    "C4",    # flake8-comprehensions
+    "C90",   # mccabe
+    "E",     # pycodestyle error
+    "ERA",   # eradicate
+    "F",     # Pyflakes
+    "I",     # isort
+    "N",     # pep8-naming
+    "PL",    # Pylint
+    "PT",    # flake8-pytest-style
+    "UP",    # pyupgrade
+]
+
+[tool.ruff.lint.isort]
+force-single-line = true
+known-local-folder = [
+    "renault_api",
+]
+
+[tool.ruff.lint.mccabe]
+max-complexity = 10
+
+[tool.ruff.lint.pydocstyle]
+convention = "google"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `renault_api-0.2.1/src/renault_api/cli/__main__.py` & `renault_api-0.2.2/src/renault_api/cli/__main__.py`

 * *Ordering differences only*

 * *Files identical despite different names*

```diff
@@ -1,8 +1,9 @@
 """Command-line interface."""
+
 import errno
 import json
 import logging
 import os
 from datetime import datetime
 from io import TextIOWrapper
 from typing import Any
@@ -18,15 +19,14 @@
 from . import renault_client
 from . import renault_settings
 from . import renault_vehicle
 from .charge import commands as charge_commands
 from .hvac import commands as hvac_commands
 from renault_api.credential_store import FileCredentialStore
 
-
 _WARNING_DEBUG_ENABLED = (
     "Debug output enabled. Logs may contain personally identifiable "
     "information and account credentials! Be sure to sanitise these logs "
     "before sending them to a third party or posting them online."
 )
```

### Comparing `renault_api-0.2.1/src/renault_api/cli/charge/control.py` & `renault_api-0.2.2/src/renault_api/cli/charge/control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI function for a vehicle."""
+
 from typing import Any
 from typing import Dict
 from typing import Optional
 
 import aiohttp
 import click
```

### Comparing `renault_api-0.2.1/src/renault_api/cli/charge/history.py` & `renault_api-0.2.2/src/renault_api/cli/charge/history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI function for a vehicle."""
+
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import aiohttp
 import click
```

### Comparing `renault_api-0.2.1/src/renault_api/cli/charge/schedule.py` & `renault_api-0.2.2/src/renault_api/cli/charge/schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI function for a vehicle."""
+
 import re
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 
@@ -13,24 +14,24 @@
 from renault_api.cli import helpers
 from renault_api.cli import renault_vehicle
 from renault_api.kamereon.helpers import DAYS_OF_WEEK
 from renault_api.kamereon.models import ChargeDaySchedule
 from renault_api.kamereon.models import ChargeSchedule
 from renault_api.renault_vehicle import RenaultVehicle
 
-
 _DAY_SCHEDULE_REGEX = re.compile(
     "(?P<prefix>T?)"
     "(?P<hours>[0-2][0-9])"
     ":"
     "(?P<minutes>[0-5][0-9])"
     "(?P<suffix>Z?)"
     ","
     "(?P<duration>[0-9]+)"
 )
+_HOURS_PER_DAY = 24
 
 
 @click.group()
 def schedule() -> None:
     """Display or update charge schedules."""
     pass
 
@@ -204,15 +205,15 @@
     if not match:  # pragma: no cover
         raise ValueError(
             f"Invalid specification for charge schedule: `{raw}`. "
             "Should be of the form HH:MM,DURATION or THH:MMZ,DURATION"
         )
 
     hours = int(match.group("hours"))
-    if hours > 23:  # pragma: no cover
+    if hours >= _HOURS_PER_DAY:  # pragma: no cover
         raise ValueError(
             f"Invalid specification for charge schedule: `{raw}`. "
             "Hours should be less than 24."
         )
     minutes = int(match.group("minutes"))
     if (minutes % 15) != 0:  # pragma: no cover
         raise ValueError(
```

### Comparing `renault_api-0.2.1/src/renault_api/cli/helpers.py` & `renault_api-0.2.2/src/renault_api/cli/helpers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helpers for Renault API."""
+
 import asyncio
 import functools
 from datetime import datetime
 from datetime import timedelta
 from typing import Any
 from typing import Callable
 from typing import Optional
@@ -12,15 +13,14 @@
 import click
 import dateparser
 import tzlocal
 
 from renault_api.exceptions import RenaultException
 from renault_api.kamereon.helpers import DAYS_OF_WEEK
 
-
 _DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def coro_with_websession(func: Callable[..., Any]) -> Callable[..., Any]:
     """Ensure the routine runs on an event loop with a websession."""
 
     async def run_command(func: Callable[..., Any], *args: Any, **kwargs: Any) -> None:
```

### Comparing `renault_api-0.2.1/src/renault_api/cli/hvac/control.py` & `renault_api-0.2.2/src/renault_api/cli/hvac/control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI function for a vehicle."""
+
 from typing import Any
 from typing import Dict
 from typing import Optional
 
 import aiohttp
 import click
 import dateparser
```

### Comparing `renault_api-0.2.1/src/renault_api/cli/hvac/history.py` & `renault_api-0.2.2/src/renault_api/cli/hvac/history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI function for a vehicle."""
+
 from typing import Any
 from typing import Dict
 from typing import Optional
 
 import aiohttp
 import click
```

### Comparing `renault_api-0.2.1/src/renault_api/cli/renault_account.py` & `renault_api-0.2.2/src/renault_api/cli/renault_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI function for a vehicle."""
+
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import aiohttp
```

### Comparing `renault_api-0.2.1/src/renault_api/cli/renault_client.py` & `renault_api-0.2.2/src/renault_api/cli/renault_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Singletons for the CLI."""
+
 import json
 from locale import getdefaultlocale
 from typing import Any
 from typing import Dict
 from typing import Optional
 
 import aiohttp
```

### Comparing `renault_api-0.2.1/src/renault_api/cli/renault_settings.py` & `renault_api-0.2.2/src/renault_api/cli/renault_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Singletons for the CLI."""
+
 import os
 from textwrap import TextWrapper
 from typing import Any
 from typing import Dict
 from typing import Optional
 
 import aiohttp
@@ -43,18 +44,18 @@
         credential_store[CONF_VIN] = Credential(vin)
 
 
 def display_settings(ctx_data: Dict[str, Any]) -> None:
     """Get the current configuration keys."""
     credential_store: CredentialStore = ctx_data["credential_store"]
     wrapper = TextWrapper(width=80)
-    items = list(
+    items = [
         [key, "\n".join(wrapper.wrap(credential_store.get_value(key) or "-"))]
         for key in credential_store._store.keys()
-    )
+    ]
     click.echo(tabulate(items, headers=["Key", "Value"]))
 
 
 def reset() -> None:
     """Clear all credentials/settings from the credential store."""
     try:
         os.remove(os.path.expanduser(CREDENTIAL_PATH))
```

### Comparing `renault_api-0.2.1/src/renault_api/cli/renault_vehicle.py` & `renault_api-0.2.2/src/renault_api/cli/renault_vehicle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI function for a vehicle."""
+
 import json
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
```

### Comparing `renault_api-0.2.1/src/renault_api/const.py` & `renault_api-0.2.2/src/renault_api/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Constants for Renault API."""
+
 CONF_COUNTRY = "country"
 CONF_LOCALE = "locale"
 CONF_GIGYA_APIKEY = "gigya-api-key"
 CONF_GIGYA_URL = "gigya-root-url"
 CONF_KAMEREON_APIKEY = "kamereon-api-key"
 CONF_KAMEREON_URL = "kamereon-root-url"
```

### Comparing `renault_api-0.2.1/src/renault_api/credential.py` & `renault_api-0.2.2/src/renault_api/credential.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Credential dataclass."""
+
 import time
 from dataclasses import dataclass
 
 import jwt
 
 
 @dataclass
```

### Comparing `renault_api-0.2.1/src/renault_api/credential_store.py` & `renault_api-0.2.2/src/renault_api/credential_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Kamereon client for interaction with Renault servers."""
+
 import json
 import os
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import jwt
```

### Comparing `renault_api-0.2.1/src/renault_api/gigya/__init__.py` & `renault_api-0.2.2/src/renault_api/gigya/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Gigya API."""
+
 import logging
 from json import JSONDecodeError
 from typing import Any
-from typing import cast
 from typing import Dict
+from typing import cast
 
 import aiohttp
 from marshmallow.schema import Schema
 
 from . import models
 from . import schemas
 from .exceptions import GigyaException
@@ -26,21 +27,15 @@
     url: str,
     data: Dict[str, Any],
     schema: Schema,
 ) -> models.GigyaResponse:
     """Send request to Gigya."""
     async with websession.request(method, url, data=data) as http_response:
         response_text = await http_response.text()
-        # Disable logging on Gigya, to avoid unnecessary exposure.
-        # _LOGGER.debug(
-        #    "Received Gigya response %s on %s: %s",
-        #    http_response.status,
-        #    url,
-        #    response_text,
-        # )
+        # Don't log on Gigya, to avoid unnecessary exposure.
         try:
             gigya_response: models.GigyaResponse = schema.loads(response_text)
         except JSONDecodeError as err:
             raise GigyaException("Gigya responded with invalid JSON") from err
         # Check for Gigya error
         gigya_response.raise_for_error_code()
         # Check for HTTP error
```

### Comparing `renault_api-0.2.1/src/renault_api/gigya/exceptions.py` & `renault_api-0.2.2/src/renault_api/gigya/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Gigya exceptions."""
+
 from typing import Optional
 
 from renault_api.exceptions import RenaultException
 
 
 class GigyaException(RenaultException):
     """Base exception for Gigya errors."""
```

### Comparing `renault_api-0.2.1/src/renault_api/gigya/models.py` & `renault_api-0.2.2/src/renault_api/gigya/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Gigya models."""
+
 from dataclasses import dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from . import exceptions
```

### Comparing `renault_api-0.2.1/src/renault_api/gigya/schemas.py` & `renault_api-0.2.2/src/renault_api/gigya/schemas.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Gigya schemas."""
+
 import marshmallow_dataclass
 
 from . import models
 from renault_api.models import BaseSchema
 
-
 GigyaResponseSchema = marshmallow_dataclass.class_schema(
     models.GigyaResponse, base_schema=BaseSchema
 )()
 
 
 GigyaLoginResponseSchema = marshmallow_dataclass.class_schema(
     models.GigyaLoginResponse, base_schema=BaseSchema
```

### Comparing `renault_api-0.2.1/src/renault_api/helpers.py` & `renault_api-0.2.2/src/renault_api/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helpers for Renault API."""
+
 import asyncio
 import functools
 import logging
 from typing import Dict
 from typing import Optional
 
 import aiohttp
```

### Comparing `renault_api-0.2.1/src/renault_api/kamereon/__init__.py` & `renault_api-0.2.2/src/renault_api/kamereon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """Kamereon API."""
+
 import logging
 from json import dumps as json_dumps
 from typing import Any
-from typing import cast
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import cast
 from warnings import warn
 
 import aiohttp
 from marshmallow.schema import Schema
 
 from . import models
 from . import schemas
 from .exceptions import KamereonResponseException
 
-
 _LOGGER = logging.getLogger(__name__)
 
 
 _KCA_GET_ENDPOINTS: Dict[str, Any] = {
     "": {"version": 2},
     "battery-status": {"version": 2},
     "charge-history": {"version": 1},
     "charge-mode": {"version": 1},
     "charges": {"version": 1},
     "charging-settings": {"version": 1},
-    "cockpit": {"version": 2},
+    "cockpit": {"version": 1},
     "hvac-history": {"version": 1},
     "hvac-sessions": {"version": 1},
     "hvac-status": {"version": 1},
     "hvac-settings": {"version": 1},
     "location": {"version": 1},
     "lock-status": {"version": 1},
     "notification-settings": {"version": 1},
@@ -142,17 +142,15 @@
             http_response.url,
             response_text,
         )
 
         # Some endpoints return arrays instead of objects.
         # These need to be wrapped in an object.
         if response_text.startswith("["):
-            response_text = (
-                f'{{"{wrap_array_in or "data"}": {response_text}}}'  # noqa: B907
-            )
+            response_text = f'{{"{wrap_array_in or "data"}": {response_text}}}'  # noqa: B907
         if not response_text.startswith("{"):
             # Check for HTTP error
             http_response.raise_for_status()
             raise KamereonResponseException("Invalid JSON", response_text)
 
         kamereon_response: models.KamereonResponse = schema.loads(response_text)
         # Check for Kamereon error
```

### Comparing `renault_api-0.2.1/src/renault_api/kamereon/enums.py` & `renault_api-0.2.2/src/renault_api/kamereon/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Kamereon enums."""
+
 from enum import Enum
 
 
 class ChargeState(Enum):
     """Enum for battery-status charge state."""
 
     NOT_IN_CHARGE = 0.0
```

### Comparing `renault_api-0.2.1/src/renault_api/kamereon/exceptions.py` & `renault_api-0.2.2/src/renault_api/kamereon/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Kamereon exceptions."""
+
 from typing import Optional
 
 from renault_api.exceptions import RenaultException
 
 
 class KamereonException(RenaultException):
     """Base exception for Kamereon errors."""
```

### Comparing `renault_api-0.2.1/src/renault_api/kamereon/helpers.py` & `renault_api-0.2.2/src/renault_api/kamereon/helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """Helpers for Kamereon models."""
+
 from __future__ import annotations
 
 from typing import Any
-from typing import Dict
-from typing import Optional
 
 from . import models
 
 DAYS_OF_WEEK = [
     "monday",
     "tuesday",
     "wednesday",
     "thursday",
     "friday",
     "saturday",
     "sunday",
 ]
 
 
-def update_schedule(schedule: models.ChargeSchedule, settings: Dict[str, Any]) -> None:
+def update_schedule(schedule: models.ChargeSchedule, settings: dict[str, Any]) -> None:
     """Update schedule."""
     if "activated" in settings:
         schedule.activated = settings["activated"]
     for day in DAYS_OF_WEEK:
         if day in settings:
             day_settings = settings[day]
 
@@ -36,31 +35,31 @@
                     schedule,
                     day,
                     models.ChargeDaySchedule(day_settings, start_time, duration),
                 )
 
 
 def create_schedule(
-    settings: Dict[str, Any]
+    settings: dict[str, Any],
 ) -> models.ChargeSchedule:  # pragma: no cover
     """Update schedule."""
     raise NotImplementedError
 
 
-def get_end_time(start_time: str, duration: Optional[int] = None) -> str:
+def get_end_time(start_time: str, duration: int | None = None) -> str:
     """Compute end time."""
     total_minutes = get_total_minutes(start_time, duration)
     return format_time(total_minutes)
 
 
 def format_time(total_minutes: int) -> str:
     """Format time."""
     end_hours, end_minutes = divmod(total_minutes, 60)
     end_hours = end_hours % 24
     return f"T{end_hours:02g}:{end_minutes:02g}Z"
 
 
-def get_total_minutes(start_time: Optional[str], duration: Optional[int] = None) -> int:
+def get_total_minutes(start_time: str | None, duration: int | None = None) -> int:
     """Get total minutes from a `Thh:mmZ` formatted time."""
     if not start_time:  # pragma: no cover
         return 0
     return int(start_time[1:3]) * 60 + int(start_time[4:6]) + (duration or 0)
```

### Comparing `renault_api-0.2.1/src/renault_api/kamereon/models.py` & `renault_api-0.2.2/src/renault_api/kamereon/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Kamereon models."""
+
 import json
 from dataclasses import dataclass
 from typing import Any
-from typing import cast
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import cast
 
 from marshmallow.schema import Schema
 
 from . import enums
 from . import exceptions
 from . import helpers
 from .enums import AssetPictureSize
```

### Comparing `renault_api-0.2.1/src/renault_api/kamereon/schemas.py` & `renault_api-0.2.2/src/renault_api/kamereon/schemas.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Kamereon schemas."""
+
 import marshmallow_dataclass
 
 from . import models
 from renault_api.models import BaseSchema
 
-
 KamereonResponseSchema = marshmallow_dataclass.class_schema(
     models.KamereonResponse, base_schema=BaseSchema
 )()
 
 
 KamereonPersonResponseSchema = marshmallow_dataclass.class_schema(
     models.KamereonPersonResponse, base_schema=BaseSchema
```

### Comparing `renault_api-0.2.1/src/renault_api/models.py` & `renault_api-0.2.2/src/renault_api/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Models for Renault API."""
+
 from dataclasses import dataclass
 from typing import Any
 from typing import Dict
 
 import marshmallow
```

### Comparing `renault_api-0.2.1/src/renault_api/renault_account.py` & `renault_api-0.2.2/src/renault_api/renault_account.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Client for Renault API."""
+
 import logging
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import aiohttp
 
 from .credential_store import CredentialStore
 from .exceptions import RenaultException
 from .kamereon import models
 from .renault_session import RenaultSession
 from .renault_vehicle import RenaultVehicle
 
-
 _LOGGER = logging.getLogger(__name__)
 
 
 class RenaultAccount:
     """Proxy to a Renault account."""
 
     def __init__(
```

### Comparing `renault_api-0.2.1/src/renault_api/renault_client.py` & `renault_api-0.2.2/src/renault_api/renault_client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Client for Renault API."""
+
 import logging
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import aiohttp
 
 from .credential_store import CredentialStore
 from .exceptions import RenaultException
 from .kamereon import models
 from .renault_account import RenaultAccount
 from .renault_session import RenaultSession
 
-
 _LOGGER = logging.getLogger(__name__)
 
 
 class RenaultClient:
     """Proxy to a Renault profile."""
 
     def __init__(
```

### Comparing `renault_api-0.2.1/src/renault_api/renault_session.py` & `renault_api-0.2.2/src/renault_api/renault_session.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Session provider for interaction with Renault servers."""
+
 import asyncio
 import logging
 from typing import Any
 from typing import Dict
 from typing import Optional
 
 import aiohttp
@@ -20,15 +21,14 @@
 from .credential_store import CredentialStore
 from .exceptions import NotAuthenticatedException
 from .exceptions import RenaultException
 from .gigya.exceptions import GigyaResponseException
 from .kamereon import models
 from renault_api.helpers import get_api_keys
 
-
 _LOGGER = logging.getLogger(__name__)
 
 
 class RenaultSession:
     """Renault session for interaction with Renault servers."""
 
     def __init__(
```

### Comparing `renault_api-0.2.1/src/renault_api/renault_vehicle.py` & `renault_api-0.2.2/src/renault_api/renault_vehicle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Client for Renault API."""
+
 import logging
 from datetime import datetime
 from datetime import timezone
-from typing import cast
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import cast
 from warnings import warn
 
 import aiohttp
 
 from .credential_store import CredentialStore
 from .exceptions import RenaultException
 from .kamereon import models
 from .kamereon import schemas
 from .renault_session import RenaultSession
 
-
 _LOGGER = logging.getLogger(__name__)
 
 PERIOD_DAY_FORMAT = "%Y%m%d"
 PERIOD_MONTH_FORMAT = "%Y%m"
 PERIOD_TZ_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
 PERIOD_FORMATS = {"day": PERIOD_DAY_FORMAT, "month": PERIOD_MONTH_FORMAT}
 
@@ -108,149 +108,138 @@
             models.KamereonVehicleCarAdapterData,
             response.get_attributes(schemas.KamereonVehicleCarAdapterDataSchema),
         )
         return self._car_adapter
 
     async def get_contracts(self) -> List[models.KamereonVehicleContract]:
         """Get vehicle contracts."""
-        # await self.warn_on_method("get_contracts")
         if self._contracts:
             return self._contracts
 
         response = await self.session.get_vehicle_contracts(
             account_id=self.account_id,
             vin=self.vin,
         )
         if response.contractList is None:  # pragma: no cover
             raise ValueError("response.contractList is None")
         self._contracts = response.contractList
         return self._contracts
 
     async def get_battery_status(self) -> models.KamereonVehicleBatteryStatusData:
         """Get vehicle battery status."""
-        # await self.warn_on_method("get_battery_status")
         response = await self.session.get_vehicle_data(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="battery-status",
         )
         return cast(
             models.KamereonVehicleBatteryStatusData,
             response.get_attributes(schemas.KamereonVehicleBatteryStatusDataSchema),
         )
 
     async def get_location(self) -> models.KamereonVehicleLocationData:
         """Get vehicle location."""
-        # await self.warn_on_method("get_location")
         response = await self.session.get_vehicle_data(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="location",
         )
         return cast(
             models.KamereonVehicleLocationData,
             response.get_attributes(schemas.KamereonVehicleLocationDataSchema),
         )
 
     async def get_hvac_status(self) -> models.KamereonVehicleHvacStatusData:
         """Get vehicle hvac status."""
-        # await self.warn_on_method("get_hvac_status")
         response = await self.session.get_vehicle_data(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="hvac-status",
         )
         return cast(
             models.KamereonVehicleHvacStatusData,
             response.get_attributes(schemas.KamereonVehicleHvacStatusDataSchema),
         )
 
     async def get_hvac_settings(self) -> models.KamereonVehicleHvacSettingsData:
         """Get vehicle hvac settings (schedule+mode)."""
-        # await self.warn_on_method("get_hvac_settings")
         response = await self.session.get_vehicle_data(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="hvac-settings",
         )
         return cast(
             models.KamereonVehicleHvacSettingsData,
             response.get_attributes(schemas.KamereonVehicleHvacSettingsDataSchema),
         )
 
     async def get_charge_mode(self) -> models.KamereonVehicleChargeModeData:
         """Get vehicle charge mode."""
-        # await self.warn_on_method("get_charge_mode")
         response = await self.session.get_vehicle_data(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="charge-mode",
         )
         return cast(
             models.KamereonVehicleChargeModeData,
             response.get_attributes(schemas.KamereonVehicleChargeModeDataSchema),
         )
 
     async def get_cockpit(self) -> models.KamereonVehicleCockpitData:
         """Get vehicle cockpit."""
-        # await self.warn_on_method("get_cockpit")
         response = await self.session.get_vehicle_data(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="cockpit",
         )
         return cast(
             models.KamereonVehicleCockpitData,
             response.get_attributes(schemas.KamereonVehicleCockpitDataSchema),
         )
 
     async def get_lock_status(self) -> models.KamereonVehicleLockStatusData:
         """Get vehicle lock status."""
-        # await self.warn_on_method("get_lock_status")
         response = await self.session.get_vehicle_data(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="lock-status",
         )
         return cast(
             models.KamereonVehicleLockStatusData,
             response.get_attributes(schemas.KamereonVehicleLockStatusDataSchema),
         )
 
     async def get_res_state(self) -> models.KamereonVehicleResStateData:
         """Get vehicle res state."""
-        # await self.warn_on_method("get_res_state")
         response = await self.session.get_vehicle_data(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="res-state",
         )
         return cast(
             models.KamereonVehicleResStateData,
             response.get_attributes(schemas.KamereonVehicleResStateDataSchema),
         )
 
     async def get_charging_settings(self) -> models.KamereonVehicleChargingSettingsData:
         """Get vehicle charging settings."""
-        # await self.warn_on_method("get_charging_settings")
         response = await self.session.get_vehicle_data(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="charging-settings",
         )
         return cast(
             models.KamereonVehicleChargingSettingsData,
             response.get_attributes(schemas.KamereonVehicleChargingSettingsDataSchema),
         )
 
     async def get_notification_settings(
         self,
     ) -> models.KamereonVehicleNotificationSettingsData:
         """Get vehicle notification settings."""
-        # await self.warn_on_method("get_notification_settings")
         response = await self.session.get_vehicle_data(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="notification-settings",
         )
         return cast(
             models.KamereonVehicleNotificationSettingsData,
@@ -259,26 +248,23 @@
             ),
         )
 
     async def get_charge_history(
         self, start: datetime, end: datetime, period: str
     ) -> models.KamereonVehicleChargeHistoryData:
         """Get vehicle charge history."""
-        # await self.warn_on_method("get_charge_history")
         if not isinstance(start, datetime):  # pragma: no cover
             raise TypeError(
-                "`start` should be an instance of datetime.datetime, not {}".format(
-                    start.__class__
-                )
+                "`start` should be an instance of datetime.datetime, "
+                f"not {start.__class__}"
             )
         if not isinstance(end, datetime):  # pragma: no cover
             raise TypeError(
-                "`end` should be an instance of datetime.datetime, not {}".format(
-                    end.__class__
-                )
+                "`end` should be an instance of datetime.datetime, "
+                f"not {end.__class__}"
             )
         if period not in PERIOD_FORMATS.keys():  # pragma: no cover
             raise TypeError("`period` should be one of `month`, `day`")
 
         params = {
             "type": period,
             "start": start.strftime(PERIOD_FORMATS[period]),
@@ -295,26 +281,23 @@
             response.get_attributes(schemas.KamereonVehicleChargeHistoryDataSchema),
         )
 
     async def get_charges(
         self, start: datetime, end: datetime
     ) -> models.KamereonVehicleChargesData:
         """Get vehicle charges."""
-        # await self.warn_on_method("get_charges")
         if not isinstance(start, datetime):  # pragma: no cover
             raise TypeError(
-                "`start` should be an instance of datetime.datetime, not {}".format(
-                    start.__class__
-                )
+                "`start` should be an instance of datetime.datetime, "
+                f"not {start.__class__}"
             )
         if not isinstance(end, datetime):  # pragma: no cover
             raise TypeError(
-                "`end` should be an instance of datetime.datetime, not {}".format(
-                    end.__class__
-                )
+                "`end` should be an instance of datetime.datetime, "
+                f"not {end.__class__}"
             )
 
         params = {
             "start": start.strftime(PERIOD_DAY_FORMAT),
             "end": end.strftime(PERIOD_DAY_FORMAT),
         }
         response = await self.session.get_vehicle_data(
@@ -328,26 +311,23 @@
             response.get_attributes(schemas.KamereonVehicleChargesDataSchema),
         )
 
     async def get_hvac_history(
         self, start: datetime, end: datetime, period: str
     ) -> models.KamereonVehicleHvacHistoryData:
         """Get vehicle hvac history."""
-        # await self.warn_on_method("get_hvac_history")
         if not isinstance(start, datetime):  # pragma: no cover
             raise TypeError(
-                "`start` should be an instance of datetime.datetime, not {}".format(
-                    start.__class__
-                )
+                "`start` should be an instance of datetime.datetime, "
+                f"not {start.__class__}"
             )
         if not isinstance(end, datetime):  # pragma: no cover
             raise TypeError(
-                "`end` should be an instance of datetime.datetime, not {}".format(
-                    end.__class__
-                )
+                "`end` should be an instance of datetime.datetime, "
+                f"not {end.__class__}"
             )
         if period not in PERIOD_FORMATS.keys():  # pragma: no cover
             raise TypeError("`period` should be one of `month`, `day`")
 
         params = {
             "type": period,
             "start": start.strftime(PERIOD_FORMATS[period]),
@@ -364,26 +344,23 @@
             response.get_attributes(schemas.KamereonVehicleHvacHistoryDataSchema),
         )
 
     async def get_hvac_sessions(
         self, start: datetime, end: datetime
     ) -> models.KamereonVehicleHvacSessionsData:
         """Get vehicle hvac sessions."""
-        # await self.warn_on_method("get_hvac_sessions")
         if not isinstance(start, datetime):  # pragma: no cover
             raise TypeError(
-                "`start` should be an instance of datetime.datetime, not {}".format(
-                    start.__class__
-                )
+                "`start` should be an instance of datetime.datetime, "
+                f"not {start.__class__}"
             )
         if not isinstance(end, datetime):  # pragma: no cover
             raise TypeError(
-                "`end` should be an instance of datetime.datetime, not {}".format(
-                    end.__class__
-                )
+                "`end` should be an instance of datetime.datetime, "
+                f"not {end.__class__}"
             )
 
         params = {
             "start": start.strftime(PERIOD_DAY_FORMAT),
             "end": end.strftime(PERIOD_DAY_FORMAT),
         }
         response = await self.session.get_vehicle_data(
@@ -397,26 +374,24 @@
             response.get_attributes(schemas.KamereonVehicleHvacSessionsDataSchema),
         )
 
     async def set_ac_start(
         self, temperature: float, when: Optional[datetime] = None
     ) -> models.KamereonVehicleHvacStartActionData:
         """Start vehicle ac."""
-        # await self.warn_on_method("set_ac_start")
         attributes = {
             "action": "start",
             "targetTemperature": temperature,
         }
 
         if when:
             if not isinstance(when, datetime):  # pragma: no cover
                 raise TypeError(
-                    "`when` should be an instance of datetime.datetime, not {}".format(
-                        when.__class__
-                    )
+                    "`when` should be an instance of datetime.datetime, "
+                    f"not {when.__class__}"
                 )
             start_date_time = when.astimezone(timezone.utc).strftime(PERIOD_TZ_FORMAT)
             attributes["startDateTime"] = start_date_time
 
         response = await self.session.set_vehicle_action(
             account_id=self.account_id,
             vin=self.vin,
@@ -444,23 +419,21 @@
             response.get_attributes(schemas.KamereonVehicleHvacStartActionDataSchema),
         )
 
     async def set_hvac_schedules(
         self, schedules: List[models.HvacSchedule]
     ) -> models.KamereonVehicleHvacScheduleActionData:
         """Set vehicle charge schedules."""
-        # await self.warn_on_method("set_hvac_schedules")
         for schedule in schedules:
             if not isinstance(schedule, models.HvacSchedule):  # pragma: no cover
                 raise TypeError(
-                    "`schedules` should be a list of HvacSchedule, not {}".format(
-                        schedules.__class__
-                    )
+                    "`schedules` should be a list of HvacSchedule, "
+                    f"not {schedules.__class__}"
                 )
-        attributes = {"schedules": list(schedule.for_json() for schedule in schedules)}
+        attributes = {"schedules": [schedule.for_json() for schedule in schedules]}
 
         response = await self.session.set_vehicle_action(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="actions/hvac-schedule",
             attributes=attributes,
         )
@@ -471,23 +444,21 @@
             ),
         )
 
     async def set_charge_schedules(
         self, schedules: List[models.ChargeSchedule]
     ) -> models.KamereonVehicleChargeScheduleActionData:
         """Set vehicle charge schedules."""
-        # await self.warn_on_method("set_charge_schedules")
         for schedule in schedules:
             if not isinstance(schedule, models.ChargeSchedule):  # pragma: no cover
                 raise TypeError(
-                    "`schedules` should be a list of ChargeSchedule, not {}".format(
-                        schedules.__class__
-                    )
+                    "`schedules` should be a list of ChargeSchedule, "
+                    f"not {schedules.__class__}"
                 )
-        attributes = {"schedules": list(schedule.for_json() for schedule in schedules)}
+        attributes = {"schedules": [schedule.for_json() for schedule in schedules]}
 
         response = await self.session.set_vehicle_action(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="actions/charge-schedule",
             attributes=attributes,
         )
@@ -498,15 +469,14 @@
             ),
         )
 
     async def set_charge_mode(
         self, charge_mode: str
     ) -> models.KamereonVehicleChargeModeActionData:
         """Set vehicle charge mode."""
-        # await self.warn_on_method("set_charge_mode")
         attributes = {"action": charge_mode}
 
         response = await self.session.set_vehicle_action(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="actions/charge-mode",
             attributes=attributes,
@@ -518,15 +488,15 @@
 
     async def set_charge_start(self) -> models.KamereonVehicleChargingStartActionData:
         """Start vehicle charge."""
         details = await self.get_details()
 
         if details.controls_action_via_kcm("charge"):
             attributes = {"action": "resume"}
-            response = response = await self.session.set_vehicle_action(
+            response = await self.session.set_vehicle_action(
                 account_id=self.account_id,
                 vin=self.vin,
                 endpoint="charge/pause-resume",
                 attributes=attributes,
                 adapter_type="kcm",
             )
         else:
@@ -546,15 +516,15 @@
 
     async def set_charge_stop(self) -> models.KamereonVehicleChargingStartActionData:
         """Start vehicle charge."""
         details = await self.get_details()
 
         if details.controls_action_via_kcm("charge"):
             attributes = {"action": "pause"}
-            response = response = await self.session.set_vehicle_action(
+            response = await self.session.set_vehicle_action(
                 account_id=self.account_id,
                 vin=self.vin,
                 endpoint="charge/pause-resume",
                 attributes=attributes,
                 adapter_type="kcm",
             )
         else:
```

### Comparing `renault_api-0.2.1/PKG-INFO` & `renault_api-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renault-api
-Version: 0.2.1
+Version: 0.2.2
 Summary: Renault API
 Home-page: https://github.com/hacf-fr/renault-api
 License: MIT
 Author: epenet
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: cli
 Requires-Dist: aiohttp (>=3.8.5)
 Requires-Dist: click (>=8.0.1) ; extra == "cli"
+Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: dateparser (>=1.0.0) ; extra == "cli"
 Requires-Dist: marshmallow-dataclass (>=8.2.0)
 Requires-Dist: pyjwt (>=2.4.0)
 Requires-Dist: tabulate (>=0.8.7) ; extra == "cli"
 Project-URL: Changelog, https://github.com/hacf-fr/renault-api/releases
 Project-URL: Documentation, https://renault-api.readthedocs.io
 Project-URL: Repository, https://github.com/hacf-fr/renault-api
@@ -28,15 +29,15 @@
 Renault API
 ===========
 
 |PyPI| |Python Version| |License|
 
 |Read the Docs| |Tests| |Codecov|
 
-|pre-commit| |Black|
+|pre-commit| |Ruff|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/renault-api.svg
    :target: https://pypi.org/project/renault-api/
    :alt: PyPI
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/renault-api
    :target: https://pypi.org/project/renault-api
    :alt: Python Version
@@ -51,17 +52,17 @@
    :alt: Tests
 .. |Codecov| image:: https://codecov.io/gh/hacf-fr/renault-api/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/hacf-fr/renault-api
    :alt: Codecov
 .. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
-.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Black
+.. |Ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
 
 
 Features
 --------
 
 This Python package manages the communication with the private Renault API used by the official MyRenault application.
```

