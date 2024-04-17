# Comparing `tmp/delvewheel-1.5.4.tar.gz` & `tmp/delvewheel-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delvewheel-1.5.4.tar", last modified: Thu Mar  7 19:43:12 2024, max compression
+gzip compressed data, was "delvewheel-1.6.0.tar", last modified: Wed Apr 17 17:40:38 2024, max compression
```

## Comparing `delvewheel-1.5.4.tar` & `delvewheel-1.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 19:43:12.365558 delvewheel-1.5.4/
--rw-rw-rw-   0        0        0     1073 2024-03-07 19:42:49.000000 delvewheel-1.5.4/LICENSE
--rw-rw-rw-   0        0        0    11674 2024-03-07 19:43:12.365558 delvewheel-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0    10531 2024-03-07 19:42:49.000000 delvewheel-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-07 19:43:12.365558 delvewheel-1.5.4/delvewheel/
--rw-rw-rw-   0        0        0        0 2024-03-07 19:42:49.000000 delvewheel-1.5.4/delvewheel/__init__.py
--rw-rw-rw-   0        0        0     6020 2024-03-07 19:42:49.000000 delvewheel-1.5.4/delvewheel/__main__.py
--rw-rw-rw-   0        0        0   140462 2024-03-07 19:42:49.000000 delvewheel-1.5.4/delvewheel/_dll_list.py
--rw-rw-rw-   0        0        0    35567 2024-03-07 19:42:49.000000 delvewheel-1.5.4/delvewheel/_dll_utils.py
--rw-rw-rw-   0        0        0       23 2024-03-07 19:42:49.000000 delvewheel-1.5.4/delvewheel/_version.py
--rw-rw-rw-   0        0        0    54598 2024-03-07 19:42:49.000000 delvewheel-1.5.4/delvewheel/_wheel_repair.py
-drwxrwxrwx   0        0        0        0 2024-03-07 19:43:12.365558 delvewheel-1.5.4/delvewheel.egg-info/
--rw-rw-rw-   0        0        0    11674 2024-03-07 19:43:12.000000 delvewheel-1.5.4/delvewheel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-03-07 19:43:12.000000 delvewheel-1.5.4/delvewheel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 19:43:12.000000 delvewheel-1.5.4/delvewheel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-03-07 19:43:12.000000 delvewheel-1.5.4/delvewheel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2024-03-07 19:43:12.000000 delvewheel-1.5.4/delvewheel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-07 19:43:12.000000 delvewheel-1.5.4/delvewheel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2024-03-07 19:42:49.000000 delvewheel-1.5.4/pyproject.toml
--rw-rw-rw-   0        0        0     1214 2024-03-07 19:43:12.365558 delvewheel-1.5.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 17:40:38.040904 delvewheel-1.6.0/
+-rw-rw-rw-   0        0        0     1073 2024-04-17 17:40:13.000000 delvewheel-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0    11925 2024-04-17 17:40:38.040904 delvewheel-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10782 2024-04-17 17:40:13.000000 delvewheel-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 17:40:38.040904 delvewheel-1.6.0/delvewheel/
+-rw-rw-rw-   0        0        0        0 2024-04-17 17:40:13.000000 delvewheel-1.6.0/delvewheel/__init__.py
+-rw-rw-rw-   0        0        0     6181 2024-04-17 17:40:13.000000 delvewheel-1.6.0/delvewheel/__main__.py
+-rw-rw-rw-   0        0        0   140462 2024-04-17 17:40:13.000000 delvewheel-1.6.0/delvewheel/_dll_list.py
+-rw-rw-rw-   0        0        0    36257 2024-04-17 17:40:13.000000 delvewheel-1.6.0/delvewheel/_dll_utils.py
+-rw-rw-rw-   0        0        0       23 2024-04-17 17:40:13.000000 delvewheel-1.6.0/delvewheel/_version.py
+-rw-rw-rw-   0        0        0    54806 2024-04-17 17:40:13.000000 delvewheel-1.6.0/delvewheel/_wheel_repair.py
+drwxrwxrwx   0        0        0        0 2024-04-17 17:40:38.040904 delvewheel-1.6.0/delvewheel.egg-info/
+-rw-rw-rw-   0        0        0    11925 2024-04-17 17:40:38.000000 delvewheel-1.6.0/delvewheel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-04-17 17:40:38.000000 delvewheel-1.6.0/delvewheel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 17:40:38.000000 delvewheel-1.6.0/delvewheel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-17 17:40:38.000000 delvewheel-1.6.0/delvewheel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-04-17 17:40:38.000000 delvewheel-1.6.0/delvewheel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-17 17:40:38.000000 delvewheel-1.6.0/delvewheel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2024-04-17 17:40:13.000000 delvewheel-1.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1214 2024-04-17 17:40:38.040904 delvewheel-1.6.0/setup.cfg
```

### Comparing `delvewheel-1.5.4/LICENSE` & `delvewheel-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `delvewheel-1.5.4/PKG-INFO` & `delvewheel-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delvewheel
-Version: 1.5.4
+Version: 1.6.0
 Summary: Self-contained wheels for Windows
 Home-page: https://github.com/adang1345/delvewheel
 Author: Aohan Dang
 Author-email: adang1345@gmail.com
 License: MIT
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
@@ -92,14 +92,15 @@
 - `--no-mangle-all`: don't mangle any DLL names
 - `--strip`: strip DLLs that contain an overlay when name-mangling. The GNU `strip` utility must be present in `PATH`.
 - `-L`,`--lib-sdir`: subdirectory suffix to store vendored DLLs (default `.libs`). For example, if your wheel is named `mywheel-0.0.1-cp310-cp310-win_amd64.whl`, then the vendored DLLs are stored in `mywheel.libs` by default. If your wheel contains a top-level extension module that is not in any package, then this setting is ignored, and vendored DLLs are instead placed directly into `site-packages` when the wheel is installed.
 - `--namespace-pkg`: namespace packages, specified in case-sensitive dot notation and delimited by the path separator. Normally, we patch or create `__init__.py` in each top-level package to add the vendored DLL location to the DLL search path at runtime. If you have a top-level namespace package that requires `__init__.py` to be absent or unmodified, then this technique can cause problems. This option tells `delvewheel` to use an alternate strategy that does not create or modify `__init__.py` at the root of the given namespace package(s). For example,
   - `--namespace-pkg package1` declares `package1` as a namespace package.
   - On Windows, `--namespace-pkg package1.package2;package3` declares `package1`, `package1\package2`, and `package3` as namespace packages.
 - `--include-symbols`: include `.pdb` symbol files with the vendored DLLs. To be included, a symbol file must be in the same directory as the DLL and have the same filename before the extension, e.g. `example.dll` and `example.pdb`.
+- `--include-imports`: include `.lib` import library files with the vendored DLLs. To be included, an import library file must be in the same directory as the DLL and have the same filename before the extension, e.g. `example.dll` and `example.lib`.
 
 ## Limitations
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. We avoid vendoring system libraries that are provided by Windows 7 SP1 or later. If you intend to create a wheel for an older Windows system that requires an extra DLL, use the `--add-dll` flag to vendor additional DLLs into the wheel.
 - To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain an overlay at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, the overlay consists of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the overlay, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the overlay and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
```

### Comparing `delvewheel-1.5.4/README.md` & `delvewheel-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 - `--no-mangle-all`: don't mangle any DLL names
 - `--strip`: strip DLLs that contain an overlay when name-mangling. The GNU `strip` utility must be present in `PATH`.
 - `-L`,`--lib-sdir`: subdirectory suffix to store vendored DLLs (default `.libs`). For example, if your wheel is named `mywheel-0.0.1-cp310-cp310-win_amd64.whl`, then the vendored DLLs are stored in `mywheel.libs` by default. If your wheel contains a top-level extension module that is not in any package, then this setting is ignored, and vendored DLLs are instead placed directly into `site-packages` when the wheel is installed.
 - `--namespace-pkg`: namespace packages, specified in case-sensitive dot notation and delimited by the path separator. Normally, we patch or create `__init__.py` in each top-level package to add the vendored DLL location to the DLL search path at runtime. If you have a top-level namespace package that requires `__init__.py` to be absent or unmodified, then this technique can cause problems. This option tells `delvewheel` to use an alternate strategy that does not create or modify `__init__.py` at the root of the given namespace package(s). For example,
   - `--namespace-pkg package1` declares `package1` as a namespace package.
   - On Windows, `--namespace-pkg package1.package2;package3` declares `package1`, `package1\package2`, and `package3` as namespace packages.
 - `--include-symbols`: include `.pdb` symbol files with the vendored DLLs. To be included, a symbol file must be in the same directory as the DLL and have the same filename before the extension, e.g. `example.dll` and `example.pdb`.
+- `--include-imports`: include `.lib` import library files with the vendored DLLs. To be included, an import library file must be in the same directory as the DLL and have the same filename before the extension, e.g. `example.dll` and `example.lib`.
 
 ## Limitations
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. We avoid vendoring system libraries that are provided by Windows 7 SP1 or later. If you intend to create a wheel for an older Windows system that requires an extra DLL, use the `--add-dll` flag to vendor additional DLLs into the wheel.
 - To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain an overlay at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, the overlay consists of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the overlay, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the overlay and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
```

### Comparing `delvewheel-1.5.4/delvewheel/__main__.py` & `delvewheel-1.6.0/delvewheel/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     parser_repair.add_argument('--no-mangle', default='', metavar='DLLS', type=_dll_names, help=f'DLL names(s) not to mangle, {os.pathsep!r}-delimited')
     parser_repair.add_argument('--no-mangle-all', action='store_true', help="don't mangle any DLL names")
     parser_repair.add_argument('--strip', action='store_true', help='strip DLLs that contain trailing data when name-mangling')
     parser_repair.add_argument('-L', '--lib-sdir', default='.libs', type=_subdir_suffix, help='directory suffix in package to store vendored DLLs (default .libs)')
     parser_repair.add_argument('--namespace-pkg', default='', metavar='PKGS', type=_namespace_pkgs, help=f'namespace package(s), {os.pathsep!r}-delimited')
     parser_repair.add_argument('--no-diagnostic', action='store_true', help=argparse.SUPPRESS)  # don't write diagnostic information to DELVEWHEEL metadata file
     parser_repair.add_argument('--include-symbols', action='store_true', help='include .pdb symbol files with vendored DLLs')
+    parser_repair.add_argument('--include-imports', action='store_true', help='include .lib import library files with the vendored DLLs')
     parser_needed.add_argument('file', help='path to a DLL or PYD file')
     parser_needed.add_argument('-v', action='count', default=0, help='verbosity')
     args = parser.parse_args()
 
     # handle command
     if args.command in ('show', 'repair'):
         add_paths = dict.fromkeys(os.path.abspath(path) for path in args.add_path.split(os.pathsep) if path)
@@ -77,15 +78,15 @@
         for wheel in args.wheel:
             wr = WheelRepair(wheel, args.extract_dir, add_dlls, no_dlls, args.ignore_in_wheel, args.v, args.test.split(','))
             if args.command == 'show':
                 wr.show()
             else:  # args.command == 'repair'
                 no_mangles = set(dll_name.lower() for dll_name in args.no_mangle.split(os.pathsep) if dll_name)
                 namespace_pkgs = set(tuple(namespace_pkg.split('.')) for namespace_pkg in args.namespace_pkg.split(os.pathsep) if namespace_pkg)
-                wr.repair(args.target, no_mangles, args.no_mangle_all, args.strip, args.lib_sdir, not args.no_diagnostic and 'SOURCE_DATE_EPOCH' not in os.environ, namespace_pkgs, args.include_symbols)
+                wr.repair(args.target, no_mangles, args.no_mangle_all, args.strip, args.lib_sdir, not args.no_diagnostic and 'SOURCE_DATE_EPOCH' not in os.environ, namespace_pkgs, args.include_symbols, args.include_imports)
     else:  # args.command == 'needed'
         for dll_name in sorted(_dll_utils.get_direct_needed(args.file, args.v), key=str.lower):
             print(dll_name)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `delvewheel-1.5.4/delvewheel/_dll_list.py` & `delvewheel-1.6.0/delvewheel/_dll_list.py`

 * *Files identical despite different names*

### Comparing `delvewheel-1.5.4/delvewheel/_dll_utils.py` & `delvewheel-1.6.0/delvewheel/_dll_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -229,69 +229,84 @@
         return lambda directory, arch: translate_system32_to_syswow64(directory) if arch is MachineType.I386 else directory
     return null_translator
 
 
 _translate_directory = _translate_directory()
 
 
-def find_library(name: str, wheel_dirs: typing.Optional[typing.Iterable], arch: MachineType, include_symbols: bool) -> typing.Optional[typing.Tuple[str, typing.Optional[str]]]:
+def find_library(
+        name: str,
+        wheel_dirs: typing.Optional[typing.Iterable],
+        arch: MachineType,
+        include_symbols: bool,
+        include_imports: bool) -> typing.Optional[typing.Tuple[str, typing.List[str]]]:
     """Given the name of a DLL, return a tuple where
     - the 1st element is the path to the DLL
-    - the 2nd element is
-      - if include_symbols is False, then None
-      - if include_symbols is True, then the path to the .pdb symbol file next
-        to the DLL if it exists, None otherwise. Excluding the file extension,
-        the name of the symbol file is assumed to be the same as the name of
-        the DLL.
-    If the DLL cannot be found, then return None. DLL and symbol file names are
-    searched in a case-insensitive fashion. The search goes in the following
-    order and considers only the DLLs with the architecture arch.
+    - the 2nd element is a list that may contain paths to the .pdb symbol file
+      and/or the .lib import library file associated with the DLL. If
+      include_symbols is True, then search for the .pdb symbol file. If
+      include_imports is True, then search for the .lib import library file.
+      Excluding the file extension, the name of the associated file is assumed
+      to be the same as the name of the DLL.
+
+    If the DLL cannot be found, then return None. All file names are searched
+    in a case-insensitive fashion. If we are on a case-sensitive file system
+    and a directory contains more than one file whose name matches what we're
+    searching for, and the file names differ by case only, then choose one
+    arbitrarily. The search goes in the following order and considers only the
+    DLLs with the architecture arch.
 
     1. If not None, the directories in wheel_dirs. We never search for symbol
-       files in wheel_dirs.
+       files or import library files in wheel_dirs.
     2. The PATH environment variable, with any applicable adjustments due to
-       the Windows file system redirector. If we are on a case-sensitive file
-       system and a directory contains more than one DLL with the correct
-       architecture that differs by case only, then choose one arbitrarily."""
+       the Windows file system redirector."""
     name = name.lower()
     if wheel_dirs is not None:
         for wheel_dir in wheel_dirs:
             try:
                 contents = os.listdir(wheel_dir)
             except FileNotFoundError:
                 continue
             for item in contents:
                 if name == item.lower():
                     path = os.path.join(wheel_dir, item)
                     if os.path.isfile(path) and get_arch(path) == arch:
-                        return path, None
+                        return path, []
     for directory in os.environ['PATH'].split(os.pathsep):
         directory = _translate_directory(directory, arch)
         try:
             contents = os.listdir(directory)
         except FileNotFoundError:
             continue
         dll_path = None
         for item in contents:
             if name == item.lower():
                 path = os.path.join(directory, item)
                 if os.path.isfile(path) and get_arch(path) == arch:
                     dll_path = path
                     break
-        symbol_path = None
-        if dll_path and include_symbols:
+        associated_paths = []
+        if include_symbols:
             symbol_name = os.path.splitext(name)[0] + '.pdb'
             for item in contents:
                 if symbol_name == item.lower():
                     path = os.path.join(directory, item)
                     if os.path.isfile(path):
-                        symbol_path = path
+                        associated_paths.append(path)
+                        break
+        if include_imports:
+            imports_name = os.path.splitext(name)[0] + '.lib'
+            for item in contents:
+                if imports_name == item.lower():
+                    path = os.path.join(directory, item)
+                    if os.path.isfile(path):
+                        associated_paths.append(path)
                         break
         if dll_path:
-            return dll_path, symbol_path
+            return dll_path, associated_paths
     return None
 
 
 def get_direct_needed(lib_path: str, verbose: int) -> set:
     """Given the path to a shared library, return a set containing the DLL
     names of all its direct dependencies. Regular and delay-load dependencies
     are included. The DLL names are in the original case."""
@@ -342,40 +357,44 @@
 
 
 def get_all_needed(lib_path: str,
                    no_dlls: set,
                    wheel_dirs: typing.Optional[typing.Iterable],
                    on_error: str,
                    include_symbols: bool,
+                   include_imports: bool,
                    verbose: int) -> typing.Tuple[typing.Set[str], typing.Set[str], typing.Set[str], typing.Set[str]]:
     """Given the path to a shared library, return a 4-tuple of sets
     (discovered, symbols, ignored, not_found).
     - discovered contains the original-case DLL paths of all direct and
       indirect dependencies of that shared library that should be bundled into
       the wheel.
-    - symbols contains the original-case paths of any .pdb symbol files
+    - associated contains the original-case paths of any .pdb or .lib files
       corresponding to the DLLs in discovered.
     - ignored contains the lowercased DLL names of all direct and indirect
       dependencies of that shared library that will not be bundled into the
       wheel because they are assumed to be on the target system.
     - If on_error is 'raise', FileNotFoundError is raised if a dependent
       library cannot be found. If on_error is 'ignore', not_found contains the
       lowercased DLL names of all dependent DLLs that cannot be found.
 
     no_dlls is a set of DLL names to force exclusion from the wheel. We do not
     search for dependencies of these DLLs.
 
     If wheel_dirs is not None, it is an iterable of directories in the wheel
     where dependencies are searched first.
 
-    include_symbols specifies whether to search for .pdb symbol files"""
+    include_symbols specifies whether to search for .pdb symbol files
+
+    include_imports specifies whether to search for .lib import library
+    files"""
     first_lib_path = lib_path.lower()
     stack = [first_lib_path]
     discovered = set()
-    symbols = set()
+    associated = set()
     ignored = set()
     not_found = set()
     while stack:
         lib_path = stack.pop()
         if lib_path not in discovered:
             discovered.add(lib_path)
             with PEContext(lib_path, None, True, verbose) as pe:
@@ -390,27 +409,26 @@
                 lib_name_lower = os.path.basename(lib_path).lower()
                 for entry in imports:
                     dll_name = entry.dll.decode('utf-8').lower()
                     if dll_name not in ignore_names and \
                             not any(r.fullmatch(dll_name) for r in _dll_list.ignore_regexes) and \
                             dll_name not in no_dlls and \
                             (lib_name_lower not in _dll_list.ignore_dependency or dll_name not in _dll_list.ignore_dependency[lib_name_lower]):
-                        dll_info = find_library(dll_name, wheel_dirs, lib_arch, include_symbols)
+                        dll_info = find_library(dll_name, wheel_dirs, lib_arch, include_symbols, include_imports)
                         if dll_info:
                             stack.append(dll_info[0])
-                            if dll_info[1]:
-                                symbols.add(dll_info[1])
+                            associated.update(dll_info[1])
                         elif on_error == 'raise':
                             raise FileNotFoundError(f'Unable to find library: {dll_name}')
                         else:
                             not_found.add(dll_name)
                     else:
                         ignored.add(dll_name)
     discovered.remove(first_lib_path)
-    return discovered, symbols, ignored, not_found
+    return discovered, associated, ignored, not_found
 
 
 def _round_to_next(size: int, alignment: int) -> int:
     """Return smallest n such that n % alignment == 0 and n >= size."""
     if size % alignment == 0:
         return size
     else:
```

### Comparing `delvewheel-1.5.4/delvewheel/_wheel_repair.py` & `delvewheel-1.6.0/delvewheel/_wheel_repair.py`

 * *Files 2% similar despite different names*

```diff
@@ -625,23 +625,23 @@
         for root, dirnames, filenames in os.walk(self._extract_dir):
             if root == self._data_dir:
                 dirnames[:] = set(dirnames) & {'platlib', 'purelib'}
             for filename in filenames:
                 if filename.lower().endswith('.pyd'):
                     extension_module_path = os.path.join(root, filename)
                     extension_module_paths.append(extension_module_path)
-                    discovered, _, ignored, not_found = _dll_utils.get_all_needed(extension_module_path, self._no_dlls, self._wheel_dirs, 'ignore', False, self._verbose)
+                    discovered, _, ignored, not_found = _dll_utils.get_all_needed(extension_module_path, self._no_dlls, self._wheel_dirs, 'ignore', False, False, self._verbose)
                     dependency_paths |= discovered
                     ignored_dll_names |= ignored
                     not_found_dll_names |= not_found
 
         # find extra dependencies specified with --add-dll
         extra_dependency_paths = set()
         for dll_name in self._add_dlls:
-            dll_info = _dll_utils.find_library(dll_name, None, self._arch, False)
+            dll_info = _dll_utils.find_library(dll_name, None, self._arch, False, False)
             if dll_info:
                 extra_dependency_paths.add(dll_info[0])
             else:
                 not_found_dll_names.add(dll_name)
 
         if self._ignore_in_wheel:
             dependency_paths_in_wheel, dependency_paths_outside_wheel = self._split_dependency_paths(dependency_paths)
@@ -682,16 +682,27 @@
             for ignored_dll_name in ignored_dll_names:
                 print(f'    {ignored_dll_name}')
         else:
             print('    None')
         if not_found_dll_names:
             print('\nWarning: At least one dependent DLL needs to be copied into the wheel but was not found.')
 
-    def repair(self, target: str, no_mangles: set, no_mangle_all: bool, strip: bool, lib_sdir: str, log_diagnostics: bool, namespace_pkgs: typing.Set[typing.Tuple[str]], include_symbols: bool) -> None:
+    def repair(
+            self,
+            target: str,
+            no_mangles: set,
+            no_mangle_all: bool,
+            strip: bool,
+            lib_sdir: str,
+            log_diagnostics: bool,
+            namespace_pkgs: typing.Set[typing.Tuple[str]],
+            include_symbols: bool,
+            include_imports: bool) -> None:
         """Repair the wheel in a manner similar to auditwheel.
+
         target is the target directory for storing the repaired wheel
         no_mangles is a set of lowercase DLL names that will not be mangled
         no_mangle_all is True if no DLL name mangling should happen at all
         strip is True if we should strip DLLs that contain trailing data when
             name-mangling
         lib_sdir is the suffix for the directory to store the DLLs
         log_diagnostics is True if diagnostic information is written to the
@@ -708,15 +719,15 @@
         if repair_version:
             print(f'Delvewheel {repair_version} has already repaired this wheel.')
             return
 
         # find dependencies
         print('finding DLL dependencies')
         dependency_paths = set()
-        symbol_paths = set()
+        associated_paths = set()
         ignored_dll_names = set()
         extension_module_paths = []
         has_top_level_ext_module = False
         for root, dirnames, filenames in os.walk(self._extract_dir):
             if root == self._data_dir:
                 dirnames[:] = set(dirnames) & {'platlib', 'purelib'}
             for filename in filenames:
@@ -728,17 +739,17 @@
                     if self._get_site_packages_relpath(root) == os.curdir:
                         if self._verbose >= 1:
                             print(f'analyzing top-level extension module {os.path.relpath(extension_module_path, self._extract_dir)}')
                         has_top_level_ext_module = True
                     elif self._verbose >= 1:
                         print(f'analyzing package-level extension module {os.path.relpath(extension_module_path, self._extract_dir)}')
                     extension_module_paths.append(extension_module_path)
-                    discovered, symbols, ignored = _dll_utils.get_all_needed(extension_module_path, self._no_dlls, self._wheel_dirs, 'raise', include_symbols, self._verbose)[:3]
+                    discovered, associated, ignored = _dll_utils.get_all_needed(extension_module_path, self._no_dlls, self._wheel_dirs, 'raise', include_symbols, include_imports, self._verbose)[:3]
                     dependency_paths |= discovered
-                    symbol_paths |= symbols
+                    associated_paths |= associated
                     ignored_dll_names |= ignored
 
         # if --ignore-in-wheel is specified, ignore DLLs that were found inside
         # the wheel unless they are specified with --add-dll
         if self._ignore_in_wheel:
             dependency_paths_in_wheel, dependency_paths_outside_wheel = self._split_dependency_paths(dependency_paths)
             for p in dependency_paths_in_wheel:
@@ -753,19 +764,18 @@
         # been found
         dependency_names = {os.path.basename(p) for p in dependency_paths}  # this is NOT lowercased
         dependency_names_lower = {name.lower() for name in dependency_names}
         extra_dependency_paths = set()
         for dll_name in self._add_dlls:
             if dll_name in dependency_names_lower:
                 continue
-            dll_info = _dll_utils.find_library(dll_name, None, self._arch, include_symbols)
+            dll_info = _dll_utils.find_library(dll_name, None, self._arch, include_symbols, include_imports)
             if dll_info:
                 extra_dependency_paths.add(dll_info[0])
-                if dll_info[1]:
-                    symbol_paths.add(dll_info[1])
+                associated_paths.update(dll_info[1])
             else:
                 raise FileNotFoundError(f'{dll_name} not found')
         if not dependency_paths and not extra_dependency_paths:
             print('no external dependencies are needed')
             os.makedirs(target, exist_ok=True)
             shutil.copy2(self._whl_path, target)
             print(f'wheel copied to {os.path.abspath(os.path.join(target, self._whl_name))}')
@@ -802,18 +812,18 @@
             libs_dir = os.path.join(self._extract_dir, libs_dir_name)
         os.makedirs(libs_dir, exist_ok=True)
         print(f'copying DLLs into {os.path.relpath(libs_dir, self._extract_dir)}')
         for dependency_path in dependency_paths | extra_dependency_paths:
             if self._verbose >= 1:
                 print(f'copying {dependency_path} -> {os.path.join(libs_dir, os.path.basename(dependency_path))}')
             shutil.copy2(dependency_path, libs_dir)
-        for symbol_path in symbol_paths:
+        for associated_path in associated_paths:
             if self._verbose >= 1:
-                print(f'copying {symbol_path} -> {os.path.join(libs_dir, os.path.basename(symbol_path))}')
-            shutil.copy2(symbol_path, libs_dir)
+                print(f'copying {associated_path} -> {os.path.join(libs_dir, os.path.basename(associated_path))}')
+            shutil.copy2(associated_path, libs_dir)
 
         # mangle library names
         name_mangler = {}  # dict from lowercased old name to new name
         if no_mangle_all:
             print('skip mangling DLL names')
         else:
             print('mangling DLL names')
```

### Comparing `delvewheel-1.5.4/delvewheel.egg-info/PKG-INFO` & `delvewheel-1.6.0/delvewheel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delvewheel
-Version: 1.5.4
+Version: 1.6.0
 Summary: Self-contained wheels for Windows
 Home-page: https://github.com/adang1345/delvewheel
 Author: Aohan Dang
 Author-email: adang1345@gmail.com
 License: MIT
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
@@ -92,14 +92,15 @@
 - `--no-mangle-all`: don't mangle any DLL names
 - `--strip`: strip DLLs that contain an overlay when name-mangling. The GNU `strip` utility must be present in `PATH`.
 - `-L`,`--lib-sdir`: subdirectory suffix to store vendored DLLs (default `.libs`). For example, if your wheel is named `mywheel-0.0.1-cp310-cp310-win_amd64.whl`, then the vendored DLLs are stored in `mywheel.libs` by default. If your wheel contains a top-level extension module that is not in any package, then this setting is ignored, and vendored DLLs are instead placed directly into `site-packages` when the wheel is installed.
 - `--namespace-pkg`: namespace packages, specified in case-sensitive dot notation and delimited by the path separator. Normally, we patch or create `__init__.py` in each top-level package to add the vendored DLL location to the DLL search path at runtime. If you have a top-level namespace package that requires `__init__.py` to be absent or unmodified, then this technique can cause problems. This option tells `delvewheel` to use an alternate strategy that does not create or modify `__init__.py` at the root of the given namespace package(s). For example,
   - `--namespace-pkg package1` declares `package1` as a namespace package.
   - On Windows, `--namespace-pkg package1.package2;package3` declares `package1`, `package1\package2`, and `package3` as namespace packages.
 - `--include-symbols`: include `.pdb` symbol files with the vendored DLLs. To be included, a symbol file must be in the same directory as the DLL and have the same filename before the extension, e.g. `example.dll` and `example.pdb`.
+- `--include-imports`: include `.lib` import library files with the vendored DLLs. To be included, an import library file must be in the same directory as the DLL and have the same filename before the extension, e.g. `example.dll` and `example.lib`.
 
 ## Limitations
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. We avoid vendoring system libraries that are provided by Windows 7 SP1 or later. If you intend to create a wheel for an older Windows system that requires an extra DLL, use the `--add-dll` flag to vendor additional DLLs into the wheel.
 - To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain an overlay at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, the overlay consists of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the overlay, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the overlay and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
```

### Comparing `delvewheel-1.5.4/setup.cfg` & `delvewheel-1.6.0/setup.cfg`

 * *Files identical despite different names*

