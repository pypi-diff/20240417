# Comparing `tmp/cuid2-2.0.0.tar.gz` & `tmp/cuid2-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuid2-2.0.0.tar", last modified: Sun May 21 15:33:47 2023, max compression
+gzip compressed data, was "cuid2-2.0.1.tar", last modified: Tue Apr 16 23:51:48 2024, max compression
```

## Comparing `cuid2-2.0.0.tar` & `cuid2-2.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2023-05-21 15:33:27.914489 cuid2-2.0.0/LICENSE
--rw-r--r--   0        0        0     2184 2023-05-21 15:33:27.914489 cuid2-2.0.0/README.md
--rw-r--r--   0        0        0     3827 2023-05-21 15:33:47.286849 cuid2-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      255 2023-05-21 15:33:27.918489 cuid2-2.0.0/src/cuid2/__init__.py
--rw-r--r--   0        0        0      231 2023-05-21 15:33:27.918489 cuid2-2.0.0/src/cuid2/cli.py
--rw-r--r--   0        0        0     4759 2023-05-21 15:33:27.918489 cuid2-2.0.0/src/cuid2/generator.py
--rw-r--r--   0        0        0        0 2023-05-21 15:33:27.918489 cuid2-2.0.0/src/cuid2/py.typed
--rw-r--r--   0        0        0     5816 2023-05-21 15:33:27.918489 cuid2-2.0.0/src/cuid2/utils.py
--rw-r--r--   0        0        0     4183 1970-01-01 00:00:00.000000 cuid2-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-16 23:51:34.634870 cuid2-2.0.1/LICENSE
+-rw-r--r--   0        0        0     2184 2024-04-16 23:51:34.634870 cuid2-2.0.1/README.md
+-rw-r--r--   0        0        0     4001 2024-04-16 23:51:48.298983 cuid2-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      256 2024-04-16 23:51:34.634870 cuid2-2.0.1/src/cuid2/__init__.py
+-rw-r--r--   0        0        0      231 2024-04-16 23:51:34.634870 cuid2-2.0.1/src/cuid2/cli.py
+-rw-r--r--   0        0        0     4771 2024-04-16 23:51:34.634870 cuid2-2.0.1/src/cuid2/generator.py
+-rw-r--r--   0        0        0        0 2024-04-16 23:51:34.634870 cuid2-2.0.1/src/cuid2/py.typed
+-rw-r--r--   0        0        0     5844 2024-04-16 23:51:34.634870 cuid2-2.0.1/src/cuid2/utils.py
+-rw-r--r--   0        0        0     4183 1970-01-01 00:00:00.000000 cuid2-2.0.1/PKG-INFO
```

### Comparing `cuid2-2.0.0/LICENSE` & `cuid2-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cuid2-2.0.0/README.md` & `cuid2-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cuid2-2.0.0/pyproject.toml` & `cuid2-2.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -27,170 +27,178 @@
     "crypt",
     "security",
     "uuid",
     "guid",
     "cuid",
     "cryptography",
 ]
-version = "2.0.0"
+version = "2.0.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 repository = "https://github.com/gordon-code/cuid2/"
 
 [project.scripts]
 cuid2 = "cuid2.cli:main"
 
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.scripts]
-black = "black {args:src/ local/tests/}"
-ruff = "ruff check --fix --exit-zero {args:src/ local/tests/}"
+ruff-check = "ruff check --fix --exit-zero {args:src/ local/tests/}"
+ruff-format = "ruff format {args:src/ local/tests/}"
 spelling = "codespell {args:src/ local/tests/}"
 pylint = "pylint {args:src/ local/tests/}"
-safety = "safety check --bare"
+safety = "safety {args:check --bare}"
 typing = "mypy {args:src/ local/tests/}"
+update-pip = "pip install --upgrade pip"
 testing = "pytest local/tests"
 testing-slow = "pytest local/tests --runslow"
 tox = "tox --parallel auto"
 
-[tool.pdm.scripts.lint-fast]
+[tool.pdm.scripts.ruff-fix]
 composite = [
-    "black",
-    "ruff",
+    "ruff-check",
+    "ruff-format",
 ]
 
 [tool.pdm.scripts.lint-full]
 composite = [
-    "lint-fast",
+    "ruff-fix",
     "spelling",
     "pylint",
     "typing",
     "safety",
 ]
 
+[tool.pdm.scripts.tox-full]
+composite = [
+    "update-pip",
+    "lint-full",
+]
+
 [tool.pdm.dev-dependencies]
 lint = [
-    "black~=23.3.0",
-    "codespell~=2.2.4",
-    "pylint~=2.17.4",
-    "ruff~=0.0.269",
-    "safety==2.4.0b1",
+    "codespell~=2.2.6",
+    "pylint~=3.1.0",
+    "requests>=2.31.0",
+    "ruff~=0.3.7",
+    "safety==3.1.0",
 ]
 test = [
-    "pytest~=7.3.1",
-    "pytest-mock~=3.10.0",
-    "pytest-sugar~=0.9.7",
+    "pytest~=8.1.1",
+    "pytest-mock~=3.14.0",
+    "pytest-sugar~=1.0.0",
 ]
 tox = [
-    "tox~=4.4.12",
-    "tox-pdm~=0.6.1",
+    "tox~=4.14.2",
+    "tox-pdm~=0.7.2",
 ]
 typing = [
-    "mypy~=1.3.0",
+    "mypy~=1.9.0",
 ]
 
 [tool.tox]
-legacy_tox_ini = "    [tox]\n    min_version = 4\n    env_list = py3{8,9,10,11}, check\n    work_dir = local/.tox\n    isolated_build = True\n\n    [testenv]\n    description = run unit tests\n    groups = test\n    commands = testing\n\n    [testenv:check]\n    description = run linters and typing\n    skip_install = true\n    groups = lint, typing, test\n    commands = lint-full\n"
-
-[tool.black]
-line-length = 120
-target_version = [
-    "py38",
-]
+legacy_tox_ini = "    [tox]\n    min_version = 4\n    env_list = py3{8,9,10,11,12}, check\n    work_dir = local/.tox\n    isolated_build = True\n\n    [testenv]\n    description = run unit tests\n    groups = test\n    commands = testing\n\n    [testenv:check]\n    description = run linters and typing\n    skip_install = true\n    groups = lint, typing, test\n    commands = tox-full\n"
 
 [tool.ruff]
 line-length = 120
 src = [
     "src",
 ]
 target-version = "py38"
 cache-dir = "local/.ruff_cache"
-extend-select = [
+force-exclude = true
+
+[tool.ruff.lint]
+select = [
+    "F",
+    "E",
     "W",
     "C90",
     "I",
     "N",
-    "UP",
+    "ASYNC",
+    "TRIO",
     "S",
     "BLE",
     "B",
     "A",
     "COM",
     "C4",
     "DTZ",
     "T10",
     "EM",
+    "FA",
     "ISC",
     "ICN",
     "G",
     "INP",
     "PIE",
     "T20",
     "PT",
     "Q",
     "RSE",
     "RET",
     "SLF",
+    "SLOT",
     "SIM",
     "INT",
     "ARG",
     "PTH",
     "PGH",
     "PL",
     "TRY",
+    "FLY",
+    "PERF",
+    "LOG",
     "RUF",
-    "D",
-    "ANN",
-    "PYI",
-    "TCH",
-    "ERA",
 ]
-extend-ignore = [
+ignore = [
     "D100",
     "D101",
     "D102",
     "D104",
     "D205",
     "D401",
+    "COM812",
+    "ISC001",
 ]
 unfixable = [
     "T201",
     "F401",
     "F841",
 ]
-force-exclude = true
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "test_*.py" = [
     "S101",
     "PLR2004",
     "SLF001",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = [
     "src",
 ]
 section-order = [
     "future",
     "standard-library",
     "third-party",
     "first-party",
     "local-folder",
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.pytest.ini_options]
-minversion = "7.3"
+minversion = "8.1"
 cache_dir = "local/.pytest_cache"
 python_files = "test_*.py"
 
 [tool.pylint.master]
 ignore-patterns = "test_.*.py"
 
 [tool.pylint.format]
```

### Comparing `cuid2-2.0.0/src/cuid2/generator.py` & `cuid2-2.0.1/src/cuid2/generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
+from __future__ import annotations
+
 import time
 from math import floor
 from secrets import SystemRandom
 from typing import TYPE_CHECKING, Callable, Final, Optional, Protocol
 
 from cuid2 import utils
 
 if TYPE_CHECKING:
     from _random import Random
 
     class FingerprintCallable(Protocol):  # pylint: disable=too-few-public-methods
-        def __call__(self: "FingerprintCallable", random_generator: Random) -> str:
-            ...
+        def __call__(self: FingerprintCallable, random_generator: Random) -> str: ...
 
 
 # ~22k hosts before 50% chance of initial counter collision
 # with a remaining counter range of 9.0e+15 in JavaScript.
 INITIAL_COUNT_MAX: Final[int] = 476782367
 DEFAULT_LENGTH: Final = 24
 MAXIMUM_LENGTH: Final = 98
 
 
 class Cuid:  # pylint: disable=too-few-public-methods
     def __init__(
-        self: "Cuid",
-        random_generator: Callable[[], "Random"] = SystemRandom,
+        self: Cuid,
+        random_generator: Callable[[], Random] = SystemRandom,
         counter: Callable[[int], Callable[[], int]] = utils.create_counter,
         length: int = DEFAULT_LENGTH,
-        fingerprint: "FingerprintCallable" = utils.create_fingerprint,
+        fingerprint: FingerprintCallable = utils.create_fingerprint,
     ) -> None:
         """Initialization function for the Cuid class that generates a universally unique,
         base36 encoded string.
 
         Parameters
         ----------
         random_generator : Callable[[], "Random"], default=SystemRandom
@@ -51,20 +52,20 @@
         ValueError
             If the length parameter is greater than `MAXIMUM_LENGTH` (98 characters).
         """
         if length > MAXIMUM_LENGTH:
             msg = "Length must never exceed 98 characters."
             raise ValueError(msg)
 
-        self._random: "Random" = random_generator()
+        self._random: Random = random_generator()
         self._counter: Callable[[], int] = counter(floor(self._random.random() * INITIAL_COUNT_MAX))
         self._length: int = length
         self._fingerprint: str = fingerprint(random_generator=self._random)
 
-    def generate(self: "Cuid", length: Optional[int] = None) -> str:
+    def generate(self: Cuid, length: Optional[int] = None) -> str:
         """Generates a universally unique, base36 encoded string with a specified length.
 
         Parameters
         ----------
         length : int, optional
             The length parameter is an optional integer value that specifies the length of the generated string.
             If it is not provided, the default length value provided during class initialization is used.
```

### Comparing `cuid2-2.0.0/src/cuid2/utils.py` & `cuid2-2.0.1/src/cuid2/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import socket
 import string
 from math import floor
 from typing import TYPE_CHECKING, Callable, Final, Optional
 
 try:
@@ -42,15 +44,15 @@
         nonlocal count
         count += 1
         return count
 
     return counter
 
 
-def create_fingerprint(random_generator: "Random", fingerprint_data: Optional[str] = "") -> str:
+def create_fingerprint(random_generator: Random, fingerprint_data: Optional[str] = "") -> str:
     """Creates a fingerprint, by default combining process ID, hostname, and environment variables
     with entropy and then hashing the result.
 
     Parameters
     ----------
     random_generator : "Random"
         Used as the base generator to generate some entropy.
@@ -72,15 +74,15 @@
 
         fingerprint_data: str = str(process_id) + hostname + env_variables  # type: ignore[no-redef]
 
     fingerprint: str = str(fingerprint_data) + create_entropy(random_generator, BIG_LENGTH)
     return create_hash(fingerprint)[0:BIG_LENGTH]
 
 
-def create_entropy(random_generator: "Random", length: int = 4) -> str:
+def create_entropy(random_generator: Random, length: int = 4) -> str:
     """Creates a random string of specified length using a base36 encoding.
 
     Parameters
     ----------
     random_generator : "Random"
         Used as the base generator to generate a random string.
     length : int, default=4
@@ -122,22 +124,22 @@
 
     Returns
     -------
     str
         Base36 encoding of the SHA-512 hash of the input string `data`, with the first character dropped.
 
     """
-    hashed_value: "_Hash" = sha512(data.encode())
+    hashed_value: _Hash = sha512(data.encode())
     hashed_int: int = int.from_bytes(hashed_value.digest(), byteorder="big")
 
     # Drop the first character because it will bias the histogram to the left.
     return base36_encode(hashed_int)[1:]
 
 
-def create_letter(random_generator: "Random") -> str:
+def create_letter(random_generator: Random) -> str:
     """Generates a random lowercase letter using a given random number generator.
 
     Parameters
     ----------
     random_generator : "Random"
         Used as the base generator to generate a random letter.
```

### Comparing `cuid2-2.0.0/PKG-INFO` & `cuid2-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cuid2
-Version: 2.0.0
+Version: 2.0.1
 Summary: Next generation GUIDs. Collision-resistant ids optimized for horizontal scaling and performance.
-Keywords: crypt security uuid guid cuid cryptography
+Keywords: crypt,security,uuid,guid,cuid,cryptography
 Author-Email: Will Gordon <wgordon@redhat.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Gordon Code
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

