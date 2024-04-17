# Comparing `tmp/inigrep-0.5.2.tar.gz` & `tmp/inigrep-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inigrep-0.5.2.tar", last modified: Mon Apr  1 15:45:18 2024, max compression
+gzip compressed data, was "inigrep-0.5.3.tar", last modified: Wed Apr 17 07:19:56 2024, max compression
```

## Comparing `inigrep-0.5.2.tar` & `inigrep-0.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 15:45:18.095987 inigrep-0.5.2/
--rw-r--r--   0 netvor    (9860) netvor    (9860)    26338 2020-08-03 17:39:27.000000 inigrep-0.5.2/LICENSE.md
--rw-r--r--   0 netvor    (9860) netvor    (9860)     1689 2024-04-01 15:45:18.095987 inigrep-0.5.2/PKG-INFO
--rw-r--r--   0 netvor    (9860) netvor    (9860)       38 2023-04-05 14:47:14.000000 inigrep-0.5.2/README.md
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 15:45:18.095987 inigrep-0.5.2/inigrep.egg-info/
--rw-r--r--   0 netvor    (9860) netvor    (9860)     1689 2024-04-01 15:45:18.000000 inigrep-0.5.2/inigrep.egg-info/PKG-INFO
--rw-r--r--   0 netvor    (9860) netvor    (9860)      325 2024-04-01 15:45:18.000000 inigrep-0.5.2/inigrep.egg-info/SOURCES.txt
--rw-r--r--   0 netvor    (9860) netvor    (9860)        1 2024-04-01 15:45:18.000000 inigrep-0.5.2/inigrep.egg-info/dependency_links.txt
--rw-r--r--   0 netvor    (9860) netvor    (9860)        8 2024-04-01 15:45:18.000000 inigrep-0.5.2/inigrep.egg-info/top_level.txt
--rw-r--r--   0 netvor    (9860) netvor    (9860)       38 2024-04-01 15:45:18.095987 inigrep-0.5.2/setup.cfg
--rw-r--r--   0 netvor    (9860) netvor    (9860)    12664 2024-04-01 15:45:13.000000 inigrep-0.5.2/setup.py
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 15:45:18.095987 inigrep-0.5.2/src/
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 15:45:18.095987 inigrep-0.5.2/src/inigrep/
--rw-r--r--   0 netvor    (9860) netvor    (9860)      175 2023-03-12 00:22:00.000000 inigrep-0.5.2/src/inigrep/__init__.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)       68 2024-04-01 15:37:56.000000 inigrep-0.5.2/src/inigrep/__main__.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)      546 2024-04-01 15:45:12.000000 inigrep-0.5.2/src/inigrep/_meta.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)     7401 2024-04-01 15:37:56.000000 inigrep-0.5.2/src/inigrep/cli.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)    15540 2024-04-01 15:37:56.000000 inigrep-0.5.2/src/inigrep/core.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)    10558 2023-03-12 00:22:00.000000 inigrep-0.5.2/src/inigrep/front.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)        0 2023-03-12 00:22:00.000000 inigrep-0.5.2/src/inigrep/py.typed
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 15:45:18.095987 inigrep-0.5.2/tests/
--rw-r--r--   0 netvor    (9860) netvor    (9860)    26767 2024-04-01 15:44:20.000000 inigrep-0.5.2/tests/test_inigrep.py
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-17 07:19:56.488013 inigrep-0.5.3/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    26338 2020-08-03 17:39:27.000000 inigrep-0.5.3/LICENSE.md
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     1189 2024-04-17 07:19:56.488013 inigrep-0.5.3/PKG-INFO
+-rw-r--r--   0 netvor    (9860) netvor    (9860)       38 2023-04-05 14:47:14.000000 inigrep-0.5.3/README.md
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-17 07:19:56.488013 inigrep-0.5.3/inigrep.egg-info/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     1189 2024-04-17 07:19:56.000000 inigrep-0.5.3/inigrep.egg-info/PKG-INFO
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      325 2024-04-17 07:19:56.000000 inigrep-0.5.3/inigrep.egg-info/SOURCES.txt
+-rw-r--r--   0 netvor    (9860) netvor    (9860)        1 2024-04-17 07:19:56.000000 inigrep-0.5.3/inigrep.egg-info/dependency_links.txt
+-rw-r--r--   0 netvor    (9860) netvor    (9860)        8 2024-04-17 07:19:56.000000 inigrep-0.5.3/inigrep.egg-info/top_level.txt
+-rw-r--r--   0 netvor    (9860) netvor    (9860)       38 2024-04-17 07:19:56.488013 inigrep-0.5.3/setup.cfg
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    12645 2024-04-17 07:19:51.000000 inigrep-0.5.3/setup.py
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-17 07:19:56.488013 inigrep-0.5.3/src/
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-17 07:19:56.488013 inigrep-0.5.3/src/inigrep/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      175 2023-03-12 00:22:00.000000 inigrep-0.5.3/src/inigrep/__init__.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)       68 2024-04-01 15:37:56.000000 inigrep-0.5.3/src/inigrep/__main__.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      546 2024-04-17 07:19:50.000000 inigrep-0.5.3/src/inigrep/_meta.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     7610 2024-04-17 07:17:01.000000 inigrep-0.5.3/src/inigrep/cli.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    14796 2024-04-17 07:17:01.000000 inigrep-0.5.3/src/inigrep/core.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    10494 2024-04-17 07:17:01.000000 inigrep-0.5.3/src/inigrep/front.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)        0 2023-03-12 00:22:00.000000 inigrep-0.5.3/src/inigrep/py.typed
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-17 07:19:56.488013 inigrep-0.5.3/tests/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    26767 2024-04-16 17:32:54.000000 inigrep-0.5.3/tests/test_inigrep.py
```

### Comparing `inigrep-0.5.2/LICENSE.md` & `inigrep-0.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inigrep-0.5.2/setup.py` & `inigrep-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 VDK_PYLIB_CLASSIFIERS = [
     'Intended Audience :: Developers',
     'Intended Audience :: Information Technology',
     'Natural Language :: English',
 ]
 
 VDK_PYLIB_PYTHON_GE = """
-__VDK_PYLIB_PYTHON_GE__
+3.10
 """
 
 VDK_PYLIB_PYTHON_LT = """
 __VDK_PYLIB_PYTHON_LT__
 """
 
 VDK_PYPI_REQUIRES = [
@@ -359,12 +359,12 @@
     maintainer_email='Alois Mahdal <netvor+inigrep@vornet.cz>',
     name='inigrep',
     packages=VDK_PACKAGEINFO['packages'],
     package_dir=VDK_PACKAGEINFO['package_dir'],
     package_data=VDK_PACKAGEINFO['package_data'],
     url='https://gitlab.com/vornet/python/python-inigrep',
     requires=vdk_cleanup(VDK_PYPI_REQUIRES),
-    version='0.5.2',
+    version='0.5.3',
     classifiers=VDK_PACKAGEINFO['classifiers'],
 )
 
 # setup.py built with MKit 0.1.3 and vdk-pylib-0.1.1
```

### Comparing `inigrep-0.5.2/src/inigrep/_meta.py` & `inigrep-0.5.3/src/inigrep/_meta.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 CODENAME: str = """
 
 """.strip()
 
 GIT_LASTHASH: str = """
-b4e61008e20de4be7668eb67fe728c7038557c05
+31a5719d4e4a3ef8e74d67249a475aeef67be105
 """.strip()
 
 GIT_LASTSUMMARY: str = """
-Bump version to 0.5.2
+Bump version to 0.5.3
 """.strip()
 
 LICENSE: str = """
 LGPLv2
 """.strip()
 
 MAINTAINER: str = """
@@ -31,9 +31,9 @@
 """.strip()
 
 VCS_BROWSER: str = """
 https://gitlab.com/vornet/python/python-inigrep
 """.strip()
 
 VERSION: str = """
-0.5.2
+0.5.3
 """.strip()
```

### Comparing `inigrep-0.5.2/src/inigrep/cli.py` & `inigrep-0.5.3/src/inigrep/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 from __future__ import annotations
 import sys
-import typing
+from typing import Iterable
+from dataclasses import dataclass, field
 
+from ._meta import VERSION
+from .core import (
+    ClonedLineT,
+    LineT,
+    ValueT,
+    RawValueT,
+    KeyT,
+    SectionT,
+    KeypathT,
+    _r_values,
+    _r_raw_values,
+    _r_clone,
+    _r_list_keys,
+    _r_list_sections,
+    _r_list_paths,
+    KeypathError,
+)
 import inigrep
-import inigrep.core
 import inigrep.front
 
 
 _USAGE: str = """
 usage:
     inigrep [-1] [section].[key] [file]...
     inigrep [-1] -c|--clone [file]...
@@ -85,18 +102,17 @@
     pass
 
 
 class VersionNeeded(RuntimeError):
     pass
 
 
+@dataclass
 class Args:
-
-    def __init__(self, args: list[str]) -> None:
-        self.args = args
+    args: list[str]
 
     def take1(self) -> str:
         if not self.args:
             raise UsageError('missing argument')
         return self.args.pop(0)
 
     def take2(self) -> tuple[str, str]:
@@ -115,143 +131,157 @@
 
 
 class Engine:
 
     def __init__(self, **fnargs):
         self.fnargs = fnargs
 
-    def _r_run(self, reader: inigrep.core.LineGenT
-               ) -> typing.Iterator[str]:
+    def _r_run(self, reader: Iterable[LineT]
+               ) -> Iterable[str]:
         raise NotImplementedError
 
-    def run(self, files: list[str]) -> typing.Iterator[str]:
+    def run(self, files: list[str]) -> Iterable[str]:
         raise NotImplementedError
 
 
 class NoEngine(Engine):
 
     pass
 
 
 class BasicEngine(Engine):
 
-    def _r_run(self, reader: inigrep.core.LineGenT
-               ) -> inigrep.core.ValueGenT:
-        return inigrep.core._r_values(reader=reader, **self.fnargs)
+    def _r_run(self, reader: Iterable[LineT]
+               ) -> Iterable[ValueT]:
+        return _r_values(reader=reader, **self.fnargs)
 
-    def run(self, files: list[str]) -> typing.Iterator[str]:
+    def run(self, files: list[str]) -> Iterable[str]:
         return inigrep.front.values(files=files, **self.fnargs)
 
 
 class RawEngine(Engine):
 
-    def _r_run(self, reader: inigrep.core.LineGenT
-               ) -> inigrep.core.RawValueGenT:
-        return inigrep.core._r_raw_values(reader=reader, **self.fnargs)
+    def _r_run(self, reader: Iterable[LineT]
+               ) -> Iterable[RawValueT]:
+        return _r_raw_values(reader=reader, **self.fnargs)
 
-    def run(self, files: list[str]) -> typing.Iterator[str]:
+    def run(self, files: list[str]) -> Iterable[str]:
         return inigrep.front.raw_values(files=files, **self.fnargs)
 
 
 class ListKeysEngine(Engine):
 
-    def _r_run(self, reader: inigrep.core.LineGenT
-               ) -> inigrep.core.KeyGenT:
-        return inigrep.core._r_list_keys(reader=reader, **self.fnargs)
+    def _r_run(self, reader: Iterable[LineT]
+               ) -> Iterable[KeyT]:
+        return _r_list_keys(reader=reader, **self.fnargs)
 
-    def run(self, files: list[str]) -> typing.Iterator[str]:
+    def run(self, files: list[str]) -> Iterable[str]:
         return inigrep.front.list_keys(files=files, **self.fnargs)
 
 
 class ListSectionsEngine(Engine):
 
-    def _r_run(self, reader: inigrep.core.LineGenT
-               ) -> inigrep.core.SectionGenT:
-        return inigrep.front._r_list_sections(reader=reader)
+    def _r_run(self, reader: Iterable[LineT]
+               ) -> Iterable[SectionT]:
+        return _r_list_sections(reader=reader)
 
-    def run(self, files: list[str]) -> typing.Iterator[str]:
+    def run(self, files: list[str]) -> Iterable[str]:
         return inigrep.front.list_sections(files=files)
 
 
 class ListPathsEngine(Engine):
 
-    def _r_run(self, reader: inigrep.core.LineGenT
-               ) -> inigrep.core.KeypathGenT:
-        return inigrep.core._r_list_paths(reader=reader, **self.fnargs)
+    def _r_run(self, reader: Iterable[LineT]
+               ) -> Iterable[KeypathT]:
+        return _r_list_paths(reader=reader, **self.fnargs)
 
-    def run(self, files: list[str]) -> typing.Iterator[str]:
+    def run(self, files: list[str]) -> Iterable[str]:
         return inigrep.front.list_paths(files=files, **self.fnargs)
 
 
 class CloneEngine(Engine):
 
-    def _r_run(self, reader: inigrep.core.LineGenT
-               ) -> inigrep.core.ClonedLineGenT:
-        return inigrep.core._r_clone(reader=reader, **self.fnargs)
+    def _r_run(self, reader: Iterable[LineT]
+               ) -> Iterable[ClonedLineT]:
+        return _r_clone(reader=reader, **self.fnargs)
 
-    def run(self, files: list[str]) -> typing.Iterator[str]:
+    def run(self, files: list[str]) -> Iterable[str]:
         return inigrep.front.clone(files=files, **self.fnargs)
 
 
+@dataclass
 class Options:
+    engine: Engine = NoEngine()
+    oneline: bool = False
+    files: list[str] = field(default_factory=list)
 
     @classmethod
     def from_args(cls, args: list[str]) -> Options:
         o = cls()
         a = Args(args)
         while a.rest():
-            if a.next_is('--help'): raise HelpNeeded()
-            if a.next_is('--version'): raise VersionNeeded()
-            elif a.next_is('-1'):             o.oneline = True; a.take1()
-            elif a.next_is('-c', '--clone'):  o.engine = CloneEngine();        a.take1()
-            elif a.next_is('-s', '--clsct'):  o.engine = CloneEngine(kpath=a.take2()[1] + '.')
-            elif a.next_is('-e', '--basic'):  o.engine = BasicEngine(kpath=a.take2()[1])
-            elif a.next_is('-r', '--raw'):    o.engine = RawEngine(kpath=a.take2()[1])
-            elif a.next_is('-K', '--lskey'):  o.engine = ListKeysEngine(section=a.take2()[1])
-            elif a.next_is('-S', '--lssct'):  o.engine = ListSectionsEngine(); a.take1()
-            elif a.next_is('-P', '--lspth'):  o.engine = ListPathsEngine();    a.take1()
+            if a.next_is('--help'):
+                raise HelpNeeded()
+            if a.next_is('--version'):
+                raise VersionNeeded()
+            elif a.next_is('-1'):
+                o.oneline = True
+                a.take1()
+            elif a.next_is('-c', '--clone'):
+                o.engine = CloneEngine()
+                a.take1()
+            elif a.next_is('-s', '--clsct'):
+                o.engine = CloneEngine(kpath=a.take2()[1] + '.')
+            elif a.next_is('-e', '--basic'):
+                o.engine = BasicEngine(kpath=a.take2()[1])
+            elif a.next_is('-r', '--raw'):
+                o.engine = RawEngine(kpath=a.take2()[1])
+            elif a.next_is('-K', '--lskey'):
+                o.engine = ListKeysEngine(section=a.take2()[1])
+            elif a.next_is('-S', '--lssct'):
+                o.engine = ListSectionsEngine()
+                a.take1()
+            elif a.next_is('-P', '--lspth'):
+                o.engine = ListPathsEngine()
+                a.take1()
             elif a.next().startswith('-'):
                 raise UsageError('unknown engine: %s' % a.next())
-            else: break
+            else:
+                break
         if isinstance(o.engine, NoEngine):
             o.engine = BasicEngine(kpath=a.take1())
         files = a.rest()
         if not files:
             files = ['-']
         elif files == ['']:
             # FIXME: this is strange but turns out saturnin relies on it
             files = ['-']
         o.files = files
         return o
 
-    def __init__(self):
-        self.engine: Engine = NoEngine()
-        self.oneline: bool = False
-        self.files: list[str] = []
-
 
 def main() -> None:
 
     try:
         options = Options.from_args(sys.argv[1:])
     except UsageError as e:
         sys.stderr.write('%s\n' % _USAGE[1:])
         sys.stderr.write('error: %s\n' % e)
         sys.exit(2)
     except HelpNeeded as e:
         sys.stderr.write('%s\n' % __doc__)
         sys.stderr.write('%s\n' % e)
         sys.exit(0)
     except VersionNeeded:
-        sys.stderr.write('%s\n' % inigrep.__version__)
+        sys.stderr.write('%s\n' % VERSION)
         sys.exit(0)
 
     gen = options.engine.run(files=options.files)
 
     try:
         for line in gen:
             print(line)
             if options.oneline:
                 break
-    except inigrep.core.KeypathError as e:
+    except KeypathError as e:
         sys.stderr.write('%s\n' % e)
         sys.exit(2)
```

### Comparing `inigrep-0.5.2/src/inigrep/core.py` & `inigrep-0.5.3/src/inigrep/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/python3
 
 from __future__ import annotations
 
+from dataclasses import dataclass
+from typing import Iterable
 import os
 import re
 import sys
 import typing
 
 
 class NIL:
@@ -23,119 +25,103 @@
 KeyT = typing.NewType('KeyT', str)
 KeypathT = typing.NewType('KeypathT', str)
 LineT = typing.NewType('LineT', str)
 RawValueT = typing.NewType('RawValueT', str)
 SectionT = typing.NewType('SectionT', str)
 ValueT = typing.NewType('ValueT', str)
 
-NoClonedLineT = NIL('NoClonedLineT')
 NoKey = NIL('NoKey')
 NoKeypath = NIL('NoKeypath')
 NoRawValue = NIL('NoRawValue')
 NoSection = NIL('NoSection')
 NoValue = NIL('NoValue')
 
-MaybeClonedLineT = typing.Union[ClonedLineT, NIL]
-MaybeKeyT = typing.Union[KeyT, NIL]
-MaybeKeypathT = typing.Union[KeypathT, NIL]
-MaybeRawValueT = typing.Union[RawValueT, NIL]
-MaybeSectionT = typing.Union[SectionT, NIL]
-MaybeValueT = typing.Union[ValueT, NIL]
-
 IniDataT = dict[KeypathT, typing.List[ValueT]]
 IniRawDataT = dict[KeypathT, typing.List[RawValueT]]
 
-ClonedLineGenT = typing.Iterator[ClonedLineT]
-KeyGenT = typing.Iterator[KeyT]
-KeypathGenT = typing.Iterator[KeypathT]
-LineGenT = typing.Iterator[LineT]
-RawValueGenT = typing.Iterator[RawValueT]
-SectionGenT = typing.Iterator[SectionT]
-ValueGenT = typing.Iterator[ValueT]
-
 
 class KeypathError(ValueError):
     pass
 
 
 def check_kpath(v, vn, t):
     if not isinstance(v, t):
         raise KeypathError("invalid type: %s must be %s, got %s"
                            % (vn, t.__name__, type(v).__name__))
 
 
+@dataclass
 class Unit:
     """
     A parsed line
     """
+    ctx_section: SectionT | NIL
+    raw_line: LineT
+    section: SectionT | NIL = NoSection
+    key: KeyT | NIL = NoKey
+    value: ValueT | NIL = NoValue
+    raw_value: RawValueT | NIL = NoRawValue
 
     @classmethod
     def mkcomment(cls,
-                  ctx_section: MaybeSectionT,
+                  ctx_section: SectionT | NIL,
                   raw_line: LineT,
                   ) -> Unit:
-        return cls(ctx_section, raw_line)
+        return cls(
+            ctx_section=ctx_section,
+            raw_line=raw_line,
+        )
 
     @classmethod
     def mksection(cls,
-                  ctx_section: MaybeSectionT,
+                  ctx_section: SectionT | NIL,
                   raw_line: LineT,
                   section: SectionT,
                   ) -> Unit:
-        return cls(section, raw_line, section=section)
+        return cls(
+            ctx_section=section,
+            raw_line=raw_line,
+            section=section,
+        )
 
     @classmethod
     def mkjunk(cls,
-               ctx_section: MaybeSectionT,
+               ctx_section: SectionT | NIL,
                raw_line: LineT,
                ) -> Unit:
-        return cls(ctx_section, raw_line)
-
-    def __init__(self,
-                 ctx_section: MaybeSectionT,
-                 raw_line: LineT,
-                 section: MaybeSectionT = NoSection,
-                 key: MaybeKeyT = NoKey,
-                 value: MaybeValueT = NoValue,
-                 raw_value: MaybeRawValueT = NoRawValue,
-                 ):
-        self.raw_line = raw_line
-        self.ctx_section = ctx_section
-        self.section = section
-        self.key = key
-        self.value = value
-        self.raw_value = raw_value
+        return cls(
+            ctx_section=ctx_section,
+            raw_line=raw_line,
+        )
 
     def __str__(self):
         cn = self.__class__.__name__
         return f'{cn}[{self.ctx_section}](s={self.section},k={self.key})'
 
     @property
-    def keypath(self) -> MaybeKeypathT:
+    def keypath(self) -> KeypathT | NIL:
         if isinstance(self.ctx_section, NIL):
             return NoKeypath
         if isinstance(self.key, NIL):
             return NoKeypath
         return KeypathT(self.ctx_section + '.' + self.key)
 
     @property
-    def cloned_lines(self) -> ClonedLineGenT:
+    def cloned_lines(self) -> Iterable[ClonedLineT]:
         if not isinstance(self.section, NIL):
             yield ClonedLineT('')
             yield ClonedLineT(f'[{self.section}]')
         if isinstance(self.ctx_section, NIL):
             return
         if isinstance(self.key, NIL):
             return
         yield ClonedLineT(f'    {self.key} ={self.raw_value}')
 
 
-UnitGenT = typing.Iterator[Unit]
-
-
+@dataclass
 class Cond:
 
     @classmethod
     def from_arg(cls, arg: str,
                  require_key: bool = True,
                  require_sct: bool = True) -> Cond:
         def refuse_kp(msg):
@@ -170,150 +156,138 @@
                                % type(sct).__name__)
         if not sct:
             raise KeypathError(r"section must not be empty: %r" % sct)
         if r']' in sct:
             raise KeypathError(r"invalid char ']' in section name: %r" % sct)
         return SectionCond(sct)
 
-    def __init__(self, pat: typing.Any):
-        self.pat = pat
-
-    def __str__(self):
-        cn = self.__class__.__name__
-        return f'{cn}(pat={self.pat})'
-
     def match(self, unit: Unit) -> bool:
         raise NotImplementedError
 
 
+@dataclass
 class AlwaysMatchingCond(Cond):
 
-    def __init__(self):
-        pass
-
     def __str__(self):
         cn = self.__class__.__name__
         return f'{cn}()'
 
     def match(self, unit: Unit) -> bool:
         return True
 
 
+@dataclass
 class SectionCond(Cond):
+    want_sct: str
 
     @classmethod
     def _from_arg(cls, arg: str) -> SectionCond:
         if r']' in arg:
             raise KeypathError(r"invalid char ']' in section name: %r" % arg)
         return cls(arg)
 
-    def __init__(self, want_sct: str):
-        self.want_sct = want_sct
-
     def __str__(self):
         cn = self.__class__.__name__
         return f'{cn}(want={self.want_sct})'
 
     def match(self, unit: Unit) -> bool:
         return unit.ctx_section == self.want_sct
 
 
+@dataclass
 class KeyCond(Cond):
+    pat: str
 
     @classmethod
     def _from_arg(cls, arg: str) -> KeyCond:
         if r'\\'[0] in arg:
             raise KeypathError(r"invalid char '\' in key name: %r" % arg)
         if r'[' in arg:
             raise KeypathError(r"invalid char '[' in key name: %r" % arg)
         if r'=' in arg:
             raise KeypathError(r"invalid char '=' in key name: %r" % arg)
         return cls(arg)
 
-    def __init__(self, pat: str):
-        self.pat = pat
-
     def __str__(self):
         cn = self.__class__.__name__
         return f'{cn}(want={self.pat})'
 
     def match(self, unit: Unit) -> bool:
         return unit.key == self.pat
 
 
+@dataclass
 class KeypathCond(Cond):
-
-    def __init__(self, sctcond: SectionCond, keycond: KeyCond):
-        self.sctcond = sctcond
-        self.keycond = keycond
+    sctcond: SectionCond
+    keycond: KeyCond
 
     def __str__(self):
         cn = self.__class__.__name__
         return f'{cn}(s={self.sctcond},k={self.keycond})'
 
     def match(self, unit: Unit) -> bool:
         return self.sctcond.match(unit) and self.keycond.match(unit)
 
 
-def extract_sections(units: typing.Iterator[Unit]) -> SectionGenT:
+def extract_sections(units: typing.Iterator[Unit]) -> Iterable[SectionT]:
     seen = set()
     for unit in units:
         if isinstance(unit.section, NIL):
             continue
         if unit.section in seen:
             continue
         seen.add(unit.section)
         yield unit.section
 
 
-def extract_clones(units: typing.Iterator[Unit]) -> ClonedLineGenT:
+def extract_clones(units: typing.Iterator[Unit]) -> Iterable[ClonedLineT]:
     for unit in units:
         if isinstance(unit.cloned_lines, NIL):
             continue
         for cloned_line in unit.cloned_lines:
             yield cloned_line
 
 
-def extract_keypaths(units: typing.Iterator[Unit]) -> KeypathGenT:
+def extract_keypaths(units: typing.Iterator[Unit]) -> Iterable[KeypathT]:
     seen = set()
     for unit in units:
         if isinstance(unit.keypath, NIL):
             continue
         if unit.keypath in seen:
             continue
         seen.add(unit.keypath)
         yield unit.keypath
 
 
-def extract_keys(units: typing.Iterator[Unit]) -> KeyGenT:
+def extract_keys(units: typing.Iterator[Unit]) -> Iterable[KeyT]:
     seen = set()
     for unit in units:
         if isinstance(unit.key, NIL):
             continue
         if unit.key in seen:
             continue
         seen.add(unit.key)
         yield unit.key
 
 
-def extract_values(units: typing.Iterator[Unit]) -> ValueGenT:
+def extract_values(units: typing.Iterator[Unit]) -> Iterable[ValueT]:
     for unit in units:
         if isinstance(unit.value, NIL):
             continue
         yield unit.value
 
 
-def extract_raw_values(units: typing.Iterator[Unit]) -> RawValueGenT:
+def extract_raw_values(units: typing.Iterator[Unit]) -> Iterable[RawValueT]:
     for unit in units:
         if isinstance(unit.raw_value, NIL):
             continue
         yield unit.raw_value
 
 
-def mkpipe(reader: LineGenT,
+def mkpipe(reader: Iterable[LineT],
            cond: Cond,
            extractor: typing.Callable[[typing.Iterator[Unit]], typing.Any],
            ):
     parser = Parser()
 #   matched = []
 #   units = list(parser.parse(reader))
 #   for unit in units:
@@ -333,68 +307,68 @@
 #       yield thing
 #   return extractor(matched)
     units = (unit for unit in parser.parse(reader)
              if cond.match(unit))
     return extractor(units)
 
 
+@dataclass
 class Parser:
     """
     Parse lines to units
     """
-
-    def __init__(self):
-        self.ctx_section = NoSection
+    ctx_section: SectionT | NIL = NoSection
 
     def _parse_line(self,
                     line: LineT,
-                    ctx_section: MaybeSectionT = NoSection
+                    ctx_section: SectionT | NIL = NoSection
                     ) -> Unit:
         def strip_raw(V):
             return re.sub(r'  *[#;].*', '', V.strip())
         if re.match(r'^\s*[#;]', line):
             return Unit.mkcomment(ctx_section, line)
         if re.match(r'^\s*\[[^]]+\]', line):
             left, _ = line.split(']', maxsplit=1)
             _, sctn = left.split('[', maxsplit=1)
             return Unit.mksection(ctx_section, line, SectionT(sctn))
         if '=' not in line:
             return Unit.mkjunk(ctx_section, line)
         key, raw_value = line.lstrip().split('=', 1)
         return Unit(
-            ctx_section, line,
-            NoSection,
-            KeyT(key.strip()),
-            ValueT(strip_raw(raw_value)),
-            RawValueT(raw_value),
+            ctx_section=ctx_section,
+            raw_line=line,
+            section=NoSection,
+            key=KeyT(key.strip()),
+            value=ValueT(strip_raw(raw_value)),
+            raw_value=RawValueT(raw_value),
         )
 
     def parse(self,
-              lines: LineGenT,
-              ) -> UnitGenT:
+              lines: Iterable[LineT],
+              ) -> Iterable[Unit]:
         for line in lines:
             unit = self._parse_line(line, self.ctx_section)
             self.ctx_section = unit.ctx_section
             yield unit
 
 
-def _r_clone(reader: LineGenT, kpath: str = '.') -> ClonedLineGenT:
+def _r_clone(reader: Iterable[LineT], kpath: str = '.') -> Iterable[ClonedLineT]:
     """
     Return replica of INI file provided by *reader*.
     """
     pipe = mkpipe(
         reader=reader,
         cond=Cond.from_arg(kpath, require_sct=False, require_key=False),
         extractor=extract_clones,
     )
     for line in pipe:
         yield ClonedLineT(line)
 
 
-def _r_data(reader: LineGenT) -> dict[KeyT, list[ValueT]]:
+def _r_data(reader: Iterable[LineT]) -> dict[KeyT, list[ValueT]]:
     """
     Return dict of all keypaths and values found by *reader*
 
     *reader* must be instance of FileReader generator or any similar
     generator that will yield lines.
     """
     lines = list(reader)
@@ -412,15 +386,15 @@
         )
         if keypath not in out:
             out[keypath] = []
         out[keypath].extend(value_pipe)
     return out
 
 
-def _r_raw_data(reader: LineGenT) -> dict[KeyT, list[RawValueT]]:
+def _r_raw_data(reader: Iterable[LineT]) -> dict[KeyT, list[RawValueT]]:
     """
     Return dict of all keypaths and raw values found by *reader*
 
     *reader* must be instance of FileReader generator or any similar
     generator that will yield lines.
     """
     lines = list(reader)
@@ -438,15 +412,15 @@
         )
         if keypath not in out:
             out[keypath] = []
         out[keypath].extend(value_pipe)
     return out
 
 
-def _r_values(reader: LineGenT, kpath: str) -> ValueGenT:
+def _r_values(reader: Iterable[LineT], kpath: str) -> Iterable[ValueT]:
     """
     Return list of values found by *reader* at key path *kpath*.
 
     *kpath* must be key path, i.e. string containing section and
     key names delimited by period.
 
     *reader* must be instance of FileReader generator or any similar
@@ -457,15 +431,15 @@
         cond=Cond.from_arg(kpath),
         extractor=extract_values,
     )
     for line in pipe:
         yield ValueT(line)
 
 
-def _r_raw_values(reader: LineGenT, kpath: str) -> RawValueGenT:
+def _r_raw_values(reader: Iterable[LineT], kpath: str) -> Iterable[RawValueT]:
     """
     Return list of raw values found by *reader* at key path *kpath*.
 
     Same as _r_values(), but uses raw inigrep engine, which keeps in-line
     comments and value leading/trailing whitespace.
     """
     pipe = mkpipe(
@@ -473,76 +447,76 @@
         cond=Cond.from_arg(kpath),
         extractor=extract_raw_values,
     )
     for line in pipe:
         yield RawValueT(line)
 
 
-def _r_list_sections(reader: LineGenT) -> SectionGenT:
+def _r_list_sections(reader: Iterable[LineT]) -> Iterable[SectionT]:
     """
     Return list of sections found by *reader*.
     """
     pipe = mkpipe(
         reader=reader,
         cond=AlwaysMatchingCond(),
         extractor=extract_sections,
     )
     for line in pipe:
         yield SectionT(line)
 
 
-def _r_list_keys(reader: LineGenT, section: str) -> KeyGenT:
+def _r_list_keys(reader: Iterable[LineT], section: str) -> Iterable[KeyT]:
     """
     Return list of keys found by *reader* under *section*.
     """
     pipe = mkpipe(
         reader=reader,
         cond=Cond.from_sct(section),
         extractor=extract_keys,
     )
     for line in pipe:
         yield KeyT(line)
 
 
-def _r_list_paths(reader: LineGenT, keypath: str = '.') -> KeypathGenT:
+def _r_list_paths(reader: Iterable[LineT], keypath: str = '.') -> Iterable[KeypathT]:
     """
     Return list of all key paths found by *reader*.
     """
     pipe = mkpipe(
         reader=reader,
         cond=Cond.from_arg(keypath, require_sct=False, require_key=False),
         extractor=extract_keypaths,
     )
     for line in pipe:
         yield KeypathT(line)
 
 
-def FileReader(files: list[str]) -> LineGenT:
+def FileReader(files: list[str]) -> Iterable[LineT]:
     """
     Line generator that reads multiple files
     """
     for path in files:
         for line in SingleFileReader(path):
             yield line
 
 
-def ExistingFileReader(files: list[str]) -> LineGenT:
+def ExistingFileReader(files: list[str]) -> Iterable[LineT]:
     """
     Line generator that reads multiple existent files
 
     Non-existent files are silently ignored.
     """
     for path in files:
         if not os.path.exists(path):
             continue
         for line in SingleFileReader(path):
             yield line
 
 
-def SingleFileReader(path: str) -> LineGenT:
+def SingleFileReader(path: str) -> Iterable[LineT]:
     """
     Line generator that reads single path
     """
     if path == '-':
         while True:
             line = sys.stdin.readline()
             if line:
```

### Comparing `inigrep-0.5.2/src/inigrep/front.py` & `inigrep-0.5.3/src/inigrep/front.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 #!/usr/bin/python3
 
 from __future__ import annotations
+from typing import Callable, Iterable
+import functools
+import os
 
 from .core import (
-    Cond,
     FileReader,
     _r_clone,
     _r_list_keys,
     _r_list_paths,
     _r_list_sections,
     _r_raw_values,
     _r_values,
     SingleFileReader,
     KeypathT,
-    KeyT,
     SectionT,
 )
 
-import functools
-import os
-import typing
-
-
 __doc__ = """
 inigrep
 =======
 
 grep for (some) INIs
 
 inigrep is designed to read a particular simplistic dialect of
@@ -125,62 +121,62 @@
 would list all keys from section 'foo'
 
     bar
     qux
 """
 
 
-def clone(files: list[str], kpath: str = '.') -> typing.Iterator[str]:
+def clone(files: list[str], kpath: str = '.') -> Iterable[str]:
     """
     Return replica of INI file that is concatenation of *files*.
     """
     for value in _r_clone(reader=FileReader(files), kpath=kpath):
         yield str(value)
 
 
-def values(files: list[str], kpath: str) -> typing.Iterator[str]:
+def values(files: list[str], kpath: str) -> Iterable[str]:
     """
     Return list of values from files *files* at key path *kpath*.
 
     *kpath* must be key path, i.e. string containing section and
     key names delimited by period.
 
     *files* must list of file paths.
     """
     for value in _r_values(reader=FileReader(files), kpath=kpath):
         yield str(value)
 
 
-def raw_values(files: list[str], kpath: str) -> typing.Iterator[str]:
+def raw_values(files: list[str], kpath: str) -> Iterable[str]:
     """
     Return list of raw values found in *files* at key path *kpath*.
 
     Same as values(), but uses raw inigrep engine, which keeps in-line
     comments and value leading/trailing whitespace.
     """
     for value in _r_raw_values(reader=FileReader(files), kpath=kpath):
         yield str(value)
 
 
-def list_sections(files: list[str]) -> typing.Iterator[str]:
+def list_sections(files: list[str]) -> Iterable[str]:
     """
     Return list of sections found in *files*.
     """
     for value in _r_list_sections(reader=FileReader(files)):
         yield str(value)
 
 
-def list_keys(files: list[str], section: str) -> typing.Iterator[str]:
+def list_keys(files: list[str], section: str) -> Iterable[str]:
     """
     Return list of keys found in *files* under *section*.
     """
     return _r_list_keys(reader=FileReader(files), section=section)
 
 
-def list_paths(files: list[str], keypath: str = '.') -> typing.Iterator[str]:
+def list_paths(files: list[str], keypath: str = '.') -> Iterable[str]:
     """
     Return list of all key paths found by *in files*.
     """
     return _r_list_paths(reader=FileReader(files), keypath=keypath)
 
 
 def load(files: list[str]) -> Ini:
@@ -250,15 +246,15 @@
             lines.append('[%s]' % sct)
             for key in self.list_keys('%s.%s' % (prefix, sct)):
                 branch_keypath = '%s.%s.%s' % (prefix, sct, key)
                 for value in self.raw_values(branch_keypath):
                     lines.append('    %s =%s' % (key, value))
         return self.__class__(lines)
 
-    def mkreader1(self, *kpath: str) -> typing.Callable:
+    def mkreader1(self, *kpath: str) -> Callable[[], str | None]:
         """
         Create function to read single-line value at *kpath*.
 
         *kpath* must be list of the path elements.
 
         Return function which can be called without parameters and
         will return either single-line string corresponding to value
@@ -268,15 +264,15 @@
         def _read1(*kpath):
             out = list(self.values('.'.join(kpath)))
             if out:
                 return out[0]
             return None
         return functools.partial(_read1, *kpath)
 
-    def mkreaderN(self, *kpath: str) -> typing.Callable:
+    def mkreaderN(self, *kpath: str) -> Callable[[], list[str]]:
         """
         Create function to read multi-line value at *kpath*.
 
         *kpath* must be list of the path elements.
 
         Return function which can be called without parameters and
         will return either list of strings corresponding to values
@@ -301,17 +297,17 @@
         keypaths to lists of lines.
         """
         data: dict[str, list[str]] = {}
         for kpath in self.list_paths():
             data[kpath] = list(self.values(kpath))
         return data
 
-    def clone(self, kpath: str = '.') -> typing.Iterator[str]:
+    def clone(self, kpath: str = '.') -> Iterable[str]:
         """
-        Return replica of INI file that is concatenation of *files*.
+        Return lines of INI file with the same data as in this object
         """
         vg = _r_clone(
             reader=self._cache_reader(),
             kpath=KeypathT(kpath),
         )
         return (str(v) for v in vg)
 
@@ -323,63 +319,63 @@
         comments and value leading/trailing whitespace).
         """
         data: dict[str, list[str]] = {}
         for kpath in self.list_paths():
             data[kpath] = list(self.raw_values(kpath))
         return data
 
-    def values(self, kpath: str) -> typing.Iterator[str]:
+    def values(self, kpath: str) -> Iterable[str]:
         """
         Return list of values at key path *kpath*.
 
         Uses basic inigrep engine.
         """
         vg = _r_values(
             reader=self._cache_reader(),
             kpath=KeypathT(kpath),
         )
         return (str(v) for v in vg)
 
-    def raw_values(self, kpath: str) -> typing.Iterator[str]:
+    def raw_values(self, kpath: str) -> Iterable[str]:
         """
         Return list of values at key path *kpath*.
 
         Same as Ini.values(), but uses raw inigrep engine (keeps
         comments and value leading/trailing whitespace).
         """
         vg = _r_raw_values(
             reader=self._cache_reader(),
             kpath=KeypathT(kpath),
         )
         return (str(v) for v in vg)
 
-    def list_sections(self) -> typing.Iterator[str]:
+    def list_sections(self) -> Iterable[str]:
         """
         Return list of sections.
 
         Similar to Ini.values(), but uses section listing engine.
         """
         vg = _r_list_sections(
             reader=self._cache_reader(),
         )
         return (str(v) for v in vg)
 
-    def list_keys(self, section: str) -> typing.Iterator[str]:
+    def list_keys(self, section: str) -> Iterable[str]:
         """
         Return list of keys under *section*.
 
         Similar to Ini.values(), but uses key listing engine.
         """
         vg = _r_list_keys(
             reader=self._cache_reader(),
             section=SectionT(section),
         )
         return (str(v) for v in vg)
 
-    def list_paths(self, keypath: str = '.') -> typing.Iterator[str]:
+    def list_paths(self, keypath: str = '.') -> Iterable[str]:
         """
         Return list of all defined key paths.
 
         Similar to Ini.values(), but uses key path listing engine.
         """
         vg = _r_list_paths(
             reader=self._cache_reader(),
```

### Comparing `inigrep-0.5.2/tests/test_inigrep.py` & `inigrep-0.5.3/tests/test_inigrep.py`

 * *Files identical despite different names*

