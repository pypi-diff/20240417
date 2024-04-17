# Comparing `tmp/pyproject_fmt-1.7.0.tar.gz` & `tmp/pyproject_fmt-1.8.0.tar.gz`

## Comparing `pyproject_fmt-1.7.0.tar` & `pyproject_fmt-1.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/tox.ini
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/src/pyproject_fmt/__init__.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/src/pyproject_fmt/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/src/pyproject_fmt/_version.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/src/pyproject_fmt/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/src/pyproject_fmt/py.typed
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/build_system.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/config.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/pep508.py
--rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/project.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/tools.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/util.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/tests/__init__.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/tests/test_cli.py
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/tests/test_main.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/tests/test_pyproject_toml_fmt.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/tests/formatter/conftest.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/tests/formatter/test_build_system.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/tests/formatter/test_pep508.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/tests/formatter/test_project.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/tests/formatter/test_tools.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/LICENSE.txt
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/README.md
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pyproject_fmt-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tox.ini
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/__init__.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/_version.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/py.typed
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/__init__.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/build_system.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/config.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/pep508.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/project.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/tools.py
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/util.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/test_cli.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/test_main.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/test_pyproject_toml_fmt.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/formatter/conftest.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/formatter/test_build_system.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/formatter/test_pep508.py
+-rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/formatter/test_project.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/formatter/test_tools.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/README.md
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/PKG-INFO
```

### Comparing `pyproject_fmt-1.7.0/tox.ini` & `pyproject_fmt-1.8.0/tox.ini`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-1.7.0/src/pyproject_fmt/__main__.py` & `pyproject_fmt-1.8.0/src/pyproject_fmt/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Main entry point for the formatter."""
+
 from __future__ import annotations
 
 import difflib
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterable, Sequence
```

### Comparing `pyproject_fmt-1.7.0/src/pyproject_fmt/cli.py` & `pyproject_fmt-1.8.0/src/pyproject_fmt/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI interface parser."""
+
 from __future__ import annotations
 
 import os
 from argparse import (
     ArgumentDefaultsHelpFormatter,
     ArgumentParser,
     ArgumentTypeError,
@@ -47,15 +48,15 @@
     Validate that pyproject.toml can be formatted.
 
     :param argument: the string argument passed in
     :return: the pyproject.toml path
     """
     path = Path(argument).absolute()
     if path.is_dir():
-        path = path / "pyproject.toml"
+        path /= "pyproject.toml"
     if not path.exists():
         msg = "path does not exist"
         raise ArgumentTypeError(msg)
     if not path.is_file():
         msg = "path is not a file"
         raise ArgumentTypeError(msg)
     if not os.access(path, os.R_OK):
@@ -113,10 +114,10 @@
     parser = _build_cli()
     result = PyProjectFmtNamespace()
     parser.parse_args(namespace=result, args=args)
     return result
 
 
 __all__ = [
-    "cli_args",
     "PyProjectFmtNamespace",
+    "cli_args",
 ]
```

### Comparing `pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/__init__.py` & `pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Logic related to how to format."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from tomlkit import parse
 
 from .build_system import fmt_build_system
```

### Comparing `pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/build_system.py` & `pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/build_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Logic related to formatting the build system."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional, cast
 
 from tomlkit.items import Array, Table
 
 from .pep508 import normalize_pep508_array
```

### Comparing `pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/config.py` & `pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Defines configuration for the formatter."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, TypedDict
 
 from packaging.version import Version
 
@@ -53,11 +54,11 @@
             indent=overrides.get("indent", self.indent),
             keep_full_version=overrides.get("keep_full_version", self.keep_full_version),
             max_supported_python=Version(max_supported_version) if max_supported_version else self.max_supported_python,
         )
 
 
 __all__ = [
-    "Config",
     "DEFAULT_INDENT",
     "DEFAULT_MAX_SUPPORTED_PYTHON",
+    "Config",
 ]
```

### Comparing `pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/pep508.py` & `pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/pep508.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Apply package name normalization."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from packaging.requirements import Requirement
 from tomlkit.api import string as toml_string
 
@@ -17,15 +18,15 @@
     Normalize a python requirement.
 
     :param req: the raw requirement
     :return: normalized name
     """
     parsed = Requirement(req)
     for spec in parsed.specifier:
-        if spec.operator in (">=", "=="):
+        if spec.operator in {">=", "=="}:
             version = spec.version
             while version.endswith(".0"):
                 version = version[:-2]
             spec._spec = (spec._spec[0], version)  # noqa: SLF001
     return str(parsed)
 
 
@@ -56,10 +57,10 @@
         normalized = _best_effort_string_repr(req=req_string)
         requires_array[at] = normalized
     # then sort
     sorted_array(requires_array, indent, key=lambda e: Requirement(e.text).name.lower())
 
 
 __all__ = [
-    "normalize_req",
     "normalize_pep508_array",
+    "normalize_req",
 ]
```

### Comparing `pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/project.py` & `pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Format the project table."""
+
 from __future__ import annotations
 
+import operator
 import re
 from shutil import which
-from subprocess import CalledProcessError, check_output
+from subprocess import CalledProcessError, check_output  # noqa: S404
 from typing import TYPE_CHECKING, Optional, cast
 
 from packaging.specifiers import SpecifierSet
 from packaging.utils import canonicalize_name
 from packaging.version import Version
 from tomlkit.items import Array, String, Table, Trivia
 
@@ -16,14 +18,15 @@
 
 if TYPE_CHECKING:
     from tomlkit.toml_document import TOMLDocument
 
     from .config import Config
 
 _PY_MIN_VERSION: int = 7
+_ANY_WHITESPACE = re.compile(r"\s+")
 
 
 def fmt_project(parsed: TOMLDocument, conf: Config) -> None:  # noqa: C901
     """
     Format the project table.
 
     :param parsed: the raw parsed table
@@ -34,15 +37,17 @@
         return
 
     if "name" in project:  # normalize names to hyphen so sdist / wheel have the same prefix
         name = project["name"]
         assert isinstance(name, str)  # noqa: S101
         project["name"] = canonicalize_name(name)
     if "description" in project:
-        project["description"] = String.from_raw(str(project["description"]).strip())
+        # Convert multiline description to a single line
+        _description = _ANY_WHITESPACE.sub(" ", str(project["description"]).strip())
+        project["description"] = String.from_raw(_description, escape=False)
 
     sorted_array(cast(Optional[Array], project.get("keywords")), indent=conf.indent)
     sorted_array(cast(Optional[Array], project.get("dynamic")), indent=conf.indent)
 
     if "requires-python" in project:
         _add_py_classifiers(project, py_max_version=conf.max_supported_python)
 
@@ -57,26 +62,26 @@
         opt_deps = cast(Table, project["optional-dependencies"])
         for value in opt_deps.values():
             normalize_pep508_array(
                 requires_array=cast(Array, value),
                 indent=conf.indent,
                 keep_full_version=conf.keep_full_version,
             )
-        order_keys(opt_deps, (), sort_key=lambda k: k[0])  # pragma: no branch
+        order_keys(opt_deps, (), sort_key=operator.itemgetter(0))  # pragma: no branch
 
     for of_type in ("scripts", "gui-scripts", "entry-points", "urls"):
         if of_type in project:
             table = cast(Table, project[of_type])
-            order_keys(table, (), sort_key=lambda k: k[0])  # pragma: no branch
+            order_keys(table, (), sort_key=operator.itemgetter(0))  # pragma: no branch
 
     if "entry-points" in project:  # order entry points sub-table
         entry_points = cast(Table, project["entry-points"])
-        order_keys(entry_points, (), sort_key=lambda k: k[0])  # pragma: no branch
+        order_keys(entry_points, (), sort_key=operator.itemgetter(0))  # pragma: no branch
         for entry_point in entry_points.values():
-            order_keys(entry_point, (), sort_key=lambda k: k[0])  # pragma: no branch
+            order_keys(entry_point, (), sort_key=operator.itemgetter(0))  # pragma: no branch
 
     # order maintainers and authors table
     # handle readme table
 
     key_order = [
         "name",
         "version",
```

### Comparing `pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/tools.py` & `pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Format custom tools."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, cast
 
 from tomlkit.items import Table
 
 from .util import ensure_newline_at_end, order_keys
```

### Comparing `pyproject_fmt-1.7.0/src/pyproject_fmt/formatter/util.py` & `pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility methods."""
+
 from __future__ import annotations
 
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Any, Callable, Iterable, Protocol, Sequence, TypeVar
 
 from natsort import natsorted
@@ -14,38 +15,35 @@
     Comment,
     Item,
     Key,
     String,
     Table,
     Trivia,
     Whitespace,
-    _ArrayItemGroup,
+    _ArrayItemGroup,  # noqa: PLC2701
 )
 
 
 class SupportsDunderLT(Protocol):
-    def __lt__(self, __other: Any) -> bool:
-        ...
+    def __lt__(self, __other: Any) -> bool: ...
 
 
 class SupportsDunderGT(Protocol):
-    def __gt__(self, __other: Any) -> bool:
-        ...
+    def __gt__(self, __other: Any) -> bool: ...
 
 
 T = TypeVar("T")
 
 
 class SortingFunction(Protocol[T]):
     def __call__(
         self,
         __seq: Iterable[T],
         key: Callable[[T], SupportsDunderLT],
-    ) -> list[T]:
-        ...
+    ) -> list[T]: ...
 
 
 def sort_inline_table(item: tuple[str, Any | Table]) -> str:
     key, value = item
     return f"{key}{'-'.join(value) if isinstance(value, Table) else ''}"
 
 
@@ -171,11 +169,11 @@
         insert_body[-1] = insert_body[-1][0], whitespace
     else:
         insert_body.append((None, whitespace))
 
 
 __all__ = [
     "ArrayEntries",
-    "sorted_array",
-    "order_keys",
     "ensure_newline_at_end",
+    "order_keys",
+    "sorted_array",
 ]
```

### Comparing `pyproject_fmt-1.7.0/tests/test_cli.py` & `pyproject_fmt-1.8.0/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from pathlib import Path
 
 
 def test_cli_version(capsys: pytest.CaptureFixture[str]) -> None:
     with pytest.raises(SystemExit) as context:
         cli_args(["--version"])
     assert context.value.code == 0
-    out, err = capsys.readouterr()
+    out, _err = capsys.readouterr()
     assert out == f"pyproject-fmt ({__version__})\n"
 
 
 def test_cli_pyproject_toml_ok(tmp_path: Path) -> None:
     path = tmp_path / "tox.ini"
     path.write_text("")
     result = cli_args([str(path)])
```

### Comparing `pyproject_fmt-1.7.0/tests/test_main.py` & `pyproject_fmt-1.8.0/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             '[build-system]\nrequires = ["hatchling>=0.14.0"]',
             '[build-system]\nrequires = [\n  "hatchling>=0.14",\n]\n',
             "--- {0}\n\n+++ {0}\n\n@@ -1,2 +1,4 @@\n\n [build-system]\n-requires = "
             '["hatchling>=0.14.0"]\n+requires = [\n+  "hatchling>=0.14",\n+]\n',
         ),
     ],
 )
-def test_main(  # noqa: PLR0913
+def test_main(
     tmp_path: Path,
     capsys: pytest.CaptureFixture[str],
     in_place: bool,
     start: str,
     outcome: str,
     output: str,
     monkeypatch: pytest.MonkeyPatch,
```

### Comparing `pyproject_fmt-1.7.0/tests/formatter/conftest.py` & `pyproject_fmt-1.8.0/tests/formatter/conftest.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-1.7.0/tests/formatter/test_build_system.py` & `pyproject_fmt-1.8.0/tests/formatter/test_build_system.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-1.7.0/tests/formatter/test_pep508.py` & `pyproject_fmt-1.8.0/tests/formatter/test_pep508.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-1.7.0/tests/formatter/test_project.py` & `pyproject_fmt-1.8.0/tests/formatter/test_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from pathlib import Path
-from subprocess import CalledProcessError
+from subprocess import CalledProcessError  # noqa: S404
 from textwrap import dedent
 from typing import TYPE_CHECKING
 
 import pytest
 from packaging.version import Version
 
 from pyproject_fmt.formatter.config import Config
@@ -111,14 +111,27 @@
 
 def test_project_description(fmt: Fmt) -> None:
     start = '[project]\ndescription=" Magical stuff\t"'
     expected = '[project]\ndescription="Magical stuff"\n'
     fmt(fmt_project, start, expected)
 
 
+def test_project_description_multiline(fmt: Fmt) -> None:
+    start = dedent('''\
+        [project]
+        description="""A multi-line
+                       description."""
+    ''')
+    expected = dedent("""\
+        [project]
+        description="A multi-line description."
+    """)
+    fmt(fmt_project, start, expected)
+
+
 def test_project_scripts(fmt: Fmt) -> None:
     start = """
     [project.scripts]
     c = "d"
     a = "b"
     """
     expected = """
```

### Comparing `pyproject_fmt-1.7.0/tests/formatter/test_tools.py` & `pyproject_fmt-1.8.0/tests/formatter/test_tools.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-1.7.0/LICENSE.txt` & `pyproject_fmt-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-1.7.0/README.md` & `pyproject_fmt-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-1.7.0/pyproject.toml` & `pyproject_fmt-1.8.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -58,34 +58,48 @@
 build.dev-mode-dirs = ["src"]
 build.hooks.vcs.version-file = "src/pyproject_fmt/_version.py"
 build.targets.sdist.include = ["/src", "/tests","tox.ini"]
 version.source = "vcs"
 
 [tool.ruff]
 line-length = 120
-src = ["src", ""]
+target-version = "py38"
+lint.isort = { known-first-party = ["pyproject_fmt"], required-imports = ["from __future__ import annotations"] }
 lint.select = ["ALL"]
-lint.isort.required-imports = ["from __future__ import annotations"]
 lint.ignore = [
   "ANN101",  # no type annotation for self
   "ANN401",  # allow Any as type annotation
   "D203",  # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
   "D212",  # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
   "S104",  # Possible binding to all interface
+  "COM812", # Conflict with formatter
+  "ISC001", # Conflict with formatter
+  "CPY",    # No copyright statements
 ]
+lint.preview = true
+format.preview = true
+format.docstring-code-format = true
+format.docstring-code-line-length = 100
 [tool.ruff.lint.per-file-ignores]
 "tests/**/*.py" = [
   "S101",  # asserts allowed in tests...
   "FBT",  # don"t care about booleans as positional arguments in tests
   "INP001", # no implicit namespace
   "D",  # don"t care about documentation in tests
   "S603",  # `subprocess` call: check for execution of untrusted input
   "PLR2004",  # Magic value used in comparison, consider replacing with a constant variable
+  "PLR0913", # any number of arguments in tests
+  "PLR0917", # any number of arguments in tests
+  "PLC2701", # private import
 ]
 
+[tool.codespell]
+builtin = "clear,usage,en-GB_to_en-US"
+count = true
+
 [tool.pytest]
 ini_options.testpaths = ["tests"]
 
 [tool.coverage]
 html.show_contexts = true
 html.skip_covered = false
 paths.source = ["src", ".tox/*/lib/python*/site-packages", "*/src"]
```

### Comparing `pyproject_fmt-1.7.0/PKG-INFO` & `pyproject_fmt-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pyproject-fmt
-Version: 1.7.0
+Version: 1.8.0
 Summary: Format your pyproject.toml file
 Project-URL: Bug Tracker, https://github.com/tox-dev/pyproject-fmt/issues
 Project-URL: Changelog, https://github.com/tox-dev/pyproject-fmt/releases
 Project-URL: Documentation, https://github.com/tox-dev/pyproject-fmt/
 Project-URL: Source Code, https://github.com/tox-dev/pyproject-fmt
 Author-email: Bernat Gabor <gaborjbernat@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a
```

