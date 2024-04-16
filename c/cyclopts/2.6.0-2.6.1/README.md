# Comparing `tmp/cyclopts-2.6.0.tar.gz` & `tmp/cyclopts-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclopts-2.6.0.tar", max compression
+gzip compressed data, was "cyclopts-2.6.1.tar", max compression
```

## Comparing `cyclopts-2.6.0.tar` & `cyclopts-2.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2024-04-10 23:33:32.015391 cyclopts-2.6.0/LICENSE
--rw-r--r--   0        0        0    10910 2024-04-10 23:33:32.015391 cyclopts-2.6.0/README.md
--rw-r--r--   0        0        0      974 2024-04-10 23:33:47.123394 cyclopts-2.6.0/cyclopts/__init__.py
--rw-r--r--   0        0        0    12220 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/_convert.py
--rw-r--r--   0        0        0    13552 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/bind.py
--rw-r--r--   0        0        0    34480 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/core.py
--rw-r--r--   0        0        0     9637 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/exceptions.py
--rw-r--r--   0        0        0     4989 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/group.py
--rw-r--r--   0        0        0     2639 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/group_extractors.py
--rw-r--r--   0        0        0     9704 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/help.py
--rw-r--r--   0        0        0     7991 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/parameter.py
--rw-r--r--   0        0        0      190 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/protocols.py
--rw-r--r--   0        0        0        0 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/py.typed
--rw-r--r--   0        0        0     9514 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/resolve.py
--rw-r--r--   0        0        0     3851 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/types.py
--rw-r--r--   0        0        0     6027 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/utils.py
--rw-r--r--   0        0        0      205 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/validators/__init__.py
--rw-r--r--   0        0        0     1233 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/validators/_group.py
--rw-r--r--   0        0        0     1459 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/validators/_number.py
--rw-r--r--   0        0        0     1298 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/validators/_path.py
--rw-r--r--   0        0        0     4370 2024-04-10 23:33:47.123394 cyclopts-2.6.0/pyproject.toml
--rw-r--r--   0        0        0    11886 1970-01-01 00:00:00.000000 cyclopts-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-16 22:38:05.108343 cyclopts-2.6.1/LICENSE
+-rw-r--r--   0        0        0    10910 2024-04-16 22:38:05.108343 cyclopts-2.6.1/README.md
+-rw-r--r--   0        0        0      974 2024-04-16 22:38:17.328337 cyclopts-2.6.1/cyclopts/__init__.py
+-rw-r--r--   0        0        0    12220 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/_convert.py
+-rw-r--r--   0        0        0    13552 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/bind.py
+-rw-r--r--   0        0        0    34683 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/core.py
+-rw-r--r--   0        0        0     9666 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/exceptions.py
+-rw-r--r--   0        0        0     4989 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/group.py
+-rw-r--r--   0        0        0     2639 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/group_extractors.py
+-rw-r--r--   0        0        0     9889 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/help.py
+-rw-r--r--   0        0        0     7991 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/parameter.py
+-rw-r--r--   0        0        0      190 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/protocols.py
+-rw-r--r--   0        0        0        0 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/py.typed
+-rw-r--r--   0        0        0     9514 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/resolve.py
+-rw-r--r--   0        0        0     3851 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/types.py
+-rw-r--r--   0        0        0     6027 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/utils.py
+-rw-r--r--   0        0        0      205 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/validators/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-16 22:38:05.116343 cyclopts-2.6.1/cyclopts/validators/_group.py
+-rw-r--r--   0        0        0     1459 2024-04-16 22:38:05.116343 cyclopts-2.6.1/cyclopts/validators/_number.py
+-rw-r--r--   0        0        0     1298 2024-04-16 22:38:05.116343 cyclopts-2.6.1/cyclopts/validators/_path.py
+-rw-r--r--   0        0        0     4458 2024-04-16 22:38:17.324337 cyclopts-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0    11886 1970-01-01 00:00:00.000000 cyclopts-2.6.1/PKG-INFO
```

### Comparing `cyclopts-2.6.0/LICENSE` & `cyclopts-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.0/README.md` & `cyclopts-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.0/cyclopts/__init__.py` & `cyclopts-2.6.1/cyclopts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Don't manually change, let poetry-dynamic-versioning handle it.
-__version__ = "2.6.0"
+__version__ = "2.6.1"
 
 __all__ = [
     "App",
     "CoercionError",
     "CommandCollisionError",
     "CycloptsError",
     "Dispatcher",
```

### Comparing `cyclopts-2.6.0/cyclopts/_convert.py` & `cyclopts-2.6.1/cyclopts/_convert.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.0/cyclopts/bind.py` & `cyclopts-2.6.1/cyclopts/bind.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.0/cyclopts/core.py` & `cyclopts-2.6.1/cyclopts/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,26 @@
-import asyncio
-import importlib
 import inspect
 import os
 import sys
 import traceback
 from contextlib import suppress
 from copy import copy
 from functools import partial
 from pathlib import Path
-from typing import Callable, Dict, Iterable, Iterator, List, Literal, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Callable, Dict, Iterable, Iterator, List, Literal, Optional, Tuple, Union
 
 import cyclopts.utils
 
 if sys.version_info < (3, 9):
     from typing_extensions import Annotated
 else:
     from typing import Annotated
 
-try:
-    from pydantic import ValidationError as PydanticValidationError
-except ImportError:
-    PydanticValidationError = None
 
-
-import attrs
 from attrs import define, field
-from rich.console import Console
-
-if sys.version_info < (3, 10):  # pragma: no cover
-    from importlib_metadata import PackageNotFoundError
-    from importlib_metadata import version as importlib_metadata_version
-else:  # pragma: no cover
-    from importlib.metadata import PackageNotFoundError
-    from importlib.metadata import version as importlib_metadata_version
 
 from cyclopts.bind import create_bound_arguments, normalize_tokens
 from cyclopts.exceptions import (
     CommandCollisionError,
     CycloptsError,
     InvalidCommandError,
     UnusedCliTokensError,
@@ -57,14 +41,17 @@
 from cyclopts.resolve import ResolvedCommand
 from cyclopts.utils import default_name_transform, optional_to_tuple_converter, to_list_converter, to_tuple_converter
 
 with suppress(ImportError):
     # By importing, makes things like the arrow-keys work.
     import readline  # Not available on windows
 
+if TYPE_CHECKING:
+    from rich.console import Console
+
 
 class _CannotDeriveCallingModuleNameError(Exception):
     pass
 
 
 def _get_root_module_name():
     """Get the calling package name from the call-stack."""
@@ -84,14 +71,23 @@
     """Attempts to get the calling code's version.
 
     Returns
     -------
     version: str
         ``default`` if it cannot determine version.
     """
+    import importlib
+
+    if sys.version_info < (3, 10):  # pragma: no cover
+        from importlib_metadata import PackageNotFoundError
+        from importlib_metadata import version as importlib_metadata_version
+    else:  # pragma: no cover
+        from importlib.metadata import PackageNotFoundError
+        from importlib.metadata import version as importlib_metadata_version
+
     try:
         root_module_name = _get_root_module_name()
     except _CannotDeriveCallingModuleNameError:  # pragma: no cover
         return default
 
     # Attempt to get the Distribution Package’s version number.
     try:
@@ -180,15 +176,15 @@
         converter=to_tuple_converter,
         alias="version_flags",
         kw_only=True,
     )
 
     show: bool = field(default=True, kw_only=True)
 
-    console: Optional[Console] = field(default=None, kw_only=True)
+    console: Optional["Console"] = field(default=None, kw_only=True)
 
     # This can ONLY ever be a Tuple[str, ...]
     _help_flags: Union[str, Iterable[str]] = field(
         default=["--help", "-h"],
         converter=to_tuple_converter,
         alias="help_flags",
         kw_only=True,
@@ -512,15 +508,15 @@
             self.validator = validator
         return obj
 
     def parse_known_args(
         self,
         tokens: Union[None, str, Iterable[str]] = None,
         *,
-        console: Optional[Console] = None,
+        console: Optional["Console"] = None,
     ) -> Tuple[Callable, inspect.BoundArguments, List[str]]:
         """Interpret arguments into a function, :class:`~inspect.BoundArguments`, and any remaining unknown tokens.
 
         Parameters
         ----------
         tokens: Union[None, str, Iterable[str]]
             Either a string, or a list of strings to launch a command.
@@ -626,15 +622,15 @@
 
         return command, bound, unused_tokens
 
     def parse_args(
         self,
         tokens: Union[None, str, Iterable[str]] = None,
         *,
-        console: Optional[Console] = None,
+        console: Optional["Console"] = None,
         print_error: bool = True,
         exit_on_error: bool = True,
         verbose: bool = False,
     ) -> Tuple[Callable, inspect.BoundArguments]:
         """Interpret arguments into a function and :class:`~inspect.BoundArguments`.
 
         Raises
@@ -694,15 +690,15 @@
 
         return command, bound
 
     def __call__(
         self,
         tokens: Union[None, str, Iterable[str]] = None,
         *,
-        console: Optional[Console] = None,
+        console: Optional["Console"] = None,
         print_error: bool = True,
         exit_on_error: bool = True,
         verbose: bool = False,
     ):
         """Interprets and executes a command.
 
         Parameters
@@ -735,41 +731,52 @@
             console=console,
             print_error=print_error,
             exit_on_error=exit_on_error,
             verbose=verbose,
         )
         try:
             if inspect.iscoroutinefunction(command):
+                import asyncio
+
                 return asyncio.run(command(*bound.args, **bound.kwargs))
             else:
                 return command(*bound.args, **bound.kwargs)
         except Exception as e:
+            try:
+                from pydantic import ValidationError as PydanticValidationError
+            except ImportError:
+                PydanticValidationError = None  # noqa: N806
+
             if PydanticValidationError is not None and isinstance(e, PydanticValidationError):
                 if print_error:
                     console = self._resolve_console(tokens, console)
                     console.print(format_cyclopts_error(e))
 
                 if exit_on_error:
                     sys.exit(1)
             raise
 
-    def _resolve_console(self, tokens: Union[None, str, Iterable[str]], console: Optional[Console] = None) -> Console:
+    def _resolve_console(
+        self, tokens: Union[None, str, Iterable[str]], console: Optional["Console"] = None
+    ) -> "Console":
         if console is not None:
             return console
         _, apps, _ = self.parse_commands(tokens)
         for app in reversed(apps):
             if app.console:
                 return app.console
+        from rich.console import Console
+
         return Console()
 
     def help_print(
         self,
         tokens: Annotated[Union[None, str, Iterable[str]], Parameter(show=False)] = None,
         *,
-        console: Annotated[Optional[Console], Parameter(parse=False)] = None,
+        console: Annotated[Optional["Console"], Parameter(parse=False)] = None,
     ) -> None:
         """Print the help page.
 
         Parameters
         ----------
         tokens: Union[None, str, Iterable[str]]
             Tokens to interpret for traversing the application command structure.
```

### Comparing `cyclopts-2.6.0/cyclopts/exceptions.py` & `cyclopts-2.6.1/cyclopts/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-import difflib
 import inspect
 import re
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Type
 
 from attrs import define, field
-from rich import box
-from rich.console import Console
-from rich.panel import Panel
-from rich.text import Text
 
 import cyclopts.utils
 from cyclopts.group import Group
 from cyclopts.utils import ParameterDict
 
 if TYPE_CHECKING:
+    from rich.console import Console
+
     from cyclopts.core import App
 
 
 __all__ = [
     "CoercionError",
     "CommandCollisionError",
     "CycloptsError",
@@ -94,15 +91,15 @@
     """
 
     app: Optional["App"] = None
     """
     The Cyclopts application itself.
     """
 
-    console: Optional[Console] = field(default=None, kw_only=True)
+    console: Optional["Console"] = field(default=None, kw_only=True)
     """
     Rich console to display runtime errors.
     """
 
     def __str__(self):
         if self.msg is not None:
             return self.msg
@@ -217,14 +214,16 @@
         return super().__str__() + response + "."
 
 
 class InvalidCommandError(CycloptsError):
     """CLI token combination did not yield a valid command."""
 
     def __str__(self):
+        import difflib
+
         assert self.unused_tokens
         token = self.unused_tokens[0]
         response = super().__str__() + f'Unable to interpret valid command from "{token}".'
 
         if self.app and self.app._commands:
             close_matches = difflib.get_close_matches(token, self.app._commands, n=1, cutoff=0.8)
             if close_matches:
@@ -300,14 +299,18 @@
     def __str__(self):
         assert self.parameter2cli is not None
         parameter_cli_name = ",".join(self.parameter2cli[self.parameter])
         return super().__str__() + f"Parameter {parameter_cli_name} specified multiple times."
 
 
 def format_cyclopts_error(e: Any):
+    from rich import box
+    from rich.panel import Panel
+    from rich.text import Text
+
     panel = Panel(
         Text(str(e), "default"),
         title="Error",
         box=box.ROUNDED,
         expand=True,
         title_align="left",
         style="red",
```

### Comparing `cyclopts-2.6.0/cyclopts/group.py` & `cyclopts-2.6.1/cyclopts/group.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.0/cyclopts/group_extractors.py` & `cyclopts-2.6.1/cyclopts/group_extractors.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.0/cyclopts/help.py` & `cyclopts-2.6.1/cyclopts/help.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 from enum import Enum
 from functools import lru_cache, partial
 from inspect import isclass
 from typing import TYPE_CHECKING, Callable, List, Literal, Tuple, Type, Union, get_args, get_origin
 
 import docstring_parser
 from attrs import define, field, frozen
-from rich import box, console
-from rich.panel import Panel
-from rich.table import Table
-from rich.text import Text
 
 import cyclopts.utils
 from cyclopts.group import Group
 from cyclopts.parameter import Parameter, get_hint_parameter
 
 if TYPE_CHECKING:
     from cyclopts.core import App
@@ -59,21 +55,28 @@
 
     def sort(self):
         self.entries.sort(key=lambda x: (x.name.startswith("-"), x.name))
 
     def __rich__(self):
         if not self.entries:
             return _silent
+        from rich.box import ROUNDED
+        from rich.console import Group as RichGroup
+        from rich.table import Table
+        from rich.text import Text
+
         table = Table.grid(padding=(0, 1))
         text = Text(end="")
         if self.description:
             text.append(self.description + "\n\n")
+        from rich.panel import Panel
+
         panel = Panel(
-            console.Group(text, table),
-            box=box.ROUNDED,
+            RichGroup(text, table),
+            box=ROUNDED,
             expand=True,
             title_align="left",
             title=self.title,
         )
 
         if self.format == "command":
             table.add_column(justify="left", style="cyan")
@@ -129,14 +132,16 @@
     return not s.startswith("--") and s.startswith("-")
 
 
 def format_usage(
     app,
     command_chain: List[str],
 ):
+    from rich.text import Text
+
     usage = []
     usage.append("Usage:")
     usage.append(app.name[0])
     usage.extend(command_chain)
 
     for command in command_chain:
         app = app[command]
@@ -153,14 +158,17 @@
                 to_show.add("[OPTIONS]")
         usage.extend(sorted(to_show))
 
     return Text(" ".join(usage) + "\n", style="bold")
 
 
 def format_doc(root_app, app: "App", format: str = "restructuredtext"):
+    from rich.console import Group as RichGroup
+    from rich.text import Text
+
     from cyclopts.core import App  # noqa: F811
 
     raw_doc_string = app.help
 
     if not raw_doc_string:
         return _silent
 
@@ -177,15 +185,15 @@
 
     format = format.lower()
     if format == "plaintext":
         return Text.assemble(*components)
     elif format in ("markdown", "md"):
         from rich.markdown import Markdown
 
-        return console.Group(Markdown("".join(x[0] for x in components)), Text(""))
+        return RichGroup(Markdown("".join(x[0] for x in components)), Text(""))
     elif format in ("restructuredtext", "rst"):
         from rich_rst import RestructuredText
 
         return RestructuredText("".join(x[0] for x in components))
     else:
         raise ValueError(f'Unknown help_format "{format}"')
```

### Comparing `cyclopts-2.6.0/cyclopts/parameter.py` & `cyclopts-2.6.1/cyclopts/parameter.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.0/cyclopts/resolve.py` & `cyclopts-2.6.1/cyclopts/resolve.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.0/cyclopts/types.py` & `cyclopts-2.6.1/cyclopts/types.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.0/cyclopts/utils.py` & `cyclopts-2.6.1/cyclopts/utils.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.0/cyclopts/validators/_group.py` & `cyclopts-2.6.1/cyclopts/validators/_group.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.0/cyclopts/validators/_number.py` & `cyclopts-2.6.1/cyclopts/validators/_number.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.0/cyclopts/validators/_path.py` & `cyclopts-2.6.1/cyclopts/validators/_path.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.0/pyproject.toml` & `cyclopts-2.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "cyclopts"
-version = "2.6.0"  # Do not change, let poetry-dynamic-versioning handle it.
+version = "2.6.1"  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/BrianPugh/cyclopts"
 repository = "https://github.com/BrianPugh/cyclopts"
 license = "Apache-2.0"
 description = ""
 authors = ["Brian Pugh"]
 readme = "README.md"
 packages = [{include = "cyclopts"}]
@@ -47,15 +47,15 @@
 pre_commit = ">=2.16.0"
 pytest = ">=7.1.2"
 pytest-cov = ">=3.0.0"
 pytest-mock = ">=3.7.0"
 typer = "0.12.0"
 arguably = "^1.2.5"
 fire = ">=0.5,<0.7"
-pydantic = "^2.5.3"
+pydantic = "^2.7.0"
 
 [tool.poetry.group.debug]
 optional = true
 
 [tool.poetry.group.debug.dependencies]
 ipdb = ">=0.13.9"
 line_profiler = ">=3.5.1"
@@ -197,9 +197,10 @@
 venvs=[".venv"]
 paths=["cyclopts"]
 deps-file="pyproject.toml"
 sections=["tool.poetry.dependencies"]
 exclude-deps =[
   "importlib-metadata",
   "typing-extensions",
-  "rich-rst",
+  "rich-rst",  # Not detected due to deferred import
+  "rich",  # Not detected due to deferred import
 ]
```

### Comparing `cyclopts-2.6.0/PKG-INFO` & `cyclopts-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclopts
-Version: 2.6.0
+Version: 2.6.1
 Summary: 
 Home-page: https://github.com/BrianPugh/cyclopts
 License: Apache-2.0
 Author: Brian Pugh
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

