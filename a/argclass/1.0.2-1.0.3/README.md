# Comparing `tmp/argclass-1.0.2.tar.gz` & `tmp/argclass-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argclass-1.0.2.tar", max compression
+gzip compressed data, was "argclass-1.0.3.tar", max compression
```

## Comparing `argclass-1.0.2.tar` & `argclass-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0    11359 2024-04-06 07:45:43.603917 argclass-1.0.2/COPYING
--rw-r--r--   0        0        0    11478 2024-04-09 22:38:26.351024 argclass-1.0.2/README.md
--rw-r--r--   0        0        0    28738 2024-04-09 22:36:31.846086 argclass-1.0.2/argclass.py
--rw-r--r--   0        0        0     2038 2024-04-09 22:39:00.274123 argclass-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    12967 1970-01-01 00:00:00.000000 argclass-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    13251 2024-04-17 10:28:59.591736 argclass-1.0.3/README.md
+-rw-r--r--   0        0        0    29540 2024-04-17 10:28:59.592385 argclass-1.0.3/argclass.py
+-rw-r--r--   0        0        0     2085 2024-04-17 10:29:50.759858 argclass-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    14690 1970-01-01 00:00:00.000000 argclass-1.0.3/PKG-INFO
```

### Comparing `argclass-1.0.2/README.md` & `argclass-1.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -165,14 +165,16 @@
 
 ## Configs
 
 The parser objects might be get default values from environment variables or
 one of passed configuration files.
 
 ```python
+import argclass
+
 class AddressPortGroup(argclass.Group):
     address: str = argclass.Argument(default="127.0.0.1")
     port: int
 
 
 class Parser(argclass.Parser):
     spam: str
@@ -191,15 +193,15 @@
     config_files=[".example.ini", "~/.example.ini", "/etc/example.ini"],
 )
 parser.parse_args()
 ```
 
 In this case each passed and existent configuration file will be opened.
 
-The root level arguments might described in the ``[DEFAULT]`` section.
+The root level arguments might be described in the ``[DEFAULT]`` section.
 
 Other arguments might be described in group specific sections.
 
 So the full example of config file for above example is:
 
 ```ini
 [DEFAULT]
@@ -259,16 +261,19 @@
 
 This library provides base class for writing custom configuration parsers.
 
 
 ### YAML parser
 
 ```python
-import yaml
+from typing import Mapping, Any
+from pathlib import Path
+
 import argclass
+import yaml
 
 
 class YAMLConfigAction(argclass.ConfigAction):
     def parse_file(self, file: Path) -> Mapping[str, Any]:
         with file.open("r") as fp:
             return yaml.load_all(fp)
 
@@ -284,16 +289,17 @@
     )
 ```
 
 ### TOML parser
 
 ```python
 import tomli
-
 import argclass
+from pathlib import Path
+from typing import Mapping, Any
 
 
 class TOMLConfigAction(argclass.ConfigAction):
     def parse_file(self, file: Path) -> Mapping[str, Any]:
         with file.open("r") as fp:
             return tomli.load(fp)
 
@@ -304,23 +310,79 @@
 class Parser(argclass.Parser):
     config = argclass.Config(
         required=True,
         config_class=TOMLConfigArgument,
     )
 ```
 
-Subparsers
-==========
+## Subparsers
+
+There are two ways to work with subparsers: either by calling the parser as a regular function, and in this case, 
+the subparser must implement the `__call__` method, otherwise help will be printed and the program will exit with
+an error. Or you can directly look at the `.current_subparser` attribute in the parser. The second method seems 
+more complicated, but it becomes less difficult if you use singledispatch from the standard library.
+
+### Using `__call__`
+
+Just implement `__call__` method for subparsers and call
+
+```python
+from typing import Optional
+
+import argclass
+
+
+class AddressPortGroup(argclass.Group):
+    address: str = "127.0.0.1"
+    port: int = 8080
+
+
+class CommitCommand(argclass.Parser):
+    comment: str = argclass.Argument()
+
+    def __call__(self):
+        endpoint: AddressPortGroup = self.__parent__.endpoint
+        print(
+            "Commit command called", self, 
+            "endpoint", endpoint.address, "port", endpoint.port
+        )
+
+
+class PushCommand(argclass.Parser):
+    comment: str = argclass.Argument()
+
+    def __call__(self):
+        endpoint: AddressPortGroup = self.__parent__.endpoint
+        print(
+            "Push command called", self, 
+            "endpoint", endpoint.address, "port", endpoint.port
+        )
+
+
+class Parser(argclass.Parser):
+    log_level: int = argclass.LogLevel
+    endpoint = AddressPortGroup(title="Endpoint options")
+    commit: Optional[CommitCommand] = CommitCommand()
+    push: Optional[PushCommand] = PushCommand()
+
+
+parser = Parser(
+    config_files=["example.ini", "~/.example.ini", "/etc/example.ini"],
+    auto_env_var_prefix="EXAMPLE_"
+)
+parser.parse_args()
+parser()
+```
+
+### Using singledispatch
 
 Complex example with subparsers:
 
 ```python
-import logging
 from functools import singledispatch
-from pathlib import Path
 from typing import Optional, Any
 
 import argclass
 
 
 class AddressPortGroup(argclass.Group):
     address: str = argclass.Argument(default="127.0.0.1")
```

### Comparing `argclass-1.0.2/argclass.py` & `argclass-1.0.3/argclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 import argparse
 import ast
 import collections
 import configparser
+import errno
 import json
 import logging
 import os
 import sys
 import traceback
 from abc import ABCMeta
 from argparse import Action, ArgumentParser
-from enum import Enum, IntEnum
+from enum import Enum, EnumMeta, IntEnum
 from functools import partial
 from pathlib import Path
 from types import MappingProxyType
 from typing import (
     Any, Callable, Dict, Iterable, Iterator, List, Literal, Mapping,
     MutableMapping, NamedTuple, Optional, Sequence, Set, Tuple, Type, TypeVar,
     Union,
 )
 
 
-try:
-    from enum import EnumType
-except ImportError:
-    from enum import EnumMeta as EnumType
-
-
 ConverterType = Callable[[str], Any]
 NoneType = type(None)
 UnionClass = Union[None, int].__class__
+EnumType = EnumMeta
 
 
 def read_configs(
-    *paths: Union[str, Path], **kwargs: Any
+    *paths: Union[str, Path], **kwargs: Any,
 ) -> Tuple[Mapping[str, Any], Tuple[Path, ...]]:
     kwargs.setdefault("allow_no_value", True)
     kwargs.setdefault("strict", False)
     parser = configparser.ConfigParser(**kwargs)
 
     filenames = list(
         map(
@@ -200,15 +196,15 @@
     for base in bases:
         if hasattr(base, name):
             return getattr(base, name)
     raise KeyError(f"Key {name} was not declared")
 
 
 def merge_annotations(
-    annotations: Dict[str, Any], *bases: Type
+    annotations: Dict[str, Any], *bases: Type,
 ) -> Dict[str, Any]:
     result: Dict[str, Any] = {}
 
     for base in bases:
         result.update(getattr(base, "__annotations__", {}))
     result.update(annotations)
     return result
@@ -216,15 +212,15 @@
 
 class StoreMeta(type):
     def __new__(
         mcs, name: str, bases: Tuple[Type["StoreMeta"], ...],
         attrs: Dict[str, Any],
     ) -> "StoreMeta":
         annotations = merge_annotations(
-            attrs.get("__annotations__", {}), *bases
+            attrs.get("__annotations__", {}), *bases,
         )
         attrs["__annotations__"] = annotations
         attrs["_fields"] = tuple(
             filter(
                 lambda x: not x.startswith("_"),
                 annotations.keys(),
             ),
@@ -355,22 +351,25 @@
 
 
 class AbstractGroup:
     pass
 
 
 class AbstractParser:
-    __parent__: Optional["AbstractParser"] = None
+    __parent__: Union["Parser", None] = None
 
     def _get_chain(self) -> Iterator["AbstractParser"]:
         yield self
         if self.__parent__ is None:
             return
         yield from self.__parent__._get_chain()
 
+    def __call__(self) -> None:
+        raise NotImplementedError()
+
 
 TEXT_TRUE_VALUES = frozenset((
     "y", "yes", "true", "t", "enable", "enabled", "1", "on",
 ))
 
 
 def parse_bool(value: str) -> bool:
@@ -416,15 +415,15 @@
 
 class Meta(ABCMeta):
     def __new__(
         mcs, name: str, bases: Tuple[Type["Meta"], ...],
         attrs: Dict[str, Any],
     ) -> "Meta":
         annotations = merge_annotations(
-            attrs.get("__annotations__", {}), *bases
+            attrs.get("__annotations__", {}), *bases,
         )
 
         arguments = {}
         argument_groups = {}
         subparsers = {}
         for key, kind in annotations.items():
             if key.startswith("_"):
@@ -462,15 +461,15 @@
                         kind = unwrap_optional(kind)
                         argument.default = None
                     argument.type = kind
                 arguments[key] = argument
             elif isinstance(argument, AbstractGroup):
                 argument_groups[key] = argument
 
-            if isinstance(kind, EnumType):
+            if isinstance(kind, EnumMeta):
                 arguments[key] = EnumArgument(kind)
 
         for key, value in attrs.items():
             if key.startswith("_"):
                 continue
 
             if isinstance(value, _Argument):
@@ -632,15 +631,15 @@
         return self.current_subparsers[0]
 
     def _make_parser(
         self, parser: Optional[ArgumentParser] = None,
     ) -> Tuple[ArgumentParser, DestinationsType]:
         if parser is None:
             parser = ArgumentParser(
-                epilog=self._epilog, **self._parser_kwargs
+                epilog=self._epilog, **self._parser_kwargs,
             )
 
         destinations: DestinationsType = collections.defaultdict(set)
 
         self._fill_arguments(destinations, parser)
         self._fill_groups(destinations, parser)
         if self.__subparsers__:
@@ -699,15 +698,15 @@
                     name, group._defaults.get(name, argument.default),
                 )
                 argument = argument.copy(
                     default=default,
                     env_var=self.get_env_var(dest, argument),
                 )
                 dest, action = self._add_argument(
-                    group_parser, argument, dest, *aliases
+                    group_parser, argument, dest, *aliases,
                 )
                 destinations[dest].add(
                     Destination(
                         target=group,
                         attribute=name,
                         argument=argument,
                         action=action,
@@ -728,15 +727,15 @@
             ),
         )
 
         for subparser_name, subparser in self.__subparsers__.items():
             current_parser, subparser_dests = (
                 subparser._make_parser(
                     subparsers.add_parser(
-                        subparser_name, **subparser._parser_kwargs
+                        subparser_name, **subparser._parser_kwargs,
                     ),
                 )
             )
             subparser.__parent__ = self
             current_parser.set_defaults(
                 current_subparsers=tuple(subparser._get_chain()),
             )
@@ -798,14 +797,38 @@
         return parser.print_help()
 
     def sanitize_env(self) -> None:
         for name in self._used_env_vars:
             os.environ.pop(name, None)
         self._used_env_vars.clear()
 
+    def __call__(self) -> None:
+        """
+        Override this function if you want to equip your parser with an action.
+        It will be like replacing the main function in a classical case.
+
+        >>> import argclass
+        >>> class MyParser(argclass.Parser):
+        ...    dry_run: bool = False
+        ...    def __call__(self):
+        ...        print("Dry run mode is:", self.dry_run)
+        ...
+        >>> parser = MyParser()
+        >>> parser.parse_args([])
+        >>> parser()
+        Dry run mode is: False
+        >>> parser.parse_args(['--dry-run'])
+        >>> parser()
+        Dry run mode is: True
+        """
+        if self.current_subparser is not None:
+            return self.current_subparser()
+        self.print_help()
+        exit(errno.EINVAL)
+
 
 NargsType = Union[Nargs, Literal["*", "+", "?"], int, None]
 
 
 # noinspection PyPep8Naming
 def Argument(
     *aliases: str,
@@ -816,15 +839,15 @@
     default: Optional[Any] = None,
     secret: bool = False,
     env_var: Optional[str] = None,
     help: Optional[str] = None,
     metavar: Optional[str] = None,
     nargs: NargsType = None,
     required: Optional[bool] = None,
-    type: Optional[Callable[[str], Any]] = None
+    type: Optional[Callable[[str], Any]] = None,
 ) -> Any:
     return _Argument(
         action=action,
         aliases=aliases,
         choices=choices,
         const=const,
         converter=converter,
@@ -837,28 +860,28 @@
         required=required,
         type=type,
     )    # type: ignore
 
 
 # noinspection PyPep8Naming
 def EnumArgument(
-    enum: EnumType,
+    enum: EnumMeta,
     *aliases: str,
     action: Union[Actions, Type[Action]] = Actions.default(),
     const: Optional[Any] = None,
     default: Optional[Any] = None,
     secret: bool = False,
     env_var: Optional[str] = None,
     help: Optional[str] = None,
     metavar: Optional[str] = None,
     nargs: NargsType = None,
     required: Optional[bool] = None,
 ) -> Any:
 
-    def converter(value: Any) -> EnumType:
+    def converter(value: Any) -> EnumMeta:
         if isinstance(value, Enum):
             return value        # type: ignore
         return enum[value]
 
     return _Argument(    # type: ignore
         aliases=aliases,
         action=action,
@@ -887,15 +910,15 @@
     const: Optional[Any] = None,
     default: Optional[Any] = None,
     env_var: Optional[str] = None,
     help: Optional[str] = None,
     metavar: Optional[str] = None,
     nargs: NargsType = None,
     required: Optional[bool] = None,
-    config_class: Type[ConfigArgument] = INIConfig
+    config_class: Type[ConfigArgument] = INIConfig,
 ) -> Any:
     return config_class(
         search_paths=search_paths,
         aliases=aliases,
         choices=choices,
         const=const,
         converter=converter,
```

### Comparing `argclass-1.0.2/pyproject.toml` & `argclass-1.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "argclass"
-version = "1.0.2"
+version = "1.0.3"
 description = "A wrapper around the standard argparse module that allows you to describe argument parsers declaratively"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.md"
 license = "Apache 2"
 homepage = "https://github.com/mosquito/argclass"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -14,18 +14,19 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Operating System :: POSIX",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python",
 ]
 packages = [
     { include = "argclass.py" },
 ]
 
 [tool.poetry.urls]
```

### Comparing `argclass-1.0.2/PKG-INFO` & `argclass-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argclass
-Version: 1.0.2
+Version: 1.0.3
 Summary: A wrapper around the standard argparse module that allows you to describe argument parsers declaratively
 Home-page: https://github.com/mosquito/argclass
 License: Apache 2
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Project-URL: Documentation, https://github.com/mosquito/argclass/blob/master/README.md
 Project-URL: Source, https://github.com/mosquito/argclass
 Project-URL: Tracker, https://github.com/mosquito/argclass/issues
 Description-Content-Type: text/markdown
 
 # argclass
 
@@ -198,14 +197,16 @@
 
 ## Configs
 
 The parser objects might be get default values from environment variables or
 one of passed configuration files.
 
 ```python
+import argclass
+
 class AddressPortGroup(argclass.Group):
     address: str = argclass.Argument(default="127.0.0.1")
     port: int
 
 
 class Parser(argclass.Parser):
     spam: str
@@ -224,15 +225,15 @@
     config_files=[".example.ini", "~/.example.ini", "/etc/example.ini"],
 )
 parser.parse_args()
 ```
 
 In this case each passed and existent configuration file will be opened.
 
-The root level arguments might described in the ``[DEFAULT]`` section.
+The root level arguments might be described in the ``[DEFAULT]`` section.
 
 Other arguments might be described in group specific sections.
 
 So the full example of config file for above example is:
 
 ```ini
 [DEFAULT]
@@ -292,16 +293,19 @@
 
 This library provides base class for writing custom configuration parsers.
 
 
 ### YAML parser
 
 ```python
-import yaml
+from typing import Mapping, Any
+from pathlib import Path
+
 import argclass
+import yaml
 
 
 class YAMLConfigAction(argclass.ConfigAction):
     def parse_file(self, file: Path) -> Mapping[str, Any]:
         with file.open("r") as fp:
             return yaml.load_all(fp)
 
@@ -317,16 +321,17 @@
     )
 ```
 
 ### TOML parser
 
 ```python
 import tomli
-
 import argclass
+from pathlib import Path
+from typing import Mapping, Any
 
 
 class TOMLConfigAction(argclass.ConfigAction):
     def parse_file(self, file: Path) -> Mapping[str, Any]:
         with file.open("r") as fp:
             return tomli.load(fp)
 
@@ -337,23 +342,79 @@
 class Parser(argclass.Parser):
     config = argclass.Config(
         required=True,
         config_class=TOMLConfigArgument,
     )
 ```
 
-Subparsers
-==========
+## Subparsers
+
+There are two ways to work with subparsers: either by calling the parser as a regular function, and in this case, 
+the subparser must implement the `__call__` method, otherwise help will be printed and the program will exit with
+an error. Or you can directly look at the `.current_subparser` attribute in the parser. The second method seems 
+more complicated, but it becomes less difficult if you use singledispatch from the standard library.
+
+### Using `__call__`
+
+Just implement `__call__` method for subparsers and call
+
+```python
+from typing import Optional
+
+import argclass
+
+
+class AddressPortGroup(argclass.Group):
+    address: str = "127.0.0.1"
+    port: int = 8080
+
+
+class CommitCommand(argclass.Parser):
+    comment: str = argclass.Argument()
+
+    def __call__(self):
+        endpoint: AddressPortGroup = self.__parent__.endpoint
+        print(
+            "Commit command called", self, 
+            "endpoint", endpoint.address, "port", endpoint.port
+        )
+
+
+class PushCommand(argclass.Parser):
+    comment: str = argclass.Argument()
+
+    def __call__(self):
+        endpoint: AddressPortGroup = self.__parent__.endpoint
+        print(
+            "Push command called", self, 
+            "endpoint", endpoint.address, "port", endpoint.port
+        )
+
+
+class Parser(argclass.Parser):
+    log_level: int = argclass.LogLevel
+    endpoint = AddressPortGroup(title="Endpoint options")
+    commit: Optional[CommitCommand] = CommitCommand()
+    push: Optional[PushCommand] = PushCommand()
+
+
+parser = Parser(
+    config_files=["example.ini", "~/.example.ini", "/etc/example.ini"],
+    auto_env_var_prefix="EXAMPLE_"
+)
+parser.parse_args()
+parser()
+```
+
+### Using singledispatch
 
 Complex example with subparsers:
 
 ```python
-import logging
 from functools import singledispatch
-from pathlib import Path
 from typing import Optional, Any
 
 import argclass
 
 
 class AddressPortGroup(argclass.Group):
     address: str = argclass.Argument(default="127.0.0.1")
```

